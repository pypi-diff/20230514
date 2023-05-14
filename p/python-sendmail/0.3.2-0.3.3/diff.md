# Comparing `tmp/python-sendmail-0.3.2.tar.gz` & `tmp/python-sendmail-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sendmail-0.3.2.tar", last modified: Wed Sep 14 07:09:22 2022, max compression
+gzip compressed data, was "python-sendmail-0.3.3.tar", last modified: Sun May 14 14:34:55 2023, max compression
```

## Comparing `python-sendmail-0.3.2.tar` & `python-sendmail-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-09-14 07:09:22.538012 python-sendmail-0.3.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-09-14 06:53:54.000000 python-sendmail-0.3.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      136 2022-09-14 06:53:54.000000 python-sendmail-0.3.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3354 2022-09-14 07:09:22.537841 python-sendmail-0.3.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2664 2022-09-14 07:04:46.000000 python-sendmail-0.3.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-09-14 07:09:22.537641 python-sendmail-0.3.2/python_sendmail.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3354 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      303 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)      145 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/entry_points.txt
--rw-r--r--   0 test       (501) staff       (20)        6 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)        9 2022-09-14 07:09:22.000000 python-sendmail-0.3.2/python_sendmail.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        7 2022-09-14 06:53:54.000000 python-sendmail-0.3.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)     8725 2022-09-14 07:00:22.000000 python-sendmail-0.3.2/sendmail.py
--rw-r--r--   0 test       (501) staff       (20)       38 2022-09-14 07:09:22.538057 python-sendmail-0.3.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1678 2022-09-14 07:06:54.000000 python-sendmail-0.3.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-14 14:34:55.147947 python-sendmail-0.3.3/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-09-14 06:53:54.000000 python-sendmail-0.3.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      136 2022-09-14 06:53:54.000000 python-sendmail-0.3.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3387 2023-05-14 14:34:55.147821 python-sendmail-0.3.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2735 2023-05-14 12:27:23.000000 python-sendmail-0.3.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-14 14:34:55.147395 python-sendmail-0.3.3/python_sendmail.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3387 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      336 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)      144 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/entry_points.txt
+-rw-r--r--   0 test       (501) staff       (20)        6 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       15 2023-05-14 14:34:55.000000 python-sendmail-0.3.3/python_sendmail.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        7 2022-09-14 06:53:54.000000 python-sendmail-0.3.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)    10620 2023-05-14 14:13:37.000000 python-sendmail-0.3.3/sendmail.py
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-05-14 14:34:55.147982 python-sendmail-0.3.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1766 2023-05-14 12:28:24.000000 python-sendmail-0.3.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-14 14:34:55.147640 python-sendmail-0.3.3/tests/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-05-14 11:06:18.000000 python-sendmail-0.3.3/tests/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     2060 2023-05-14 14:29:36.000000 python-sendmail-0.3.3/tests/test1.py
```

### Comparing `python-sendmail-0.3.2/LICENSE` & `python-sendmail-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sendmail-0.3.2/PKG-INFO` & `python-sendmail-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: python-sendmail
-Version: 0.3.2
+Version: 0.3.3
 Summary: Sendmail client. send mail via stmp server.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: python-sendmail,pysendmail,sendmail,pysendeml,sendeml,mail
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: click
@@ -100,20 +98,24 @@
 
 ```
 pysendmail -f sender@exmaple.com -t recipient@exmaple.com -s 'just a test mail' -a /path/to/attachment.pdf 'just a test mail'
 ```
 
 ## Releases
 
+### v0.3.3
+
+- Fix ssl context problem.
+- Add attach filename support.
+
 ### v0.3.2
 
 - Add verify option. By default python-sendmail will ignore the ssl verify.
 
 ### v0.3.1
 
 - Change help information to english.
 - Use new style to release.
 
 ### v0.3.0
 
 - Old style release.
-
```

### Comparing `python-sendmail-0.3.2/README.md` & `python-sendmail-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
 ```
 pysendmail -f sender@exmaple.com -t recipient@exmaple.com -s 'just a test mail' -a /path/to/attachment.pdf 'just a test mail'
 ```
 
 ## Releases
 
+### v0.3.3
+
+- Fix ssl context problem.
+- Add attach filename support.
+
 ### v0.3.2
 
 - Add verify option. By default python-sendmail will ignore the ssl verify.
 
 ### v0.3.1
 
 - Change help information to english.
