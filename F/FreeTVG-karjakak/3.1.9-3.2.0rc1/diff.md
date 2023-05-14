# Comparing `tmp/FreeTVG-karjakak-3.1.9.tar.gz` & `tmp/FreeTVG-karjakak-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.1.9.tar", last modified: Tue Jan 10 15:44:45 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.0rc1.tar", last modified: Sun May 14 10:01:54 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.1.9.tar` & `FreeTVG-karjakak-3.2.0rc1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.535956 FreeTVG-karjakak-3.1.9/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.534245 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      426 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      118 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.1.9/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-10 15:44:45.536033 FreeTVG-karjakak-3.1.9/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.1.9/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.534966 FreeTVG-karjakak-3.1.9/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   158552 2023-01-06 16:19:56.000000 FreeTVG-karjakak-3.1.9/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   521169 2022-12-20 04:59:38.000000 FreeTVG-karjakak-3.1.9/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.1.9/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.535687 FreeTVG-karjakak-3.1.9/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.1.9/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.1.9/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     5637 2023-01-10 15:40:05.000000 FreeTVG-karjakak-3.1.9/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.1.9/TVG/utility/term.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.1.9/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      941 2023-01-10 15:44:45.536316 FreeTVG-karjakak-3.1.9/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.151575 FreeTVG-karjakak-3.2.0rc1/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.147400 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      483 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      118 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-14 10:01:54.151651 FreeTVG-karjakak-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.0rc1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.149397 FreeTVG-karjakak-3.2.0rc1/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   144471 2023-05-14 09:35:11.000000 FreeTVG-karjakak-3.2.0rc1/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.0rc1/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.0rc1/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.150027 FreeTVG-karjakak-3.2.0rc1/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.0rc1/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14763 2023-05-14 09:14:42.000000 FreeTVG-karjakak-3.2.0rc1/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.151347 FreeTVG-karjakak-3.2.0rc1/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/term.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      944 2023-05-14 10:01:54.151941 FreeTVG-karjakak-3.2.0rc1/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.1.9
+Version: 3.2.0rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.1.9/LICENSE.txt` & `FreeTVG-karjakak-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.9/PKG-INFO` & `FreeTVG-karjakak-3.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.1.9
+Version: 3.2.0rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.1.9/README.md` & `FreeTVG-karjakak-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.9/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.0rc1/TVG/FreeTVG.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,53 @@
 import string
 import sys
 from datetime import datetime as dt
 from functools import partial
 from itertools import islice
 from pathlib import Path
 from sys import platform
-from tkinter import *
-from tkinter import colorchooser, font, messagebox, simpledialog, ttk
+from tkinter import (
+    BROWSE,
+    DISABLED,
+    END,
+    GROOVE,
+    INSERT,
+    LEFT,
+    MULTIPLE,
+    NONE,
+    NORMAL,
+    RIGHT,
+    SEL_FIRST,
+    SEL_LAST,
+    TOP,
+    WORD,
+    Button,
+    E,
+    Entry,
+    Frame,
+    Label,
+    Listbox,
+    Message,
+    Tk,
+    Toplevel,
+    X,
+    colorchooser,
+    font,
+    messagebox,
+    simpledialog,
+    ttk,
+)
 
 import tomlkit
 from treeview import TreeView as tv
 from treeview.dbase import Datab as db
 
 from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excp, excpcls
 
+from .structure import Lay1, Lay2, Lay3, Lay4, Lay5, Lay6, Lay7, Lay8, Scribe
 from .utility.mdh import convhtml
 from .utility.RegMail import composemail, wrwords
 from .utility.term import ctlight
 
 __all__ = ["main"]
 
 
@@ -93,14 +123,30 @@
         if os.path.exists(gpath):
             with open(gpath, "rb") as geo:
                 gem = ast.literal_eval(geo.read().decode("utf-8"))
                 self.root.geometry(gem["geo"])
                 self.GEO = gem["geo"]
         del gpath
         del gem
+
+        # Variables for functions and other purposes
+        self.bt = {}
+        self.lock = False
+        self.unlock = True
+        self.store = None
+        self.editorsel = None
+        self.tpl = None
+        self.ai = None
+        self.ew = None
+
+        # Creating style "clam" style for TVG
+        self.stl = ttk.Style(self.root)
+        self.stl.theme_use("clam")
+
+        # All root bindings
         self.root.bind_all("<Control-f>", self.fcsent)
         self.root.bind_all("<Control-r>", self.fcsent)
         self.root.bind_all("<Control-t>", self.fcsent)
         self.root.bind_all("<Control-i>", self.fcsent)
         self.root.bind_all("<Control-w>", self.fcsent)
         self.root.bind_all("<Control-b>", self.fcsent)
         self.root.bind_all("<Control-l>", self.fcsent)
@@ -111,26 +157,14 @@
         self.root.bind_all("<Control-o>", self.fcsent)
         self.root.bind_all("<Control-p>", self.fcsent)
         self.root.bind_all("<Control-h>", self.fcsent)
         self.root.bind_all("<Control-a>", self.fcsent)
         self.root.bind_all("<Control-e>", self.fcsent)
         self.root.bind_all("<Shift-Up>", self.scru)
         self.root.bind_all("<Shift-Down>", self.scrd)
-        if self.plat.startswith("win"):
-            self.root.bind("<Control-Up>", self.fcsent)
-            self.root.bind("<Control-Down>", self.fcsent)
-            self.root.bind("<Control-Left>", self.fcsent)
-            self.root.bind("<Control-Right>", self.fcsent)
-            self.root.bind_all("<Control-n>", self.fcsent)
-        else:
-            self.root.bind_all("<Control-Shift-Up>", self.fcsent)
-            self.root.bind_all("<Control-Shift-Down>", self.fcsent)
-            self.root.bind_all("<Control-Shift-Left>", self.fcsent)
-            self.root.bind_all("<Control-Shift-Right>", self.fcsent)
-            self.root.bind_all("<Command-n>", self.fcsent)
         self.root.bind_all("<Control-y>", self.fcsent)
         self.root.bind_all("<Control-0>", self.fcsent)
         self.root.bind_all("<Control-minus>", self.fcsent)
         self.root.bind_all("<Control-Key-2>", self.lookup)
         self.root.bind_all("<Control-Key-3>", self.dattim)
         self.root.bind_all("<Control-Key-6>", self.fcsent)
         self.root.bind_all("<Control-Key-7>", self.fcsent)
@@ -144,21 +178,31 @@
         self.root.bind_all("<Control-Key-question>", self.fcsent)
         self.root.bind_all("<Shift-Return>", self.inenter)
         self.root.bind_all("<Control-Shift-F>", self.fcsent)
         self.root.bind_all("<Control-Shift-S>", self.fcsent)
         self.root.bind_all("<Control-Shift-U>", self.fcsent)
 
         if self.plat.startswith("win"):
+            self.root.bind("<Control-Up>", self.fcsent)
+            self.root.bind("<Control-Down>", self.fcsent)
+            self.root.bind("<Control-Left>", self.fcsent)
+            self.root.bind("<Control-Right>", self.fcsent)
+            self.root.bind_all("<Control-n>", self.fcsent)
             self.root.bind_all("<Control-Key-F1>", self.fcsent)
             self.root.bind_all("<Control-Key-F2>", self.fcsent)
             self.root.bind_all("<Control-Key-F3>", self.fcsent)
             self.root.bind_all("<Control-Key-F5>", self.configd)
             if self._addon:
                 self.root.bind_all("<Control-Key-F4>", self.exprsum)
         else:
+            self.root.bind_all("<Control-Shift-Up>", self.fcsent)
+            self.root.bind_all("<Control-Shift-Down>", self.fcsent)
+            self.root.bind_all("<Control-Shift-Left>", self.fcsent)
+            self.root.bind_all("<Control-Shift-Right>", self.fcsent)
+            self.root.bind_all("<Command-n>", self.fcsent)
             self.root.bind_all("<Key-F1>", self.fcsent)
             self.root.bind_all("<Key-F2>", self.fcsent)
             self.root.bind_all("<Key-F3>", self.fcsent)
             self.root.bind_all("<Key-F5>", self.configd)
             if self._addon:
                 self.root.bind_all("<Key-F4>", self.exprsum)
 
@@ -168,523 +212,199 @@
             self.root.bind_all("<Control-Key-5>", self.fcsent)
 
         self.root.bind_class("TButton", "<Enter>", self.ttip)
         self.root.bind_class("TButton", "<Leave>", self.leave)
         self.root.bind_class("TRadiobutton", "<Enter>", self.ttip)
         self.root.bind_class("TRadiobutton", "<Leave>", self.leave)
 
