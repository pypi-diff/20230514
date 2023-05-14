# Comparing `tmp/MyConnect - SQL-1.0.8.tar.gz` & `tmp/MyConnect - SQL-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyConnect - SQL-1.0.8.tar", last modified: Sat May 13 22:13:13 2023, max compression
+gzip compressed data, was "MyConnect - SQL-1.1.0.tar", last modified: Sun May 14 12:32:55 2023, max compression
```

## Comparing `MyConnect - SQL-1.0.8.tar` & `MyConnect - SQL-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.572566 MyConnect - SQL-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.532386 MyConnect - SQL-1.0.8/MyConnect/
--rw-rw-rw-   0        0        0     6326 2023-05-13 22:11:42.000000 MyConnect - SQL-1.0.8/MyConnect/AuthLogin.py
--rw-rw-rw-   0        0        0      421 2023-05-13 22:10:57.000000 MyConnect - SQL-1.0.8/MyConnect/moduleTest.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.513811 MyConnect - SQL-1.0.8/MyConnect/venv/
-drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.535910 MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-05-13 19:48:27.000000 MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/activate_this.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:13:13.566037 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/
--rw-rw-rw-   0        0        0      590 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-13 22:13:13.000000 MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2023-05-13 22:13:13.568562 MyConnect - SQL-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-05-13 16:40:01.000000 MyConnect - SQL-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 22:13:13.576570 MyConnect - SQL-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-05-13 22:01:23.000000 MyConnect - SQL-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 12:32:55.975629 MyConnect - SQL-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-14 12:32:55.894662 MyConnect - SQL-1.1.0/MyConnect/
+-rw-rw-rw-   0        0        0     6610 2023-05-14 12:32:31.000000 MyConnect - SQL-1.1.0/MyConnect/AuthLogin.py
+-rw-rw-rw-   0        0        0      615 2023-05-14 12:29:27.000000 MyConnect - SQL-1.1.0/MyConnect/main.py
+drwxrwxrwx   0        0        0        0 2023-05-14 12:32:55.825137 MyConnect - SQL-1.1.0/MyConnect/venv/
+drwxrwxrwx   0        0        0        0 2023-05-14 12:32:55.898190 MyConnect - SQL-1.1.0/MyConnect/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-05-13 19:48:27.000000 MyConnect - SQL-1.1.0/MyConnect/venv/Scripts/activate_this.py
+drwxrwxrwx   0        0        0        0 2023-05-14 12:32:55.964997 MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-05-14 12:32:55.000000 MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-14 12:32:55.000000 MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 12:32:55.000000 MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 12:32:55.000000 MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2023-05-14 12:32:55.973598 MyConnect - SQL-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-05-14 09:08:23.000000 MyConnect - SQL-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 12:32:55.977143 MyConnect - SQL-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-05-14 12:32:44.000000 MyConnect - SQL-1.1.0/setup.py
```

### Comparing `MyConnect - SQL-1.0.8/MyConnect/AuthLogin.py` & `MyConnect - SQL-1.1.0/MyConnect/AuthLogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 # Var
 
 
 global lg
 global LoginFrame
 u1 = ""
+usernameGL = ""
+lgn = ""
 lg = Tk()
 LoginFrame = Frame(lg, width=350, height=350, bg="white")
 
 # Def
 
 class login():
     # Windows
@@ -118,38 +120,40 @@
 
         def buttonLogin(text="Sign in", widht=39, pady=7, bg="#57a1f8", fg="white", border=0):
 
             def signin():
                 username = userInputLogin.get()
                 password = passwordInputLogin.get()
 
-
                 try:
                     if usernameGL != "":
                         if username == usernameGL:
                             if password == passwordGL:
-                                print("Correct")
+                                u1 = username
+                                print("Welcome "+username)
+                                lg.destroy()
                             else: 
                                 messagebox.showerror("Login", "Password is incorrect !")
-                        else:
+                        else:  
                             messagebox.showerror("Login", "Username is incorrect !")
+                    else:
+                        try:
+                            query='select * from '+Table+' where '+TableUser+'=%s and '+TablePassword+'=%s'
+                            cursor.execute(query ,(username ,password))
+                            row = cursor.fetchone()
+                            if row == None:
+                                messagebox.showerror('Login', 'Invalid username or/and password')
+                            else:
+                                u1 = username
+                                print("Welcome "+username)
+                                lg.destroy()
+                        except MC.Error as err:
+                            messagebox.showerror("MySQL Error", err)
                 except:
