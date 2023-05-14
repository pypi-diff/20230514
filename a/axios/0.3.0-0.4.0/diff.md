# Comparing `tmp/axios-0.3.0.tar.gz` & `tmp/axios-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axios-0.3.0.tar", last modified: Fri Mar 24 06:04:55 2023, max compression
+gzip compressed data, was "axios-0.4.0.tar", last modified: Sun May 14 20:41:46 2023, max compression
```

## Comparing `axios-0.3.0.tar` & `axios-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:04:55.086854 axios-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-03-24 06:04:55.082853 axios-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-03-24 06:04:38.000000 axios-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:04:55.082853 axios-0.3.0/axios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:04:38.000000 axios-0.3.0/axios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 06:04:38.000000 axios-0.3.0/axios/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-24 06:04:38.000000 axios-0.3.0/axios/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-24 06:04:38.000000 axios-0.3.0/axios/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-03-24 06:04:38.000000 axios-0.3.0/axios/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-24 06:04:38.000000 axios-0.3.0/axios/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:04:55.082853 axios-0.3.0/axios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 06:04:55.000000 axios-0.3.0/axios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 06:04:38.000000 axios-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 06:04:55.086854 axios-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-24 06:04:38.000000 axios-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:04:55.082853 axios-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-03-24 06:04:38.000000 axios-0.3.0/tests/test_axios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:41:46.069734 axios-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-14 20:41:46.069734 axios-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-14 20:41:31.000000 axios-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:41:46.069734 axios-0.4.0/axios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:41:31.000000 axios-0.4.0/axios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 20:41:31.000000 axios-0.4.0/axios/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-14 20:41:31.000000 axios-0.4.0/axios/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 20:41:31.000000 axios-0.4.0/axios/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-14 20:41:31.000000 axios-0.4.0/axios/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-14 20:41:31.000000 axios-0.4.0/axios/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:41:46.069734 axios-0.4.0/axios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 20:41:46.000000 axios-0.4.0/axios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-14 20:41:31.000000 axios-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:41:46.069734 axios-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-14 20:41:31.000000 axios-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:41:46.069734 axios-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-14 20:41:31.000000 axios-0.4.0/tests/test_axios.py
```

### Comparing `axios-0.3.0/PKG-INFO` & `axios-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axios
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command line utility to access https://family.axioscloud.it
 Home-page: https://github.com/zmoog/axios
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/axios/issues
 Project-URL: CI, https://github.com/zmoog/axios/actions
 Project-URL: Changelog, https://github.com/zmoog/axios/releases
@@ -41,65 +41,65 @@
 To list latest grades, run:
 
     $ axios grades list
                                                                                             Grades
 
       Data         Materia                      Tipo      Voto   Obiettivi   Commento                                                                                Docente
      ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
-      06/12/2022   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
-      02/12/2022   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
-      01/12/2022   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
-      01/12/2022   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
-      30/11/2022   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      24/11/2022   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
-      23/11/2022   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
-      23/11/2022   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      18/11/2022   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
-      16/11/2022   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
-      10/11/2022   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
-      09/11/2022   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
+      2022-12-06   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
+      2022-12-02   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
+      2022-12-01   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
+      2022-12-01   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
+      2022-11-30   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-24   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
+      2022-11-23   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
+      2022-11-23   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-18   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
+      2022-11-16   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
+      2022-11-10   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
+      2022-11-09   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
 
 Defaults to current year and period.
 
 To select a different year or period, run:
 
     # allowed values: FT01 and FT02
     axios --period FT02 grades list 
 
     # the year classes started
     axios --year 2021 grades list 
     
     # you can combine them, of course
     axios --year 2021 --period FT01
 
-To format the output in JSON or JDJSON, run:
+To format the output in JSON or NDJSON, run:
 
     $ axios --output-format json grades list
     [
         {
-            "date": "23/03/2023",
+            "date": "2023-03-23",
             "subject": "ARTE E IMMAGINE",
             "kind": "Grafico",
             "value": "9",
             "teacher": "Pagliarulo Veronica",
             "comment": "Concorso LAV"
         },
         {
-            "date": "20/03/2023",
+            "date": "2023-03-20",
             "subject": "STORIA",
             "kind": "Orale",
             "value": "10",
             "teacher": "Novelli Cristina",
             "comment": ""
         }
     ]
 
     $ axios --output-format ndjson grades list