-        self.bt = {}
-        self.rb = StringVar()
-        self.lock = False
-        self.store = None
-        self.editorsel = None
-        self.stl = ttk.Style(self.root)
-        self.stl.theme_use("clam")
-        if self.plat.startswith("win"):
-            self.stl.map("Horizontal.TScrollbar", background=[("active", "#eeebe7")])
-            self.stl.map("Vertical.TScrollbar", background=[("active", "#eeebe7")])
-        else:
-            self.stl.element_create("My.Horizontal.Scrollbar.trough", "from", "default")
-            self.stl.layout(
-                "My.Horizontal.TScrollbar",
-                [
-                    (
-                        "My.Horizontal.Scrollbar.trough",
-                        {
-                            "children": [
-                                (
-                                    "Horizontal.Scrollbar.leftarrow",
-                                    {"side": "left", "sticky": ""},
-                                ),
-                                (
-                                    "Horizontal.Scrollbar.rightarrow",
-                                    {"side": "right", "sticky": ""},
-                                ),
-                                (
-                                    "Horizontal.Scrollbar.thumb",
-                                    {
-                                        "unit": "0",
-                                        "children": [
-                                            (
-                                                "Horizontal.Scrollbar.grip",
-                                                {"sticky": ""},
-                                            )
-                                        ],
-                                        "sticky": "nswe",
-                                    },
-                                ),
-                            ],
-                            "sticky": "we",
-                        },
-                    )
-                ],
-            )
-            self.stl.element_create("My.Vertical.Scrollbar.trough", "from", "default")
-            self.stl.layout(
-                "My.Vertical.TScrollbar",
-                [
-                    (
-                        "My.Vertical.Scrollbar.trough",
-                        {
-                            "children": [
-                                (
-                                    "Vertical.Scrollbar.uparrow",
-                                    {"side": "top", "sticky": ""},
-                                ),
-                                (
-                                    "Vertical.Scrollbar.downarrow",
-                                    {"side": "bottom", "sticky": ""},
-                                ),
-                                (
-                                    "Vertical.Scrollbar.thumb",
-                                    {
-                                        "unit": "0",
-                                        "children": [
-                                            ("Vertical.Scrollbar.grip", {"sticky": ""})
-                                        ],
-                                        "sticky": "nswe",
-                                    },
-                                ),
-                            ],
-                            "sticky": "ns",
-                        },
-                    )
-                ],
-            )
-            self.stl.map("My.Horizontal.TScrollbar", background=[("active", "#eeebe7")])
-            self.stl.map("My.Vertical.TScrollbar", background=[("active", "#eeebe7")])
-
         # 1st frame.
-        # Frame for label and Entry.
-        self.fframe = ttk.Frame(root)
-        self.fframe.pack(side=TOP, fill="x")
-        self.label = ttk.Label(self.fframe, text="Words")
-        self.label.pack(side=LEFT, pady=3, fill="x")
-        self.bt["label"] = self.label
-        self.entry = ttk.Entry(
-            self.fframe,
-            validate="focusin",
-            validatecommand=self.focus,
-            font="consolas 12",
-        )
-        self.entry.pack(side=LEFT, ipady=5, pady=(3, 1), fill="both", expand=1)
-        self.entry.config(state="disable")
-        self.bt["entry"] = self.entry
-
-        # 2nd frame in first frame.
-        # Frame for radios button.
-        self.frbt = ttk.Frame(self.fframe)
-        self.frbt.pack()
-        self.frrb = ttk.Frame(self.frbt)
-        self.frrb.pack(side=BOTTOM)
-        self.radio1 = ttk.Radiobutton(
-            self.frbt, text="parent", value="parent", var=self.rb, command=self.radiobut
-        )
-        self.radio1.pack(side=LEFT, anchor="w")
-        self.bt["radio1"] = self.radio1
-        self.radio2 = ttk.Radiobutton(
-            self.frbt, text="child", value="child", var=self.rb, command=self.radiobut
-        )
-        self.radio2.pack(side=RIGHT, anchor="w")
-        self.bt["radio2"] = self.radio2
+        # Frame for labels, Entry, radio-buttons and combobox.
+        self.fframe = Lay1(self.root)
+        self.bt["label"] = self.fframe.label
+        self.bt["entry"] = self.fframe.entry
+        self.bt["radio1"] = self.fframe.radio1
+        self.bt["radio2"] = self.fframe.radio2
+        self.bt["label3"] = self.fframe.label3
+        self.bt["entry3"] = self.fframe.entry3
 
-        # 3rd frame in 2nd frame.
-        # Frame for Child ComboBox
-        self.frcc = ttk.Frame(self.frrb)
-        self.frcc.pack(side=TOP)
-        self.label3 = ttk.Label(self.frcc, text="Child")
-        self.label3.pack(side=LEFT, padx=1, pady=(0, 1), fill="x")
-        self.bt["label3"] = self.label3
-        self.entry3 = ttk.Combobox(
-            self.frcc,
-            width=8,
-            exportselection=False,
-            state="readonly",
-            justify="center",
-        )
-        self.entry3.pack(side=LEFT, padx=1, pady=(0, 1), fill="x")
-        self.bt["entry3"] = self.entry3
-
-        # 3rd frame for top buttons.
+        # 2nd frame.
         # Frame for first row Buttons.
-        self.bframe = ttk.Frame(self.root)
-        self.bframe.pack(side=TOP, fill="x")
-        self.button5 = ttk.Button(
-            self.bframe, text="Insert", width=1, command=self.insertwords
-        )
-        self.button5.pack(side=LEFT, pady=(2, 3), padx=(1, 1), fill="x", expand=1)
-        self.button5.propagate(0)
-        self.bt["button5"] = self.button5
-        self.button6 = ttk.Button(
-            self.bframe, text="Write", width=1, command=self.writefile
-        )
-        self.button6.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button6"] = self.button6
-        self.button9 = ttk.Button(
-            self.bframe, text="Delete", width=1, command=self.deleterow
-        )
-        self.button9.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button9"] = self.button9
-        self.button7 = ttk.Button(
-            self.bframe, text="BackUp", width=1, command=self.backup
-        )
-        self.button7.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button7"] = self.button7
-        self.button8 = ttk.Button(
-            self.bframe, text="Load", width=1, command=self.loadbkp
-        )
-        self.button8.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button8"] = self.button8
-        self.button3 = ttk.Button(
-            self.bframe, text="Move Child", width=1, command=self.move_lr
-        )
-        self.button3.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button3"] = self.button3
-        self.button16 = ttk.Button(
-            self.bframe, text="Change File", width=1, command=self.chgfile
-        )
-        self.button16.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button16"] = self.button16
-        self.button33 = ttk.Button(
-            self.bframe, text="Fold Childs", width=1, command=self.fold_childs
-        )
-        self.button33.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button33"] = self.button33
-        self.button17 = ttk.Button(
-            self.bframe, text="CPP", width=1, command=self.cmrows
-        )
-        self.button17.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button17"] = self.button17
+        self.bframe = Lay2(self.root)
+        self.bt["Insert"] = self.bframe.button5
+        self.bt["Insert"].configure(command=self.insertwords)
+        self.bt["Write"] = self.bframe.button6
+        self.bt["Write"].configure(command=self.writefile)
+        self.bt["Delete"] = self.bframe.button9
+        self.bt["Delete"].configure(command=self.deleterow)
+        self.bt["BackUp"] = self.bframe.button7
+        self.bt["BackUp"].configure(command=self.backup)
+        self.bt["Load"] = self.bframe.button8
+        self.bt["Load"].configure(command=self.loadbkp)
+        self.bt["Move Child"] = self.bframe.button3
+        self.bt["Move Child"].configure(command=self.move_lr)
+        self.bt["Change File"] = self.bframe.button16
+        self.bt["Change File"].configure(command=self.chgfile)
+        self.bt["Fold Childs"] = self.bframe.button33
+        self.bt["Fold Childs"].configure(command=self.fold_childs)
+        self.bt["CPP"] = self.bframe.button17
+        self.bt["CPP"].configure(command=self.cmrows)
 
-        # 4th frame for below buttons.
+        # 3rd frame.
         # Frame for second row buttons.
