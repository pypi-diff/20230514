# Comparing `tmp/EclipsingBinaries-2.8.4a6.tar.gz` & `tmp/EclipsingBinaries-2.8.4a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a6.tar", last modified: Thu Apr 27 19:38:45 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a7.tar", last modified: Sun May 14 20:54:09 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a6.tar` & `EclipsingBinaries-2.8.4a7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:38:45.951466 EclipsingBinaries-2.8.4a6/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-04-27 19:38:15.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 19:38:45.000000 EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:38:45.955466 EclipsingBinaries-2.8.4a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-27 19:38:21.000000 EclipsingBinaries-2.8.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Kyle Koeller
 Created: 11/08/2022
-Last Edited: 04/17/2023
+Last Edited: 05/09/2023
 
 This program is meant to automatically do the data reduction of the raw images from the
 Ball State University Observatory (BSUO) and SARA data. The new calibrated images are placed into a new folder as to
 not overwrite the original images.
 """
 # import sys
 from pathlib import Path
@@ -46,36 +46,36 @@
 
     :return: outputs all calibration images into a new reduced folder designated by the user.
     """
 
     # allows the user to input where the raw images are and where the calibrated images go to
     path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the raw images are or type "
                  "the word 'Close' to leave: ")
-    # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration2"
+    # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration"
     if path.lower() == "close":
         exit()
     # path = "Calibration2"
     calibrated = input("Please enter a file pathway for a new calibrated folder to not overwrite the original images "
-                        "(C:\\folder1\\folder2\\[calibrated]): ")
+                       "(C:\\folder1\\folder2\\[calibrated]): ")
     # calibrated = "C:\\test"
     # checks whether the file paths from above are real
     while True:
         try:
             images_path = Path(path)
             calibrated_data = Path(calibrated)
             break
         except FileNotFoundError:
             print("Files were not found. Please try again.\n")
             path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
             calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
     print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
     while True:
-        # default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
-        default_ans = "default"
+        default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
+        # default_ans = "default"
         if default_ans.lower() == "default":
             break
         elif default_ans.lower() == "new":
             default()
             break
         else:
             print("Please either enter 'Default' or 'New'.\n")
@@ -139,29 +139,20 @@
     :return: depends on the stage of process, but will return a final image for each process
     """
 
     # subtract overscan, trims image, and gain corrects
     if overscan_region.lower() == "none":
         pass
     else:
-        new_ccd = ccdp.ccd_process(ccd, oscan=overscan_region, trim=trim_region, gain=gain * u.electron / u.adu,
-                                   readnoise=rdnoise * u.electron, error=False)
-        # ccd = ccdp.subtract_overscan(ccd, fits_section=overscan_region, median=True, overscan_axis=None)
-
-    # Subtract the overscan, ccd[columns, rows] I think?
-    # # Trim the overscan and gain correct the image
-    # while True:
-    #     try:
-    #         ccd = ccdp.trim_image(ccd, fits_section=trim_region)
-    #         break
-    #     except ValueError:
-    #         print("You have entered the wrong format for the Data Section. Please try again.\n")
-    #         trim_region = input("Please enter the data region. Example '[20:2060, 12:2057]': ")
-    #
-    # new_ccd = ccdp.gain_correct(ccd, gain=gain * u.electron / u.adu)  # gain correct the image
+        # new_ccd = ccdp.ccd_process(ccd, fits_section=overscan_region, trim=trim_region, gain=gain * u.electron / u.adu,
+        #                            readnoise=rdnoise * u.electron, error=False)
+        ccd = ccdp.subtract_overscan(ccd, fits_section=overscan_region, median=True, overscan_axis=None)
+
+    trim_ccd = ccdp.trim_image(ccd, fits_section=trim_region)
+    new_ccd = ccdp.gain_correct(trim_ccd, gain=gain * u.electron / u.adu)  # gain correct the image
 
     # this if statement checks whether the input is bias, dark, flat, or science reduction
     # bias combining
     if num == 0:
         return new_ccd
     # dark combining
     elif num == 1:
@@ -216,16 +207,17 @@
     """
 
     # plots one of the flat image mean count values across all columns to find the trim and overscan regions
     print("\n\nThe flat image that you enter next should be inside the " + "\033[1m" + "\033[93m" + "FIRST" +
           "\033[00m" + " folder that you entered above or this will crash.")
     while True:
         try:
-            image = input(
-                "Please enter the name of one of the flat image to be looked at for overscan and data regions: ")
+            # image = input(
+            #     "Please enter the name of one of the flat image to be looked at for overscan and data regions: ")
+            image = "Flat-Empty-B-Bin2-001-NoGEM.fts"
             cryo_path = Path(path)
             bias_1 = CCDData.read(cryo_path / image, unit='adu')
             break
         except FileNotFoundError:
             print("\nThe file you entered could not be found, please try entering " 
                   "\033[1m" + "\033[93m" + "JUST" + "\033[00m" + " the file name only.\n")
     # bias_1 = CCDData.read(cryo_path / 'bias-0001.fits', unit='adu')  # testing
@@ -246,15 +238,15 @@
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         new_ccd.write(calibrated_data / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_data, new_fname, "BIAS", "None", None, None, None)
+        add_header(calibrated_data, new_fname, "BIAS", "None", None, None, None, trim_region, overscan_region)
 
         # output that an image is finished for updates to the user
         print("Finished overscan correction for " + str(new_fname))
 
     print("\nFinished overscan correcting bias frames.")
     # combine all the output bias images into a master bias
     reduced_images = ccdp.ImageFileCollection(calibrated_data)
@@ -268,15 +260,15 @@
                                  mem_limit=mem_limit
                                  )
 
     fname = "zero.fits"
     combined_bias.meta['combined'] = True
     combined_bias.write(calibrated_data / fname, overwrite=overwrite)
 
-    add_header(calibrated_data, fname, "BIAS", "None", None, None, None)
+    add_header(calibrated_data, fname, "BIAS", "None", None, None, None, trim_region, overscan_region)
 
     print("\nFinished creating zero.fits\n")
 
     return combined_bias, overscan_region, trim_region
 
 
 def bias_plot(ccd):
@@ -292,15 +284,15 @@
     plt.axvline(x=2077, color='black', linewidth=2, linestyle='dashed', label='Suggested Start of Overscan')
     plt.legend()
     # plt.ylim(0, 60000)
     plt.xlim(-50, 2130)
     plt.xlabel('pixel number')
     plt.ylabel('Counts')
     # plt.title('Count Values for Row 1000')
-    plt.show()
+    # plt.show()
 
 
 def dark(files, zero, calibrated_path, overscan_region, trim_region):
     """
     Calibrates the dark frames.
 
     :param files: file location of raw images
@@ -318,15 +310,15 @@
         # new file name that uses the number from the original image
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         sub_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_path, new_fname, "DARK", "None", None, None, None)
+        add_header(calibrated_path, new_fname, "DARK", "None", None, None, None, trim_region, overscan_region)
 
         print("Finished overscan correction and bias subtraction for " + str(new_fname))
 
     print("\nFinished overscan correcting and bias subtracting all dark frames.")
     print("\nStarting combining dark frames.\n")
     time.sleep(10)
     reduced_images = ccdp.ImageFileCollection(calibrated_path)
@@ -340,15 +332,15 @@
                                  rdnoise=rdnoise * u.electron, gain=gain * u.electron / u.adu, mem_limit=mem_limit
                                  )
 
     fname = "master_dark.fits"
     combined_dark.meta['combined'] = True
     combined_dark.write(calibrated_path / fname, overwrite=overwrite)
 
-    add_header(calibrated_path, fname, "DARK", "None", None, None, None)
+    add_header(calibrated_path, fname, "DARK", "None", None, None, None, trim_region, overscan_region)
 
     print("Finished creating a master dark.\n")
     return combined_dark
 
 
 def flat(files, zero, combined_dark, calibrated_path, overscan_region, trim_region):
     """
@@ -371,15 +363,15 @@
         # new file name with the filter and number from the original file
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
 
         # Save the result
         final_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
-        add_header(calibrated_path, new_fname, "FLAT", "None", None, None, None)
+        add_header(calibrated_path, new_fname, "FLAT", "None", None, None, None, trim_region, overscan_region)
 
         print("Finished overscan correction, bias subtraction, and dark subtraction for " + str(new_fname))
 
     print("\nFinished overscan, bias subtracting, and dark subtracting of flat frames.\n")
     print("Starting flat combination.\n")
     time.sleep(10)
 
@@ -396,15 +388,15 @@
                                       )
 
         combined_flats.meta['combined'] = True
         flat_file_name = 'master_flat_{}.fits'.format(filt.replace("Empty/", ""))
 
         combined_flats.write(calibrated_path / flat_file_name, overwrite=overwrite)
 
-        add_header(calibrated_path, flat_file_name, "FLAT", "None", None, None, None)
+        add_header(calibrated_path, flat_file_name, "FLAT", "None", None, None, None, trim_region, overscan_region)
 
         print("Finished combining flat " + str(flat_file_name))
 
     print("\nFinished creating the master flats by filter.\n")
 
 
 def science_images(files, calibrated_data, zero, combined_dark, trim_region, overscan_region):