```

### Comparing `python-sendmail-0.3.2/python_sendmail.egg-info/PKG-INFO` & `python-sendmail-0.3.3/python_sendmail.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: python-sendmail
-Version: 0.3.2
+Version: 0.3.3
 Summary: Sendmail client. send mail via stmp server.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: python-sendmail,pysendmail,sendmail,pysendeml,sendeml,mail
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: click
@@ -100,20 +98,24 @@
 
 ```
 pysendmail -f sender@exmaple.com -t recipient@exmaple.com -s 'just a test mail' -a /path/to/attachment.pdf 'just a test mail'
 ```
 
 ## Releases
 
+### v0.3.3
+
+- Fix ssl context problem.
+- Add attach filename support.
+
 ### v0.3.2
 
 - Add verify option. By default python-sendmail will ignore the ssl verify.
 
 ### v0.3.1
 
 - Change help information to english.
 - Use new style to release.
 
 ### v0.3.0
 
 - Old style release.
-
```

### Comparing `python-sendmail-0.3.2/sendmail.py` & `python-sendmail-0.3.3/sendmail.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 
 import os
 import io
 from io import open
 import ssl as openssl
 import smtplib
 from email import generator
@@ -14,192 +22,476 @@
 from email.header import Header
 from email.parser import Parser
 import click
 
 
 def ignore_default_codec_map():
     from email import charset
+
     _names = list(charset.CODEC_MAP.keys())
     for _name in _names:
         del charset.CODEC_MAP[_name]
 
 
-def get_content(content, encoding="utf-8"):
+def get_content(
+    content,
+    encoding="utf-8",
+):
     if not content:
         if hasattr(os.sys.stdin, "reconfigure"):
             os.sys.stdin.reconfigure(encoding=encoding)
             content = os.sys.stdin.read()
             return content
         else:
             import codecs
+
             content = codecs.getreader(encoding)(os.sys.stdin).read()
             return content
     if os.path.exists(content):
         with open(content, "r", encoding=encoding) as fobj:
             return fobj.read()
     return content
 
 
-def addresses_encode(addresses, charset="utf-8"):
+def addresses_encode(
+    addresses,
+    charset="utf-8",
+):
     return ", ".join([address_encode(address, charset) for address in addresses])
 
 
-def address_encode(value, charset="utf-8"):
+def address_encode(
+    value,
+    charset="utf-8",
+):
     if "<" in value:
         name, email = value.split("<")
         name = name.strip()
         email = email.replace(">", "")
     else:
         name = value
         email = value
     return "{0} <{1}>".format(header_encode(name, charset), email)
 
 
-def header_encode(value, charset="utf-8"):
+def header_encode(
+    value,
+    charset="utf-8",
+):
     return Header(value, charset).encode()
 
 
-def get_smtp_service(host="127.0.0.1", port=25, ssl=False, user=None, password=None, verify=False):
+def get_smtp_service(
+    host="127.0.0.1",
+    port=25,
+    ssl=False,
+    user=None,
+    password=None,
+    verify=False,
+):
     if ssl:
-        if not verify:
-            context = openssl._create_unverified_context()
-        else:
-            context = None
+        context = openssl.create_default_context()
+        context.set_ciphers("ALL")
+        context.check_hostname = verify
         smtp_service = smtplib.SMTP_SSL(host, port, context=context)
     else:
         smtp_service = smtplib.SMTP(host, port)
     if user and password:
         smtp_service.login(user, password)
     return smtp_service
 
 
-def get_message_from_eml_content(content):
+def get_message_from_eml_content(
+    content,
+):
     parser = Parser()
     return parser.parsestr(content)
 
 
-def make_message(from_address, to_addresses, content, subject, attachs=None, is_html_content=False, charset="utf-8"):
+def make_message(
+    from_address,
+    to_addresses,
+    content,
+    subject,
+    attachs=None,
+    is_html_content=False,
+    charset="utf-8",
+):
+    """
+    An attach format:
+        1. a file path string
+        2. a tuple of (filepath, filename)
+        3. a tuple of (filepath,)
+        4. a dict of {"filepath": "xxx", "filename": "xxx"}
+        5. a dict of {"filepath": "xxx}
+    """
     message = MIMEMultipart()
     if subject:
         message["Subject"] = header_encode(subject, charset)
     message["From"] = address_encode(from_address, charset)
     message["To"] = addresses_encode(to_addresses, charset)
 
     if is_html_content:
         main_content = MIMEText(content, "html", charset)
     else:
         main_content = MIMEText(content, "plain", charset)
     message.attach(main_content)
 
     attachs = attachs or []
     for attach in attachs:
