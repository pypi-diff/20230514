# Comparing `tmp/reytool-0.98-py3-none-any.whl.zip` & `tmp/reytool-0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30413 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat      689 b- defN 23-Mar-30 02:58 reytool/__init__.py
+Zip file size: 30399 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat      689 b- defN 23-Mar-30 03:12 reytool/__init__.py
 -rw-rw-rw-  2.0 fat     9488 b- defN 23-Mar-22 06:06 reytool/rbasic.py
 -rw-rw-rw-  2.0 fat     8690 b- defN 23-Mar-22 06:07 reytool/rcommon.py
 -rw-rw-rw-  2.0 fat     3271 b- defN 23-Mar-21 09:55 reytool/rcompress.py
 -rw-rw-rw-  2.0 fat    11618 b- defN 23-Mar-27 05:35 reytool/rdata.py
 -rw-rw-rw-  2.0 fat    22814 b- defN 23-Mar-29 14:19 reytool/rdatabase.py
 -rw-rw-rw-  2.0 fat    16116 b- defN 23-Mar-23 02:47 reytool/rdatetime.py
--rw-rw-rw-  2.0 fat     6809 b- defN 23-Mar-30 02:59 reytool/remail.py
+-rw-rw-rw-  2.0 fat     6097 b- defN 23-Mar-30 03:12 reytool/remail.py
 -rw-rw-rw-  2.0 fat     4045 b- defN 23-Mar-22 06:00 reytool/rmonkey.py
 -rw-rw-rw-  2.0 fat     3054 b- defN 23-Mar-22 06:09 reytool/rmultitask.py
 -rw-rw-rw-  2.0 fat      786 b- defN 23-Mar-21 09:55 reytool/roption.py
 -rw-rw-rw-  2.0 fat     2607 b- defN 23-Mar-22 06:00 reytool/rregular.py
 -rw-rw-rw-  2.0 fat     5173 b- defN 23-Mar-22 06:11 reytool/rrequest.py
 -rw-rw-rw-  2.0 fat     8760 b- defN 23-Mar-22 06:10 reytool/rtext.py
 -rw-rw-rw-  2.0 fat     8402 b- defN 23-Mar-24 07:00 reytool/rwrap.py
--rw-rw-rw-  2.0 fat      370 b- defN 23-Mar-30 02:59 reytool-0.98.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-30 02:59 reytool-0.98.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-30 02:59 reytool-0.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1422 b- defN 23-Mar-30 02:59 reytool-0.98.dist-info/RECORD
-19 files, 114214 bytes uncompressed, 28151 bytes compressed:  75.4%
+-rw-rw-rw-  2.0 fat      370 b- defN 23-Mar-30 03:12 reytool-0.99.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-30 03:12 reytool-0.99.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-30 03:12 reytool-0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1422 b- defN 23-Mar-30 03:12 reytool-0.99.dist-info/RECORD
+19 files, 113502 bytes uncompressed, 28137 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: reytool/rtext.py
 Comment: 
 
 Filename: reytool/rwrap.py
 Comment: 
 
-Filename: reytool-0.98.dist-info/METADATA
+Filename: reytool-0.99.dist-info/METADATA
 Comment: 
 
-Filename: reytool-0.98.dist-info/WHEEL
+Filename: reytool-0.99.dist-info/WHEEL
 Comment: 
 
-Filename: reytool-0.98.dist-info/top_level.txt
+Filename: reytool-0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: reytool-0.98.dist-info/RECORD
+Filename: reytool-0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reytool/__init__.py

```diff
@@ -22,8 +22,8 @@
 from . import roption
 from .rregular import res
 from .rrequest import request
 from .rtext import rprint
 from .rwrap import runtime
 
 
-__version__: Final[str] = "0.98"
+__version__: Final[str] = "0.99"
```

## reytool/remail.py