@@ -427,82 +419,76 @@
         all_reds.append(reduced)
         reduced.write(calibrated_data / new_fname, overwrite=overwrite)
 
         hjd = light.header["JD-HELIO"]
         ra = light.header["RA"]
         dec = light.header["DEC"]
 
-        add_header(calibrated_data, new_fname, science_imagetyp, "None", hjd, ra, dec)
+        add_header(calibrated_data, new_fname, science_imagetyp, "None", hjd, ra, dec, trim_region, overscan_region)
 
         print("Finished calibration of " + str(new_fname))
     print("\nFinished calibrating all science images.")
 
 
-def add_header(pathway, fname, imagetyp, filter_name, hjd, ra, dec):
+def add_header(pathway, fname, imagetyp, filter_name, hjd, ra, dec, trim_region, overscan_region):
     """
     Adds values to the header of each image reduced
 
+    :param overscan_region: BIASSEC for the header
+    :param trim_region: DATASEC for the header
     :param dec: declination of target object
     :param ra: right ascension of target object
     :param hjd: time of mid-exposure for each image
     :param pathway: pathway to the new file
     :param fname: file name
     :param imagetyp: image type (bias, flat, dark, light)
     :param filter_name: filter type (B, V, R)
     :return: None
     """
     # bias_image = get_pkg_data_filename(pathway + "\\" + fname)
     image_name = pathway / fname
     fits.setval(image_name, "GAIN", value=gain, comment="Units of e-/ADU")
     fits.setval(image_name, "RDNOISE", value=rdnoise, comment="UNits of e-")
-    fits.setval(image_name, "OBSERVAT", value=location, comment="Obs. loc.")
+    fits.setval(image_name, "OBSERVAT", value=location, comment="Obs. Loc.")
     fits.setval(image_name, "IMAGETYP", value=imagetyp, comment="Image type")
-    # BIASSEC
-    # DATASEC
-    # EPOCH
+    fits.setval(image_name, "DATASEC", value=trim_region, comment="Trim data section")
+    fits.setval(image_name, "BIASSEC", value=overscan_region, comment="Overscan section")
+    fits.setval(image_name, "EPOCH", value="J2000.0")
     # fits.setval(bias_image, "FILTER", value=filter_name)
     if imagetyp == "LIGHT":
-        bjd = BJD_TDB(hjd, location, ra, dec)
-        fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
+        if location.lower() == "bsuo":
+            # location of BSUO
+            obs_location = {
+                'lon': -85.411896,  # degrees
+                'lat': 40.199879,  # degrees
+                'elevation': 0.2873  # kilometers
+            }
+            bjd = BJD_TDB(hjd, obs_location, ra, dec)
+            fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
 
 
 def BJD_TDB(hjd, loc, ra, dec):
     """
     Converts HJD to BJD_TDB
 
     :param ra: right ascension of target object
     :param dec: declination of target object
     :param hjd: HJD time for the mid-exposure image
     :param loc: location of the observations
     :return: Newly calculated BJD_TDB that is light time corrected
     """
-    # Define the HJD time in JD format
-    hjd = hjd * u.day
-
-    # Convert HJD to TDB
-    if loc.lower() == "ctio" or loc.lower() == "kpno" or loc.lower() == "lapalma":
-        t = Time(hjd.value, format='jd', scale='utc', location=loc)
-        t = t.tdb
-        # obs_location = EarthLocation.from_geodetic(obs_longitude, obs_latitude, obs_height)
-    elif loc.lower() == "bsuo":
-        # Define the location of the Ball State University Observatory (BSUO)
-        obs_latitude = 40.199910 * u.deg  # lat of the BSUO site
-        obs_longitude = -85.411513 * u.deg  # long of the BSUO site
-        obs_height = 292 * u.m  # height above sea level of the BSUO site
-        obs_location = EarthLocation.from_geodetic(obs_longitude, obs_latitude, obs_height)
-        t = Time(hjd, format='jd', scale='utc', location=obs_location)
-        t = t.tdb
-    else:
-        pass
-
-    # Compute the light travel time from the target to the observer
-    coord = SkyCoord(ra=ra, dec=dec, unit=(u.h, u.deg), obstime=t, frame='icrs')
-
-    ltt = Time.light_travel_time(coord, obs_location, kind='barycentric')
-    bjd_corr = t + ltt
+    helio = Time(hjd, scale='utc', format='jd')
+    obs = EarthLocation.from_geodetic(loc["lon"], loc["lat"], loc["elevation"])
+    star = SkyCoord(ra, dec, unit=(u.hour, u.deg))
+    ltt = helio.light_travel_time(star, 'heliocentric', location=obs)
+    guess = helio - ltt
+    # if we assume guess is correct - how far is heliocentric time away from true value?
+    delta = (guess + guess.light_travel_time(star, 'heliocentric', obs)).jd - helio.jd
+    # apply this correction
+    guess -= delta * u.d
 
