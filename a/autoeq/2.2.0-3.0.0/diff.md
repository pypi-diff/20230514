# Comparing `tmp/autoeq-2.2.0.tar.gz` & `tmp/autoeq-3.0.0.tar.gz`

## Comparing `autoeq-2.2.0.tar` & `autoeq-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/__init__.py
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/__main__.py
--rw-r--r--   0        0        0    10475 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/batch_processing.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/constants.py
--rw-r--r--   0        0        0    62318 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/frequency_response.py
--rw-r--r--   0        0        0    30461 2020-02-02 00:00:00.000000 autoeq-2.2.0/autoeq/peq.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 autoeq-2.2.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 autoeq-2.2.0/LICENSE
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 autoeq-2.2.0/README.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 autoeq-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 autoeq-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/__init__.py
+-rw-r--r--   0        0        0    17078 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/__main__.py
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/batch_processing.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/constants.py
+-rw-r--r--   0        0        0    63461 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/frequency_response.py
+-rw-r--r--   0        0        0    33134 2020-02-02 00:00:00.000000 autoeq-3.0.0/autoeq/peq.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 autoeq-3.0.0/webapp/ui/node_modules/big.js/LICENCE
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 autoeq-3.0.0/webapp/ui/node_modules/duplexer/LICENCE
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 autoeq-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 autoeq-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 autoeq-3.0.0/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 autoeq-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 autoeq-3.0.0/PKG-INFO
```

### Comparing `autoeq-2.2.0/autoeq/__main__.py` & `autoeq-3.0.0/autoeq/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import argparse
 import multiprocessing
 import warnings
 
 from autoeq.constants import DEFAULT_MAX_GAIN, DEFAULT_TREBLE_F_LOWER, DEFAULT_TREBLE_F_UPPER, \
     DEFAULT_TREBLE_GAIN_K, DEFAULT_FS, DEFAULT_BIT_DEPTH, DEFAULT_PHASE, DEFAULT_F_RES, DEFAULT_BASS_BOOST_FC, \
     DEFAULT_BASS_BOOST_Q, DEFAULT_SMOOTHING_WINDOW_SIZE, DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE, DEFAULT_TREBLE_BOOST_FC, \
-    DEFAULT_TREBLE_BOOST_Q, DEFAULT_PREAMP
+    DEFAULT_TREBLE_BOOST_Q, DEFAULT_PREAMP, DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE, DEFAULT_MAX_SLOPE
 from autoeq.batch_processing import batch_processing
 
 
 def cli_args():
     """Parses command line arguments."""
     arg_parser = argparse.ArgumentParser()
-    arg_parser.add_argument('--input-dir', type=str, required=True,
+    arg_parser.add_argument('--input-file', type=str, required=False,
+                            help='Path to measurement CSV data')
+    arg_parser.add_argument('--input-dir', type=str, required=False,
                             help='Path to input data directory. Will look for CSV files in the data directory and '
                                  'recursively in sub-directories.')
     arg_parser.add_argument('--output-dir', type=str, required=True,
                             help='Path to results directory. Will keep the same relative paths for files found '
                                  'in input-dir.')
     arg_parser.add_argument('--standardize-input', action='store_true',
                             help='Overwrite input data in standardized sampling and bias?')
@@ -114,19 +116,25 @@
                                  'the CSV file contains an error column and otherwise the raw column will be used. '
                                  'This means there are two different options for using sound signature: 1st is '
                                  'pointing it to a result CSV file of a previous run and the 2nd is to create a '
                                  'CSV file with just frequency and raw columns by hand (or other means). The Sound '
                                  'signature graph will be interpolated so any number of point at any frequencies '
                                  'will do, making it easy to create simple signatures with as little as two or '
                                  'three points.')
+    arg_parser.add_argument('--sound-signature-smoothing-window-size', type=float,
+                            help=f'Smoothing window size for sound signature. '
+                                 f'Defaults to {DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE}.')
     arg_parser.add_argument('--max-gain', type=float, default=DEFAULT_MAX_GAIN,
                             help='Maximum positive gain in equalization. Higher max gain allows to equalize deeper '
                                  'dips in  frequency response but will limit output volume if no analog gain is '
                                  'available because positive gain requires negative digital preamp equal to '
                                  f'maximum positive gain. Defaults to {DEFAULT_MAX_GAIN}.')