-        self.frb1 = ttk.Frame(self.root)
-        self.frb1.pack(fill=X)
-        self.button10 = ttk.Button(
-            self.frb1, text="Insight", width=1, command=self.insight
-        )
-        self.button10.pack(side=LEFT, pady=(0, 3), padx=(1, 1), fill="x", expand=1)
-        self.bt["button10"] = self.button10
-        self.button13 = ttk.Button(
-            self.frb1, text="Arrange", width=1, command=self.spaces
-        )
-        self.button13.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button13"] = self.button13
-        self.button11 = ttk.Button(self.frb1, text="Paste", width=1, command=self.copas)
-        self.button11.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button11"] = self.button11
-        self.button4 = ttk.Button(
-            self.frb1, text="Checked", width=1, command=self.checked
-        )
-        self.button4.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button4"] = self.button4
-        self.button = ttk.Button(self.frb1, text="Up", width=1, command=self.moveup)
-        self.button.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button"] = self.button
-        self.button2 = ttk.Button(
-            self.frb1, text="Down", width=1, command=self.movedown
-        )
-        self.button2.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button2"] = self.button2
-        self.button14 = ttk.Button(
-            self.frb1, text="Hide Parent", width=1, command=self.hiddenchl
-        )
-        self.button14.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button14"] = self.button14
-        self.button34 = ttk.Button(
-            self.frb1, text="Fold selected", width=1, command=self.fold_selected
-        )
-        self.button34.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button34"] = self.button34
-        self.button15 = ttk.Button(
-            self.frb1, text="Clear hide", width=1, command=self.delhid
-        )
-        self.button15.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-        self.bt["button15"] = self.button15
+        self.frb1 = Lay3(self.root)
+        self.bt["Insight"] = self.frb1.button10
+        self.bt["Insight"].configure(command=self.insight)
+        self.bt["Arrange"] = self.frb1.button13
+        self.bt["Arrange"].configure(command=self.spaces)
+        self.bt["Paste"] = self.frb1.button11
+        self.bt["Paste"].configure(command=self.copas)
+        self.bt["Checked"] = self.frb1.button4
+        self.bt["Checked"].configure(command=self.checked)
+        self.bt["Up"] = self.frb1.button
+        self.bt["Up"].configure(command=self.moveup)
+        self.bt["Down"] = self.frb1.button2
+        self.bt["Down"].configure(command=self.movedown)
+        self.bt["Hide Parent"] = self.frb1.button14
+        self.bt["Hide Parent"].configure(command=self.hiddenchl)
+        self.bt["Fold selected"] = self.frb1.button34
+        self.bt["Fold selected"].configure(command=self.fold_selected)
+        self.bt["Clear hide"] = self.frb1.button15
+        self.bt["Clear hide"].configure(command=self.delhid)
 
-        # 7th Frame
+        # 4th Frame
         # For third row  of buttons
-        self.frb2 = ttk.Frame(self.root)
-        self.frb2.pack(fill=X)
-        self.button23 = ttk.Button(
-            self.frb2, text="Create file", width=1, command=self.createf
-        )
-        self.button23.pack(side=LEFT, pady=(0, 2), padx=(1, 1), fill="x", expand=1)
-        self.bt["button23"] = self.button23
-        self.button24 = ttk.Button(
-            self.frb2, text="Editor", width=1, command=self.editor
-        )
-        self.button24.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button24"] = self.button24
-        self.button25 = ttk.Button(
-            self.frb2, text="Un/Wrap", width=1, command=self.wrapped
-        )
-        self.button25.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button25"] = self.button25
-        self.button27 = ttk.Button(self.frb2, text="Ex", width=1, command=self.editex)
-        self.button27.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button27"] = self.button27
-        self.button28 = ttk.Button(
-            self.frb2, text="Template", width=1, command=self.temp
-        )
-        self.button28.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button28"] = self.button28
-        self.button20 = ttk.Button(
-            self.frb2, text="Date-Time", width=1, command=self.dattim
-        )
-        self.button20.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button20"] = self.button20
-        self.button19 = ttk.Button(
-            self.frb2, text="Look Up", width=1, command=self.lookup
-        )
-        self.button19.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button19"] = self.button19
-        self.button35 = ttk.Button(
-            self.frb2, text="Unfold", width=1, command=self.unfolding
-        )
-        self.button35.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button35"] = self.button35
-        self.button12 = ttk.Button(
-            self.frb2, text="Printing", width=1, command=self.saveaspdf
-        )
-        self.button12.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-        self.bt["button12"] = self.button12
-
-        self.frb3 = ttk.Frame(self.root)
-        self.frb3.pack(fill=X)
-        self.frb3.pack_forget()
+        self.frb2 = Lay4(self.root)
+        self.bt["Create file"] = self.frb2.button23
+        self.bt["Create file"].configure(command=self.createf)
+        self.bt["Editor"] = self.frb2.button24
+        self.bt["Editor"].configure(command=self.editor)
+        self.bt["Un/Wrap"] = self.frb2.button25
+        self.bt["Un/Wrap"].configure(command=self.wrapped)
+        self.bt["Ex"] = self.frb2.button27
+        self.bt["Ex"].configure(command=self.editex)
+        self.bt["Template"] = self.frb2.button28
+        self.bt["Template"].configure(command=self.temp)
+        self.bt["Date-Time"] = self.frb2.button20
+        self.bt["Date-Time"].configure(command=self.dattim)
+        self.bt["Look Up"] = self.frb2.button19
+        self.bt["Look Up"].configure(command=self.lookup)
+        self.bt["Unfold"] = self.frb2.button35
+        self.bt["Unfold"].configure(command=self.unfolding)
+        self.bt["Printing"] = self.frb2.button12
+        self.bt["Printing"].configure(command=self.saveaspdf)
+
+        # 5th Frame
+        # For MD buttons in editor
+        self.frb3 = Lay5(self.root)
 
+        # 6th Frame
+        # For addon buttons
         if self._addon:
-            self.button30 = ttk.Button(
-                self.bframe, text="Sum-Up", width=1, command=self.gettotsum
-            )
-            self.button30.pack(side=LEFT, pady=(2, 3), padx=(0, 1), fill="x", expand=1)
-            self.bt["button30"] = self.button30
-            self.button31 = ttk.Button(
-                self.frb1, text="Pie-Chart", width=1, command=self.createpg
-            )
-            self.button31.pack(side=LEFT, pady=(0, 3), padx=(0, 1), fill="x", expand=1)
-            self.bt["button31"] = self.button31
-            self.button32 = ttk.Button(
-                self.frb2, text="Del Total", width=1, command=self.deltots
-            )
-            self.button32.pack(side=LEFT, pady=(0, 2), padx=(0, 1), fill="x", expand=1)
-            self.bt["button32"] = self.button32
+            self.addonb = Lay6(self.bframe, self.frb1, self.frb2)
+            self.bt["Sum-Up"] = self.addonb.button30
+            self.bt["Sum-Up"].configure(command=self.gettotsum)
+            self.bt["Pie-Chart"] = self.addonb.button31
+            self.bt["Pie-Chart"].configure(command=self.createpg)
+            self.bt["Del Total"] = self.addonb.button32
+            self.bt["Del Total"].configure(command=self.deltots)
 
-        self.stl.configure(
-            "TButton",
-            font="verdana 7 bold" if self.plat.startswith("win") else "verdana 8 bold",
-        )
-
-        # 5th frame.
+        # 7th frame.
         # Frame for text, listbox and scrollbars.
-        frw = int(round(self.root.winfo_screenwidth() * 0.9224011713030746))
-        lbw = int(round(frw * 0.09285714285714286))
-        scw = int(round(frw * 0.011904761904761904))
-        ftt = "verdana 11"
-        self.tframe = ttk.Frame(root)
-        self.tframe.pack(anchor="w", side=TOP, fill="both", expand=1)
-        self.txframe = ttk.Frame(self.tframe)
-        self.txframe.pack(anchor="w", side=LEFT, fill="both", expand=1)
-        self.txframe.pack_propagate(0)
-        self.text = Text(
-            self.txframe,
-            font=ftt,
-            padx=5,
-            pady=3,
-            wrap=self.wrapping,
-            undo=True,
-            autoseparators=True,
-            maxundo=-1,
-        )
-        self.text.config(state="disable")
-        self.text.pack(side=LEFT, fill="both", padx=(2, 1), pady=(1, 0), expand=1)
+        self.tframe = Lay7(self.root)
+        self.text = self.tframe.text
+        self.text.configure(wrap=self.wrapping)
         self.text.bind("<MouseWheel>", self.mscrt)
         if self.plat.startswith("win"):
             self.text.bind("<Control-z>", self.undo)
             self.text.bind("<Control-Shift-Key-Z>", self.redo)
         else:
             self.text.bind("<Command-z>", self.undo)
             self.text.bind("<Command-y>", self.redo)
-        self.text.pack_propagate(0)
         self.bt["text"] = self.text
-        self.sc1frame = ttk.Frame(self.tframe, width=scw - 1)
-        self.sc1frame.pack(anchor="w", side=LEFT, fill="y", pady=1)
-        self.sc1frame.pack_propagate(0)
-        if self.plat.startswith("win"):
-            self.scrollbar1 = ttk.Scrollbar(self.sc1frame, orient="vertical")
-        else:
-            self.scrollbar1 = ttk.Scrollbar(
-                self.sc1frame, orient="vertical", style="My.Vertical.TScrollbar"
-            )
-        self.scrollbar1.config(command=self.text.yview)
-        self.scrollbar1.pack(side="left", fill="y")
+
+        self.scrollbar1 = self.tframe.scrollbar1
         self.scrollbar1.bind("<ButtonRelease>", self.mscrt)
-        self.text.config(yscrollcommand=self.scrollbar1.set)
         self.bt["scrollbar1"] = self.scrollbar1