```diff
@@ -56,37 +56,25 @@
     ) -> str:
         """
         Create string in E-mail format.
 
         Parameters
         ----------
         text : E-mail text.
-            - None : Not set.
-            - str : Set this value.
-
         title : E-mail title.
-            - None : Not set.
-            - str : Set this value.
-
         attachment : E-mail attachment.
-            - None : Not set.
             - Dict[str, str] : File name and path.
             - Dict[str, bytes] : File name and stream.
 
         display_from_email : Displayed from E-mail.
-            - None : Not set.
-            - str : Set this value.
-
         display_to_email : Displayed to E-mail.
-            - None : Not set.
             - str : Set this value.
             - Iterable[str] : Set multiple values.
 
         display_cc_email : Displayed cc E-mail.
-            - None : Not set.
             - str : Set this value.
             - Iterable[str] : Set multiple values.
 
         Returns
         -------
         String in E-mail format.
         """
@@ -125,79 +113,64 @@
         # Create string in E-mail format.
         email_str = mime.as_string()
 
         return email_str
 
     def send_email(
         self,
+        to_email: Union[str, Iterable[str]],
         text: Optional[str] = None,
         title: Optional[str] = None,
         attachment: Optional[Dict[str, Union[str, bytes]]] = None,
-        to_email: Optional[Union[str, Iterable[str]]] = None,
         cc_email: Optional[Union[str, Iterable[str]]] = None,
         display_from_email: Optional[str] = None,
         display_to_email: Optional[Union[str, Iterable[str]]] = None,
         display_cc_email: Optional[Union[str, Iterable[str]]] = None
     ) -> None:
         """
         Send E-mail.
 
         Parameters
         ----------
-        text : E-mail text.
-            - None : Not set.
+        to_email : To E-mail.
             - str : Set this value.
+            - Iterable[str] : Set multiple values.
 
+        text : E-mail text.
         title : E-mail title.
-            - None : Not set.
-            - str : Set this value.
-
         attachment : E-mail attachment.
-            - None : Not set.
             - Dict[str, str] : File name and path.
             - Dict[str, bytes] : File name and stream.
 
-        to_email : To E-mail.
-            - None : Not set.
-            - str : Set this value.
-            - Iterable[str] : Set multiple values.
-
         cc_email : Cc E-mail.
-            - None : Not set.
             - str : Set this value.
             - Iterable[str] : Set multiple values.
 
         display_from_email : Displayed from E-mail.
-            - None : Not set.
-            - str : Set this value.
-
         display_to_email : Displayed to E-mail.
-            - None : Not set.
             - str : Set this value.
             - Iterable[str] : Set multiple values.
 
         display_cc_email : Displayed cc E-mail.
-            - None : Not set.
             - str : Set this value.
             - Iterable[str] : Set multiple values.
         """
 
         # Get parameters by priority.
         display_from_email = get_first_notnull(display_from_email, self.display_from_email, self.email_username)
         display_to_email = get_first_notnull(display_to_email, to_email)
         display_cc_email = get_first_notnull(display_cc_email, cc_email)
 
         # Handle parameters.
         if type(to_email) == str:
             to_email = [to_email]
         if cc_email != None:
             if type(cc_email) == str:
-                to_email.append(cc_email)
-            else:
-                to_email.extend(cc_email)
+                cc_email = [cc_email]
+            to_email.extend(cc_email)
 
         # Create string in E-mail format.
         email_str = self.create_email(title, text, attachment, display_from_email, display_to_email, display_cc_email)
 
         # Send E-mail.
         server_domain_name = self.email_username.split("@")[-1]
         server_host = "smtp." + server_domain_name
```

## Comparing `reytool-0.98.dist-info/RECORD` & `reytool-0.99.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-reytool/__init__.py,sha256=q0-MJg0CmfFtn_0FUbys3HtSFVFCGI43ZIpfpiCakoM,689
+reytool/__init__.py,sha256=XbUVkFcf75Mpcz3qqvVfFIJIUqWe9cQ2FjoZdcCnFic,689
 reytool/rbasic.py,sha256=ByCfh0pF2wAMlS4WxHYSbhpMjao51xLyPM3VGP4PWIE,9488
 reytool/rcommon.py,sha256=21KWXntOPYWRbq7fb_QZDBgalwFveqGm_tzSXxV0-Qg,8690
 reytool/rcompress.py,sha256=NNJP5sJ4DJM7Is_6liI_9UWm4o9QrImhYucGLxmR90g,3271
 reytool/rdata.py,sha256=QC6Zi-xTveJbrVkbyxzN8QgROIEA1FlUpC64lhpTFUo,11618
 reytool/rdatabase.py,sha256=jtuvwlYz9rLEiTkloILTI8t4jf-M-997oa27sNJWO8U,22814
 reytool/rdatetime.py,sha256=F1TQanWlGW3k2XtsXXIAcDR3PRkgi1oemzU8VmcLh3A,16116
-reytool/remail.py,sha256=b-E6jrXWtlW7TiP7fZMkJlf_EElMPvAEqZsTUTGjxK8,6809
+reytool/remail.py,sha256=RC4nEWPrE5jRB_FBiR7h3a73t1tPUIe5FUZKk1z1FTk,6097
 reytool/rmonkey.py,sha256=l4KT3nuxjkDmkkEoRoW8BmK-zNjgXaDx1osrHuZOGQ8,4045
 reytool/rmultitask.py,sha256=Ez7dadQbl7lgYx9E62OXfpGuoCNdGiz2Ul3tL6IqpMg,3054
 reytool/roption.py,sha256=tneCpHg1LWBuIaDdNcWjzuIKsPVDlJ9fuf4dDPQB_p0,786
 reytool/rregular.py,sha256=T2v_xiAWNOlbBnoO0kK3sO9uxQHqcFUudYSphuK0ob8,2607
 reytool/rrequest.py,sha256=8PCpmxwLD2CQzbgh2bbNPrdPe6ZIawCDGmUNtfhq5pc,5173
 reytool/rtext.py,sha256=qqO1FRc84fWEb4PmLoIn6zxQDHUHOEXzPy3Kbd7owWk,8760
 reytool/rwrap.py,sha256=Z33X_DlNE_Pcbtrrqm63xS1ajgDGhaZS5UAczs9WFNg,8402
-reytool-0.98.dist-info/METADATA,sha256=bOolnY-2_m_NJZre2zf2c7C6CANo8Jer_CX-r1hRXVs,370
-reytool-0.98.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-reytool-0.98.dist-info/top_level.txt,sha256=oa4bcLMAc4eg9F4D5oaTgmmEpr1XH2rxFGm0K0QIZPw,8
-reytool-0.98.dist-info/RECORD,,
+reytool-0.99.dist-info/METADATA,sha256=NiJlhPfUK2OLZg0lYO6QRz2nQtKyere3zvoG9DM1cCE,370
+reytool-0.99.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+reytool-0.99.dist-info/top_level.txt,sha256=oa4bcLMAc4eg9F4D5oaTgmmEpr1XH2rxFGm0K0QIZPw,8
+reytool-0.99.dist-info/RECORD,,
```

