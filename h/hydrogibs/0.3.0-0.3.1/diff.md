# Comparing `tmp/hydrogibs-0.3.0.tar.gz` & `tmp/hydrogibs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.0.tar", last modified: Sun Apr 30 23:00:36 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.1.tar", last modified: Sun May 14 17:16:03 2023, max compression
```

## Comparing `hydrogibs-0.3.0.tar` & `hydrogibs-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 23:00:36.424786 hydrogibs-0.3.0/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.0/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-30 23:00:36.424786 hydrogibs-0.3.0/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.0/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 23:00:36.420786 hydrogibs-0.3.0/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    12695 2023-04-30 22:49:03.000000 hydrogibs-0.3.0/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5125 2023-04-30 22:48:31.000000 hydrogibs-0.3.0/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.0/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     8711 2023-04-30 22:49:19.000000 hydrogibs-0.3.0/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.3.0/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.0/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.0/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.3.0/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 23:00:36.424786 hydrogibs-0.3.0/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-30 23:00:36.000000 hydrogibs-0.3.0/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-04-30 23:00:36.000000 hydrogibs-0.3.0/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-30 23:00:36.000000 hydrogibs-0.3.0/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-30 23:00:36.000000 hydrogibs-0.3.0/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-30 23:00:12.000000 hydrogibs-0.3.0/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-30 23:00:36.424786 hydrogibs-0.3.0/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.1/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.1/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.003904 hydrogibs-0.3.1/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    12664 2023-05-14 16:53:37.000000 hydrogibs-0.3.1/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5149 2023-05-14 16:38:39.000000 hydrogibs-0.3.1/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.1/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     8243 2023-05-14 16:42:20.000000 hydrogibs-0.3.1/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.1/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.1/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.1/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.1/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-14 17:15:52.000000 hydrogibs-0.3.1/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/setup.cfg
```

### Comparing `hydrogibs-0.3.0/LICENSE` & `hydrogibs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.0/PKG-INFO` & `hydrogibs-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # hydrogibs
 
 Baby hydrology package
```

### Comparing `hydrogibs-0.3.0/hydrogibs/GR4.py` & `hydrogibs-0.3.1/hydrogibs/GR4.py`

 * *Files 14% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
         self.colors = colors
         self.flows_margin = flows_margin
         self.rain_margin = rain_margin
 
         time = event.time
         rain = event.rainfall
-        dT = event.water_flow
+        V = event.volume
         Qp = event.discharge_rain
         Qv = event.discharge_volume
         Q = event.discharge
 
         with plt.style.context(style):
 
             c1, c2, c3, c4, c5 = self.colors
@@ -244,73 +244,73 @@
             ax1.set_yticks(yticks)
             ax1.set_yticklabels(yticks, color=c1)
 
             ax2 = ax1.twinx()
             lineP, = ax2.step(
                 time,
                 rain,
-                alpha=0.5,
+                lw=1.5,
                 color=c2,
                 label="Rainfall"
             )
             max_rain = rain.max()
             ax2.set_ylim(((1 + self.rain_margin) * max_rain, 0))
             ax2.grid(False)
             ax2.set_yticks((0, max_rain))
             ax2.set_yticklabels(ax2.get_yticklabels(), color=c2)
 
             ax3 = ax2.twinx()
-            lineT, = ax3.plot(time, dT, ":",
-                              color=c3, label="Water flow", lw=1.5)
-            ax3.set_ylabel("$\\dot{T}$ (mm/h)", color=c3)
+            lineV, = ax3.plot(time, V, ":",
+                              color=c3, label="Storage volume", lw=1.5)
+            ax3.set_ylabel("$V$ (mm)", color=c3)
             ax3.set_xlabel("$t$ (h)")
-            ax3.set_ylim((0, (1 + self.flows_margin) * dT.max()))
+            ax3.set_ylim((0, (1 + self.flows_margin) * V.max()))
             yticks = ax3.get_yticks()
             yticks = [
                 y for y in yticks
                 if y < max(yticks)/(1 + self.flows_margin)
             ]
             ax3.set_yticks(yticks)
             ax3.set_yticklabels(ax3.get_yticks(), color=c3)
             ax3.set_yscale("linear")
             ax3.grid(False)
 
-            lines = (lineP, lineQ, lineQp, lineQv, lineT)
+            lines = (lineP, lineQ, lineQp, lineQv, lineV)
             labs = [line.get_label() for line in lines]
             ax1.legend(lines, labs)
 
             plt.tight_layout()
 
             self.figure, self.axes, self.lines = fig, (ax1, ax2, ax3), lines
 
         if show:
             plt.show()
 
     def update(self, event):
 
         time = event.time
         rainfall = event.rainfall
-        rain, discharge, discharge_p, discharge_v, water_flow = self.lines
+        rain, discharge, discharge_p, discharge_v, storage_vol = self.lines
 
         discharge.set_data(time, event.discharge)
         discharge_p.set_data(time, event.discharge_rain)
         discharge_v.set_data(time, event.discharge_volume)
-        water_flow.set_data(time, event.water_flow)
+        storage_vol.set_data(time, event.volume)
         rain.set_data(time, rainfall)
 
     def zoom(self, canvas):
 
-        rain, discharge, _, _, water_flow = self.lines
+        rain, discharge, _, _, storage_vol = self.lines
         ax1, ax2, ax3 = self.axes
 
         t, Q = discharge.get_data()
         Qm = Q.max()
         Imax = rain.get_data()[1].max()
-        dT = water_flow.get_data()[1]
-        dTm = dT.max()
+        V = storage_vol.get_data()[1]
+        Vm = V.max()
 
         ax1.set_yscale("linear")
         ylim = Qm * (1 + self.flows_margin)
         ax1.set_ylim((0, ylim if ylim else 1))
         ax1.set_xlim((0, t.max()))
         yticks = [
             ytick for ytick in ax1.get_yticks()
@@ -321,24 +321,24 @@
 
         ax2.set_yscale("linear")
         ylim = Imax * (1 + self.rain_margin)
         ax2.set_ylim((ylim if ylim else 1, 0))
         ax2.set_yticks((0, Imax))
 
         ax3.set_yscale("linear")
-        ylim = dTm * (1 + self.flows_margin)
+        ylim = Vm * (1 + self.flows_margin)
         ax3.set_ylim((0, ylim if ylim else 1))
 
         plt.tight_layout()
         canvas.draw()
 
 
-def GR4app(catchment: Catchment = None,
-           rain: Rain = None,
-           *args, **kwargs):
+def App(catchment: Catchment = None,
+        rain: Rain = None,
+        *args, **kwargs):
     if catchment is None:
         catchment = Catchment(8/100, 40, 0.1, 1)
     if rain is None:
         rain = BlockRain(50, duration=1.8)
     entries = [
         ("catchment", "X1", "-"),
         ("catchment", "X2", "mm"),
@@ -412,12 +412,12 @@
         rainfall = np.full_like(time, 50)
         rainfall[(3 <= time) & (time <= 7) | (time >= 9)] = 0
         rain = Rain(
             time=time,
             rainfall=rainfall
         )
     # GR4h(Catchment(8/100, 40, 0.1, 1), rain).App()
-    GR4app(Catchment(8/100, 40, 0.1, 1), rain)
+    App(Catchment(8/100, 40, 0.1, 1), rain)
 
 
 if __name__ == "__main__":
     GR4_demo("block")
```