-        self.tlframe = ttk.Frame(self.tframe, width=lbw)
-        self.tlframe.pack(anchor="w", side=LEFT, fill="y")
-        self.tlframe.pack_propagate(0)
-        self.listb = Listbox(self.tlframe, font=ftt, exportselection=False)
-        self.listb.pack(side=LEFT, fill="both", expand=1)
-        self.listb.pack_propagate(0)
-        self.bt["listb"] = self.listb
-        self.sc2frame = ttk.Frame(self.tframe, width=scw)
-        self.sc2frame.pack(anchor="w", side=LEFT, fill="y", pady=1)
-        self.sc2frame.pack_propagate(0)
-        if self.plat.startswith("win"):
-            self.scrollbar2 = ttk.Scrollbar(self.sc2frame, orient="vertical")
-        else:
-            self.scrollbar2 = ttk.Scrollbar(
-                self.sc2frame, orient="vertical", style="My.Vertical.TScrollbar"
-            )
-        self.scrollbar2.config(command=self.listb.yview)
-        self.scrollbar2.pack(side="left", fill="y")
-        self.scrollbar2.bind("<ButtonRelease>", self.mscrl)
-        self.listb.config(yscrollcommand=self.scrollbar2.set)
+
+        self.listb = self.tframe.listb
         self.listb.bind("<<ListboxSelect>>", self.infobar)
         self.listb.bind("<MouseWheel>", self.mscrl)
         self.listb.bind("<Up>", self.mscrl)
         self.listb.bind("<Down>", self.mscrl)
         self.listb.bind("<FocusIn>", self.flb)
+        self.bt["listb"] = self.listb
+
+        self.scrollbar2 = self.tframe.scrollbar2
+        self.scrollbar2.bind("<ButtonRelease>", self.mscrl)
         self.bt["scrollbar2"] = self.scrollbar2
 
-        # 6th frame.
+        # 8th frame.
         # Frame for horizontal scrollbar and info label.
-        self.fscr = ttk.Frame(self.root)
-        self.fscr.pack(fill="x")
-        self.frsc = ttk.Frame(self.fscr, height=scw + 1)
-        self.frsc.pack(side=LEFT, fill="x", padx=(2, 1), expand=1)
-        self.frsc.propagate(0)
-        if self.plat.startswith("win"):
-            self.scrolh = ttk.Scrollbar(self.frsc, orient="horizontal")
-        else:
-            self.scrolh = ttk.Scrollbar(
-                self.frsc, orient="horizontal", style="My.Horizontal.TScrollbar"
-            )
-        self.scrolh.pack(side=LEFT, fill="x", expand=1)
+        self.fscr = Lay8(self.root)
+        self.scrolh = self.fscr.scrolh
         self.scrolh.config(command=self.text.xview)
-        self.scrolh.propagate(0)
         self.text.config(xscrollcommand=self.scrolh.set)
-        self.info = StringVar()
-        self.info.set(f'{dt.strftime(dt.today(),"%a %d %b %Y")}')
-        self.frlab = ttk.Frame(self.fscr, width=lbw + (scw * 2), height=scw)
-        self.frlab.pack(side=LEFT, fill="x")
-        self.frlab.propagate(0)
-        self.labcor = Label(
-            self.frlab, textvariable=self.info, font="consolas 10 bold", justify=CENTER
-        )
-        self.labcor.pack(side=LEFT, fill="x", expand=1)
-        self.labcor.propagate(0)
-        self.unlock = True
-
-        if os.path.exists(self.glop.joinpath(self.glop.parent, "ft.tvg")):
-            self.ft(path=self.glop.joinpath(self.glop.parent, "ft.tvg"))
 
-        if os.path.exists(self.glop.joinpath(self.glop.parent, "theme.tvg")):
-            self.txtcol(
-                path=self.glop.joinpath(self.glop.parent, "theme.tvg"), wr=False
-            )
-
-        if os.path.isfile(self.glop.joinpath(self.glop.parent, "hbts.tvg")):
-            frm = [self.bframe, self.frb1, self.frb2]
-            for fr in frm:
-                fr.pack_forget()
-            del frm
-
-        if os.path.exists(self.glop.absolute().joinpath("fold.tvg")):
-            self.fold = True
-
-        self.ldmode()
-
-        self.tpl = None
-        self.ai = None
-        self.scribe = {
-            "Insert": "Insert word in outline on selected row",
-            "Write": "Write word to outline base on chosen as parent or child",
-            "Delete": "Delete an outline row",
-            "BackUp": "Backup outline note [max 10 and recycle]",
-            "Load": "Load a backuped note",
-            "Move Child": "Move a child base note to left or right",
-            "Change File": "Change to another existing file",
-            "CPP": "Copy or move selected outline rows",
-            "Send Note": "Switch to TeleTVG for sending note or chat",
-            "Look Up": "Look up word in outline list and in Editor mode",
-            "Insight": "Details about outline position rows",
-            "Arrange": "Clear selected row and arrange outline internally",
-            "Paste": "Paste selected row to word for editing",
-            "Checked": 'Insert "Check mark" or "Done" in selected row ',
-            "Up": "Move selected row up",
-            "Down": "Move selected row down",
-            "Printing": "Create html page for printing",
-            "Hide Parent": "Hiding parent and its childs or reverse",
-            "Clear hide": "Clearing hidden back to appearing again",
-            "Date-Time": "Insert time-stamp in Word and Editor mode",
-            "Save": "Save note as encrypted text and can be send",
-            "Open": "Open the encrypted TVG text file and can be saved",
-            "Create file": "Create new empty note",
-            "Editor": "To create outline note without restriction with proper format",
-            "Un/Wrap": "Wrap or unwrap outline note",
-            "Calculator": "Switch to calculator",
-            "Ex": "Edit whole notes or selected parent in Editor mode",
-            "Template": "Create template for use frequently in Editor mode",
-            "Emoji": "Insert emoji to note",
-            "HTML View": "Viewing html page that has been created before",
-            "parent": "Create parent",
-            "child": 'Create child ["Child" for positioning]',
-            "B": "Bold for Markdown",
-            "I": "Italic for Markdown",
-            "U": "Underline for Markdown",
-            "S": "Strikethrough for Markdown",
-            "M": "Marking highlight for markdown",
-            "SA": "Special attribute for markdown",
-            "L": "Link url for Markdown",
-            "SP": "Super-script for Markdown",
-            "SB": "Sub-script for Markdown",
-            "C": "Checked for Markdown",
-            "AR": "Arrow-right for Markdown",
-            "AL": "Arrow-left for Markdown",
-            "AT": "Arrow-right-left for Markdown",
-            "PM": "Plus-Minus for Markdown",
-            "TM": "Trade Mark for Markdown",
-            "CR": "Copy-Right for Markdown",
-            "R": "Right for Markdown",
-            "Fold Childs": "Folding all childs",
-            "Fold selected": "Folding selected rows",
-            "Unfold": "Unfolding selected or all childs",
-        }
+        self.info = self.fscr.info
+        self.info.set(f'{dt.strftime(dt.today(),"%a %d %b %Y")}')
 
-        self.ew = None
+        # Creating tool-tip for all buttons and radio-buttons
+        self.scribe = Scribe().scribe()
         if self._addon:
             on = {
                 "Sum-Up": "Summing all add-on",
                 "Pie-Chart": "Graph base on all sums",
                 "Del Total": "Delete all totals",
             }
             self.scribe = self.scribe | on
             self.ew = list(on) + ["child", "R"]
             if os.path.exists(self.glop.absolute().joinpath("sumtot.tvg")):
                 self.sumtot = True
                 os.remove(self.glop.absolute().joinpath("sumtot.tvg"))
         else:
             self.ew = ["CPP", "Clear hide", "Printing", "child", "R"]
-        self.rsv_frame = None
 
+        # cheking existing paths for early configuration on TVG
+        if os.path.exists(self.glop.joinpath(self.glop.parent, "ft.tvg")):
+            self.ft(path=self.glop.joinpath(self.glop.parent, "ft.tvg"))
+        if os.path.exists(self.glop.joinpath(self.glop.parent, "theme.tvg")):
+            self.txtcol(
+                path=self.glop.joinpath(self.glop.parent, "theme.tvg"), wr=False
+            )
+        if os.path.isfile(self.glop.joinpath(self.glop.parent, "hbts.tvg")):
+            frm = [self.bframe, self.frb1, self.frb2]
+            for fr in frm:
+                fr.pack_forget()
+            del frm
+        if os.path.exists(self.glop.absolute().joinpath("fold.tvg")):
+            self.fold = True
+        if not self.glop.parent.joinpath("TVG_config.toml").exists():
+            _create_config(self.glop.parent.joinpath("TVG_config.toml"))
+
+        # Last touch configuration for font in buttons,
+        # and for creating font-chooser that callable in a function
+        self.stl.configure(
+            "TButton",
+            font="verdana 7 bold" if self.plat.startswith("win") else "verdana 8 bold",
+        )
         self.root.tk.call(
             "tk",
             "fontchooser",
             "configure",
             "-font",
             self.text["font"],
             "-command",
             self.root.register(self.clb),
             "-parent",
             self.root,
         )
 
+        # Checking theme mode!
+        self.ldmode()
+
     def ldmode(self):
         """Dark mode for easing the eye"""
 
         oribg = "#dcdad5"
         chbg = "grey30"
         orifg = "black"
         chfg = "white"
@@ -716,63 +436,30 @@
             )
             self.stl.map(
                 "Vertical.TScrollbar",
                 background=[("active", "gold")],
                 arrowcolor=[("active", "black")],
             )
             self.stl.configure("TEntry", fieldbackground=chbg)