-        basename = header_encode(os.path.basename(attach), charset)
+        if isinstance(attach, str):
+            filename = os.path.basename(attach)
+            filepath = attach
+        elif isinstance(attach, (list, tuple)):
+            filepath = attach[0]
+            if len(attach) > 1:
+                filename = attach[1]
+            else:
+                filename = os.path.basename(filename)
+        elif isinstance(attach, dict):
+            filepath = attach["filepath"]
+            filename = attach.get("filename", os.path.basename(filepath))
+        basename = header_encode(filename, charset)
         part = None
-        with open(attach, "rb") as attach_file:
+        with open(filepath, "rb") as attach_file:
             part = MIMEApplication(attach_file.read(), Name=basename)
         part.add_header("Content-Disposition", "attachment", filename=basename)
         message.attach(part)
 
     return message
 
 
-def makemail(from_address, to_addresses, subject, attach, html, encoding, charset, output, content):
+def makemail(
+    from_address,
+    to_addresses,
+    subject,
+    attach,
+    html,
+    encoding,
+    charset,
+    output,
+    content,
+):
     content = get_content(content, encoding)
-    message = make_message(from_address, to_addresses, content, subject, attach, html, charset)
+    message = make_message(
+        from_address, to_addresses, content, subject, attach, html, charset
+    )
     buffer = io.StringIO()
     gen = generator.Generator(buffer)
     gen.flatten(message)
     if output:
         with open(output, "w") as fobj:
             fobj.write(buffer.getvalue())
     else:
         click.echo(buffer.getvalue())
     return message
 
 
-def sendmail(from_address, to_addresses, content, subject, attachs=None, is_html_content=False, encoding="utf-8", charset="utf-8", host="127.0.0.1", port=25, ssl=False, user=None, password=None, verify=False):
+def sendmail(
+    from_address,
+    to_addresses,
+    content,
+    subject="",
+    attachs=None,
+    is_html_content=False,
+    encoding="utf-8",
+    charset="utf-8",
+    host="127.0.0.1",
+    port=25,
+    ssl=False,
+    user=None,
+    password=None,
+    verify=False,
+):
     content = get_content(content, encoding)
     smtp_service = get_smtp_service(host, port, ssl, user, password, verify=verify)
-    message = make_message(from_address, to_addresses, content, subject, attachs, is_html_content, charset)
+    message = make_message(
+        from_address, to_addresses, content, subject, attachs, is_html_content, charset
+    )
     smtp_service.send_message(message)
     smtp_service.quit()
 
 
-def sendeml(content, encoding="utf-8", host="127.0.0.1", port=25, ssl=False, user=None, password=None, verify=False):
+def sendeml(
+    content,
+    encoding="utf-8",
+    host="127.0.0.1",
+    port=25,
+    ssl=False,
+    user=None,
+    password=None,
+    verify=False,
+):
     content = get_content(content, encoding)
     smtp_service = get_smtp_service(host, port, ssl, user, password, verify=verify)
     message = get_message_from_eml_content(content)
     smtp_service.send_message(message)
     smtp_service.quit()
 
 
 @click.group()
 def main():
     """Sendmail client
 
-Notice:
+    Notice:
 
-1. Empty content means read mail content from stdin.
-2. If the content argument is a file path, read mail content from the file.
-3. Otherwise use the content argument as the mail content.
+    1. Empty content means read mail content from stdin.
+    2. If the content argument is a file path, read mail content from the file.
+    3. Otherwise use the content argument as the mail content.
     """
     pass
 
 
 @main.command(name="makemail")
-@click.option("-f", "--from-address", required=True, help="Mail sender, e.g. Name <name@example.com> or name@example.com.")
-@click.option("-t", "--to-address", multiple=True, required=True, help="Mail recipients, e.g. Name <name@example.com> or name@example.com.")
+@click.option(
+    "-f",
+    "--from-address",
+    required=True,
+    help="Mail sender, e.g. Name <name@example.com> or name@example.com.",
+)
+@click.option(
+    "-t",
+    "--to-address",
+    multiple=True,
+    required=True,
+    help="Mail recipients, e.g. Name <name@example.com> or name@example.com.",
+)
 @click.option("-s", "--subject", help="Mail subject")
