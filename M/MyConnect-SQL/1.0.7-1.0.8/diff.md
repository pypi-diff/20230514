# Comparing `tmp/MyConnect - SQL-1.0.7.tar.gz` & `tmp/MyConnect - SQL-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyConnect - SQL-1.0.7.tar", last modified: Sat May 13 21:58:08 2023, max compression
+gzip compressed data, was "MyConnect - SQL-1.0.8.tar", last modified: Sat May 13 22:13:13 2023, max compression
```

## Comparing `MyConnect - SQL-1.0.7.tar` & `MyConnect - SQL-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 21:58:08.888697 MyConnect - SQL-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-13 21:58:08.847367 MyConnect - SQL-1.0.7/MyConnect/
--rw-rw-rw-   0        0        0     6427 2023-05-13 21:51:22.000000 MyConnect - SQL-1.0.7/MyConnect/AuthLogin.py
--rw-rw-rw-   0        0        0      544 2023-05-13 21:11:26.000000 MyConnect - SQL-1.0.7/MyConnect/moduleTest.py
-drwxrwxrwx   0        0        0        0 2023-05-13 21:58:08.834837 MyConnect - SQL-1.0.7/MyConnect/venv/
-drwxrwxrwx   0        0        0        0 2023-05-13 21:58:08.851365 MyConnect - SQL-1.0.7/MyConnect/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-05-13 19:48:27.000000 MyConnect - SQL-1.0.7/MyConnect/venv/Scripts/activate_this.py
-drwxrwxrwx   0        0        0        0 2023-05-13 21:58:08.879150 MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/
--rw-rw-rw-   0        0        0      590 2023-05-13 21:58:08.000000 MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-13 21:58:08.000000 MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:58:08.000000 MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:58:08.000000 MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2023-05-13 21:58:08.886663 MyConnect - SQL-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-05-13 16:40:01.000000 MyConnect - SQL-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 21:58:08.889700 MyConnect - SQL-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-05-13 21:58:06.000000 MyConnect - SQL-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.572566 MyConnect - SQL-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.532386 MyConnect - SQL-1.0.8/MyConnect/
+-rw-rw-rw-   0        0        0     6326 2023-05-13 22:11:42.000000 MyConnect - SQL-1.0.8/MyConnect/AuthLogin.py
+-rw-rw-rw-   0        0        0      421 2023-05-13 22:10:57.000000 MyConnect - SQL-1.0.8/MyConnect/moduleTest.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.513811 MyConnect - SQL-1.0.8/MyConnect/venv/
+drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.535910 MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-05-13 19:48:27.000000 MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/activate_this.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.566037 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2023-05-13 22:13:13.568562 MyConnect - SQL-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-05-13 16:40:01.000000 MyConnect - SQL-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-13 22:13:13.576570 MyConnect - SQL-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-05-13 22:01:23.000000 MyConnect - SQL-1.0.8/setup.py
```

### Comparing `MyConnect - SQL-1.0.7/MyConnect/AuthLogin.py` & `MyConnect - SQL-1.0.8/MyConnect/AuthLogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from tkinter import *
 from tkinter import messagebox
 import mysql.connector as MC 
 from mysql.connector import errorcode
 
 # Var
 
-u1 = open("user.txt", "r")
 
 global lg
 global LoginFrame
+u1 = ""
 lg = Tk()
 LoginFrame = Frame(lg, width=350, height=350, bg="white")
 
 # Def
 
 class login():
     # Windows
@@ -137,17 +137,16 @@
                         query='select * from '+Table+' where '+TableUser+'=%s and '+TablePassword+'=%s'
                         cursor.execute(query ,(username ,password))
                         row = cursor.fetchone()
                         if row == None:
                             messagebox.showerror('Login', 'Invalid username or/and password')
                         else:
                             messagebox.showinfo('Succes', 'Login is sucessful')
-                            u1 = open("user.txt", "w+")
-                            u1.write(username)
-                            u1.close()
+                            global u1
+                            u1 = username
                             print("Welcome "+username)
                     except MC.Error as err:
                         messagebox.showerror("MySQL Error", err)
 
                     
                     
 
@@ -201,9 +200,8 @@
                 messagebox.showerror("MySQL Error" ,err)
         
     # MainLoop
 
     def loop():
         lg.mainloop()
 
-username = u1.read()
-u1.close()
+username = u1
```

### Comparing `MyConnect - SQL-1.0.7/MyConnect/venv/Scripts/activate_this.py` & `MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `MyConnect - SQL-1.0.7/MyConnect_SQL.egg-info/PKG-INFO` & `MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyConnect-SQL
-Version: 1.0.7
+Version: 1.0.8
 Summary: Auth Login simplifies the creation of login page and account creation.
 Home-page: https://github.com/Rayanis55/AuthLogin
 Author: Venorix - Rayanis55
 License: MIT
 Requires-Python: >=3.0
 
 Auth Login simplifies the creation of login page and account creation.         AuthLogin is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
```

### Comparing `MyConnect - SQL-1.0.7/PKG-INFO` & `MyConnect - SQL-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyConnect - SQL
-Version: 1.0.7
+Version: 1.0.8
 Summary: Auth Login simplifies the creation of login page and account creation.
 Home-page: https://github.com/Rayanis55/AuthLogin
 Author: Venorix - Rayanis55
 License: MIT
 Requires-Python: >=3.0
 
 Auth Login simplifies the creation of login page and account creation.         AuthLogin is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
```

### Comparing `MyConnect - SQL-1.0.7/README.md` & `MyConnect - SQL-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `MyConnect - SQL-1.0.7/setup.py` & `MyConnect - SQL-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
   name = "MyConnect - SQL",
-  version = "1.0.7",
+  version = "1.0.8",
   author="Venorix - Rayanis55",
   license='MIT',
   description='Auth Login simplifies the creation of login page and account creation.',
   long_description="Auth Login simplifies the creation of login page and account creation. \
     \
     AuthLogin is a module that facilitates the creation of login and registration pages \
     The module is rather a simplification because if we can say that it compresses \
     the tkinter variables (That's why you have to put a login.loop() at the end).",
-  packages=find_packages(),
   url="https://github.com/Rayanis55/AuthLogin",
   python_requires='>=3.0',
 )
```