-            self.labcor.config(bg=chbg, fg=chfg)
-            if str(self.text.cget("background")) == "SystemWindow":
+            if self.text.cget("background") == "SystemWindow":
                 with open(
                     self.glop.joinpath(self.glop.parent, "theme.tvg"), "w"
                 ) as thm:
                     thm.write("#4d4d4d")
                 self.txtcol(
                     path=self.glop.joinpath(self.glop.parent, "theme.tvg"), wr=False
                 )
             del oribg, chbg, orifg, chfg
         elif self.tmode == "light":
-            self.stl.configure(
-                ".",
-                background=oribg,
-                foreground=orifg,
-                fieldbackground=oribg,
-                insertcolor=orifg,
-                troughcolor=oribg,
-                arrowcolor=orifg,
-                bordercolor=oribg,
-            )
-            self.stl.configure("TEntry", fieldbackground="white")
-            self.stl.map(
-                "TCombobox",
-                fieldbackground=[
-                    ("focus", "dark blue"),
-                    ("readonly", oribg),
-                    ("disabled", "white"),
-                ],
-                background=[("active", "#eeebe7")],
-            )
-            self.stl.map("Horizontal.TScrollbar", background=[("active", "#eeebe7")])
-            self.stl.map("Vertical.TScrollbar", background=[("active", "#eeebe7")])
-            self.labcor.config(bg="White", fg=orifg)
-            del oribg, chbg, orifg, chfg
+            self.stl.theme_use("clam")
 
     def ttip(self, event=None):
         """Tooltip for TVG buttons"""
 
-        ckframe = (
-            ".!frame.!frame",
-            ".!frame2",
-            ".!frame3",
-            ".!frame4",
-            self.rsv_frame,
-        )
-        if event.widget.winfo_parent() in ckframe and (
-            tx := self.scribe.get(event.widget["text"], None)
-        ):
+        if tx := self.scribe.get(event.widget["text"], None):
 
             def exit():
                 self.root.update()
                 self.ai = None
                 self.tpl = None
                 master.destroy()
 
@@ -886,17 +573,17 @@
     def infobar(self, event=None):
         """Info Bar telling the selected rows in listbox.
         If nothing, it will display today's date.
         """
 
         if os.path.exists(f"{self.filename}_hid.json"):
             self.info.set("Hidden Mode")
-        elif self.FREEZE and str(self.bt["button17"]["state"]) == "normal":
+        elif self.FREEZE and str(self.bt["CPP"]["state"]) == "normal":
             self.info.set("CPP Mode")
-        elif self.FREEZE and str(self.bt["button24"]["state"]) == "normal":
+        elif self.FREEZE and str(self.bt["Editor"]["state"]) == "normal":
             self.info.set("Editor Mode")
         elif self.listb.curselection():
             st = int(self.listb.curselection()[0])
             insight = None
             with tv(f"{self.filename}") as tvg:
                 insight = tuple(islice(tvg.compdatch(True), st, st + 1))
                 ck = insight[0][1][:12]
@@ -951,17 +638,17 @@
 
     def fcsent(self, event=None):
         """Key Bindings to keyboards"""
 
         fcom = str(self.root.focus_get())
         if self.FREEZE is False:
             if event.keysym == "f":
-                self.entry.focus()
+                self.bt["entry"].focus()
             elif event.keysym == "r":
-                self.entry3.focus()
+                self.bt["entry3"].focus()
             elif event.keysym == "t":
                 st = self.listb.curselection()
                 if st:
                     self.listb.focus()
                     self.listb.activate(int(st[0]))
                     self.listb.see(int(st[0]))
                     self.text.yview_moveto(self.listb.yview()[0])
@@ -986,20 +673,20 @@
             elif event.keysym == "o":
                 self.movedown()
             elif event.keysym == "p":
                 self.saveaspdf()
             elif event.keysym == "h":
                 self.hiddenchl()
             elif event.keysym == "a":
-                if self.rb.get() == "parent":
-                    self.rb.set("child")
-                    self.radiobut()
+                if self.fframe.rb.get() == "parent":
+                    self.fframe.rb.set("child")
+                    self.fframe.radiobut()
                 else:
-                    self.rb.set("parent")
-                    self.radiobut()
+                    self.fframe.rb.set("parent")
+                    self.fframe.radiobut()
             elif event.keysym == "e":
                 self.copas()
             elif event.keysym == "y":
                 self.checked()
             elif event.keysym == "0":
                 self.spaces()
             elif event.keysym == "minus":
@@ -1050,81 +737,37 @@
                 self.fold_childs()
             elif event.keysym == "U":
                 self.unfolding()
             elif event.keysym == "S":
                 self.fold_selected()
         else:
             if self.lock is False:
-                if str(self.bt["button17"].cget("state")) == "normal":
+                if str(self.bt["CPP"].cget("state")) == "normal":
                     if event.keysym == "n":
                         self.cmrows()
                     elif event.keysym == "s":
                         self.insight()
-                elif str(self.bt["button14"].cget("state")) == "normal":
+                elif str(self.bt["Hide Parent"].cget("state")) == "normal":
                     if event.keysym == "h":
                         self.hiddenchl()
                     elif event.keysym == "s":
                         self.insight()
                 elif (
-                    str(self.bt["button24"].cget("state")) == "normal"
+                    str(self.bt["Editor"].cget("state")) == "normal"
                     and event.keysym == "7"
                 ):
                     self.editor()
-                elif str(self.bt["button34"].cget("state")) == "normal":
+                elif str(self.bt["Fold selected"].cget("state")) == "normal":
                     if event.keysym == "S":
                         self.fold_selected()
                     elif event.keysym == "s":
                         self.insight()
 
         del fcom
 
-    def radiobut(self, event=None):
-        """These are the switches on radio buttons, to apply certain rule on child"""
-
-        case = {"": self.rb.get(), "child": "child", "parent": "parent"}
-        self.entry.config(state="normal")
-        if self.entry.get() in case:
-            if case[self.rb.get()] == "child":
-                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
-                self.entry3.current(0)
-            elif case[self.rb.get()] != "child":
-                self.entry3.config(values="")
-                self.entry3.config(state="normal")
-                self.entry3.delete(0, END)
-                self.entry3.config(state="readonly")
-            self.entry.delete(0, END)
-            if len(str(self.entry.focus_get())) > 5:
-                if str(self.entry.focus_get())[-5:] != "entry":
-                    self.entry.insert(0, case[""])
-            else:
-                self.entry.insert(0, case[""])
-        else:
-            if case[self.rb.get()] == "child":
-                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
-                self.entry3.current(0)
-            elif case[self.rb.get()] != "child":
-                self.entry3.config(values="")
-                self.entry3.config(state="normal")
-                self.entry3.delete(0, END)
-                self.entry3.config(state="readonly")
-            self.entry.selection_clear()
-        del case
-
-    def focus(self, event=None):
-        """Validation for Entry"""
-
-        if self.entry.validate:
-            case = ["child", "parent"]
-            if self.entry.get() in case:
-                self.entry.delete(0, END)
-                return True
-            else:
-                return False
-            del case
-
     def scrd(self, event=None):
         """Scroll to the bottom on keyboard, down arrow button"""
 
         a = self.text.yview()[0]
         a = eval(f"{a}") + 0.01
         self.text.yview_moveto(str(a))
         self.listb.yview_moveto(str(a + 0.01))