+    arg_parser.add_argument('--max-slope', type=float, default=DEFAULT_MAX_SLOPE,
+                            help='Maximum slope steepness for equalizer frequency response in dB/oct. Defaults to '
+                                 f'{DEFAULT_MAX_SLOPE}')
     arg_parser.add_argument('--window-size', type=float, default=DEFAULT_SMOOTHING_WINDOW_SIZE,
                             help='Smoothing window size in octaves.')
     arg_parser.add_argument('--treble-window-size', type=float, default=DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE,
                             help='Smoothing window size in octaves in the treble region.')
     arg_parser.add_argument('--treble-f-lower', type=float, default=DEFAULT_TREBLE_F_LOWER,
                             help='Lower bound for transition region between normal and treble frequencies. Treble '
                                  'frequencies can have different max gain and gain K. Defaults to '
```

### Comparing `autoeq-2.2.0/autoeq/batch_processing.py` & `autoeq-3.0.0/autoeq/batch_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,46 @@
 import tqdm
 import yaml
 
 from autoeq.constants import DEFAULT_MAX_GAIN, DEFAULT_TREBLE_F_LOWER, DEFAULT_TREBLE_F_UPPER, \
     DEFAULT_TREBLE_GAIN_K, DEFAULT_FS, DEFAULT_BIT_DEPTH, DEFAULT_PHASE, DEFAULT_F_RES, DEFAULT_BASS_BOOST_GAIN, \
     DEFAULT_BASS_BOOST_FC, DEFAULT_BASS_BOOST_Q, DEFAULT_SMOOTHING_WINDOW_SIZE, \
     DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE, PEQ_CONFIGS, DEFAULT_TREBLE_BOOST_GAIN, DEFAULT_TREBLE_BOOST_Q, \
-    DEFAULT_TREBLE_BOOST_FC, DEFAULT_PREAMP
+    DEFAULT_TREBLE_BOOST_FC, DEFAULT_PREAMP, DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE, DEFAULT_MAX_SLOPE
 from autoeq.frequency_response import FrequencyResponse
 
 
-def batch_processing(input_dir=None, output_dir=None, new_only=False, standardize_input=False, compensation=None,
-                     parametric_eq=False, fixed_band_eq=False, rockbox=False,
+def batch_processing(input_file=None, input_dir=None, output_dir=None, new_only=False, standardize_input=False,
+                     compensation=None, parametric_eq=False, fixed_band_eq=False, rockbox=False,
                      ten_band_eq=False, parametric_eq_config=None, fixed_band_eq_config=None, convolution_eq=False,
                      fs=DEFAULT_FS, bit_depth=DEFAULT_BIT_DEPTH, phase=DEFAULT_PHASE, f_res=DEFAULT_F_RES,
                      bass_boost_gain=DEFAULT_BASS_BOOST_GAIN, bass_boost_fc=DEFAULT_BASS_BOOST_FC,
                      bass_boost_q=DEFAULT_BASS_BOOST_Q, treble_boost_gain=DEFAULT_TREBLE_BOOST_GAIN,
                      treble_boost_fc=DEFAULT_TREBLE_BOOST_FC, treble_boost_q=DEFAULT_TREBLE_BOOST_Q,
-                     tilt=None, sound_signature=None, max_gain=DEFAULT_MAX_GAIN,
+                     tilt=None, sound_signature=None,
+                     sound_signature_smoothing_window_size=DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE,
+                     max_gain=DEFAULT_MAX_GAIN, max_slope=DEFAULT_MAX_SLOPE,
                      window_size=DEFAULT_SMOOTHING_WINDOW_SIZE, treble_window_size=DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE,
                      treble_f_lower=DEFAULT_TREBLE_F_LOWER, treble_f_upper=DEFAULT_TREBLE_F_UPPER,
                      treble_gain_k=DEFAULT_TREBLE_GAIN_K, preamp=DEFAULT_PREAMP, thread_count=0):
     """Parses files in input directory and produces equalization results in output directory."""
     if not compensation and (parametric_eq or fixed_band_eq or rockbox or ten_band_eq or convolution_eq):
         raise ValueError('Compensation must be specified when equalizing.')
 
-    # Dir paths to absolute
-    input_dir = os.path.abspath(input_dir)
-    glob_files = glob(os.path.join(input_dir, '**', '*.csv'), recursive=True)
-    if len(glob_files) == 0:
-        raise FileNotFoundError(f'No CSV files found in "{input_dir}"')
+    if input_file:
+        input_file_paths = [input_file]
+        input_dir = os.path.split(input_file)[0]
+    elif input_dir:
+        # Dir paths to absolute
+        input_dir = os.path.abspath(input_dir)
+        input_file_paths = glob(os.path.join(input_dir, '**', '*.csv'), recursive=True)
+        if len(input_file_paths) == 0:
+            raise FileNotFoundError(f'No CSV files found in "{input_dir}"')
+    else:
+        raise ValueError('Input file or input directory path must be specified.')
 
     if compensation:
         # Creates FrequencyResponse for compensation data
         compensation_path = os.path.abspath(compensation)
         compensation = FrequencyResponse.read_from_csv(compensation_path)
         compensation.interpolate()
         compensation.center()
@@ -84,28 +92,31 @@
                     f'If this was meant to be a file, the file does not exist.')
             fixed_band_eq_config = PEQ_CONFIGS[fixed_band_eq_config]
 
     # Prepare list of arguments for all the function calls to generate results.
     n_total = 0
     file_paths = []
     args_list = []
-    for input_file_path in glob_files:
+    for input_file_path in input_file_paths:
+        name = os.path.split(input_file_path)[1].replace('.csv', '')
         relative_path = os.path.relpath(input_file_path, input_dir)
-        output_file_path = os.path.join(output_dir, relative_path) if output_dir else None
-        output_file_dir = os.path.split(output_file_path)[0]
+        output_file_path = os.path.join(output_dir, relative_path)
+        output_file_dir, output_file_name = os.path.split(output_file_path)
+        output_file_dir = os.path.join(output_file_dir, name)
+        output_file_path = os.path.join(output_file_dir, output_file_name)
         if not new_only or not os.path.isdir(output_file_dir) or not len(os.listdir(output_file_dir)):
             # Not looking for only new ones or the output directory doesn't exist or it's empty
             file_paths.append((input_file_path, output_file_path))
             n_total += 1
             args = (input_file_path, output_file_path, bass_boost_fc, bass_boost_gain, bass_boost_q,
                     treble_boost_fc, treble_boost_gain, treble_boost_q,
                     bit_depth, compensation, convolution_eq, f_res, fixed_band_eq, fs, parametric_eq_config,
-                    fixed_band_eq_config, max_gain, window_size, treble_window_size,
-                    parametric_eq, phase, rockbox, sound_signature, standardize_input,
-                    ten_band_eq, tilt, treble_f_lower, treble_f_upper, treble_gain_k, preamp)
+                    fixed_band_eq_config, max_gain, max_slope, window_size, treble_window_size,
+                    parametric_eq, phase, rockbox, sound_signature, sound_signature_smoothing_window_size,
+                    standardize_input, ten_band_eq, tilt, treble_f_lower, treble_f_upper, treble_gain_k, preamp)
             args_list.append(args)
 
     if not thread_count:
         thread_count = multiprocessing.cpu_count()
 
     with multiprocessing.Pool(thread_count) as pool:
         results = []