-@click.option("-a", "--attach", multiple=True, required=False, help="Mail attachments, allow multiple use.")
-@click.option("--html", is_flag=True, help="Mail content is HTML format.")
-@click.option("-e", "--encoding", default="utf-8", help="Encoding of the mail content input.")
-@click.option("-c", "--charset", default="utf-8", help="Encoding of the mail content output.")
-@click.option("-o", "--output", required=False, help="Save the .eml file to the given path.")
-@click.argument("content", nargs=1, required=False)
-def makemail_cmd(from_address, to_address, subject, attach, html, encoding, charset, output, content):
-    """Make .eml file.
-    """
+@click.option(
+    "-a",
+    "--attach",
+    multiple=True,
+    required=False,
+    help="Mail attachments, allow multiple use.",
+)
+@click.option(
+    "--html",
+    is_flag=True,
+    help="Mail content is HTML format.",
+)
+@click.option(
+    "-e",
+    "--encoding",
+    default="utf-8",
+    help="Encoding of the mail content input.",
+)
+@click.option(
+    "-c",
+    "--charset",
+    default="utf-8",
+    help="Encoding of the mail content output.",
+)
+@click.option(
+    "-o",
+    "--output",
+    required=False,
+    help="Save the .eml file to the given path.",
+)
+@click.argument(
+    "content",
+    nargs=1,
+    required=False,
+)
+def makemail_cmd(
+    from_address,
+    to_address,
+    subject,
+    attach,
+    html,
+    encoding,
+    charset,
+    output,
+    content,
+):
+    """Make .eml file."""
     ignore_default_codec_map()
     to_addresses = to_address
-    makemail(from_address, to_addresses, subject, attach, html, encoding, charset, output, content)
+    makemail(
+        from_address,
+        to_addresses,
+        subject,
+        attach,
+        html,
+        encoding,
+        charset,
+        output,
+        content,
+    )
 
 
 @main.command(name="sendmail")
-@click.option("-f", "--from-address", required=True, help="Mail sender, e.g. Name <name@example.com> or name@example.com.")
-@click.option("-t", "--to-address", multiple=True, required=True, help="Mail recipients, e.g. Name <name@example.com> or name@example.com.")
-@click.option("-s", "--subject", help="Mail subject")
-@click.option("-a", "--attach", multiple=True, required=False, help="Mail attachments, allow multiple use.")
-@click.option("--html", is_flag=True, help="Mail content is HTML format.")
-@click.option("-e", "--encoding", default="utf-8", help="Encoding of the mail content input.")
-@click.option("-c", "--charset", default="utf-8", help="Encoding of the mail content output.")
-@click.option("-h", "--host", default="127.0.0.1", help="Mail server address, default to 127.0.0.1.")
-@click.option("-p", "--port", default=25, help="Mail server port, default to 25. If you are using an ssl server, mostly the port should be 465.")
-@click.option("--ssl", is_flag=True, help="Mail server using ssl encryption.")
-@click.option("-u", "--user", help="Mail server login account. Empty user means don't use login.")
-@click.option("-P", "--password", help="Mail server login password. Empty password means don't use login.")
-@click.option("--verify", is_flag=True, help="Verify ssl certificate.")
-@click.argument("content", nargs=1, required=False)
-def sendmail_cmd(from_address, to_address, subject, attach, html, encoding, charset, host, port, ssl, user, password, verify, content):
-    """Send mail.
-    """
+@click.option(
+    "-f",
+    "--from-address",
+    required=True,
+    help="Mail sender, e.g. Name <name@example.com> or name@example.com.",
+)
+@click.option(
+    "-t",
+    "--to-address",
+    multiple=True,
+    required=True,
+    help="Mail recipients, e.g. Name <name@example.com> or name@example.com.",
+)
+@click.option(
+    "-s",
+    "--subject",
+    help="Mail subject",
+)
+@click.option(
+    "-a",
+    "--attach",
+    multiple=True,
+    required=False,
+    help="Mail attachments, allow multiple use.",
+)
+@click.option(
+    "--html",
+    is_flag=True,
+    help="Mail content is HTML format.",
+)
+@click.option(
+    "-e",
+    "--encoding",
+    default="utf-8",
+    help="Encoding of the mail content input.",
+)
+@click.option(
+    "-c",
+    "--charset",
+    default="utf-8",
+    help="Encoding of the mail content output.",
+)
+@click.option(
+    "-h",
+    "--host",
+    default="127.0.0.1",
+    help="Mail server address, default to 127.0.0.1.",
+)
+@click.option(
+    "-p",
+    "--port",
+    default=25,
+    help="Mail server port, default to 25. If you are using an ssl server, mostly the port should be 465.",
+)
+@click.option(
+    "--ssl",
+    is_flag=True,
+    help="Mail server using ssl encryption.",
+)
+@click.option(
+    "-u",
+    "--user",
+    help="Mail server login account. Empty user means don't use login.",
+)
+@click.option(
+    "-P",
+    "--password",
+    help="Mail server login password. Empty password means don't use login.",
+)
+@click.option(
+    "--verify",
+    is_flag=True,
+    help="Verify ssl certificate.",
+)
+@click.argument(
+    "content",
+    nargs=1,
+    required=False,
+)
+def sendmail_cmd(
+    from_address,
+    to_address,
+    subject,
+    attach,
+    html,
+    encoding,
+    charset,
+    host,
+    port,
+    ssl,
+    user,
+    password,
+    verify,
+    content,
+):
+    """Send mail."""
     ignore_default_codec_map()
     to_addresses = to_address