@@ -1316,21 +959,21 @@
         Write also on chosen row for update.
         """
 
         self.hidcheck()
         cek = ["child", "parent"]
         if self.unlock:
             if not self.checkfile():
-                if self.entry.get():
-                    if not self.entry3.get():
-                        if self.entry.get() not in cek:
+                if self.bt["entry"].get():
+                    if not self.bt["entry3"].get():
+                        if self.bt["entry"].get() not in cek:
                             with tv(self.filename) as tvg:
-                                tvg.writetree(self.entry.get())
+                                tvg.writetree(self.bt["entry"].get())
                             del tvg
-                            self.entry.delete(0, END)
+                            self.bt["entry"].delete(0, END)
                             self.spaces()
                     else:
                         messagebox.showinfo(
                             "TreeViewGui",
                             f"No {self.filename}.txt file yet created please choose parent first!",
                             parent=self.root,
                         )
@@ -1338,16 +981,16 @@
                     messagebox.showinfo(
                         "TreeViewGui",
                         f"No {self.filename}.txt file yet created!",
                         parent=self.root,
                     )
             else:
                 rw = None
-                if self.entry3.get():
-                    if self.entry.get() and self.entry.get() not in cek:
+                if self.bt["entry3"].get():
+                    if self.bt["entry"].get() and self.bt["entry"].get() not in cek:
                         if self.MARK:
                             rw = self.listb.curselection()[0]
                             appr = messagebox.askyesno(
                                 "Edit", f"Edit cell {rw}?", parent=self.root
                             )
                             if appr:
                                 with tv(self.filename) as tvg:
@@ -1356,28 +999,30 @@
                                             tvg.compdatch(True),
                                             int(rw),
                                             int(rw) + 1,
                                         )
                                     )
                                     if insight[0][0] != "space":
                                         tvg.edittree(
-                                            self.entry.get(),
+                                            self.bt["entry"].get(),
                                             int(rw),
-                                            self.entry3.get(),
+                                            self.bt["entry3"].get(),
                                         )
                                 del tvg, insight
-                                self.entry.delete(0, END)
+                                self.bt["entry"].delete(0, END)
                         else:
                             with tv(self.filename) as tvg:
-                                tvg.quickchild(self.entry.get(), self.entry3.get())
-                            self.entry.delete(0, END)
+                                tvg.quickchild(
+                                    self.bt["entry"].get(), self.bt["entry3"].get()
+                                )
+                            self.bt["entry"].delete(0, END)
                             del tvg
                         self.spaces()
                 else:
-                    if self.entry.get() and self.entry.get() not in cek:
+                    if self.bt["entry"].get() and self.bt["entry"].get() not in cek:
                         if self.MARK:
                             rw = self.listb.curselection()[0]
                             appr = messagebox.askyesno(
                                 "Edit", f"Edit cell {rw}?", parent=self.root
                             )
                             if appr:
                                 with tv(self.filename) as tvg:
@@ -1385,22 +1030,22 @@
                                         islice(
                                             tvg.compdatch(True),
                                             int(rw),
                                             int(rw) + 1,
                                         )
                                     )
                                     if insight[0][0] != "space":
-                                        tvg.edittree(self.entry.get(), int(rw))
+                                        tvg.edittree(self.bt["entry"].get(), int(rw))
                                 del tvg, insight
-                                self.entry.delete(0, END)
+                                self.bt["entry"].delete(0, END)
                         else:
                             with tv(self.filename) as tvg:
-                                tvg.addparent(self.entry.get())
+                                tvg.addparent(self.bt["entry"].get())
                             del tvg
-                            self.entry.delete(0, END)
+                            self.bt["entry"].delete(0, END)
                         self.spaces()
                 if rw and rw < len(self.listb.get(0, END)) - 1:
                     self.text.see(f"{int(rw)}.0")
                     self.listb.see(rw)
                 del rw
         del cek
 
@@ -1457,21 +1102,21 @@
 
     def move_lr(self, event=None):
         """Moving a child row to left or right, as to define spaces needed"""
 
         self.hidcheck()
         if self.unlock:
             if self.listb.curselection():
-                if self.entry3.get():
+                if self.bt["entry3"].get():
                     self.MODE = True
                     try:
                         rw = int(self.listb.curselection()[0])
                         self.text.config(state="normal")
                         with tv(self.filename) as tvg:
-                            tvg.movechild(rw, self.entry3.get())
+                            tvg.movechild(rw, self.bt["entry3"].get())
                         del tvg
                         self.spaces()
                         self.text.config(state="disable")
                         self.listb.select_set(rw)
                         self.listb.see(rw)
                         self.text.see(f"{rw}.0")
                     except:
@@ -1566,33 +1211,35 @@
     def insertwords(self, event=None):
         """Insert a record to any row appear above the assign row"""
 
         self.hidcheck()
         if self.unlock:
             if self.nonetype():
                 cek = ["parent", "child"]
-                if self.entry.get() and self.entry.get() not in cek:
+                if self.bt["entry"].get() and self.bt["entry"].get() not in cek:
                     if self.MARK:
                         appr = messagebox.askyesno(
                             "Edit",
                             f"Edit cell {self.listb.curselection()[0]}?",
                             parent=self.root,
                         )
                         if appr:
                             if self.listb.curselection():
                                 rw = int(self.listb.curselection()[0])
                                 with tv(self.filename) as tvg:
-                                    if self.entry3.get():
+                                    if self.bt["entry3"].get():
                                         tvg.insertrow(
-                                            self.entry.get(), rw, self.entry3.get()
+                                            self.bt["entry"].get(),
+                                            rw,
+                                            self.bt["entry3"].get(),
                                         )
                                     else:
-                                        tvg.insertrow(self.entry.get(), rw)
+                                        tvg.insertrow(self.bt["entry"].get(), rw)
                                 del tvg
-                                self.entry.delete(0, END)
+                                self.bt["entry"].delete(0, END)
                                 self.spaces()
                                 self.listb.see(rw)
                                 self.text.see(f"{rw}.0")
                                 del rw
                         del appr
                 del cek
 
@@ -1673,27 +1320,27 @@
 
     def copas(self, event=None):
         """Paste a row value to Entry for fixing value"""
 
         self.hidcheck()
         if self.unlock:
             if self.listb.curselection():
-                self.entry.delete(0, END)
+                self.bt["entry"].delete(0, END)
                 rw = int(self.listb.curselection()[0])
                 paste = None
                 with tv(self.filename) as tvg:
                     for r, l in tvg.getdata():
                         if r == rw:
                             if l == "\n":
                                 break
                             elif l[0] == " ":
                                 paste = l[re.match(r"\s+", l).span()[1] + 1 : -1]
                             else:
                                 paste = l[:-2]
-                            self.entry.insert(END, paste)
+                            self.bt["entry"].insert(END, paste)
                             break
                 del tvg, rw, paste
 
     def fildat(self, dat: str, b: bool = True):
         """Returning data pattern to cmrows"""
 
         if b:
@@ -1839,15 +1486,15 @@
             self._copytofile()
         else:
             self.hidcheck()
             if self.unlock:
                 if self.nonetype():
                     if self.listb.cget("selectmode") == "browse":
                         self.listb.config(selectmode=self.cpp_select)
-                        self.disab("listb", "button17", "button10", "text")
+                        self.disab("listb", "CPP", "Insight", "text")
                     else:
                         if gcs := self.listb.curselection():
                             gcs = [int(i) for i in gcs]
                             ask = simpledialog.askinteger(
                                 "TreeViewGui",
                                 f"Move to which row? choose between 0 to {self.listb.size()-1} rows",
                                 parent=self.root,
@@ -1948,15 +1595,14 @@
                         else:
                             self.disab(dis=False)
                             self.listb.config(selectmode=BROWSE)
                     self.listb.selection_clear(0, END)
                     self.infobar()
 
     def _utilspdf(self):
-
         try:
             gttx = []
             line = None
             cg = None
             eldat = self._ckfoldtvg()
             if hasattr(self, "fold"):
                 for i in range(1, self.listb.size() + 1):
@@ -2131,15 +1777,15 @@
         if hasattr(self, "fold"):
             messagebox.showinfo("TreeViewGui", "Please unfolding first!")
         else:
             if self.nonetype():
                 if not os.path.exists(f"{self.filename}_hid.json"):
                     if self.listb.cget("selectmode") == "browse":
                         self.info.set("Hidden Mode")
-                        self.disab("listb", "button14", "button10", "text")
+                        self.disab("listb", "Hide Parent", "Insight", "text")
                         self.listb.config(selectmode=MULTIPLE)
                     else:
                         if self.listb.curselection():
                             allrows = [int(i) for i in self.listb.curselection()]
                             rows = {
                                 n: pc.split(":")[1].strip()
                                 for n, pc in enumerate(self.listb.get(0, END))
@@ -2207,15 +1853,15 @@
     def lookup(self, event=None):
         """To lookup word on row and also on editor mode"""
 
         self.hidcheck()
         if self.unlock:
             if (
                 str(self.text.cget("state")) == "normal"
-                and str(self.bt["button24"].cget("state")) == "normal"
+                and str(self.bt["Editor"].cget("state")) == "normal"
             ):
                 if self.text.count("1.0", END, "chars")[0] > 1:
 
                     @excp(2, DEFAULTFILE)
                     def searchw(words: str):
                         self.text.tag_config("hw", underline=1)
                         idx = self.text.search(words, "1.0", END, nocase=1)
@@ -2289,18 +1935,18 @@
                         self.lock = False
                         if d.result:
                             searchw(d.result)
                         self.FREEZE = False
                         del d.result
             else:
                 if self.nonetype():
-                    if self.entry.get():
+                    if self.bt["entry"].get():
                         num = self.listb.size()
                         sn = 1
-                        sw = self.entry.get()
+                        sw = self.bt["entry"].get()
                         dat = None
                         if sw.isdigit():
                             sw = int(sw)
                             if sw <= num - 1:
                                 self.listb.see(sw)
                                 self.text.see(f"{sw}.0")
                                 self.listb.focus()
@@ -2338,40 +1984,40 @@
                                 self.listb.yview_moveto(1.0)
                         del dat, num, sn, sw
                     self.infobar()
 
     def dattim(self, event=None):
         """To insert date and time"""
 
-        if str(self.entry.cget("state")) == "normal":
+        if str(self.bt["entry"].cget("state")) == "normal":
             dtt = f'[{dt.isoformat(dt.today().replace(microsecond = 0)).replace("T"," ")}]'
             ck = ["parent", "child"]
-            if self.entry.get() in ck:
-                self.entry.delete(0, END)
-            if self.entry.get():
-                hold = self.entry.get()
+            if self.bt["entry"].get() in ck:
+                self.bt["entry"].delete(0, END)
+            if self.bt["entry"].get():
+                hold = self.bt["entry"].get()
                 gt = re.match(r"\[.*?\]", hold)
                 if not gt:
-                    self.entry.delete(0, END)
-                    self.entry.insert(0, f"{dtt} {hold}")
+                    self.bt["entry"].delete(0, END)
+                    self.bt["entry"].insert(0, f"{dtt} {hold}")
                 else:
                     try:
                         if isinstance(dt.fromisoformat(gt.group()[1:20]), dt):
-                            self.entry.delete(0, END)
-                            self.entry.insert(0, f"{dtt} {hold[22:]}")
+                            self.bt["entry"].delete(0, END)
+                            self.bt["entry"].insert(0, f"{dtt} {hold[22:]}")
                     except:
-                        self.entry.delete(0, END)
-                        self.entry.insert(0, f"{dtt} {hold}")
+                        self.bt["entry"].delete(0, END)
+                        self.bt["entry"].insert(0, f"{dtt} {hold}")
                 del hold, gt
             else:
-                self.entry.insert(0, f"{dtt} ")
+                self.bt["entry"].insert(0, f"{dtt} ")
             del dtt, ck
         elif (
             str(self.text.cget("state")) == "normal"
-            and str(self.bt["button20"].cget("state")) == "normal"
+            and str(self.bt["Date-Time"].cget("state")) == "normal"
         ):
             dtt = f'[{dt.isoformat(dt.today().replace(microsecond = 0)).replace("T"," ")}]'
             self.text.insert(INSERT, f"{dtt} ")
             self.text.focus()
             del dtt
 
     def createf(self, name: str = None):
@@ -2391,17 +2037,17 @@
                 self.glop = mkd
                 self._ckfoldtvg()
                 self.filename = self.glop.name.rpartition("_")[0]
                 self.root.title(f"{self.glop.absolute().joinpath(self.filename)}.txt")
                 self.text.config(state=NORMAL)
                 self.text.delete("1.0", END)
                 self.text.config(state=DISABLED)
-                self.entry.delete(0, END)
-                self.rb.set("")
-                self.entry.config(state=DISABLED)
+                self.bt["entry"].delete(0, END)
+                self.fframe.rb.set("")
+                self.bt["entry"].config(state=DISABLED)
                 self.listb.delete(0, END)
                 self.addonchk(False)
             else:
                 messagebox.showinfo(
                     "TreeViewGui",
                     f"The file {mkd}/{titlemode(fl)}.txt is already exist!",
                     parent=self.root,
@@ -2544,15 +2190,15 @@
         """This is to compliment the editor mode.
         If you have to type several outline that has same format,
         You can save them as template and re-use again in the editor mode.
         """
 
         if (
             str(self.text.cget("state")) == "normal"
-            and str(self.bt["button24"].cget("state")) == "normal"
+            and str(self.bt["Editor"].cget("state")) == "normal"
         ):
             if not os.path.exists(os.path.join(self.glop.parent, "Templates")):
                 os.mkdir(os.path.join(self.glop.parent, "Templates"))
                 self.tempsave()
             else:
                 if self.lock is False:
                     self.FREEZE = True
@@ -2658,25 +2304,24 @@
             self.FREEZE = True
         else:
             for i in self.bt:
                 if "label" not in i and "scrollbar" not in i:
                     if i == "entry3":
                         self.bt[i].config(state="readonly")
                     elif i == "entry":
-                        if not self.rb.get():
+                        if not self.fframe.rb.get():
                             self.bt[i].config(state="disable")
                         else:
                             self.bt[i].config(state="normal")
                     else:
                         if i != "text":
                             self.bt[i].config(state="normal")
             self.FREEZE = False
 
     def _mdbuttons(self):
-
         if not hasattr(self, "mdframe"):
             self.__setattr__("mdb", None)
             self.mdb = {
                 "B": ("<Control-Shift-!>", "****"),
                 "I": ("<Control-Shift-@>", "**"),
                 "U": ("<Control-Shift-#>", "^^^^"),
                 "S": ("<Control-Shift-$>", "~~~~"),
@@ -2767,15 +2412,14 @@
             self.mdframe = ttk.Frame(self.frb3)
             self.mdframe.pack(fill=X, expand=1)
 
             mdbut = ttk.Button(self.mdframe, text=lmdb[0], width=1, command=insmd)
             mdbut.pack(side=LEFT, padx=2, pady=(0, 2), fill=X, expand=1)
             mdbut.bind("<Enter>", storbut)
             mdbut.bind_all(self.mdb[lmdb[0]][0], shortcut)
-            self.rsv_frame = mdbut.winfo_parent()
             for i in range(1, 17):
                 mdbut = ttk.Button(self.mdframe, text=lmdb[i], width=1, command=insmd)
                 mdbut.pack(side=LEFT, padx=(0, 2), pady=(0, 2), fill=X, expand=1)
                 mdbut.bind("<Enter>", storbut)
                 mdbut.bind_all(self.mdb[lmdb[i]][0], shortcut)
 
             self.tframe.pack(anchor="w", side=TOP, fill="both", expand=1)
@@ -2786,15 +2430,14 @@
         else:
             for i in self.mdframe.winfo_children():
                 i.unbind_all(self.mdb[i.cget("text")][0])
                 i.unbind("<Enter>")
                 i.destroy()
                 del i
             self.mdframe.destroy()
-            self.rsv_frame = None
             self.__delattr__("mdb")
             self.__delattr__("mdframe")
             self.frb3.pack_forget()
 
     def editor(self):
         """This is direct editor on text window.
         FORMAT:
@@ -2805,18 +2448,18 @@
 
         self.hidcheck()
         if self.unlock:
             if str(self.text.cget("state")) == "disabled":
                 self.text.config(state="normal")
                 self.text.delete("1.0", END)
                 ckb = [
-                    "button24",
-                    "button28",
-                    "button20",
-                    "button19",
+                    "Editor",
+                    "Template",
+                    "Date-Time",
+                    "Look Up",
                     "text",
                 ]
                 self.disab(*ckb)
                 self.text.edit_reset()
                 self.text.focus()
                 self._mdbuttons()
                 if not self.plat.startswith("win"):
@@ -3189,34 +2832,35 @@
                 )
 
     def gettotsum(self):
         """Get all sums on all parents that have "+" sign in front"""
 
         if self.nonetype():
             sa = SumAll(self.filename, sig="+")
-            self.listb.config(selectmode=MULTIPLE)
             match len(sa) > 0:
                 case False if hasattr(self, "sumtot"):
                     match os.path.exists(f"{self.filename}_hid.json"):
                         case False:
                             if not hasattr(self, "fold"):
+                                self.listb.config(selectmode=MULTIPLE)
                                 idx = sa.getidx(False)
                                 tot = sa.lumpsum()
                                 for i in idx:
                                     self.listb.select_set(i)
                                 self.hiddenchl()
                                 self.text.config(state=NORMAL)
                                 if (
                                     self.text.get(f"{END} - 2 lines", END)
                                     .strip()
                                     .startswith("-TOTAL")
                                 ):
                                     self.text.insert(END, f"\nTOTAL SUMS = {tot}")
                                 else:
                                     self.text.insert(END, f"TOTAL SUMS = {tot}")
+                                self.listb.config(selectmode=BROWSE)
                                 self.text.config(state=DISABLED)
                                 del idx, tot
                             else:
                                 messagebox.showwarning(
                                     "TreeViewGui",
                                     "Please unfolding first!",
                                     parent=self.root,
@@ -3238,15 +2882,14 @@
                             "Please unfolding first!",
                             parent=self.root,
                         )
                 case False:
                     messagebox.showinfo(
                         "TreeViewGui", "No data to sums!", parent=self.root
                     )
-            self.listb.config(selectmode=BROWSE)
             del sa
 
     def chktp(self):
         """Clearing Toplevel widget"""
 
         for i in self.root.winfo_children():
             if ".!toplevel" in str(i):
@@ -3306,19 +2949,17 @@
                             )
                 else:
                     messagebox.showwarning(
                         "TreeViewGui",
                         "Please unfolding first!",
                         parent=self.root,
                     )
-                del sal
                 self.spaces()
 
     def _ckwrds(self, wrd: str):
-
         if self._addon:
             nums = len(wrd)
             if nums >= 101:
                 raise Exception(f"{nums} charcters, is exceeding than 100 chars!")
 
             for i in wrd:
                 if i not in tuple("0123456789*/-+()%."):
@@ -3576,15 +3217,15 @@
         """Folding selected"""
 
         self.hidcheck()
         if self.unlock:
             if self.nonetype():
                 if self.listb.cget("selectmode") == BROWSE:
                     self.listb.config(selectmode=self.cpp_select)