@@ -118,17 +129,17 @@
 def process_file_wrapper(params):
     return process_file(*params)
 
 
 def process_file(input_file_path, output_file_path, bass_boost_fc, bass_boost_gain, bass_boost_q,
                  treble_boost_fc, treble_boost_gain, treble_boost_q, bit_depth,
                  compensation, convolution_eq, f_res, fixed_band_eq, fs, parametric_eq_config,
-                 fixed_band_eq_config, max_gain, window_size, treble_window_size, parametric_eq, phase, rockbox,
-                 sound_signature, standardize_input, ten_band_eq, tilt, treble_f_lower, treble_f_upper,
-                 treble_gain_k, preamp):
+                 fixed_band_eq_config, max_gain, max_slope, window_size, treble_window_size, parametric_eq, phase,
+                 rockbox, sound_signature, sound_signature_smoothing_window_size, standardize_input, ten_band_eq, tilt,
+                 treble_f_lower, treble_f_upper, treble_gain_k, preamp):
     # The method assumes fs is iterable, ensure it really is
     try:
         fs[0]
     except TypeError:
         fs = [fs]
 
     # Read data from input file
@@ -161,15 +172,17 @@
         bass_boost_q=bass_boost_q,
         treble_boost_gain=treble_boost_gain,
         treble_boost_fc=treble_boost_fc,
         treble_boost_q=treble_boost_q,
         tilt=tilt,
         fs=fs[0],
         sound_signature=sound_signature,
+        sound_signature_smoothing_window_size=sound_signature_smoothing_window_size,
         max_gain=max_gain,
+        max_slope=max_slope,
         window_size=window_size,
         treble_window_size=treble_window_size,
         treble_f_lower=treble_f_lower,
         treble_f_upper=treble_f_upper,
         treble_gain_k=treble_gain_k,)
 
     fr.write_eqapo_graphic_eq(output_file_path.replace('.csv', ' GraphicEQ.txt'), normalize=True, preamp=preamp)
```

### Comparing `autoeq-2.2.0/autoeq/frequency_response.py` & `autoeq-3.0.0/autoeq/frequency_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 import warnings
 from autoeq.constants import DEFAULT_F_MIN, DEFAULT_F_MAX, DEFAULT_STEP, DEFAULT_MAX_GAIN, DEFAULT_TREBLE_F_LOWER, \
     DEFAULT_TREBLE_F_UPPER, DEFAULT_TREBLE_GAIN_K, DEFAULT_SMOOTHING_WINDOW_SIZE, \
     DEFAULT_SMOOTHING_ITERATIONS, DEFAULT_TREBLE_SMOOTHING_F_LOWER, DEFAULT_TREBLE_SMOOTHING_F_UPPER, \
     DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE, DEFAULT_TREBLE_SMOOTHING_ITERATIONS, DEFAULT_TILT, DEFAULT_FS, \
     DEFAULT_F_RES, DEFAULT_BASS_BOOST_GAIN, DEFAULT_BASS_BOOST_FC, \
     DEFAULT_BASS_BOOST_Q, DEFAULT_GRAPHIC_EQ_STEP, HARMAN_INEAR_PREFENCE_FREQUENCIES, \
-    HARMAN_ONEAR_PREFERENCE_FREQUENCIES, PREAMP_HEADROOM, DEFAULT_MAX_SLOPE, \
+    HARMAN_OVEREAR_PREFERENCE_FREQUENCIES, PREAMP_HEADROOM, DEFAULT_MAX_SLOPE, \
     DEFAULT_BIQUAD_OPTIMIZATION_F_STEP, DEFAULT_TREBLE_BOOST_GAIN, DEFAULT_TREBLE_BOOST_FC, DEFAULT_TREBLE_BOOST_Q, \
-    DEFAULT_PREAMP
-from autoeq.peq import PEQ, LowShelf, HighShelf
+    DEFAULT_PREAMP, DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE
+from autoeq.peq import PEQ, LowShelf, HighShelf, Peaking
 
 warnings.filterwarnings("ignore", message="Values in x were outside bounds during a minimize step, clipping to bounds")
 
 
 class FrequencyResponse:
     def __init__(self,
                  name=None,
@@ -316,15 +316,15 @@
         file_path = os.path.abspath(file_path)
         f = self.generate_frequencies(f_step=DEFAULT_BIQUAD_OPTIMIZATION_F_STEP)
         compound = PEQ(f, peqs[0].fs, [])
         for peq in peqs:
             for filt in peq.filters:
                 compound.add_filter(filt)
 
-        types = {'Peaking': 'PK', 'LowShelf': 'LS', 'HighShelf': 'HS'}
+        types = {Peaking.__name__: 'PK', LowShelf.__name__: 'LSC', HighShelf.__name__: 'HSC'}
 
         with open(file_path, 'w', encoding='utf-8') as f:
             s = f'Preamp: {-compound.max_gain:.1f} dB\n'
             for i, filt in enumerate(compound.filters):
                 s += f'Filter {i + 1}: ON {types[filt.__class__.__name__]} Fc {filt.fc:.0f} Hz Gain {filt.gain:.1f} dB Q {filt.q:.2f}\n'
             f.write(s)
 
@@ -513,15 +513,15 @@
             if self.raw[i] is None:
                 self.raw = np.delete(self.raw, i)
                 self.frequency = np.delete(self.frequency, i)
             else:
                 i += 1
 
         # Interpolation functions
-        keys = 'raw error error_smoothed equalization equalized_raw equalized_smoothed target'.split()
+        keys = 'raw smoothed error error_smoothed equalization equalized_raw equalized_smoothed target'.split()
         interpolators = dict()
         log_f = np.log10(self.frequency)
         for key in keys:
             if len(self.__dict__[key]):
                 interpolators[key] = InterpolatedUnivariateSpline(log_f, self.__dict__[key], k=pol_order)
 
         if f is None:
@@ -642,37 +642,45 @@
                    bass_boost_q=DEFAULT_BASS_BOOST_Q,
                    treble_boost_gain=DEFAULT_TREBLE_BOOST_GAIN,
                    treble_boost_fc=DEFAULT_TREBLE_BOOST_FC,
                    treble_boost_q=DEFAULT_TREBLE_BOOST_Q,
                    tilt=None,
                    fs=DEFAULT_FS,
                    sound_signature=None,
+                   sound_signature_smoothing_window_size=DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE,
                    min_mean_error=False):
         """Sets target and error curves."""
         # Copy and center compensation data
         compensation = self.__class__(name='compensation', frequency=compensation.frequency, raw=compensation.raw)