-    # bjd_tdb_time = t
-    return bjd_corr
+    ltt = guess.light_travel_time(star, 'barycentric', obs)
+    return guess.tdb + ltt
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/find_min.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created:  07/03/2021
 Original Author: Alec Neal
 
 Last Edits Done By: Kyle Koeller
-Last Edited: 03/03/2023
+Last Edited: 05/14/2023
 """
 
 # import vseq  # testing purposes
 from . import vseq_updated as vseq
 from os import environ, path
 import matplotlib.pyplot as plt
 import numpy as np
@@ -152,14 +152,15 @@
             T_kw = -b2 / (2 * a2)
     else:
         T_kw = -b / (2 * a)
     S_at_tkw, Z = calc_S(fracHJD, flux, T_kw, npairs=npairs)
     Z /= 2
     if need_error:
         if Z <= 1:
+            # print(Z)
             print('Too few observations!')
         sigt_kw = np.sqrt(S_at_tkw / (a * (Z - 1)))
 
         print('S(T_BF) =', paraS[0])
         print('S(T_KW) =', calc_S(fracHJD, flux, T_kw, npairs=npairs))
     else:
         sigt_kw = 1
@@ -438,14 +439,15 @@
 
     return 'Done'
 
 
 def press(event):
     global rb
     global lb
+    global day
     if event.key == "d":
         # right boundary line
         lb = lb
         rb = event.xdata
         plt.close()
         plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
@@ -455,21 +457,28 @@
         rb = rb
         plt.close()
         plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method="norm")
     elif event.key == "w":
         # writes to a file
         pass
-    elif event.key == "escape":
+    elif event.key == "escape" or event.key == "q":
         # exits the program
         exit()
-    elif event.key == "f":
-        pass
+    elif event.key == "n":
+        # goes to the next "day"
+        day += 1
+        plot_obs(["896797_B.txt"], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
+                 para_range=None, norm_method="norm")
+    elif event.key == "h":
+        print("\nPress 'a' for right boundary, 'd' for left boundary, 'n' for the next day, 'w' to write to a file, "
+              "or the 'ESC' or 'q' keys to close the figure.\n")
     else:
-        print("\nPress 'a' for right boundary, 'd' for left boundary, or the 'ESC' key to close the figure.\n")
+        print("\nPress 'a' for right boundary, 'd' for left boundary, 'n' for the next day, 'w' to write to a file, "
+              "or the 'ESC' or 'q' keys to close the figure.\n")
 
 
 def zoom_factory(ax, base_scale=2.):
     def zoom_fun(event):
         # get the current x and y limits
         cur_xlim = ax.get_xlim()
         cur_ylim = ax.get_ylim()
@@ -498,14 +507,22 @@
     fig.canvas.mpl_connect('scroll_event',zoom_fun)
 
     # return the function
     return zoom_fun
 
 
 def main():
+    """
+    Main function for the program. This function will ask the user for the number of filters they have, and then call
+    the appropriate function to plot the data with the appropriate number of filters.
+
+    Returns
+    -------
+
+    """
     num_filters = input("How many filters do you have (i.e. 1-3) or type 'Close' to close the program: ")
     print()
     if num_filters == '1':
         while True:
             filter1 = input("Please enter a complete file pathway to your data file (i.e. C:\\folder1\\folder2\\data.txt: ")
             if path.exists(filter1):
                 break
```

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/menu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,93 @@
 """
 The main program helps centralize all the other programs into one selection routine that can be run and call all
 other programs.
 Author: Kyle Koeller
 Created: 8/29/2022
-Last Updated: 04/05/2023
+Last Updated: 05/14/2023
 """
 
+import pandas as pd
+
 """
 # testing imports
 from tess_data_search import main as data_search
 from Night_Filters import main as night
 from apass import comparison_selector as comp_select
 from OConnell import main as oconnell
 from color_light_curve import color_gui as gui
 from IRAF_Reduction import main as IRAF
 from OC_plot import main as data_fit