-                    self.disab("button34", "button10", "listb", "text")
+                    self.disab("Fold selected", "Insight", "listb", "text")
                     self._load_selection()
                     if not hasattr(self, "fold"):
                         self.__setattr__("fold", True)
                 else:
                     if self.listb.curselection():
                         with open(
                             self.glop.absolute().joinpath("fold.tvg"), "wb"
@@ -3609,23 +3250,105 @@
                     self.__delattr__("fold")
                     self.view()
                     self.infobar()
 
     def configd(self, event=None):
         """Deleting configuration file to default"""
 
-        if self.lock is False and os.path.exists(
-            self.glop.parent.joinpath("TVG_config.toml")
-        ):
-            os.remove(self.glop.parent.joinpath("TVG_config.toml"))
-            messagebox.showinfo(
-                "TreeViewGui",
-                "Configuration has been set to default!",
-                parent=self.root,
-            )
+        if self.lock is False:
+            TreeViewGui.FREEZE = True
+            self.lock = True
+
+            if self.glop.parent.joinpath("TVG_config.toml").exists():
+                with open(self.glop.parent.joinpath("TVG_config.toml")) as rf:
+                    cfg = tomlkit.load(rf)
+
+                @excpcls(2, DEFAULTFILE)
+                class MyDialog(simpledialog.Dialog):
+                    def body(self, master):
+                        self.title("Configure TVG")
+
+                        self.fr2 = Frame(master)
+                        self.fr2.pack(fill=X, expand=1, pady=(0, 1))
+                        Label(self.fr2, text="Select Mode: ").pack(side=LEFT)
+                        self.e2 = ttk.Combobox(self.fr2)
+                        self.e2["values"] = "extended", "multiple"
+                        self.e2.pack(side=RIGHT)
+                        self.e2.current(
+                            self.e2["values"].index(cfg["Configure"]["SELECT_MODE"])
+                        )
+                        self.e2.config(state="readonly")
+
+                        self.fr3 = Frame(master)
+                        self.fr3.pack(fill=X, expand=1, pady=(0, 1))
+                        Label(self.fr3, text="Hidden Opt: ").pack(side=LEFT)
+                        self.e3 = ttk.Combobox(self.fr3)
+                        self.e3["values"] = "False", "unreverse"
+                        self.e3.pack(side=RIGHT)
+                        self.e3.current(
+                            self.e3["values"].index(str(cfg["Configure"]["HIDDEN_OPT"]))
+                        )
+                        self.e3.config(state="readonly")
+
+                        self.fr4 = Frame(master)
+                        self.fr4.pack(fill=X, expand=1, pady=(0, 1))
+                        Label(self.fr4, text="Wrapping: ").pack(side=LEFT)
+                        self.e4 = ttk.Combobox(self.fr4)
+                        self.e4["values"] = "none", "word"
+                        self.e4.pack(side=RIGHT)
+                        self.e4.current(
+                            self.e4["values"].index(cfg["Configure"]["WRAPPING"])
+                        )
+                        self.e4.config(state="readonly")
+
+                        self.fr5 = Frame(master)
+                        self.fr5.pack(fill=X, expand=1, pady=(0, 1))
+                        Label(self.fr5, text="Checked Box: ").pack(side=LEFT)
+                        self.e5 = ttk.Combobox(self.fr5)
+                        self.e5["values"] = "off", "on"
+                        self.e5.pack(side=RIGHT)
+                        self.e5.current(
+                            self.e5["values"].index(cfg["Configure"]["CHECKED_BOX"])
+                        )
+                        self.e5.config(state="readonly")
+                        return self.e2
+
+                    def apply(self):
+                        hid = (
+                            ast.literal_eval(self.e3.get())
+                            if self.e3.get() == "False"
+                            else self.e3.get()
+                        )
+                        self.result = (
+                            self.e2.get(),
+                            hid,
+                            self.e4.get(),
+                            self.e5.get(),
+                        )
+
+                d = MyDialog(self.root)
+                self.root.update()
+                self.lock = False
+
+                if d.result:
+                    if tuple(cfg["Configure"].values()) != d.result:
+                        global SELECT_MODE, HIDDEN_OPT, WRAPPING, CHECKED_BOX
+                        self.cpp_select = SELECT_MODE = d.result[0]
+                        self.hidopt = HIDDEN_OPT = d.result[1]
+                        if WRAPPING != d.result[2]:
+                            self.wrapping = WRAPPING = d.result[2]
+                            self.wrapped()
+                        self.checked_box = CHECKED_BOX = d.result[3]
+                        _create_config(self.glop.parent.joinpath("TVG_config.toml"))
+                    else:
+                        messagebox.showinfo(
+                            "TreeViewGui", "Configuring aborted!", parent=self.root
+                        )
+
+            TreeViewGui.FREEZE = False
 
 
 @excp(m=2, filenm=DEFAULTFILE)
 def askfile(root):
     """Asking file for creating or opening initial app start"""
 
     files = [
@@ -3670,110 +3393,69 @@
         os.chdir(pth)
     else:
         os.mkdir(pth)
         os.chdir(pth)
 
 
 @excp(m=2, filenm=DEFAULTFILE)
-def _create_config():
+def _create_config(pth: str = None):
     """Configuration set according to the user's preference"""
 
-    deval = [ctlight()]
-
-    with open("TVG_config.toml", "w") as fp:
+    with open(pth := "TVG_config.toml" if pth is None else pth, "w") as fp:
         tomlkit.dump(
             {
                 "Configure": {
-                    "THEME_MODE": (
-                        THEME_MODE_ := THEME_MODE if THEME_MODE != deval[0] else 0
-                    ),
                     "SELECT_MODE": SELECT_MODE,
                     "HIDDEN_OPT": HIDDEN_OPT,
                     "WRAPPING": WRAPPING,
                     "CHECKED_BOX": CHECKED_BOX,
                 }
             },
             fp,
         )
 
-    del deval, THEME_MODE_
-
 
 @excp(m=2, filenm=DEFAULTFILE)
 def _load_config():
     """Load configuration"""
 
     if os.path.exists("TVG_config.toml"):
         global THEME_MODE, SELECT_MODE, HIDDEN_OPT, WRAPPING, CHECKED_BOX
         with open("TVG_config.toml") as rf:
             cfg = tomlkit.load(rf)
-        THEME_MODE = (
-            cfg["Configure"]["THEME_MODE"]
-            if cfg["Configure"]["THEME_MODE"] != 0
-            else THEME_MODE
-        )
         SELECT_MODE = cfg["Configure"]["SELECT_MODE"]
         HIDDEN_OPT = cfg["Configure"]["HIDDEN_OPT"]
         WRAPPING = cfg["Configure"]["WRAPPING"]
         CHECKED_BOX = cfg["Configure"]["CHECKED_BOX"]
         del cfg
 
 
 @excp(m=2, filenm=DEFAULTFILE)
 def configuring(args: list):
     """configuring TVG"""
 
-    vals = THEME_MODE, SELECT_MODE, HIDDEN_OPT, WRAPPING, CHECKED_BOX
     match ment := len(args):
         case ment if ment == 2:
             _mode(args[1])
-        case ment if ment == 3:
-            _mode(args[1])
-            _mode(args[2])
-        case ment if ment == 4:
-            _mode(args[1])
-            _mode(args[2])
-            _mode(args[3])
-        case ment if ment == 5:
-            _mode(args[1])
-            _mode(args[2])
-            _mode(args[3])
-            _mode(args[4])
-        case ment if ment == 6:
-            _mode(args[1])
-            _mode(args[2])
-            _mode(args[3])
-            _mode(args[4])
-            _mode(args[5])
         case _:
             pass
-    if vals != (THEME_MODE, SELECT_MODE, HIDDEN_OPT, WRAPPING, CHECKED_BOX):
-        _create_config()
-    del args, vals
+    del args, ment
 
 
 @excp(m=2, filenm=DEFAULTFILE)
 def _mode(mode: str):
-    global THEME_MODE, SELECT_MODE, HIDDEN_OPT, WRAPPING, CHECKED_BOX
+    global THEME_MODE
 
     match mode := mode:
         case mode if mode.lower() == "dark":
             if THEME_MODE is True:
                 THEME_MODE = "dark"
         case mode if mode.lower() == "light":
             if THEME_MODE is False:
                 THEME_MODE = "light"
-        case mode if mode.lower() == "multiple":
-            SELECT_MODE = mode
-        case mode if mode.lower() == "unreverse":
-            HIDDEN_OPT = mode
-        case mode if mode.lower() == "word":
-            WRAPPING = mode
-        case mode if mode.lower() == "on":
-            CHECKED_BOX = mode
         case _:
             pass
     del mode
 
 
 @excp(m=2, filenm=DEFAULTFILE)
 def titlemode(sent: str):
```

### Comparing `FreeTVG-karjakak-3.1.9/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.0rc1/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.9/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.0rc1/TVG/utility/mdh.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 <style>
 {setfont}
 {kbd}
 {tasklist}
 """
         printed = """@media print {
 .button { display: none; }
+
 body { 
     background-color: white !important;
     color: black !important;
     }
 
 kbd { color: black !important; }
 }
```

### Comparing `FreeTVG-karjakak-3.1.9/TVG/utility/term.py` & `FreeTVG-karjakak-3.2.0rc1/TVG/utility/term.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.9/setup.cfg` & `FreeTVG-karjakak-3.2.0rc1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.1.9
+version = 3.2.0rc1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