### Comparing `hydrogibs-0.3.0/hydrogibs/ModelApp.py` & `hydrogibs-0.3.1/hydrogibs/ModelApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,14 @@
     def update_attribute(self, object: str, key, value):
 
         if object == "catchment":
             setattr(self.catchment, key, value)
         elif object == "rain":
             setattr(self.rain, key, value)
         else:
-            raise KeyError(f"{key} not an attribute")
+            raise KeyError(f"{key} not an attribute ('catchment' or 'rain')")
 
     def update(self):
 
         event = self.rain @ self.catchment
         self.diagram.update(event)
         self.canvas.draw()
```

### Comparing `hydrogibs-0.3.0/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.1/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.0/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.1/hydrogibs/RationalMethod.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,13 +28,18 @@
         Qp * t/tc if t < tc else Qp * (2 - t/tc)
         for t in time
     ])
 
     return time, Q
 
 
-if __name__ == "__main__":
+def main():
     from matplotlib import pyplot as plt
     t, Q = rational_method(S=1, Cr=0.6, tc=1)
     plt.plot(t, Q)
     plt.xlabel("Time [h]")
     plt.ylabel("Flow [m$^3$/s]")
+    plt.show()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hydrogibs-0.3.0/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.1/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.0/hydrogibs/misc.py` & `hydrogibs-0.3.1/hydrogibs/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         Pj10 (float) [mm]: total daily rain with return period of 10 years
         R (float) [-]: regionnal coefficient, default to 1 if not specified
 
     Returns:
         Q10 (float): peak discharge flow for return period T = 10 years
     """
     if not 1.4 <= S <= 52*1000:
-        warn(f"\ncrupedix: Catchment area is not within recommended range: "
+        warn(f"\ncrupedix: Catchment area is not within recommended range:\n\t"
              f"{S:.3e} not in [1,4 * 10^3 km^2 - 52 * 10^3 km^2]")
     return R * S**0.8 * (Pj10/80)**2
 
 
 def zeller(montana_params: tuple,
            duration: float,
            vtime: float,  # TODO
```

### Comparing `hydrogibs-0.3.0/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.3.1/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # hydrogibs
 
 Baby hydrology package
```