-from gaia import main
+from gaia import target_star as gaia
+from find_min import main as find_min
 """
 from .tess_data_search import main as data_search
 from .Night_Filters import main as night
 from .apass import comparison_selector as comp_select
 from .OConnell import main as oconnell
 from .color_light_curve import color_gui as gui
 from .IRAF_Reduction import main as IRAF
 from .OC_plot import main as data_fit
 from .gaia import target_star as gaia
+from .find_min import main as find_min
 
 
 def main():
     print("If you need a description of what each option does, please refer to the README for this packages GitHub page"
-          " https://github.com/kjkoeller/Binary_Star_Research_Package")
+          " https://github.com/kjkoeller/EclipsingBinaries/")
     print("\nWhich program do you want to run?\n\n")
 
+    options = ["IRAF Reduction", "Find Minimum", "TESS Database Search/Download", "AIJ Comparison Star Selector",
+               "BSUO or SARA/TESS Night Filters", "O-C Plotting", "Gaia Search", "O'Connel Effect", "Color Light Curve",
+               "Close Program"]
+    numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+
+    total = pd.DataFrame({"Options": options,
+                          "Numbers": numbers})
+
     while True:
-        print(
-            "IRAF Reduction(1), TESS Database Search/Download(2), AIJ Comparison Star Selector(3), "
-            "BSUO or SARA/TESS Night Filters(4), O-C Plotting(5), Gaia Search(6), O'Connel Effect(7), "
-            "Color Light Curve(8), Close Program(9)\n")
+        print(total.to_string(index=False))
+        print()
         prompt = int(input("Please type out the number corresponding to the corresponding action: "))
-        if prompt == 2:
+        if prompt == 3:
             # tess data
             data_search()
-        elif prompt == 4:
+        elif prompt == 2:
+            # find minimum
+            find_min()
+        elif prompt == 5:
             # night filters for AIJ and TESS
             aij = input("BSUO/SARA or TESS or 'Go Back': ")
             if aij.lower() == "aij":
                 night(0)
             elif aij.lower() == "tess":
                 night(1)
             elif aij.lower() == "go back":
                 pass
             else:
                 print("\nYou did not enter AIJ or TESS please go back through the prompts again and enter AIJ or TESS.\n")
-        elif prompt == 3:
+        elif prompt == 4:
             # comparison finder
             comp_select()
-        elif prompt == 7:
+        elif prompt == 8:
             # o'connell effect
             oconnell()
-        elif prompt == 8:
+        elif prompt == 9:
             # color light curve
             gui(False)
         elif prompt == 1:
             # iraf reduction
             IRAF()
-        elif prompt == 5:
+        elif prompt == 6:
             # O-C plotting
             data_fit()
-        elif prompt == 9:
+        elif prompt == 10:
             # close program
             break
-        elif prompt == 6:
+        elif prompt == 7:
             gaia()
         else:
             print("\nYou have not entered any of the allowed entries, please try again.\n")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a6
+Version: 2.8.4a7
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,21 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
 
-A Python project for Ball State University's Variable Star Research Group. Check the wiki (https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+
+***
+
+## Sponsor
+
+If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
```

### Comparing `EclipsingBinaries-2.8.4a6/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 EclipsingBinaries/OConnell.py
 EclipsingBinaries/__init__.py
 EclipsingBinaries/apass.py
 EclipsingBinaries/color_light_curve.py
 EclipsingBinaries/find_min.py
 EclipsingBinaries/gaia.py
 EclipsingBinaries/menu.py
+EclipsingBinaries/multi_aperture_photometry.py
 EclipsingBinaries/tess_data_search.py
 EclipsingBinaries/tesscut.py
 EclipsingBinaries/vseq_updated.py
 EclipsingBinaries.egg-info/PKG-INFO
 EclipsingBinaries.egg-info/SOURCES.txt
 EclipsingBinaries.egg-info/dependency_links.txt
 EclipsingBinaries.egg-info/entry_points.txt
```

### Comparing `EclipsingBinaries-2.8.4a6/LICENSE` & `EclipsingBinaries-2.8.4a7/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a6/PKG-INFO` & `EclipsingBinaries-2.8.4a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a6
+Version: 2.8.4a7
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,21 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
 
-A Python project for Ball State University's Variable Star Research Group. Check the wiki (https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+
+***
+
+## Sponsor
+
+If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
```

### Comparing `EclipsingBinaries-2.8.4a6/README.md` & `EclipsingBinaries-2.8.4a7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
 
-A Python project for Ball State University's Variable Star Research Group. Check the wiki (https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+
+***
+
+## Sponsor
+
+If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
```

### Comparing `EclipsingBinaries-2.8.4a6/setup.py` & `EclipsingBinaries-2.8.4a7/setup.py`

 * *Files identical despite different names*