+        compensation.interpolate()
         compensation.center()
 
         # Set target
         self.target = compensation.raw + self.create_target(
             bass_boost_gain=bass_boost_gain,
             bass_boost_fc=bass_boost_fc,
             bass_boost_q=bass_boost_q,
             treble_boost_gain=treble_boost_gain,
             treble_boost_fc=treble_boost_fc,
             treble_boost_q=treble_boost_q,
             tilt=tilt,
             fs=fs
         )
         if sound_signature is not None:
-            # Sound signature give, add it to target curve
+            # Sound signature given, add it to target curve
             if not np.all(sound_signature.frequency == self.frequency):
                 # Interpolate sound signature to match self on the frequency axis
                 sound_signature.interpolate(self.frequency)
-            self.target += sound_signature.raw
+            if sound_signature_smoothing_window_size:
+                sound_signature.smoothen_fractional_octave(
+                    window_size=sound_signature_smoothing_window_size,
+                    treble_window_size=sound_signature_smoothing_window_size)
+                self.target += sound_signature.smoothed
+            else:
+                self.target += sound_signature.raw
 
         # Set error
         self.error = self.raw - self.target
         if min_mean_error:
             # Shift error by it's mean in range 100 Hz to 10 kHz
             delta = np.mean(self.error[np.logical_and(self.frequency >= 100, self.frequency <= 10000)])
             self.error -= delta
@@ -820,28 +828,28 @@
             equalized_raw=True,
             equalized_smoothed=True,
             target=False
         )
 
     def equalize(self,
                  max_gain=DEFAULT_MAX_GAIN,
-                 limit=DEFAULT_MAX_SLOPE,
-                 limit_decay=0.0,
+                 max_slope=DEFAULT_MAX_SLOPE,
+                 max_slope_decay=0.0,
                  concha_interference=False,
                  window_size=1 / 12,
                  treble_window_size=2,
                  treble_f_lower=DEFAULT_TREBLE_F_LOWER,
                  treble_f_upper=DEFAULT_TREBLE_F_UPPER,
                  treble_gain_k=DEFAULT_TREBLE_GAIN_K):
         """Creates equalization curve and equalized curve.
 
         Args:
             max_gain: Maximum positive gain in dB
-            limit: Maximum slope in dB per octave
-            limit_decay: Decay coefficient (per octave) for the limit. Value of 0.5 would reduce limit by 50% in an octave
+            max_slope: Maximum slope in dB per octave
+            max_slope_decay: Decay coefficient (per octave) for the limit. Value of 0.5 would reduce limit by 50% in an octave
                 when traversing a single limitation zone.
             concha_interference: Do measurements include concha interference which produced a narrow dip around 9 kHz?
             window_size: Smoothing window size in octaves.
             treble_window_size: Smoothing window size in octaves in the treble region.
             treble_f_lower: Lower boundary of transition frequency region. In the transition region normal filter is \
                             switched to treble filter with sigmoid weighting function.
             treble_f_upper: Upper boundary of transition frequency reqion. In the transition region normal filter is \
@@ -887,18 +895,18 @@
             rtl_start = self.find_rtl_start(y, peak_inds, dip_inds)
 
             # Find ltr and rtl limitations
             # limited_ltr is y but with slopes limited when traversing left to right
             # clipped_ltr is boolean mask for limited samples when traversing left to right
             # limited_rtl is found using ltr algorithm but with flipped data
             limited_ltr, clipped_ltr, regions_ltr = self.limited_ltr_slope(
-                x, y, limit, limit_decay=limit_decay, start_index=0, peak_inds=peak_inds,
+                x, y, max_slope, max_slope_decay=max_slope_decay, start_index=0, peak_inds=peak_inds,
                 limit_free_mask=limit_free_mask, concha_interference=concha_interference)
             limited_rtl, clipped_rtl, regions_rtl = self.limited_rtl_slope(
-                x, y, limit, limit_decay=limit_decay, start_index=rtl_start, peak_inds=peak_inds,
+                x, y, max_slope, max_slope_decay=max_slope_decay, start_index=rtl_start, peak_inds=peak_inds,
                 limit_free_mask=limit_free_mask, concha_interference=concha_interference)
 
             # ltr and rtl limited curves are combined with min function
             combined = self.__class__(
                 name='limiter', frequency=x, raw=np.min(np.vstack([limited_ltr, limited_rtl]), axis=0))
 
             # Limit treble gain
@@ -954,23 +962,23 @@
             target_right = dip_levels[i + 1]
             left_ind = np.argwhere(y[:dip_ind] >= target_left)[-1, 0] + 1
             right_ind = np.argwhere(y[dip_ind:] >= target_right)[0, 0] + dip_ind - 1
             mask[left_ind:right_ind + 1] = np.ones(right_ind - left_ind + 1).astype(bool)
         return mask
 
     @classmethod
-    def limited_rtl_slope(cls, x, y, limit, limit_decay=0.0, start_index=0, peak_inds=None, limit_free_mask=None,
+    def limited_rtl_slope(cls, x, y, max_slope, max_slope_decay=0.0, start_index=0, peak_inds=None, limit_free_mask=None,
                           concha_interference=False):
         """Limits right to left slope of an equalization curve.
 
             Args:
                 x: frequencies
                 y: amplitudes