-                    try:
-                        query='select * from '+Table+' where '+TableUser+'=%s and '+TablePassword+'=%s'
-                        cursor.execute(query ,(username ,password))
-                        row = cursor.fetchone()
-                        if row == None:
-                            messagebox.showerror('Login', 'Invalid username or/and password')
-                        else:
-                            messagebox.showinfo('Succes', 'Login is sucessful')
-                            global u1
-                            u1 = username
-                            print("Welcome "+username)
-                    except MC.Error as err:
-                        messagebox.showerror("MySQL Error", err)
+                    print("Erreur")
 
                     
                     
 
             buttonLogin = Button(LoginFrame, text=text, width=widht, pady=pady, bg=bg, fg=fg, border=border, command=signin)
             buttonLogin.place(x=35,y=224)
 
@@ -201,7 +205,18 @@
         
     # MainLoop
 
     def loop():
         lg.mainloop()
 
 username = u1
+
+# Def
+
+def on_closing():
+    lg.destroy()
+    exit()
+
+# While
+
+lg.protocol("WM_DELETE_WINDOW", on_closing)
+
```

### Comparing `MyConnect - SQL-1.0.8/MyConnect/venv/Scripts/activate_this.py` & `MyConnect - SQL-1.1.0/MyConnect/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `MyConnect - SQL-1.0.8/MyConnect_SQL.egg-info/PKG-INFO` & `MyConnect - SQL-1.1.0/MyConnect_SQL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyConnect-SQL
-Version: 1.0.8
+Version: 1.1.0
 Summary: Auth Login simplifies the creation of login page and account creation.
 Home-page: https://github.com/Rayanis55/AuthLogin
 Author: Venorix - Rayanis55
 License: MIT
 Requires-Python: >=3.0
 
-Auth Login simplifies the creation of login page and account creation.         AuthLogin is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
+Auth Login simplifies the creation of login page and account creation.         MyConnect is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
```

### Comparing `MyConnect - SQL-1.0.8/PKG-INFO` & `MyConnect - SQL-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyConnect - SQL
-Version: 1.0.8
+Version: 1.1.0
 Summary: Auth Login simplifies the creation of login page and account creation.
 Home-page: https://github.com/Rayanis55/AuthLogin
 Author: Venorix - Rayanis55
 License: MIT
 Requires-Python: >=3.0
 
-Auth Login simplifies the creation of login page and account creation.         AuthLogin is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
+Auth Login simplifies the creation of login page and account creation.         MyConnect is a module that facilitates the creation of login and registration pages     The module is rather a simplification because if we can say that it compresses     the tkinter variables (That's why you have to put a login.loop() at the end).
```

### Comparing `MyConnect - SQL-1.0.8/README.md` & `MyConnect - SQL-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 
 # 
 
 ## Description :
 
-AuthLogin is a module that facilitates the creation of login and registration pages 
+MyConnect is a module that facilitates the creation of login and registration pages 
 The module is rather a simplification because if we can say that it compresses the tkinter variables 
 (That's why you have to put a login.loop() at the end).
 
 
 ## Installation
 
-Install AuthLogin
+Install MyConnect
 
 ```bash
-  pip3 install AuthLogin
+  pip install MyConnect
 ```
 
 
     
 ## Documentation
 
 Create you login page
 
 ```py
-  from AuthLogin import *
+  from MyConnect import AuthLogin
 
-  if username == "":
-    # Title
+  # Title
 
-    login.setTitle("AuthLogin - Login")
+  login.setTitle("MyConnect - Login")
 
-    # Setup
+  # Setup
 
-    login.form.form('Login', '23', '#57a1f8', '300', '70')
-    login.form.userInput(widht=25)
-    login.form.passwordInput(widht=25)
-    login.form.buttonLogin()
+  login.form.form('Login', '23', '#57a1f8', '300', '70')
+  login.form.userInput(widht=25)
+  login.form.passwordInput(widht=25)
+  login.form.buttonLogin()
 
-    # Config login
+  # Config login
             
 
-    login.MySQLConfig('localhost', 'root', '', 'user', 'user')
+  login.MySQLConfig('localhost', 'root', '', 'user', 'user')
 
-    # Loop
+  # Loop
 
-    login.loop()
-  else:
-    print("Welcome "+username)
+  login.loop()
 ```
```

### Comparing `MyConnect - SQL-1.0.8/setup.py` & `MyConnect - SQL-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
   name = "MyConnect - SQL",
-  version = "1.0.8",
+  version = "1.1.0",
   author="Venorix - Rayanis55",
   license='MIT',
   description='Auth Login simplifies the creation of login page and account creation.',
   long_description="Auth Login simplifies the creation of login page and account creation. \
     \
-    AuthLogin is a module that facilitates the creation of login and registration pages \
+    MyConnect is a module that facilitates the creation of login and registration pages \
     The module is rather a simplification because if we can say that it compresses \
     the tkinter variables (That's why you have to put a login.loop() at the end).",
   url="https://github.com/Rayanis55/AuthLogin",
   python_requires='>=3.0',
 )
```