-    sendmail(from_address, to_addresses, content, subject, attach, html, encoding, charset, host, port, ssl, user, password, verify=verify)
+    sendmail(
+        from_address,
+        to_addresses,
+        content,
+        subject,
+        attach,
+        html,
+        encoding,
+        charset,
+        host,
+        port,
+        ssl,
+        user,
+        password,
+        verify=verify,
+    )
 
 
 @main.command(name="sendeml")
-@click.option("-h", "--host", default="127.0.0.1", help="Mail server address, default to 127.0.0.1.")
-@click.option("-p", "--port", default=25, help="Mail server port, default to 25. If you are using an ssl server, mostly the port should be 465.")
-@click.option("--ssl", is_flag=True, help="Mail server using ssl encryption.")
-@click.option("-u", "--user", help="Mail server login account. Empty user means don't use login.")
-@click.option("-P", "--password", help="Mail server login password. Empty password means don't use login.")
-@click.option("-e", "--encoding", default="utf-8", help="EML file encoding.")
-@click.option("--verify", is_flag=True, help="Verify ssl certificate.")
-@click.argument("content", nargs=1, required=False)
-def sendeml_cmd(host, port, ssl, user, password, encoding, content, verify):
-    """Send eml file.
-    """
+@click.option(
+    "-h",
+    "--host",
+    default="127.0.0.1",
+    help="Mail server address, default to 127.0.0.1.",
+)
+@click.option(
+    "-p",
+    "--port",
+    default=25,
+    help="Mail server port, default to 25. If you are using an ssl server, mostly the port should be 465.",
+)
+@click.option(
+    "--ssl",
+    is_flag=True,
+    help="Mail server using ssl encryption.",
+)
+@click.option(
+    "-u",
+    "--user",
+    help="Mail server login account. Empty user means don't use login.",
+)
+@click.option(
+    "-P",
+    "--password",
+    help="Mail server login password. Empty password means don't use login.",
+)
+@click.option(
+    "-e",
+    "--encoding",
+    default="utf-8",
+    help="EML file encoding.",
+)
+@click.option(
+    "--verify",
+    is_flag=True,
+    help="Verify ssl certificate.",
+)
+@click.argument(
+    "content",
+    nargs=1,
+    required=False,
+)
+def sendeml_cmd(
+    host,
+    port,
+    ssl,
+    user,
+    password,
+    encoding,
+    content,
+    verify,
+):
+    """Send eml file."""
     sendeml(content, encoding, host, port, ssl, user, password, verify=verify)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `python-sendmail-0.3.2/setup.py` & `python-sendmail-0.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 
 import os
 from io import open
 from setuptools import setup
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -13,30 +21,37 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="python-sendmail",
-    version="0.3.2",
+    version="0.3.3",
     description="Sendmail client. send mail via stmp server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
     ],
-    keywords=["python-sendmail", "pysendmail", "sendmail", "pysendeml", "sendeml", "mail"],
+    keywords=[
+        "python-sendmail",
+        "pysendmail",
+        "sendmail",
+        "pysendeml",
+        "sendeml",
+        "mail",
+    ],
     requires=requires,
     install_requires=requires,
     packages=find_packages("."),
     py_modules=["sendmail"],
     entry_points={
         "console_scripts": [
             "pymail = sendmail:main",
```