-                limit: maximum slope in dB / oct
-                limit_decay: Limit decay coefficient per octave
+                max_slope: maximum slope in dB / oct
+                max_slope_decay: Max slope decay coefficient per octave
                 start_index: Index where to start traversing, no limitations apply before this
                 peak_inds: Peak indexes. Regions will require to touch one of these if given.
                 limit_free_mask: Boolean mask for indices where limitation must not be applied
                 concha_interference: Do measurements include concha interference which produced a narrow dip around 9 kHz?
 
             Returns:
                 limited: Limited curve
@@ -979,31 +987,31 @@
         """
         start_index = len(x) - start_index - 1
         if peak_inds is not None:
             peak_inds = len(x) - peak_inds - 1
         if limit_free_mask is not None:
             limit_free_mask = np.flip(limit_free_mask)
         limited_rtl, clipped_rtl, regions_rtl = cls.limited_ltr_slope(
-            x, np.flip(y), limit, limit_decay=limit_decay, start_index=start_index, peak_inds=peak_inds,
+            x, np.flip(y), max_slope, max_slope_decay=max_slope_decay, start_index=start_index, peak_inds=peak_inds,
             limit_free_mask=limit_free_mask, concha_interference=concha_interference)
         limited_rtl = np.flip(limited_rtl)
         clipped_rtl = np.flip(clipped_rtl)
         regions_rtl = len(x) - regions_rtl - 1
         return limited_rtl, clipped_rtl, regions_rtl
 
     @classmethod
-    def limited_ltr_slope(cls, x, y, limit, limit_decay=0.0, start_index=0, peak_inds=None, limit_free_mask=None,
+    def limited_ltr_slope(cls, x, y, max_slope, max_slope_decay=0.0, start_index=0, peak_inds=None, limit_free_mask=None,
                           concha_interference=False):
         """Limits left to right slope of a equalization curve.
 
         Args:
             x: frequencies
             y: amplitudes
-            limit: maximum slope in dB / oct
-            limit_decay: Limit decay coefficient per octave
+            max_slope: maximum slope in dB / oct
+            max_slope_decay: Max slope decay coefficient per octave
             start_index: Index where to start traversing, no limitations apply before this
             peak_inds: Peak indexes. Regions will require to touch one of these if given.
             limit_free_mask: Boolean mask for indices where limitation must not be applied
             concha_interference: Do measurements include concha interference which produced a narrow dip around 9 kHz?
 
         Returns:
             limited: Limited curve
@@ -1022,19 +1030,19 @@
                 limited.append(y[i])
                 clipped.append(False)
                 continue
 
             # Calculate slope and local limit
             slope = cls.log_log_gradient(x[i], x[i - 1], y[i], limited[-1])
             # Local limit is 25% of the limit between 8 kHz and 10 kHz
-            local_limit = limit / 4 if 8000 <= x[i] <= 11500 and concha_interference else limit
+            local_limit = max_slope / 4 if 8000 <= x[i] <= 11500 and concha_interference else max_slope
 
             if clipped[-1]:
                 # Previous sample clipped, reduce limit
-                local_limit *= (1 - limit_decay) ** np.log2(x[i] / x[regions[-1][0]])
+                local_limit *= (1 - max_slope_decay) ** np.log2(x[i] / x[regions[-1][0]])
 
             if slope > local_limit and (limit_free_mask is None or not limit_free_mask[i]):
                 # Slope between the two samples is greater than the local maximum slope, clip to the max
                 if not clipped[-1]:
                     # Start of clipped region
                     regions.append([i])
                 clipped.append(True)
@@ -1235,24 +1243,24 @@
             im.save(file_path, optimize=True)
         if show:
             plt.show()
         elif close:
             plt.close(fig)
         return fig, ax
 
-    def harman_onear_preference_score(self):
+    def harman_overear_preference_score(self):
         """Calculates Harman preference score for over-ear and on-ear headphones.
 
         Returns:
             - score: Preference score
             - std: Standard deviation of error
             - slope: Slope of linear regression of error
         """
         fr = self.copy()
-        fr.interpolate(HARMAN_ONEAR_PREFERENCE_FREQUENCIES)
+        fr.interpolate(HARMAN_OVEREAR_PREFERENCE_FREQUENCIES)
         sl = np.logical_and(fr.frequency >= 50, fr.frequency <= 10000)
         x = fr.frequency[sl]
         y = fr.error[sl]
 
         std = np.std(y, ddof=1)  # ddof=1 is required to get the exact same numbers as the Excel from Listen Inc gives
         slope, _, _, _, _ = linregress(np.log(x), y)
         score = 114.490443008238 - 12.62 * std - 15.5163857197367 * np.abs(slope)
