# Comparing `tmp/SIDAnalyzer-0.0.1.tar.gz` & `tmp/SIDAnalyzer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIDAnalyzer-0.0.1.tar", last modified: Mon Apr  3 17:29:34 2023, max compression
+gzip compressed data, was "SIDAnalyzer-0.0.2.tar", last modified: Sun May 14 14:24:58 2023, max compression
```

## Comparing `SIDAnalyzer-0.0.1.tar` & `SIDAnalyzer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-03 17:29:34.213484 SIDAnalyzer-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2023-04-03 17:29:25.000000 SIDAnalyzer-0.0.1/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-03 22:57:54.000000 SIDAnalyzer-0.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2241 2023-04-03 17:29:34.213484 SIDAnalyzer-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1202 2023-04-03 23:12:38.000000 SIDAnalyzer-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-03 17:29:34.213484 SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2241 2023-04-03 17:29:34.000000 SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      197 2023-04-03 17:29:34.000000 SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-03 17:29:34.000000 SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       12 2023-04-03 17:29:34.000000 SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    21691 2023-04-03 22:57:20.000000 SIDAnalyzer-0.0.1/SIDAnalyzer.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-03 17:29:34.213484 SIDAnalyzer-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1453 2023-04-03 22:59:48.000000 SIDAnalyzer-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-14 14:24:58.549562 SIDAnalyzer-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2023-04-03 23:30:44.000000 SIDAnalyzer-0.0.2/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-03 23:30:44.000000 SIDAnalyzer-0.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2241 2023-05-14 14:24:58.549562 SIDAnalyzer-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1202 2023-04-03 23:30:44.000000 SIDAnalyzer-0.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-14 14:24:58.549562 SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2241 2023-05-14 14:24:58.000000 SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      207 2023-05-14 14:24:58.000000 SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-14 14:24:58.000000 SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       12 2023-05-14 14:24:58.000000 SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    22291 2023-05-14 01:12:22.000000 SIDAnalyzer-0.0.2/SIDAnalyzer.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-14 14:24:58.549562 SIDAnalyzer-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1453 2023-05-14 14:24:46.000000 SIDAnalyzer-0.0.2/setup.py
```

### Comparing `SIDAnalyzer-0.0.1/LICENSE.txt` & `SIDAnalyzer-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SIDAnalyzer-0.0.1/PKG-INFO` & `SIDAnalyzer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SIDAnalyzer
-Version: 0.0.1
+Version: 0.0.2
 Summary: This script analyzes Microsoft SID.
 Home-page: https://github.com/mauricelambert/SIDAnalyzer
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `SIDAnalyzer-0.0.1/README.md` & `SIDAnalyzer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SIDAnalyzer-0.0.1/SIDAnalyzer.egg-info/PKG-INFO` & `SIDAnalyzer-0.0.2/SIDAnalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SIDAnalyzer
-Version: 0.0.1
+Version: 0.0.2
 Summary: This script analyzes Microsoft SID.
 Home-page: https://github.com/mauricelambert/SIDAnalyzer
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `SIDAnalyzer-0.0.1/SIDAnalyzer.py` & `SIDAnalyzer-0.0.2/SIDAnalyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##################
 
 """
 This script analyzes Microsoft SID
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = "This script analyzes Microsoft SID."
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/SIDAnalyzer"
@@ -42,215 +42,215 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 sids = {
-    "S-1-0-0*": [
+    r"S-1-0-0(-[\d-]*\d)?": [
         "NULL",
         "No Security principal."
     ],
-    "S-1-1-0*": [
+    r"S-1-1-0(-[\d-]*\d)?": [
         "EVERYONE",
         "A group that includes all users."
     ],
-    "S-1-2-0*": [
+    r"S-1-2-0(-[\d-]*\d)?": [
         "LOCAL",
         "A group that includes all users who have logged on locally."
     ],
-    "S-1-2-1*": [
+    r"S-1-2-1(-[\d-]*\d)?": [
         "CONSOLE_LOGON",
         "A group that includes users who are logged on to the physical console. This SID can be used to implement security policies that grant different rights based on whether a user has been granted physical access to the console."
     ],
-    "S-1-3-0*": [
+    r"S-1-3-0(-[\d-]*\d)?": [
         "CREATOR_OWNER",
         "A placeholder in an inheritable access control entry (ACE). When the ACE is inherited, the system replaces this SID with the SID for the object's creator."
     ],
-    "S-1-3-1*": [
+    r"S-1-3-1(-[\d-]*\d)?": [
         "CREATOR_GROUP",
         "A placeholder in an inheritable ACE. When the ACE is inherited, the system replaces this SID with the SID for the primary group of the object's creator."
     ],
-    "S-1-3-2*": [
+    r"S-1-3-2(-[\d-]*\d)?": [
         "OWNER_SERVER",
         "A placeholder in an inheritable ACE. When the ACE is inherited, the system replaces this SID with the SID for the object's owner server."
     ],
-    "S-1-3-3*": [
+    r"S-1-3-3(-[\d-]*\d)?": [
         "GROUP_SERVER",
         "A placeholder in an inheritable ACE. When the ACE is inherited, the system replaces this SID with the SID for the object's group server."
     ],
-    "S-1-3-4*": [
+    r"S-1-3-4(-[\d-]*\d)?": [
         "OWNER_RIGHTS",
         "A group that represents the current owner of the object. When an ACE that carries this SID is applied to an object, the system ignores the implicit READ_CONTROL and WRITE_DAC permissions for the object owner."
     ],
-    "S-1-5*": [
+    r"S-1-5(-[\d-]*\d)?": [
         "NT_AUTHORITY",
         "A SID containing only the SECURITY_NT_AUTHORITY identifier authority."
     ],
-    "S-1-5-1*": [
+    r"S-1-5-1(-[\d-]*\d)?": [
         "DIALUP",
         "A group that includes all users who have logged on through a dial-up connection. "
     ],
-    "S-1-5-2*": [
+    r"S-1-5-2(-[\d-]*\d)?": [
         "NETWORK",
         "A group that includes all users who have logged on through a network connection. "
     ],
-    "S-1-5-3*": [
+    r"S-1-5-3(-[\d-]*\d)?": [
         "BATCH",
         "A group that includes all users who have logged on through a batch queue facility."
     ],
-    "S-1-5-4*": [
+    r"S-1-5-4(-[\d-]*\d)?": [
         "INTERACTIVE",
         "A group that includes all users who have logged on interactively."
     ],
-    "S-1-5-5-*-*": [
+    r"S-1-5-5(-[\d-]*\d)(-[\d-]*\d)": [
         "LOGON_ID",
         "A logon session. The X and Y values for these SIDs are different for each logon session and are recycled when the operating system is restarted."
     ],
-    "S-1-5-6*": [
+    r"S-1-5-6(-[\d-]*\d)?": [
         "SERVICE",
         "A group that includes all security principals that have logged on as a service."
     ],
-    "S-1-5-7*": [
+    r"S-1-5-7(-[\d-]*\d)?": [
         "ANONYMOUS",
         "A group that represents an anonymous logon. "
     ],
-    "S-1-5-8*": [
+    r"S-1-5-8(-[\d-]*\d)?": [
         "PROXY",
         "Identifies a SECURITY_NT_AUTHORITY Proxy."
     ],
-    "S-1-5-9*": [
+    r"S-1-5-9(-[\d-]*\d)?": [
         "ENTERPRISE_DOMAIN_CONTROLLERS",
         "A group that includes all domain controllers in a forest that uses an Active Directory directory service."
     ],
-    "S-1-5-10*": [
+    r"S-1-5-10(-[\d-]*\d)?": [
         "PRINCIPAL_SELF",
         "A placeholder in an inheritable ACE on an account object or group object in Active Directory. When the ACE is inherited, the system replaces this SID with the SID for the security principal that holds the account."
     ],
-    "S-1-5-11*": [
+    r"S-1-5-11(-[\d-]*\d)?": [
         "AUTHENTICATED_USERS",
         "A group that includes all users whose identities were authenticated when they logged on. Users authenticated as Guest or Anonymous are not members of this group. "
     ],
-    "S-1-5-12*": [
+    r"S-1-5-12(-[\d-]*\d)?": [
         "RESTRICTED_CODE",
         "This SID is used to control access by untrusted code. ACL validation against tokens with RC consists of two checks, one against the token's normal list of SIDs and one against a second list (typically containing RC - the &quot;RESTRICTED_CODE&quot; token - and a subset of the original token SIDs). Access is granted only if a token passes both tests. Any ACL that specifies RC must also specify WD - the &quot;EVERYONE&quot; token. When RC is paired with WD in an ACL, a superset of &quot;EVERYONE&quot;, including untrusted code, is described."
     ],
-    "S-1-5-13*": [
+    r"S-1-5-13(-[\d-]*\d)?": [
         "TERMINAL_SERVER_USER",
         "A group that includes all users who have logged on to a Terminal Services server. "
     ],
-    "S-1-5-14*": [
+    r"S-1-5-14(-[\d-]*\d)?": [
         "REMOTE_INTERACTIVE_LOGON",
         "A group that includes all users who have logged on through a terminal services logon. "
     ],
-    "S-1-5-15*": [
+    r"S-1-5-15(-[\d-]*\d)?": [
         "THIS_ORGANIZATION",
         "A group that includes all users and computers from another organization. If this SID is present, THIS_ORGANIZATION SID MUST NOT be present."
     ],
-    "S-1-5-17*": [
+    r"S-1-5-17(-[\d-]*\d)?": [
         "IUSR",
         "An account that is used by the default Internet Information Services (IIS) user."
     ],
-    "S-1-5-18*": [
+    r"S-1-5-18(-[\d-]*\d)?": [
         "LOCAL_SYSTEM",
         "An account that is used by the operating system."
     ],
-    "S-1-5-19*": [
+    r"S-1-5-19(-[\d-]*\d)?": [
         "LOCAL_SERVICE",
         "A local service account."
     ],
-    "S-1-5-20*": [
+    r"S-1-5-20(-[\d-]*\d)?": [
         "NETWORK_SERVICE",
         "A network service account."
     ],
-    "S-1-5-21-*-498": [
+    r"S-1-5-21(-[\d-]*\d)-498": [
         "ENTERPRISE_READONLY_DOMAIN_CONTROLLERS",
         "A universal group containing all read-only domain controllers in a forest."
     ],
     "S-1-5-21-0-0-0-496": [
         "COMPOUNDED_AUTHENTICATION",
         "Device identity is included in the Kerberos service ticket. If a forest boundary was crossed, then claims transformation occurred."
     ],
     "S-1-5-21-0-0-0-497": [
         "CLAIMS_VALID",
         "Claims were queried for in the account's domain, and if a forest boundary was crossed, then claims transformation occurred."
     ],
-    "S-1-5-21-*-500": [
+    r"S-1-5-21(-[\d-]*\d)-500": [
         "ADMINISTRATOR",
         "A user account for the system administrator. By default, it is the only user account that is given full control over the system."
     ],
-    "S-1-5-21-*-501": [
+    r"S-1-5-21(-[\d-]*\d)-501": [
         "GUEST",
         "A user account for people who do not have individual accounts. This user account does not require a password. By default, the Guest account is disabled."
     ],
-    "S-1-5-21-*-512": [
+    r"S-1-5-21(-[\d-]*\d)-512": [
         "DOMAIN_ADMINS",
         "A global group whose members are authorized to administer the domain. By default, the DOMAIN_ADMINS group is a member of the Administrators group on all computers that have joined a domain, including the domain controllers. DOMAIN_ADMINS is the default owner of any object that is created by any member of the group."
     ],
-    "S-1-5-21-*-513": [
+    r"S-1-5-21(-[\d-]*\d)-513": [
         "DOMAIN_USERS",
         "A global group that includes all user accounts in a domain. "
     ],
-    "S-1-5-21-*-514": [
+    r"S-1-5-21(-[\d-]*\d)-514": [
         "DOMAIN_GUESTS",
         "A global group that has only one member, which is the built-in Guest account of the domain."
     ],
-    "S-1-5-21-*-515": [
+    r"S-1-5-21(-[\d-]*\d)-515": [
         "DOMAIN_COMPUTERS",
         "A global group that includes all clients and servers that have joined the domain."
     ],
-    "S-1-5-21-*-516": [
+    r"S-1-5-21(-[\d-]*\d)-516": [
         "DOMAIN_DOMAIN_CONTROLLERS",
         "A global group that includes all domain controllers in the domain. "
     ],
-    "S-1-5-21-*-517": [
+    r"S-1-5-21(-[\d-]*\d)-517": [
         "CERT_PUBLISHERS",
         "A global group that includes all computers that are running an enterprise certification authority. Cert Publishers are authorized to publish certificates for User objects in Active Directory."
     ],
-    "S-1-5-21-*-*-518": [
+    r"S-1-5-21(-[\d-]*\d)(-[\d-]*\d)-518": [
         "SCHEMA_ADMINISTRATORS",
         "A universal group in a native-mode domain, or a global group in a mixed-mode domain. The group is authorized to make schema changes in Active Directory. "
     ],
-    "S-1-5-21-*-*-519": [
+    r"S-1-5-21(-[\d-]*\d)(-[\d-]*\d)-519": [
         "ENTERPRISE_ADMINS",
         "A universal group in a native-mode domain, or a global group in a mixed-mode domain. The group is authorized to make forestwide changes in Active Directory, such as adding child domains."
     ],
-    "S-1-5-21-*-520": [
+    r"S-1-5-21(-[\d-]*\d)-520": [
         "GROUP_POLICY_CREATOR_OWNERS",
         "A global group that is authorized to create new Group Policy Objects in Active Directory. "
     ],
-    "S-1-5-21-*-521": [
+    r"S-1-5-21(-[\d-]*\d)-521": [
         "READONLY_DOMAIN_CONTROLLERS",
         "A global group that includes all read-only domain controllers."
     ],
-    "S-1-5-21-*-522": [
+    r"S-1-5-21(-[\d-]*\d)-522": [
         "CLONEABLE_CONTROLLERS",
         "A global group that includes all domain controllers in the domain that can be cloned."
     ],
-    "S-1-5-21-*-525": [
+    r"S-1-5-21(-[\d-]*\d)-525": [
         "PROTECTED_USERS",
         "A global group that is afforded additional protections against authentication security threats. For more information, see [MS-APDS] and [MS-KILE]."
     ],
-    "S-1-5-21-*-526": [
+    r"S-1-5-21(-[\d-]*\d)-526": [
         "KEY_ADMINS",
         "A security group for delegated write access on the msdsKeyCredentialLink attribute only. The group is intended for use in scenarios where trusted external authorities (for example, Active Directory Federated Services) are responsible for modifying this attribute. Only trusted administrators should be made a member of this group."
     ],
-    "S-1-5-21-*-527": [
+    r"S-1-5-21(-[\d-]*\d)-527": [
         "ENTERPRISE_KEY_ADMINS",
         "A security group for delegated write access on the msdsKeyCredentialLink attribute only. The group is intended for use in scenarios where trusted external authorities (for example, Active Directory Federated Services) are responsible for modifying this attribute. Only trusted enterprise administrators should be made a member of this group."
     ],
-    "S-1-5-21-*-553": [
+    r"S-1-5-21(-[\d-]*\d)-553": [
         "RAS_SERVERS",
         "A domain local group for Remote Access Services (RAS) servers. By default, this group has no members. Servers in this group have Read Account Restrictions and Read Logon Information access to User objects in the Active Directory domain local group. "
     ],
-    "S-1-5-21-*-571": [
+    r"S-1-5-21(-[\d-]*\d)-571": [
         "ALLOWED_RODC_PASSWORD_REPLICATION_GROUP",
         "Members in this group can have their passwords replicated to all read-only domain controllers in the domain."
     ],
-    "S-1-5-21-*-572": [
+    r"S-1-5-21(-[\d-]*\d)-572": [
         "DENIED_RODC_PASSWORD_REPLICATION_GROUP",
         "Members in this group cannot have their passwords replicated to all read-only domain controllers in the domain."
     ],
     "S-1-5-32-544": [
         "BUILTIN_ADMINISTRATORS",
         "A built-in group. After the initial installation of the operating system, the only member of the group is the Administrator account. When a computer joins a domain, the Domain Administrators group is added to the Administrators group. When a server becomes a domain controller, the Enterprise Administrators group also is added to the Administrators group."
     ],
@@ -460,19 +460,20 @@
     ],
     "S-1-18-6": [
         "KEY_PROPERTY_ATTESTATION",
         "A SID that means the key trust object had the attestation property."
     ]
 }
 
-from fnmatch import fnmatch
 from sys import argv, stdin
+from re import fullmatch
 
 sids_ = argv[1:]
 
 if not sids_:
     sids_ = stdin.read().split()
 
 for sid_ in sids_:
     for sid in sids:
-        if fnmatch(sid_, sid):
+        # print(sid, sid_)
+        if fullmatch(sid, sid_):
             print("\x1b[38;2;183;121;227m", "\r" + sid_, "\x1b[38;2;255;240;175m\b", sids[sid][0], "\x1b[38;2;255;208;11m\b", sids[sid][1], "\x1b[39m")
```

### Comparing `SIDAnalyzer-0.0.1/setup.py` & `SIDAnalyzer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="SIDAnalyzer",
-    version="0.0.1",
+    version="0.0.2",
     py_modules=["SIDAnalyzer"],
     install_requires=[],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description="This script analyzes Microsoft SID.",
```