-    {"date": "23/03/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
-    {"date": "20/03/2023", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
+    {"date": "2023-03-23", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
+    {"date": "2023-03-20", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
 
 For help, run:
 
     axios --help
 
 You can also use:
```

### Comparing `axios-0.3.0/README.md` & `axios-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,65 +27,65 @@
 To list latest grades, run:
 
     $ axios grades list
                                                                                             Grades
 
       Data         Materia                      Tipo      Voto   Obiettivi   Commento                                                                                Docente
      ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
-      06/12/2022   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
-      02/12/2022   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
-      01/12/2022   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
-      01/12/2022   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
-      30/11/2022   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      24/11/2022   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
-      23/11/2022   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
-      23/11/2022   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      18/11/2022   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
-      16/11/2022   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
-      10/11/2022   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
-      09/11/2022   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
+      2022-12-06   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
+      2022-12-02   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
+      2022-12-01   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
+      2022-12-01   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
+      2022-11-30   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-24   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
+      2022-11-23   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
+      2022-11-23   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-18   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
+      2022-11-16   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
+      2022-11-10   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
+      2022-11-09   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
 
 Defaults to current year and period.
 
 To select a different year or period, run:
 
     # allowed values: FT01 and FT02
     axios --period FT02 grades list 
 
     # the year classes started
     axios --year 2021 grades list 
     
     # you can combine them, of course
     axios --year 2021 --period FT01
 
-To format the output in JSON or JDJSON, run:
+To format the output in JSON or NDJSON, run:
 
     $ axios --output-format json grades list
     [
         {
-            "date": "23/03/2023",
+            "date": "2023-03-23",
             "subject": "ARTE E IMMAGINE",
             "kind": "Grafico",
             "value": "9",
             "teacher": "Pagliarulo Veronica",
             "comment": "Concorso LAV"
         },
         {
-            "date": "20/03/2023",
+            "date": "2023-03-20",
             "subject": "STORIA",
             "kind": "Orale",
             "value": "10",
             "teacher": "Novelli Cristina",
             "comment": ""
         }
     ]
 
     $ axios --output-format ndjson grades list
-    {"date": "23/03/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
-    {"date": "20/03/2023", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
+    {"date": "2023-03-23", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
+    {"date": "2023-03-20", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
 
 For help, run:
 
     axios --help
 
 You can also use:
```

### Comparing `axios-0.3.0/axios/cli.py` & `axios-0.4.0/axios/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     "--period",
     required=True,
     default="FT01" if today.month in [1, 9, 10, 11, 12] else "FT02",
     envvar="AXIOS_STUDENT_PERIOD",
 )
 @click.option(
     "--output-format",
-    type=click.Choice(['json', 'ndjson', 'text'],
-    case_sensitive=False),
+    type=click.Choice(["json", "ndjson", "text"], case_sensitive=False),
     default="text",
 )
 @click.option(
     "-v",
     "--verbose",
     is_flag=True,
     help="Enables verbose mode",
```

### Comparing `axios-0.3.0/axios/navigator.py` & `axios-0.4.0/axios/navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from datetime import date
+from datetime import date, datetime
 from typing import Any, List
 
 import requests
 from lxml import html
 
 from .models import Credentials, Grade, Profile
 
@@ -39,24 +39,23 @@
 class Navigator:
     """Navigator for the Axios Family web application."""
 
     def __init__(
         self,
         credentials: Credentials,
         student_id: str,
-        session: requests.Session = requests.Session(),
         verbose: bool = False,
     ):
         self.credentials = credentials
         self.state = State(
             year=today.year if 9 <= today.month <= 12 else today.year - 1,
             period="FT01" if 9 < today.month < 2 else "FT02",
             student_id=student_id,
         )
-        self.session = session
+        self.session = requests.Session()
         self.verbose = verbose
 
     def login(self) -> Profile:
         """Login to the Axios Family web application."""
 
         start_url = START_URL + self.credentials.customer_id
 
@@ -151,15 +150,17 @@
         self.state.update_from(tree)
 
         rows = tree.xpath('//div[@id="votiEle"]/div/table/tbody/tr')
         grades = []
         for row in rows:
             grades.append(
                 Grade(
-                    date=first(row.xpath("td[1]/text()")),
+                    date=datetime.strptime(
+                        first(row.xpath("td[1]/text()")), "%d/%m/%Y"
+                    ),
                     subject=first(row.xpath("td[2]/text()")),
                     kind=first(row.xpath("td[3]/text()")),
                     value=first(row.xpath("td[4]/span/text()")),
                     # target=first(row.xpath("td[5]/text()")),
                     comment=first(row.xpath("td[6]/text()")),
                     teacher=first(row.xpath("td[7]/text()")),
                 )
@@ -167,17 +168,17 @@
 
         return grades
 
     def select_student(self, student_id: str) -> None:
         """Select the student"""
         self.state.student_id = student_id
 
-    def select_year(self, year: int, day=date.today()) -> None:
+    def select_year(self, year: int, day=None) -> None:
         """Select the year"""
-
+        day = day or date.today()
         if self.state.year == year:
             if self.verbose:
                 print(
                     "optimization: year is unchanged, we can avoid making a network call"
                 )
             return
```

### Comparing `axios-0.3.0/axios/result.py` & `axios-0.4.0/axios/result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import dataclasses
+import datetime
 import io
 import json
 from typing import Any, List
 
 from rich import box
 from rich.console import Console
 from rich.table import Table
@@ -18,31 +18,38 @@
         return result.json()
     elif output_format == "ndjson":
         return result.ndjson()
     else:
         raise ValueError("Unknown format: " + output_format)
 
 
+class DateTimeEncoder(json.JSONEncoder):
+    """JSON encoder for object containing datetime values."""
+
+    def default(self, obj):
+        if isinstance(obj, (datetime.date, datetime.datetime)):
+            return obj.isoformat()
+
+
 class GradesListResult:
-    
     def __init__(self, grades: List[Grade]) -> None:
         self.grades = grades
 
     def __str__(self) -> str:
         table = Table(title="Grades", box=box.SIMPLE)
         table.add_column("Data")
         table.add_column("Materia")
         table.add_column("Tipo")
         table.add_column("Voto")
         table.add_column("Commento")
         table.add_column("Docente")
 
         for g in self.grades:
             table.add_row(
-                str(g.date),
+                str(g.date.strftime("%Y-%m-%d")),
                 str(g.subject),
                 str(g.kind),
                 str(g.value),
                 str(g.comment),
                 str(g.teacher),
             )
 
@@ -52,11 +59,15 @@
         # turn table into a string using the Console
         console = Console(file=output)
         console.print(table)
 
         return output.getvalue()
 
     def json(self) -> str:
-        return json.dumps([g.__dict__ for g in self.grades])
+        return json.dumps(
+            [g.__dict__ for g in self.grades], cls=DateTimeEncoder
+        )
 
     def ndjson(self) -> str:
-        return "\n".join([json.dumps(g.__dict__) for g in self.grades])
+        return "\n".join(
+            [json.dumps(g.__dict__, cls=DateTimeEncoder) for g in self.grades],
+        )
```

### Comparing `axios-0.3.0/axios.egg-info/PKG-INFO` & `axios-0.4.0/axios.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axios
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command line utility to access https://family.axioscloud.it
 Home-page: https://github.com/zmoog/axios
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/axios/issues
 Project-URL: CI, https://github.com/zmoog/axios/actions
 Project-URL: Changelog, https://github.com/zmoog/axios/releases
@@ -41,65 +41,65 @@
 To list latest grades, run:
 
     $ axios grades list
                                                                                             Grades
 
       Data         Materia                      Tipo      Voto   Obiettivi   Commento                                                                                Docente
      ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
-      06/12/2022   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
-      02/12/2022   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
-      01/12/2022   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
-      01/12/2022   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
-      30/11/2022   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      24/11/2022   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
-      23/11/2022   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
-      23/11/2022   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
-      18/11/2022   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
-      16/11/2022   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
-      10/11/2022   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
-      09/11/2022   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
+      2022-12-06   TECNOLOGIA e INFORMATICA     Scritto   7.5                                                                                                        Pavarin Maria Luisa
+      2022-12-02   MATEMATICA                   Scritto   7,75               Verifica sugli insiemi                                                                  Micela Silvia
+      2022-12-01   ARTE E IMMAGINE              Grafico   10                 Tav.3 figura e sfondo                                                                   Pagliarulo Veronica
+      2022-12-01   ARTE E IMMAGINE              Grafico   7/8                Tav.1 Punto e linea                                                                     Pagliarulo Veronica
+      2022-11-30   MUSICA                       Orale     7                  Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-24   ITALIANO                     Scritto   8.5                Fonologia e ortografia                                                                  Rapalino Lara
+      2022-11-23   TECNOLOGIA e INFORMATICA     Grafico   6.5                                                                                                        Pavarin Maria Luisa
+      2022-11-23   MUSICA                       Orale     7,5                Verifica di carattere teorico. Interrogazione su tutto il programma svolto finora.      Cataldo Francesco
+      2022-11-18   MATEMATICA                   Grafico   8,5                Verifica sulle equivalenze e le operazioni con le misure del tempo                      Micela Silvia
+      2022-11-16   TECNOLOGIA e INFORMATICA     Grafico   7                                                                                                          Pavarin Maria Luisa
+      2022-11-10   ARTE E IMMAGINE              Grafico   8                  Poster per la pace                                                                      Pagliarulo Veronica
+      2022-11-09   LINGUA STRANIERA INGLESE     Scritto   8,5                Test units 1 e 2                                                                        Barbero Daniela
 
 Defaults to current year and period.
 
 To select a different year or period, run:
 
     # allowed values: FT01 and FT02
     axios --period FT02 grades list 
 
     # the year classes started
     axios --year 2021 grades list 
     
     # you can combine them, of course
     axios --year 2021 --period FT01
 
-To format the output in JSON or JDJSON, run:
+To format the output in JSON or NDJSON, run:
 
     $ axios --output-format json grades list
     [
         {
-            "date": "23/03/2023",
+            "date": "2023-03-23",
             "subject": "ARTE E IMMAGINE",
             "kind": "Grafico",
             "value": "9",
             "teacher": "Pagliarulo Veronica",
             "comment": "Concorso LAV"
         },
         {
-            "date": "20/03/2023",
+            "date": "2023-03-20",
             "subject": "STORIA",
             "kind": "Orale",
             "value": "10",
             "teacher": "Novelli Cristina",
             "comment": ""
         }
     ]
 
     $ axios --output-format ndjson grades list
-    {"date": "23/03/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
-    {"date": "20/03/2023", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
+    {"date": "2023-03-23", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
+    {"date": "2023-03-20", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
 
 For help, run:
 
     axios --help
 
 You can also use:
```

### Comparing `axios-0.3.0/setup.py` & `axios-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -46,11 +46,12 @@
             "pytest-recording",
             "ruff",
             "types-colorama",
             "types-lxml",
             "types-Pygments",
             "types-requests",
             "types-setuptools",
+            "urllib3<2",
         ]
     },
     python_requires=">=3.8",
 )
```

### Comparing `axios-0.3.0/tests/test_axios.py` & `axios-0.4.0/tests/test_axios.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,229 +55,233 @@
             #
             # And then copy the output from the file in the assert.
             result.output
             == """                                     Grades                                     
                                                                                 
   Data         Materia         Tipo      Voto   Commento         Docente        
  ────────────────────────────────────────────────────────────────────────────── 
-  31/01/2023   ARTE E          Grafico   10     Pittura          Pagliarulo     
+  2023-01-31   ARTE E          Grafico   10     Pittura          Pagliarulo     
                IMMAGINE                         rupestre         Veronica       
-  27/01/2023   SCIENZE         Pratico   8      IMPEGNO E        Vogliotti      
+  2023-01-27   SCIENZE         Pratico   8      IMPEGNO E        Vogliotti      
                MOTORIE E                        PARTECIPAZIONE   Enzo           
                SPORTIVE                                                         
-  27/01/2023   SCIENZE         Pratico   7      VALUTAZIONE      Vogliotti      
+  2023-01-27   SCIENZE         Pratico   7      VALUTAZIONE      Vogliotti      
                MOTORIE E                        TEST FISICI      Enzo           
                SPORTIVE                         ATTITUDINALI                    
-  26/01/2023   MUSICA          Pratico   7.5    Verifica di      Cataldo        
+  2023-01-26   MUSICA          Pratico   7.5    Verifica di      Cataldo        
                                                 carattere        Francesco      
                                                 pratico.                        
-  25/01/2023   STORIA          Orale     9                       Novelli        
+  2023-01-25   STORIA          Orale     9                       Novelli        
                                                                  Cristina       
-  25/01/2023   TECNOLOGIA e    Scritto   8                       Pavarin Maria  
+  2023-01-25   TECNOLOGIA e    Scritto   8                       Pavarin Maria  
                INFORMATICA                                       Luisa          
-  24/01/2023   SCIENZE         Scritto   9      Verifica         Micela Silvia  
+  2023-01-24   SCIENZE         Scritto   9      Verifica         Micela Silvia  
                                                 scritta                         
                                                 sull'organizz…                  
                                                 dei viventi                     
-  23/01/2023   RELIGIONE       Orale     7                       Avanzato       
+  2023-01-23   RELIGIONE       Orale     7                       Avanzato       
                                                                  Paola Carla    
-  20/01/2023   ITALIANO        Orale     7.5    Presentazione    Rapalino Lara  
+  2023-01-20   ITALIANO        Orale     7.5    Presentazione    Rapalino Lara  
                                                 libro                           
-  19/01/2023   EDUCAZIONE      Scritto   8,5    Verifica di      Micela Silvia  
+  2023-01-19   EDUCAZIONE      Scritto   8,5    Verifica di      Micela Silvia  
                CIVICA                           educazione                      
                                                 civica di                       
                                                 italiano sulla                  
                                                 comprensione                    
                                                 del testo                       
-  19/01/2023   ITALIANO        Scritto   8.5    Verifica di      Rapalino Lara  
+  2023-01-19   ITALIANO        Scritto   8.5    Verifica di      Rapalino Lara  
                                                 Educazione                      
                                                 Civica (il                      
                                                 voto fa media                   
                                                 con le altre                    
                                                 valutazioni di                  
                                                 Ed. Civica, ma                  
                                                 non con quelle                  
                                                 di Italiano):                   
                                                 il rapporto                     
                                                 tra uomini e                    
                                                 animali                         
                                                 (comprensione                   
                                                 del testo)                      
-  18/01/2023   LINGUA          Scritto   9,75   Verifica units   Barbero        
+  2023-01-18   LINGUA          Scritto   9,75   Verifica units   Barbero        
                STRANIERA                        3-4              Daniela        
                INGLESE                                                          
-  17/01/2023   ITALIANO        Scritto   9+     Grammatica:      Rapalino Lara  
+  2023-01-17   ITALIANO        Scritto   9+     Grammatica:      Rapalino Lara  
                                                 l'articolo                      
-  16/01/2023   STORIA          Scritto   7.7                     Novelli        
+  2023-01-16   STORIA          Scritto   7.7                     Novelli        
                                                                  Cristina       
-  13/01/2023   MATEMATICA      Scritto   8,75   Verifica         Micela Silvia  
+  2023-01-13   MATEMATICA      Scritto   8,75   Verifica         Micela Silvia  
                                                 scritta sui                     
                                                 numeri                          
                                                 naturali e                      
                                                 decimali                        
-  12/01/2023   ARTE E          Grafico   8      Paesaggio        Pagliarulo     
+  2023-01-12   ARTE E          Grafico   8      Paesaggio        Pagliarulo     
                IMMAGINE                                          Veronica       
-  12/01/2023   ARTE E          Grafico   9      Colori caldi e   Pagliarulo     
+  2023-01-12   ARTE E          Grafico   9      Colori caldi e   Pagliarulo     
                IMMAGINE                         freddi           Veronica       
-  11/01/2023   STORIA          Scritto   7.3                     Novelli        
+  2023-01-11   STORIA          Scritto   7.3                     Novelli        
                                                                  Cristina       
-  10/01/2023   EDUCAZIONE      Scritto   7,5    Verifica         Micela Silvia  
+  2023-01-10   EDUCAZIONE      Scritto   7,5    Verifica         Micela Silvia  
                CIVICA                           scritta di                      
                                                 educazione                      
                                                 civica -                        
                                                 Tecnologia                      
-  23/12/2022   LINGUA          Scritto   8      Da risentire     Giovannini     
+  2022-12-23   LINGUA          Scritto   8      Da risentire     Giovannini     
                STRANIERA                        sul verbo        Sonia          
                FRANCESE                         essere.                         
-  23/12/2022   ITALIANO        Scritto   6.5    Tema in classe   Rapalino Lara  
-  22/12/2022   LINGUA          Orale     8,5    Interrogazione   Barbero        
+  2022-12-23   ITALIANO        Scritto   6.5    Tema in classe   Rapalino Lara  
+  2022-12-22   LINGUA          Orale     8,5    Interrogazione   Barbero        
                STRANIERA                                         Daniela        
                INGLESE                                                          
-  21/12/2022   SCIENZE         Scritto   8      Verifica         Micela Silvia  
+  2022-12-21   SCIENZE         Scritto   8      Verifica         Micela Silvia  
                                                 scritta sugli                   
                                                 stati di                        
                                                 aggregazione e                  
                                                 i passaggi di                   
                                                 stato                           
-  19/12/2022   ITALIANO        Scritto   8-     La favola:       Rapalino Lara  
+  2022-12-19   ITALIANO        Scritto   8-     La favola:       Rapalino Lara  
                                                 comprensione                    
                                                 del testo e                     
                                                 verifica delle                  
                                                 conoscenze                      
-  15/12/2022   SCIENZE         Pratico   8      Verifica         Vogliotti      
+  2022-12-15   SCIENZE         Pratico   8      Verifica         Vogliotti      
                MOTORIE E                        intermedia       Enzo           
                SPORTIVE                         test di                         
                                                 resistenza:                     
                                                 Cooper (6                       
                                                 minuti)                         
-  13/12/2022   TECNOLOGIA e    Grafico   7                       Pavarin Maria  
+  2022-12-13   TECNOLOGIA e    Grafico   7                       Pavarin Maria  
                INFORMATICA                                       Luisa          
-  12/12/2022   GEOGRAFIA       Scritto   6.7                     Novelli        
+  2022-12-12   GEOGRAFIA       Scritto   6.7                     Novelli        
                                                                  Cristina       
-  06/12/2022   TECNOLOGIA e    Scritto   7.5                     Pavarin Maria  
+  2022-12-06   TECNOLOGIA e    Scritto   7.5                     Pavarin Maria  
                INFORMATICA                                       Luisa          
-  05/12/2022   RELIGIONE       Orale     8.5    VALUTAZIONE      Avanzato       
+  2022-12-05   RELIGIONE       Orale     8.5    VALUTAZIONE      Avanzato       
                                                 PARTECIPAZIONE   Paola Carla    
-  02/12/2022   MATEMATICA      Scritto   7,75   Verifica sugli   Micela Silvia  
+  2022-12-02   MATEMATICA      Scritto   7,75   Verifica sugli   Micela Silvia  
                                                 insiemi                         
-  01/12/2022   ARTE E          Grafico   10     Tav.3 figura e   Pagliarulo     
+  2022-12-01   ARTE E          Grafico   10     Tav.3 figura e   Pagliarulo     
                IMMAGINE                         sfondo           Veronica       
-  01/12/2022   ARTE E          Grafico   7/8    Tav.1 Punto e    Pagliarulo     
+  2022-12-01   ARTE E          Grafico   7/8    Tav.1 Punto e    Pagliarulo     
                IMMAGINE                         linea            Veronica       
-  30/11/2022   MUSICA          Orale     7      Verifica di      Cataldo        
+  2022-11-30   MUSICA          Orale     7      Verifica di      Cataldo        
                                                 carattere        Francesco      
                                                 teorico.                        
                                                 Interrogazione                  
                                                 su tutto il                     
                                                 programma                       
                                                 svolto finora.                  
-  24/11/2022   ITALIANO        Scritto   8.5    Fonologia e      Rapalino Lara  
+  2022-11-24   ITALIANO        Scritto   8.5    Fonologia e      Rapalino Lara  
                                                 ortografia                      
-  23/11/2022   TECNOLOGIA e    Grafico   6.5                     Pavarin Maria  
+  2022-11-23   TECNOLOGIA e    Grafico   6.5                     Pavarin Maria  
                INFORMATICA                                       Luisa          
-  23/11/2022   MUSICA          Orale     7,5    Verifica di      Cataldo        
+  2022-11-23   MUSICA          Orale     7,5    Verifica di      Cataldo        
                                                 carattere        Francesco      
                                                 teorico.                        
                                                 Interrogazione                  
                                                 su tutto il                     
                                                 programma                       
                                                 svolto finora.                  
-  18/11/2022   MATEMATICA      Grafico   8,5    Verifica sulle   Micela Silvia  
+  2022-11-18   MATEMATICA      Grafico   8,5    Verifica sulle   Micela Silvia  
                                                 equivalenze e                   
                                                 le operazioni                   
                                                 con le misure                   
                                                 del tempo                       
-  16/11/2022   TECNOLOGIA e    Grafico   7                       Pavarin Maria  
+  2022-11-16   TECNOLOGIA e    Grafico   7                       Pavarin Maria  
                INFORMATICA                                       Luisa          
-  10/11/2022   ARTE E          Grafico   8      Poster per la    Pagliarulo     
+  2022-11-10   ARTE E          Grafico   8      Poster per la    Pagliarulo     
                IMMAGINE                         pace             Veronica       
-  09/11/2022   LINGUA          Scritto   8,5    Test units 1 e   Barbero        
+  2022-11-09   LINGUA          Scritto   8,5    Test units 1 e   Barbero        
                STRANIERA                        2                Daniela        
                INGLESE                                                          
-  08/11/2022   LINGUA          Scritto   8      Verifica unità   Giovannini     
+  2022-11-08   LINGUA          Scritto   8      Verifica unità   Giovannini     
                STRANIERA                        1                Sonia          
                FRANCESE                                                         
-  28/10/2022   MATEMATICA      Scritto   8,5    Verifica di      Micela Silvia  
+  2022-10-28   MATEMATICA      Scritto   8,5    Verifica di      Micela Silvia  
                                                 aritmetica                      
                                                 sulle                           
                                                 rappresentazi…                  
                                                 grafiche                        
-  26/10/2022   ITALIANO        Orale     7.5    La leggenda      Rapalino Lara  
-  25/10/2022   SCIENZE         Scritto   7,75                    Micela Silvia  
-  24/10/2022   ITALIANO        Scritto   8.5    Prova di         Rapalino Lara  
+  2022-10-26   ITALIANO        Orale     7.5    La leggenda      Rapalino Lara  
+  2022-10-25   SCIENZE         Scritto   7,75                    Micela Silvia  
+  2022-10-24   ITALIANO        Scritto   8.5    Prova di         Rapalino Lara  
                                                 comprensione                    
                                                 del testo                       
-  20/10/2022   LINGUA          Scritto   9,5    Verifica unit    Barbero        
+  2022-10-20   LINGUA          Scritto   9,5    Verifica unit    Barbero        
                STRANIERA                        1                Daniela        
                INGLESE                                                          
-  20/10/2022   MUSICA          Pratico   6,5    Verifica di      Cataldo        
+  2022-10-20   MUSICA          Pratico   6,5    Verifica di      Cataldo        
                                                 carattere        Francesco      
                                                 pratico.                        
                                                 Conoscenza                      
                                                 delle prime 5                   
                                                 note,                           
                                                 posizioni                       
                                                 delle dita                      
                                                 sullo                           
                                                 strumento,                      
                                                 qualità del                     
                                                 suono.                          
-  19/10/2022   SCIENZE         Pratico   7      Valutazione      Vogliotti      
+  2022-10-19   SCIENZE         Pratico   7      Valutazione      Vogliotti      
                MOTORIE E                        test fisici      Enzo           
                SPORTIVE                         attitudinali                    
-  18/10/2022   LINGUA          Orale     8      Interrogazione   Giovannini     
+  2022-10-18   LINGUA          Orale     8      Interrogazione   Giovannini     
                STRANIERA                        u1 fino alle     Sonia          
                FRANCESE                         materie                         
                                                 scolastiche                     
-  17/10/2022   STORIA          Scritto   8.3                     Novelli        
+  2022-10-17   STORIA          Scritto   8.3                     Novelli        
                                                                  Cristina       
-  26/09/2022   STORIA          Orale     8                       Novelli        
+  2022-09-26   STORIA          Orale     8                       Novelli        
                                                                  Cristina       
                                                                                 
 
-"""
+"""  # noqa: W291 W293
         )
 
 
 @pytest.mark.vcr(filter_query_parameters=["txtUser", "txtPassword"])
 @pytest.mark.block_network
 def test_grades_list_json():
     runner = CliRunner()
     with runner.isolated_filesystem():
-        result = runner.invoke(cli, ["--output-format", "json", "grades", "list"], env=env)
+        result = runner.invoke(
+            cli, ["--output-format", "json", "grades", "list"], env=env
+        )
         with open("/tmp/sample.txt", "w") as f:
             f.write(result.output)
 
-        expected = '[{"date": "20/03/2023", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}, {"date": "17/03/2023", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "Presentazione orale del libro letto"}, {"date": "16/03/2023", "subject": "LINGUA STRANIERA INGLESE", "kind": "Scritto", "value": "8,25", "teacher": "Barbero Daniela", "comment": "Verifica units 5-6"}, {"date": "15/03/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "08/03/2023", "subject": "ITALIANO", "kind": "Scritto", "value": "8.5", "teacher": "Rapalino Lara", "comment": "Epica: epica omerica e Iliade"}, {"date": "08/03/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8.5", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "06/03/2023", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "La fiaba"}, {"date": "02/03/2023", "subject": "SCIENZE", "kind": "Scritto", "value": "8,75", "teacher": "Micela Silvia", "comment": ""}, {"date": "22/02/2023", "subject": "GEOGRAFIA", "kind": "Orale", "value": "7.75", "teacher": "Gardello Martina", "comment": ""}, {"date": "17/02/2023", "subject": "MATEMATICA", "kind": "Scritto", "value": "9", "teacher": "Micela Silvia", "comment": "Verifica scritta di aritmetica sulle quattro operazioni e le loro propriet\\u00e0."}, {"date": "16/02/2023", "subject": "MUSICA", "kind": "Scritto", "value": "6", "teacher": "Cataldo Francesco", "comment": "Verifica scritta di carattere teorico."}, {"date": "16/02/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Arte egizia"}, {"date": "15/02/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Scritto", "value": "8.75", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "07/02/2023", "subject": "LINGUA STRANIERA FRANCESE", "kind": "Scritto", "value": "8", "teacher": "Giovannini Sonia", "comment": "Verifica Unit\\u00e9 3"}]\n'
+        expected = '[{"date": "2023-03-20T00:00:00", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}, {"date": "2023-03-17T00:00:00", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "Presentazione orale del libro letto"}, {"date": "2023-03-16T00:00:00", "subject": "LINGUA STRANIERA INGLESE", "kind": "Scritto", "value": "8,25", "teacher": "Barbero Daniela", "comment": "Verifica units 5-6"}, {"date": "2023-03-15T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "2023-03-08T00:00:00", "subject": "ITALIANO", "kind": "Scritto", "value": "8.5", "teacher": "Rapalino Lara", "comment": "Epica: epica omerica e Iliade"}, {"date": "2023-03-08T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8.5", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "2023-03-06T00:00:00", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "La fiaba"}, {"date": "2023-03-02T00:00:00", "subject": "SCIENZE", "kind": "Scritto", "value": "8,75", "teacher": "Micela Silvia", "comment": ""}, {"date": "2023-02-22T00:00:00", "subject": "GEOGRAFIA", "kind": "Orale", "value": "7.75", "teacher": "Gardello Martina", "comment": ""}, {"date": "2023-02-17T00:00:00", "subject": "MATEMATICA", "kind": "Scritto", "value": "9", "teacher": "Micela Silvia", "comment": "Verifica scritta di aritmetica sulle quattro operazioni e le loro propriet\\u00e0."}, {"date": "2023-02-16T00:00:00", "subject": "MUSICA", "kind": "Scritto", "value": "6", "teacher": "Cataldo Francesco", "comment": "Verifica scritta di carattere teorico."}, {"date": "2023-02-16T00:00:00", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Arte egizia"}, {"date": "2023-02-15T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Scritto", "value": "8.75", "teacher": "Pavarin Maria Luisa", "comment": ""}, {"date": "2023-02-07T00:00:00", "subject": "LINGUA STRANIERA FRANCESE", "kind": "Scritto", "value": "8", "teacher": "Giovannini Sonia", "comment": "Verifica Unit\\u00e9 3"}]\n'
 
         assert result.exit_code == 0, result.output
         assert result.output == expected
 
 
 @pytest.mark.vcr(filter_query_parameters=["txtUser", "txtPassword"])
 @pytest.mark.block_network
 def test_grades_list_ndjson():
     runner = CliRunner()
     with runner.isolated_filesystem():
-        result = runner.invoke(cli, ["--output-format", "ndjson", "grades", "list"], env=env)
+        result = runner.invoke(
+            cli, ["--output-format", "ndjson", "grades", "list"], env=env
+        )
         with open("/tmp/sample.txt", "w") as f:
             f.write(result.output)
 
-        expected = """{"date": "23/03/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
-{"date": "20/03/2023", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
-{"date": "17/03/2023", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "Presentazione orale del libro letto"}
-{"date": "16/03/2023", "subject": "LINGUA STRANIERA INGLESE", "kind": "Scritto", "value": "8,25", "teacher": "Barbero Daniela", "comment": "Verifica units 5-6"}
-{"date": "15/03/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8", "teacher": "Pavarin Maria Luisa", "comment": ""}
-{"date": "08/03/2023", "subject": "ITALIANO", "kind": "Scritto", "value": "8.5", "teacher": "Rapalino Lara", "comment": "Epica: epica omerica e Iliade"}
-{"date": "08/03/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8.5", "teacher": "Pavarin Maria Luisa", "comment": ""}
-{"date": "06/03/2023", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "La fiaba"}
-{"date": "02/03/2023", "subject": "SCIENZE", "kind": "Scritto", "value": "8,75", "teacher": "Micela Silvia", "comment": ""}
-{"date": "22/02/2023", "subject": "GEOGRAFIA", "kind": "Orale", "value": "7.75", "teacher": "Gardello Martina", "comment": ""}
-{"date": "17/02/2023", "subject": "MATEMATICA", "kind": "Scritto", "value": "9", "teacher": "Micela Silvia", "comment": "Verifica scritta di aritmetica sulle quattro operazioni e le loro propriet\\u00e0."}
-{"date": "16/02/2023", "subject": "MUSICA", "kind": "Scritto", "value": "6", "teacher": "Cataldo Francesco", "comment": "Verifica scritta di carattere teorico."}
-{"date": "16/02/2023", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Arte egizia"}
-{"date": "15/02/2023", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Scritto", "value": "8.75", "teacher": "Pavarin Maria Luisa", "comment": ""}
-{"date": "07/02/2023", "subject": "LINGUA STRANIERA FRANCESE", "kind": "Scritto", "value": "8", "teacher": "Giovannini Sonia", "comment": "Verifica Unit\\u00e9 3"}
+        expected = """{"date": "2023-03-23T00:00:00", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Concorso LAV"}
+{"date": "2023-03-20T00:00:00", "subject": "STORIA", "kind": "Orale", "value": "10", "teacher": "Novelli Cristina", "comment": ""}
+{"date": "2023-03-17T00:00:00", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "Presentazione orale del libro letto"}
+{"date": "2023-03-16T00:00:00", "subject": "LINGUA STRANIERA INGLESE", "kind": "Scritto", "value": "8,25", "teacher": "Barbero Daniela", "comment": "Verifica units 5-6"}
+{"date": "2023-03-15T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8", "teacher": "Pavarin Maria Luisa", "comment": ""}
+{"date": "2023-03-08T00:00:00", "subject": "ITALIANO", "kind": "Scritto", "value": "8.5", "teacher": "Rapalino Lara", "comment": "Epica: epica omerica e Iliade"}
+{"date": "2023-03-08T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Grafico", "value": "8.5", "teacher": "Pavarin Maria Luisa", "comment": ""}
+{"date": "2023-03-06T00:00:00", "subject": "ITALIANO", "kind": "Orale", "value": "8", "teacher": "Rapalino Lara", "comment": "La fiaba"}
+{"date": "2023-03-02T00:00:00", "subject": "SCIENZE", "kind": "Scritto", "value": "8,75", "teacher": "Micela Silvia", "comment": ""}
+{"date": "2023-02-22T00:00:00", "subject": "GEOGRAFIA", "kind": "Orale", "value": "7.75", "teacher": "Gardello Martina", "comment": ""}
+{"date": "2023-02-17T00:00:00", "subject": "MATEMATICA", "kind": "Scritto", "value": "9", "teacher": "Micela Silvia", "comment": "Verifica scritta di aritmetica sulle quattro operazioni e le loro propriet\\u00e0."}
+{"date": "2023-02-16T00:00:00", "subject": "MUSICA", "kind": "Scritto", "value": "6", "teacher": "Cataldo Francesco", "comment": "Verifica scritta di carattere teorico."}
+{"date": "2023-02-16T00:00:00", "subject": "ARTE E IMMAGINE", "kind": "Grafico", "value": "9", "teacher": "Pagliarulo Veronica", "comment": "Arte egizia"}
+{"date": "2023-02-15T00:00:00", "subject": "TECNOLOGIA e INFORMATICA", "kind": "Scritto", "value": "8.75", "teacher": "Pavarin Maria Luisa", "comment": ""}
+{"date": "2023-02-07T00:00:00", "subject": "LINGUA STRANIERA FRANCESE", "kind": "Scritto", "value": "8", "teacher": "Giovannini Sonia", "comment": "Verifica Unit\\u00e9 3"}
 """
 
         assert result.exit_code == 0, result.output
         assert result.output == expected
```