@@ -1293,15 +1301,17 @@
                 bass_boost_q=None,
                 treble_boost_gain=None,
                 treble_boost_fc=None,
                 treble_boost_q=None,
                 tilt=None,
                 fs=DEFAULT_FS,
                 sound_signature=None,
+                sound_signature_smoothing_window_size=DEFAULT_SOUND_SIGNATURE_SMOOTHING_WINDOW_SIZE,
                 max_gain=DEFAULT_MAX_GAIN,
+                max_slope=DEFAULT_MAX_SLOPE,
                 concha_interference=False,
                 window_size=DEFAULT_SMOOTHING_WINDOW_SIZE,
                 treble_window_size=DEFAULT_TREBLE_SMOOTHING_WINDOW_SIZE,
                 treble_f_lower=DEFAULT_TREBLE_F_LOWER,
                 treble_f_upper=DEFAULT_TREBLE_F_UPPER,
                 treble_gain_k=DEFAULT_TREBLE_GAIN_K):
         """Runs processing pipeline with interpolation, centering, compensation and equalization.
@@ -1316,15 +1326,17 @@
             bass_boost_q: Bass boost low shelf quality.
             treble_boost_gain: Treble boost amount in dB.
             treble_boost_fc: Treble boost high shelf center frequency.
             treble_boost_q: Treble boost high shelf quality.
             fs: Sampling frequency
             tilt: Target frequency response tilt in db / octave
             sound_signature: Sound signature as FrequencyResponse instance. Raw data will be used.
+            sound_signature_smoothing_window_size: Smoothing window size in octaves for sound signature
             max_gain: Maximum positive gain in dB
+            max_slope: Maximum slope steepness for equalizer frequency response in db/oct.
             concha_interference: Do measurements include concha interference which produced a narrow dip around 9 kHz?
             window_size: Smoothing window size in octaves.
             treble_window_size: Smoothing window size in octaves in the treble region.
             treble_f_lower: Lower boundary of transition frequency region. In the transition region normal filter is
                             switched to treble filter with sigmoid weighting function.
             treble_f_upper: Upper boundary of transition frequency region. In the transition region normal filter is
                             switched to treble filter with sigmoid weighting function.
@@ -1340,18 +1352,19 @@
             bass_boost_q=bass_boost_q,
             treble_boost_gain=treble_boost_gain,
             treble_boost_fc=treble_boost_fc,
             treble_boost_q=treble_boost_q,
             tilt=tilt,
             fs=fs,
             sound_signature=sound_signature,
+            sound_signature_smoothing_window_size=sound_signature_smoothing_window_size,
             min_mean_error=min_mean_error
         )
         self.smoothen_fractional_octave(
             window_size=window_size,
             treble_window_size=treble_window_size,
             treble_f_lower=treble_f_lower,
             treble_f_upper=treble_f_upper
         )
         self.equalize(
-            max_gain=max_gain, concha_interference=concha_interference, treble_f_lower=treble_f_lower,
+            max_slope=max_slope, max_gain=max_gain, concha_interference=concha_interference, treble_f_lower=treble_f_lower,
             treble_f_upper=treble_f_upper, treble_gain_k=treble_gain_k)
```

### Comparing `autoeq-2.2.0/autoeq/peq.py` & `autoeq-3.0.0/autoeq/peq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from copy import deepcopy
 from time import time
 from abc import ABC, abstractmethod
 import numpy as np
 from matplotlib import pyplot as plt, ticker
 from scipy.optimize import fmin_slsqp
 from scipy.signal import find_peaks
 from tabulate import tabulate
@@ -180,32 +181,33 @@
             positive_peak_ixs, peak_props = find_peaks(np.clip(target, 0, None), width=0, prominence=0, height=0)
             negative_peak_ixs, dip_props = find_peaks(np.clip(-target, 0, None), width=0, prominence=0, height=0)
 
         # Indexes for minimum and maximum center frequency
         min_fc_ix = np.argmin(np.abs(self.f - self.min_fc))
         max_fc_ix = np.argmin(np.abs(self.f - self.max_fc))
 
-        if len(positive_peak_ixs) == 0 and len(negative_peak_ixs) == 0:
+        # All peak indexes together
+        peak_ixs = np.concatenate([positive_peak_ixs, negative_peak_ixs])
+        # Exclude peak indexes which are outside of minimum and maximum center frequency
+        mask = np.logical_and(peak_ixs >= min_fc_ix, peak_ixs <= max_fc_ix)
+
+        if (len(positive_peak_ixs) == 0 and len(negative_peak_ixs) == 0) or np.sum(mask) == 0:
             # No peaks found
             params = []
             if self.optimize_fc:
                 self.fc = self.f[(min_fc_ix + max_fc_ix) // 2]
                 params.append(np.log10(self.fc))
             if self.optimize_q:
                 self.q = np.sqrt(2)
                 params.append(self.q)
             if self.optimize_gain:
                 self.gain = 0.0
                 params.append(self.gain)
             return params
 
-        # All peak indexes together
-        peak_ixs = np.concatenate([positive_peak_ixs, negative_peak_ixs])
-        # Exclude peak indexes which are outside of minimum and maximum center frequency
-        mask = np.logical_and(peak_ixs >= min_fc_ix, peak_ixs <= max_fc_ix)
         peak_ixs = peak_ixs[mask]
         # Properties of included peaks together
         widths = np.concatenate([peak_props['widths'], dip_props['widths']])[mask]
         heights = np.concatenate([peak_props['peak_heights'], dip_props['peak_heights']])[mask]
         # Find the biggest peak, by height AND width
         sizes = widths * heights  # Size of each peak for ranking
         ixs_ix = np.argmax(sizes)  # Index to indexes array which point to the biggest peak
@@ -435,25 +437,25 @@
         self.f = np.array(f)
         self.fs = fs
         self.filters = []
         if filters is not None:
             for filt in filters:
                 self.add_filter(filt)
         self.target = np.array(target) if target is not None else None
-        self._min_f = min_f
-        self._max_f = max_f
+        self._min_f = min_f if min_f is not None else DEFAULT_PEQ_OPTIMIZER_MIN_F
+        self._max_f = max_f if max_f is not None else DEFAULT_PEQ_OPTIMIZER_MAX_F
         self._min_f_ix = np.argmin(np.abs(self.f - self._min_f))
         self._max_f_ix = np.argmin(np.abs(self.f - self._max_f))
         self._ix50 = np.argmin(np.abs(self.f - 50))
         self._10k_ix = np.argmin(np.abs(self.f - 10000))
         self._20k_ix = np.argmin(np.abs(self.f - 20000))
-        self._max_time = max_time
-        self._target_loss = target_loss
+        self._max_time = max_time if max_time is not None else DEFAULT_PEQ_OPTIMIZER_MAX_TIME
+        self._target_loss = target_loss if target_loss is not None else DEFAULT_PEQ_OPTIMIZER_TARGET_LOSS
         self._min_change_rate = min_change_rate
-        self._min_std = min_std
+        self._min_std = min_std if min_std is not None else DEFAULT_PEQ_OPTIMIZER_MIN_STD
         self.history = None
 
     @classmethod
     def from_dict(cls, config, f, fs, target=None):
         """Initializes class instance with configuration dict and target
 
         Args:
@@ -472,23 +474,53 @@
         """
         if target is not None and len(f) != len(target):
             raise ValueError('f and target must be the same length')
         optimizer_kwargs = config['optimizer'] if 'optimizer' in config else {}
         peq = cls(f, fs, target=target, **optimizer_kwargs)
         filter_classes = {'LOW_SHELF': LowShelf, 'PEAKING': Peaking, 'HIGH_SHELF': HighShelf}
         keys = ['fc', 'q', 'gain', 'min_fc', 'max_fc', 'min_q', 'max_q', 'min_gain', 'max_gain', 'type']
+        global_filter_defaults = {
+            'LOW_SHELF': {
+                'min_fc': DEFAULT_SHELF_FILTER_MIN_FC,
+                'max_fc': DEFAULT_SHELF_FILTER_MAX_FC,
+                'min_q': DEFAULT_SHELF_FILTER_MIN_Q,
+                'max_q': DEFAULT_SHELF_FILTER_MAX_Q,
+                'min_gain': DEFAULT_SHELF_FILTER_MIN_GAIN,
+                'max_gain': DEFAULT_SHELF_FILTER_MAX_GAIN
+            },
+            'PEAKING': {
+                'min_fc': DEFAULT_PEAKING_FILTER_MIN_FC,
+                'max_fc': DEFAULT_PEAKING_FILTER_MAX_FC,
+                'min_q': DEFAULT_PEAKING_FILTER_MIN_Q,
+                'max_q': DEFAULT_PEAKING_FILTER_MAX_Q,
+                'min_gain': DEFAULT_PEAKING_FILTER_MIN_GAIN,
+                'max_gain': DEFAULT_PEAKING_FILTER_MAX_GAIN
+            }
+        }
+        global_filter_defaults['HIGH_SHELF'] = deepcopy(global_filter_defaults['LOW_SHELF'])
         for filt in config['filters']:
-            if 'filter_defaults' in config:
+            if 'filter_defaults' in config and config['filter_defaults'] is not None:
                 for key in keys:
-                    if key not in filt and key in config['filter_defaults']:
+                    if (key not in filt or filt[key] is None) and key in config['filter_defaults']:
                         filt[key] = config['filter_defaults'][key]
+            for key in keys:
+                if (key not in filt or filt[key] is None) and key in global_filter_defaults[filt['type']]:
+                    filt[key] = global_filter_defaults[filt['type']][key]
+            if 'min_fc' in filt and 'max_fc' in filt and filt['min_fc'] == filt['max_fc']:
+                filt['fc'] = filt['min_fc']
+            if 'min_q' in filt and 'max_q' in filt and filt['min_q'] == filt['max_q']:
+                filt['q'] = filt['min_q']
+            if 'min_gain' in filt and 'max_gain' in filt and filt['min_gain'] == filt['max_gain']:
+                filt['gain'] = filt['min_gain']
             peq.add_filter(filter_classes[filt['type']](
                 peq.f, peq.fs,
                 **{key: filt[key] for key in keys if key in filt and key != 'type'},
-                optimize_fc='fc' not in filt, optimize_q='q' not in filt, optimize_gain='gain' not in filt
+                optimize_fc='fc' not in filt or filt['fc'] is None,
+                optimize_q='q' not in filt or filt['q'] is None,
+                optimize_gain='gain' not in filt or filt['gain'] is None
             ))
         return peq
 
     def add_filter(self, filt):
         if filt.fs != self.fs:
             raise ValueError(f'Filter sampling rate ({filt.fs}) must match equalizer sampling rate ({self.fs})')
         if not np.array_equal(filt.f, self.f):
@@ -520,14 +552,22 @@
         ]
         return tabulate(
             table_data,
             headers=['#', 'Type', 'Fc (Hz)', 'Q', 'Gain (dB)'],
             tablefmt='github'
         )
 
+    def to_dict(self):
+        """PEQ as dictionary"""
+        name_map = {LowShelf.__name__: 'LOW_SHELF', Peaking.__name__: 'PEAKING', HighShelf.__name__: 'HIGH_SHELF'}
+        return {
+            'fs': self.fs,
+            'filters': [{'type': name_map[filt.__class__.__name__], 'fc': filt.fc, 'q': filt.q, 'gain': filt.gain} for filt in self.filters]
+        }
+
     def _parse_optimizer_params(self, params):
         """Extracts fc, q and gain from optimizer params and updates filters
 
         Args:
             params: Parameter list/array passed by the optimizer. The values correspond to the initialized params
         """
         i = 0
@@ -662,26 +702,32 @@
                 # ...STD from the last N/2 loss values must be below half of the min STD
                 or (len(self.history.std) > n // 2 and std_np2 < self._min_std / 2)
         ):
             raise OptimizationFinished('STD too small')
 
     def optimize(self):
         """Optimizes filter parameters"""
+        has_free_variables = False
+        for filt in self.filters:
+            if filt.optimize_fc or filt.optimize_q or filt.optimize_gain:
+                has_free_variables = True
+                break
+        if not has_free_variables:
+            return
         self.history = OptimizationHistory()
         try:
             fmin_slsqp(  # Tested all of the scipy minimize methods, this is the best
                 self._optimizer_loss,
                 self._init_optimizer_params(),
                 bounds=self._init_optimizer_bounds(),
                 callback=self._callback,
                 iprint=0)
         except OptimizationFinished as err:
             # Restore best params
             self._parse_optimizer_params(self.history.params[np.argmin(self.history.loss)])
-            #print(err)
 
     def plot(self, fig=None, ax=None):
         if fig is None:
             fig, ax = plt.subplots()
             fig.set_size_inches(12, 8)
             fig.set_facecolor('white')
             ax.set_facecolor('white')
```

### Comparing `autoeq-2.2.0/.gitignore` & `autoeq-3.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 # dotenv
 .env
 
 # virtualenv
 .venv
 venv/
 ENV/
-env/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
@@ -110,7 +109,9 @@
 **/pdf
 **/json
 **/data/ignore
 measurements/crinacle/*data*/
 measurements/crinacle/Raw measurements (Patreon)/
 results/crinacle/*/*/*.csv
 chromedriver*
+webapp/data/*
+!webapp/data/legal/
```

### Comparing `autoeq-2.2.0/LICENSE` & `autoeq-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoeq-2.2.0/README.md` & `autoeq-3.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 curves, apply tilt for making the headphones brighter/darker and adding a bass boost. It's even possible to make one
 headphone sound (roughly) like another headphone. For more info about usage see [Usage](#usage).
 
 AutoEq [Github page](https://github.com/jaakkopasanen/AutoEq) also serves as a database for headphone frequency response
 measurements, pre-computed results and has documentation about different equalizers and how the implementation works.
 
 ### Updates
+#### 3.0.0
+* Added `--input-file`, `--max-slope` and `--sound-signature-smoothing-window-size` parameters.
+* Fixed crashing with non-standard sized compensation and measurement data.
+* Fixed parametric eq optimizer producing filters outside of specified frequency range.
+* Fixed parametric eq optimizer crashing without any free optimizeable parameters.
+* Added defaul values for some args in parametric eq optimizer.
+* Added more parametric eq optimizer configs.
+* Introduced API breaking naming changes.
+
 #### 2.2.0
 Added `--preamp` parameter
 
 #### 2.1.1
 Fixed README in PyPi package
 
 #### 2.1.0
```

### Comparing `autoeq-2.2.0/pyproject.toml` & `autoeq-3.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "autoeq"
-version = "2.2.0"
+version = "3.0.0"
 authors = [
   { name="Jaakko Pasanen", email="jaakko.o.pasanen@gmail.com" },
 ]
 description = "Automatic headphone equalizer config generator"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.7,<3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'Pillow~=9.2.0',
```

### Comparing `autoeq-2.2.0/PKG-INFO` & `autoeq-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: autoeq
-Version: 2.2.0
+Version: 3.0.0
 Summary: Automatic headphone equalizer config generator
 Project-URL: Homepage, https://github.com/jaakkopasanen/AutoEq
 Project-URL: Bug Tracker, https://github.com/jaakkopasanen/AutoEq/issues
 Author-email: Jaakko Pasanen <jaakko.o.pasanen@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: <3.10,>=3.7
 Requires-Dist: matplotlib~=3.5.2
 Requires-Dist: numpy~=1.23.1
 Requires-Dist: pandas~=1.4.3
 Requires-Dist: pillow~=9.2.0
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: scipy~=1.8.1
 Requires-Dist: soundfile~=0.11.0
@@ -29,14 +29,23 @@
 curves, apply tilt for making the headphones brighter/darker and adding a bass boost. It's even possible to make one
 headphone sound (roughly) like another headphone. For more info about usage see [Usage](#usage).
 
 AutoEq [Github page](https://github.com/jaakkopasanen/AutoEq) also serves as a database for headphone frequency response
 measurements, pre-computed results and has documentation about different equalizers and how the implementation works.
 
 ### Updates
+#### 3.0.0
+* Added `--input-file`, `--max-slope` and `--sound-signature-smoothing-window-size` parameters.
+* Fixed crashing with non-standard sized compensation and measurement data.
+* Fixed parametric eq optimizer producing filters outside of specified frequency range.
+* Fixed parametric eq optimizer crashing without any free optimizeable parameters.
+* Added defaul values for some args in parametric eq optimizer.
+* Added more parametric eq optimizer configs.
+* Introduced API breaking naming changes.
+
 #### 2.2.0
 Added `--preamp` parameter
 
 #### 2.1.1
 Fixed README in PyPi package
 
 #### 2.1.0
```

