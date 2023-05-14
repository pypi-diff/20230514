# Comparing `tmp/wwpdb.utils.emdb-1.2.tar.gz` & `tmp/wwpdb.utils.emdb-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.2.tar", last modified: Sun Apr 30 13:10:36 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.3.tar", last modified: Sun May 14 15:05:25 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.2.tar` & `wwpdb.utils.emdb-1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:10:36.631974 wwpdb.utils.emdb-1.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2223 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.619974 wwpdb.utils.emdb-1.2/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   663967 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1660129 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      329 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   217704 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:10:22.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2223 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.356523 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   664004 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2282514 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      368 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   217704 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:05:10.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.2/PKG-INFO` & `wwpdb.utils.emdb-1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.2
+Version: 1.3
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.2/setup.py` & `wwpdb.utils.emdb-1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the
 specific language governing permissions and limitations
 under the License.
 """
+
+# pylint: disable=protected-access
+
 __author__ = "Ardan Patwardhan, Sanja Abbott"
 __email__ = "ardan@ebi.ac.uk, sanja@ebi.ac.uk"
 __date__ = "2019-05-17"
 __version__ = "1.0"
 
 import os
 import sys
@@ -102,15 +105,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.3.2"
+        XML_OUT_VERSION = "3.0.3.3"
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
         EM_DEPUI = "em_depui"
@@ -1354,15 +1357,15 @@
         Write out XML file.
         A translation from cif to XML needs to have taken place.
 
         Parameters:
         @param xml_out_file_name: name of the xml file
         """
         # self.xml_out is the xml object representing conversion from cif
-        if self.xml_out is None or self.xml_out.hasContent_() is False:
+        if self.xml_out is None or self.xml_out._hasContent() is False:
             txt = u"There is no content to write out. No output file will be written."
             self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
             self.log_formatted(self.error_log_string, "(" + self.entry_in_translation_log.id + ")" + self.Constants.REQUIRED_ALERT + txt)
             return
         # xml_out_file is the actual xml file that will be written into and saved
         xml_out_file = open(xml_out_file_name, "w") if xml_out_file_name else sys.stdout
         xml_out_file.write('<?xml version="1.0" encoding="UTF-8"?>\n')
@@ -1811,17 +1814,17 @@
                 set_el_processing_details(soft, soft_in)
 
             if software_category in category_dict:
                 soft_list = emdb.software_list_type()
                 for soft_in in category_dict[software_category]:
                     soft = emdb.software_type()
                     set_software_type(software_category, soft, soft_in)
-                    if soft.hasContent_():
+                    if soft._hasContent():
                         soft_list.add_software(soft)
-                if soft_list.hasContent_():
+                if soft_list._hasContent():
                     setter_func(soft_list)
 
         def assert_get_value(key, dic):
             """
             Return dict[value] but throw an exception if key is not found
 
             @param key: key of (key,value) pair
@@ -2085,15 +2088,15 @@
                         obs_entry = emdb.supersedes_type()
                         set_supersedes_type(obs_entry, obs_in)
                         obs_list.add_entry(obs_entry)
 
                 obsolete_in = make_dict(const.EM_OBSOLETE, "id")
                 obs_list = emdb.obsolete_listType()
                 set_obsolete_list_type(obs_list, obsolete_in)
-                if obs_list.hasContent_():
+                if obs_list._hasContent():
                     admin.set_obsolete_list(obs_list)
 
             def set_el_superseded_by_list(admin):
                 """
                 If this element appears means that the current entry is obsoleted.
                 The newer entry which replaces this entry is listed here.
                 XSD: <xs:element name="superseded_by_list" minOccurs="0"> has
@@ -2145,15 +2148,15 @@
                         spr_entry = emdb.supersedes_type()
                         set_supersede_entry(spr_entry, spr_in)
                         supersed_list.add_entry(spr_entry)
 
                 supr_in = make_dict(const.EM_SUPERSEDE, "id")
                 supersede_list = emdb.superseded_by_listType()
                 set_supersede_by_list(supersede_list, supr_in)
-                if supersede_list.hasContent_():
+                if supersede_list._hasContent():
                     admin.set_superseded_by_list(supersede_list)
 
             def set_el_grant_support(admin, aud_sup_in):
                 """
                 XSD: <xs:element name="grant_support" minOccurs="0">
                 CIF: _pdbx_audit_support
                 """
@@ -2201,20 +2204,20 @@
                     for _aud_sup_key, aud_sup in aud_sup_in.items():
                         el_funding_body = get_cif_value("funding_organization", const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         # el_code = get_cif_value('grant_number', const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         # el_country = get_cif_value('country', const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         if el_funding_body is not None:  # or el_code is not None or el_country is not None:
                             grant_ref = emdb.grant_reference_type()
                             set_grant_reference_type(grant_ref, aud_sup)
-                            if grant_ref.hasContent_():
+                            if grant_ref._hasContent():
                                 grant_support.add_grant_reference(grant_ref)
 
                 grant_support = emdb.grant_supportType()
                 set_grant_support_type(grant_support, aud_sup_in)
-                if grant_support.hasContent_():
+                if grant_support._hasContent():
                     admin.set_grant_support(grant_support)
 
             def set_el_contact_author(admin, contact_auth_in):
                 """
                 XSD: <xs:element name="contact_author" maxOccurs="unbounded" minOccurs="0">
                 CIF: _pdbx_contact_author
                 """
@@ -2424,15 +2427,15 @@
                     el_email,
                     el_telephone,
                     el_fax,
                 ]
                 if any(x is not None for x in contact_author_type_list):
                     cont_author = emdb.contact_authorType()
                     set_contact_author_type(cont_author, contact_auth_in)
-                    if cont_author.hasContent_():
+                    if cont_author._hasContent():
                         admin.add_contact_author(cont_author)
 
             def set_el_title(admin):
                 """
                 XSD: <xs:element name="title" type="xs:token">
                 The value is _struct.title if _em_depui.same_title_as_pdb.
                 Otherwise it is _em_admin.title
@@ -2665,15 +2668,15 @@
                         XSD: <xs:element name="author" type="author_order_type" maxOccurs="unbounded"/>
                         Citation authors
                         """
                         if cite_id_in in auth_dict:
                             if len(auth_dict[cite_id_in]) > 0:
                                 for auth_in in auth_dict[cite_id_in]:
                                     author = emdb.author_order_type(valueOf_=format_author(auth_in[0]), ORCID=auth_in[2], order=int(auth_in[1]))
-                                    if author.hasContent_():
+                                    if author._hasContent():
                                         pub.add_author(author)
                             else:
                                 txt = u"No authors for citation id (%s) found. At least one is required." % cite_id_in
                                 self.current_entry_log.error_logs.append(
                                     self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
                                 )
                                 self.log_formatted(self.error_log_string, "(" + self.entry_in_translation_log.id + ")" + const.REQUIRED_ALERT + txt)
@@ -3182,31 +3185,31 @@
                         emdb_ref_list_in = x_ref_dict_in["EMDB"]
                         for emdb_ref_in in emdb_ref_list_in:
                             emdb_ref = emdb.emdb_cross_reference_type()
                             set_ref_el_emdb_id(emdb_ref, emdb_ref_in)
                             set_ref_el_relationship(emdb_ref, emdb_ref_in)
                             set_ref_el_details(emdb_ref, emdb_ref_in)
 
-                            if emdb_ref.hasContent_():
+                            if emdb_ref._hasContent():
                                 emdb_ref_list.add_emdb_reference(emdb_ref)
 
                     if "EMDB" in rel_entries_dict_in:
                         emdb_rel_list_in = rel_entries_dict_in["EMDB"]
                         for rel_in in emdb_rel_list_in:
                             cross_ref = emdb.emdb_cross_reference_type()
                             set_rel_el_emdb_id(cross_ref, rel_in)
                             set_rel_el_relationship(cross_ref, rel_in)
                             set_rel_el_details(cross_ref, rel_in)
 
-                            if cross_ref.hasContent_():
+                            if cross_ref._hasContent():
                                 emdb_ref_list.add_emdb_reference(cross_ref)
 
                 emdb_ref_list = emdb.emdb_cross_reference_list_type()
                 set_emdb_cross_ref_list_type(emdb_ref_list, x_ref_dict_in)
-                if emdb_ref_list.hasContent_():
+                if emdb_ref_list._hasContent():
                     cross_references.set_emdb_list(emdb_ref_list)
 
             def set_el_pdb_list(cross_references, x_ref_dict_in):
                 """
                 XSD: <xs:element name="pdb_list" type="pdb_cross_reference_list_type" minOccurs="0">
                 """
 
@@ -3235,15 +3238,15 @@
                         txt = None
                         if rel_in == "IN FRAME":
                             pdb_ref.set_relationship(emdb.relationshipType(in_frame="FULLOVERLAP"))
                             txt = u"The value (FULLOVERLAP) is given to (pdb_ref.set_relationship)."
                         else:
                             pdb_ref.set_relationship(emdb.relationshipType(other="unknown"))
                             txt = u"The value (unknown) is given to (pdb_ref.set_relationship)."
-                        if pdb_ref.hasContent_():
+                        if pdb_ref._hasContent():
                             pdb_ref_list.add_pdb_reference(pdb_ref)
                             if txt is not None:
                                 self.current_entry_log.warn_logs.append(
                                     self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.change_title + txt)
                                 )
                                 self.log_formatted(self.warn_log_string, const.CHANGE_MADE + txt)
 
@@ -3266,15 +3269,15 @@
                             set_el_relationship(pdb_ref, pdb_ref_in)
                             # element 3
                             set_el_details(pdb_ref, pdb_ref_in)
 
                 if "PDB" in x_ref_dict_in:
                     pdb_ref_list = emdb.pdb_cross_reference_list_type()
                     set_pdb_cross_ref_list_type(pdb_ref_list, x_ref_dict_in)
-                    if pdb_ref_list.hasContent_():
+                    if pdb_ref_list._hasContent():
                         cross_references.set_pdb_list(pdb_ref_list)
 
             def set_el_auxiliary_link_list(cross_references):
                 """
                 <xs:element name="auxiliary_link_list" minOccurs="0">
                 ..a list of one and only one element
                 """
@@ -3313,17 +3316,17 @@
                     set_el_details()
 
                 aux_link_list = emdb.auxiliary_link_listType()
                 aux_link_list_in = self.cif.get(const.EM_DB_REFERENCE_AUXILIARY)
                 for aux_in in aux_link_list_in:
                     aux = emdb.auxiliary_link_type()
                     set_aux_link_type(aux, aux_in)
-                    if aux.hasContent_():
+                    if aux._hasContent():
                         aux_link_list.add_auxiliary_link(aux)
-                if aux_link_list.hasContent_():
+                if aux_link_list._hasContent():
                     cross_references.set_auxiliary_link_list(aux_link_list)
 
             # element 1
             set_el_citation_list(cross_references)
             x_ref_dict_in = make_list_of_dicts(const.EM_DB_REFERENCE, "db_name")
             # element 2
             set_el_emdb_list(cross_references, x_ref_dict_in)
@@ -3696,15 +3699,15 @@
                             # element 3
                             # XSD: <xs:element name="method" type="xs:token" minOccurs="0"/>
                             # CIF: method doesn't exist in the dictionary!!!!
                             # mol_weight.set_method()
 
                     mol_weight = emdb.molecular_weight_type()
                     set_molecular_weight_type(mol_weight)
-                    if mol_weight.hasContent_():
+                    if mol_weight._hasContent():
                         supra_mol.set_molecular_weight(mol_weight)
 
                 def set_sup_mol_base_source(sup_mol, cif_category, src_in):
                     """
                     Creates the base source element for supramolecules
 
                     Parameters:
@@ -3783,15 +3786,15 @@
                         if flags_dict["add_cell"]:
                             set_el_cell(nat_src, cif_category, sup_mol_nat_src_in)
                         if flags_dict["add_organelle"]:
                             set_el_organelle(nat_src, cif_category, sup_mol_nat_src_in)
                         if flags_dict["add_cellular_location"]:
                             set_el_cellular_location(nat_src, cif_category, sup_mol_nat_src_in)
 
-                        if nat_src.hasContent_():
+                        if nat_src._hasContent():
                             if flags_dict["add_nat_src"]:
                                 sup_mol.add_natural_source(nat_src)
                             else:
                                 sup_mol.set_natural_source(nat_src)
                             break
 
                 def set_sup_mol_rec_exp(sup_mol, sup_mol_id_in, rec_exp_dict_in, add_rec_exp=False, virus=False):
@@ -3807,15 +3810,15 @@
                     @param virus: boolean - if true use host_system instead of recombinant_expression
                     """
                     if rec_exp_dict_in is not None:
                         if sup_mol_id_in in rec_exp_dict_in:
                             for rec_exp_in in rec_exp_dict_in[sup_mol_id_in]:
                                 r_exp = emdb.recombinant_source_type()
                                 set_recombinant_source_type(r_exp, rec_exp_in)
-                                if r_exp.hasContent_():
+                                if r_exp._hasContent():
                                     if add_rec_exp is False:
                                         if virus is False:
                                             sup_mol.set_recombinant_expression(r_exp)
                                         else:
                                             sup_mol.set_host_system(r_exp)
                                         break
                                     else:
@@ -3918,15 +3921,15 @@
                                 for m_in in macro_list_in:
                                     a_macromol = emdb.macromoleculeType(macromolecule_id=int(m_in))
                                     a_macromol.original_tagname_ = "macromolecule"
                                     macro_list.add_macromolecule(a_macromol)
                                 txt = u"Macromolecule (%s) added to the list of macromolecules." % int(m_in)  # pylint: disable=undefined-loop-variable
                                 self.current_entry_log.info_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.info_title + txt))
                                 self.log_formatted(self.info_log_string, const.INFO_ALERT + txt)
-                                if macro_list.hasContent_():
+                                if macro_list._hasContent():
                                     sup_mol.set_macromolecule_list(macro_list)
                             else:
                                 txt = u"No macromolecule found for (%s)." % id_list_item
                                 self.current_entry_log.warn_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt))
                                 self.log_formatted(self.warn_log_string, const.NOT_REQUIRED_ALERT + txt)
 
                     def set_el_details(sup_mol, sup_in):
@@ -4113,15 +4116,15 @@
                                 set_attr_ncbi(virus_name, nat_src_in)
                                 set_cif_value(virus_name.set_valueOf_, "organism", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, cif_list=nat_src_in)
                                 # additionally, set the supramolecule name
                                 set_cif_value(virus_sup_mol.set_name, "organism", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, cif_list=nat_src_in, constructor=emdb.sci_name_type)
 
                             virus_name = emdb.virus_species_name_type()
                             set_virus_species_name_type(virus_name)
-                            if virus_name.hasContent_():
+                            if virus_name._hasContent():
                                 virus_sup_mol.set_sci_species_name(virus_name)
 
                         def set_el_sci_species_strain(virus_sup_mol, nat_src_in):
                             """
                             XSD: <xs:element name="sci_species_strain" type="xs:string" maxOccurs="1" minOccurs="0">
                             XPath: /element(*,virus_supramolecule_type)/sci_species_strain
                             CIF: _em_entity_assembly_naturalsource.strain ?
@@ -4203,15 +4206,15 @@
                                 nat_host_list_in = virus_nat_host_dict_in[sup_mol_id_in]
                                 for nat_host_in in nat_host_list_in:
                                     attr_ncbi = get_cif_value("ncbi_tax_id", const.EM_VIRUS_NATURAL_HOST, cif_list=nat_host_in)
                                     organism = get_cif_value("organism", const.EM_VIRUS_NATURAL_HOST, cif_list=nat_host_in)
                                     if any(x is not None for x in [attr_ncbi, organism]):
                                         nat_host = emdb.virus_host_type()
                                         set_virus_natural_host_type(nat_host, nat_host_in)
-                                        if nat_host.hasContent_():
+                                        if nat_host._hasContent():
                                             virus_sup_mol.add_natural_host(nat_host)
 
                         def set_el_host_system(virus_sup_mol, sup_mol_id_in, rec_exp_dict_in):
                             """
                             XSD: <xs:element name="host_system" type="recombinant_source_type">
                             """
                             set_sup_mol_rec_exp(virus_sup_mol, sup_mol_id_in, rec_exp_dict_in, virus=True)
@@ -4269,15 +4272,15 @@
                                     # element 1
                                     set_el_name(virus_shell, vs_in)
                                     # element 2
                                     set_el_diameter(virus_shell, vs_in)
                                     # element 3
                                     set_el_triangulation(virus_shell, vs_in)
 
-                                    if virus_shell.hasContent_():
+                                    if virus_shell._hasContent():
                                         virus_sup_mol.add_virus_shell(virus_shell)
 
                         def set_el_virus_type(virus_sup_mol, virus_in):
                             """
                             XSD:  <xs:element name="virus_type">; base xs:token with restriction
                             CIF: _em_virus_entity.virus_type PRION
                             """
@@ -4616,35 +4619,35 @@
                                 # (RIBOSOME or COMPLEX), VIRUS, ORGANELLE OR CELLULAR COMPONENT,
                                 # TISSUE, CELL
                                 sup_type = get_cif_value("type", const.EM_ENTITY_ASSEMBLY, sup_in)
                                 if sup_type is not None:
                                     if sup_type in ["RIBOSOME", "COMPLEX"]:
                                         complex_sup_mol = emdb.complex_supramolecule_type()
                                         set_complex_supramolecule_type(complex_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if complex_sup_mol.hasContent_():
+                                        if complex_sup_mol._hasContent():
                                             sup_list.add_supramolecule(complex_sup_mol)
                                     elif sup_type == "VIRUS":
                                         virus_sup_mol = emdb.virus_supramolecule_type()
                                         set_virus_supramolecule_type(virus_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if virus_sup_mol.hasContent_():
+                                        if virus_sup_mol._hasContent():
                                             sup_list.add_supramolecule(virus_sup_mol)
                                     elif sup_type == "ORGANELLE OR CELLULAR COMPONENT":
                                         org_or_cell_sup_mol = emdb.organelle_or_cellular_component_supramolecule_type()
                                         set_orgorcell_supmol_type(org_or_cell_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if org_or_cell_sup_mol.hasContent_():
+                                        if org_or_cell_sup_mol._hasContent():
                                             sup_list.add_supramolecule(org_or_cell_sup_mol)
                                     elif sup_type == "TISSUE":
                                         tissue_sup_mol = emdb.tissue_supramolecule_type()
                                         set_tissue_supramolecule_type(tissue_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if tissue_sup_mol.hasContent_():
+                                        if tissue_sup_mol._hasContent():
                                             sup_list.add_supramolecule(tissue_sup_mol)
                                     elif sup_type == "CELL":
                                         cell_sup_mol = emdb.cell_supramolecule_type()
                                         set_cell_supramolecule_type(cell_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if cell_sup_mol.hasContent_():
+                                        if cell_sup_mol._hasContent():
                                             sup_list.add_supramolecule(cell_sup_mol)
                                     else:
                                         txt = u"Supramolecule type not implemented. (_em_entity_assembly.type) is (%s)" % sup_type
                                         self.current_entry_log.error_logs.append(
                                             self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
                                         )
                                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
@@ -4893,15 +4896,15 @@
                         genetically modified or synthetic sources keyed by entity_id
                     @param cif_category: contains the source info
                     XSD: <xs:element name="natural_source" type="molecule_source_type" minOccurs="0"/>
                     """
                     if ent_src_dict is not None and cif_category is not None:
                         mol_src_dict = {"add_organ": True, "add_tissue": True, "add_cell": True, "add_organelle": True, "add_cellular_location": True}
                         nat_src = make_mol_src(cif_category, ent_src_dict, mol_src_dict)
-                        if nat_src.hasContent_():
+                        if nat_src._hasContent():
                             mol.set_natural_source(nat_src)
 
                 def set_base_mol_with_dict(mol, ent_in, ent_id_in, mol_dicts):
                     """
                     Set the dictionary and cif category for base_macromolecule_type
 
                     Parameters:
@@ -5077,26 +5080,26 @@
                                     set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
 
                         if ent_id_in in ent_ref_dict:
                             ent_ref_list_in = ent_ref_dict[ent_id_in]
                             for rel_in in ent_ref_list_in:
                                 cross_ref = emdb.external_referencesType()
                                 set_external_references_type(cross_ref, rel_in)
-                                if cross_ref.hasContent_():
+                                if cross_ref._hasContent():
                                     seq.add_external_references(cross_ref)
 
                     seq = emdb.sequenceType()
                     # element 1
                     set_el_string(seq, ent_poly_in)
                     # element 2
                     set_el_discrepancy_list()
                     # element 3
                     set_el_external_references(seq, ent_id_in, ent_ref_dict)
 
-                    if seq.hasContent_():
+                    if seq._hasContent():
                         mol.set_sequence(seq)
 
                 def set_mol_rec_exp(mol, ent_id_in, mol_rec_exp_dict):
                     """
                     Set recombinant expression for a macromolecule
 
                     Parameters:
@@ -5109,15 +5112,15 @@
                     .. 5 elements
                     """
                     if mol_rec_exp_dict is not None:
                         if ent_id_in in mol_rec_exp_dict:
                             r_exp_in = mol_rec_exp_dict[ent_id_in]
                             r_exp = emdb.recombinant_source_type()
                             set_recombinant_source_type(r_exp, r_exp_in)
-                            if r_exp.hasContent_():
+                            if r_exp._hasContent():
                                 mol.set_recombinant_expression(r_exp)
                     else:
                         txt = u"The dictionary for recombinant expression for macromolecule id (%s) not found." % ent_id_in
                         self.current_entry_log.warn_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt))
                         self.log_formatted(self.warn_log_string, const.NOT_REQUIRED_ALERT + txt)
 
                 def set_mol_syn_src(syn_src, mol, cif_category, src_dict_in, flags_dict):
@@ -5187,15 +5190,15 @@
                         if flags_dict["add_cell"]:
                             set_el_cell(syn_src, cif_category, mol_syn_src_in)
                         if flags_dict["add_organelle"]:
                             set_el_organelle(syn_src, cif_category, mol_syn_src_in)
                         if flags_dict["add_cellular_location"]:
                             set_el_cellular_location(syn_src, cif_category, mol_syn_src_in)
 
-                        if syn_src.hasContent_():
+                        if syn_src._hasContent():
                             if flags_dict["add_syn_src"]:
                                 mol.add_synthetic_source(syn_src)
                             else:
                                 mol.set_synthetic_source(syn_src)
                             break
 
                 def set_rna_macromolecule_type(rna_mol, ent_in, ent_id_in, ent_poly_in, src_dicts):
@@ -5605,15 +5608,15 @@
                             self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                     elif ent_id_in in ent_non_poly_dict:
                         # Entity non-poly
                         lig_mol = emdb.ligand_macromolecule_type()
                         set_ligand_macromolecule_type(lig_mol, ent_in, ent_id_in, src_dicts)
                         mol_list.add_macromolecule(lig_mol)
 
-                    if mol_list.hasContent_():
+                    if mol_list._hasContent():
                         sample.set_macromolecule_list(mol_list)
 
             # element 1
             set_el_name()
             # element 2
             set_el_supramolecule_list(sample)
             # element 3
@@ -5805,15 +5808,15 @@
                     stain = emdb.stainingType()
                     # element 1
                     set_el_type(stain, stain_in)
                     # element 2
                     set_el_material(stain, stain_in)
                     # element 3
                     set_el_details(stain, stain_in)
-                    if stain.hasContent_():
+                    if stain._hasContent():
                         specimen.set_staining(stain)
 
             def set_el_sugar_embedding(specimen, sp_id_in, embed_dict_in):
                 """
                 XSD: <xs:element name="sugar_embedding" minOccurs="0">
                 """
 
@@ -5845,15 +5848,15 @@
                 if sp_id_in in embed_dict_in:
                     embed_in = embed_dict_in[sp_id_in]
                     el_material = get_cif_value("material", const.EM_EMBEDDING, cif_list=embed_in)
                     el_details = get_cif_value("details", const.EM_EMBEDDING, cif_list=embed_in)
                     if any(x is not None for x in [el_material, el_details]):
                         embed = emdb.sugar_embeddingType()
                         set_sugar_embedding_type(embed, embed_in)
-                        if embed.hasContent_():
+                        if embed._hasContent():
                             specimen.set_sugar_embedding(embed)
 
             def set_el_shadowing(specimen, sp_id_in, shadow_dict_in):
                 """
                 XSD: <xs:element name="shadowing" minOccurs="0">
                 """
 
@@ -5919,15 +5922,15 @@
                     el_material = get_cif_value("material", const.EM_SHADOWING, cif_list=shadow_in)
                     el_angle = get_cif_value("angle", const.EM_SHADOWING, cif_list=shadow_in)
                     el_thickness = get_cif_value("thickness", const.EM_SHADOWING, cif_list=shadow_in)
                     el_details = get_cif_value("details", const.EM_SHADOWING, cif_list=shadow_in)
                     if any(x is not None for x in [el_material, el_angle, el_thickness, el_details]):
                         shadow = emdb.shadowingType()
                         set_shadowing_type(shadow)
-                        if shadow.hasContent_():
+                        if shadow._hasContent():
                             specimen.set_shadowing(shadow)
 
             def set_el_grid(specimen, sp_id_in, grid_dict_in, film_dict_in, pretreat_dict_in):
                 """
                 XSD: <xs:element name="grid" type="grid_type">
                 """
 
@@ -6140,15 +6143,15 @@
                     # element 6
                     set_el_details(grid, grid_in)
 
                 if sp_id_in in grid_dict_in:
                     grid_in = grid_dict_in[sp_id_in]
                     grid = emdb.grid_type()
                     set_grid_type(grid, film_dict_in, pretreat_dict_in)
-                    if grid.hasContent_():
+                    if grid._hasContent():
                         specimen.set_grid(grid)
 
             def set_el_vitrification(specimen, sp_id_in, vitr_dict_in):
                 """
                 XSD: <xs:element name="vitrification" type="vitrification_type" minOccurs="0">
                 """
 
@@ -6283,15 +6286,15 @@
                     # element 7
                     set_el_method()
 
                 if sp_id_in in vitr_dict_in:
                     vitr_in = vitr_dict_in[sp_id_in]
                     vitr = emdb.vitrification_type()
                     set_vitrification_type(vitr, vitr_in)
-                    if vitr.hasContent_():
+                    if vitr._hasContent():
                         specimen.set_vitrification(vitr)
 
             def set_el_details(specimen, spec_prep_in):
                 """
                 XSD: <xs:element name="details" type="xs:string" minOccurs="0">
                 CIF: _em_specimen.details
                 """
@@ -6383,17 +6386,17 @@
                 fs_present = get_cif_value("fiducial_markers", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
                 if tom_id_in in fid_dict_in and fs_present == "YES":
                     fid_list = emdb.fiducial_markers_listType()
                     fid_list_in = fid_dict_in[tom_id_in]
                     for fid_in in fid_list_in:
                         fid = emdb.fiducial_marker_type()
                         set_fiducial_marker_type(fid, fid_in)
-                        if fid.hasContent_():
+                        if fid._hasContent():
                             fid_list.add_fiducial_marker(fid)
-                    if fid_list.hasContent_():
+                    if fid_list._hasContent():
                         tom_prep.set_fiducial_markers_list(fid_list)
 
             def set_el_high_pressure_freezing(tom_prep, tom_id_in, h_pfdict_in):
                 """
                 XSD: <xs:element name="high_pressure_freezing" minOccurs="0">
                 CIF: _em_tomography_specimen.high_pressure_freezing YES
                 """
@@ -6446,15 +6449,15 @@
                 if tom_id_in in h_pfdict_in and hpf_present == "YES":
                     h_pf_in = h_pfdict_in[tom_id_in]
                     el_instrument = get_cif_value("instrument", const.EM_HIGH_PRESSURE_FREEZING, cif_list=h_pf_in)
                     el_details = get_cif_value("details", const.EM_HIGH_PRESSURE_FREEZING, cif_list=h_pf_in)
                     if any(x is not None for x in [el_instrument, el_details]):
                         h_pf = emdb.high_pressure_freezingType()
                         set_high_pressure_freezing_type(h_pf, h_pf_in)
-                        if h_pf.hasContent_():
+                        if h_pf._hasContent():
                             tom_prep.set_high_pressure_freezing(h_pf)
 
             def set_el_embedding_material():
                 """
                 XSD: <xs:element name="embedding_material" minOccurs="0" type="xs:token">
                 CIF: ??
                 """
@@ -6674,21 +6677,21 @@
 
                 sec_in = get_cif_value("sectioning", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
                 if sec_in is not None:
                     if sec_in == "ULTRAMICROTOMY" and tom_id_in in u_tome_dict_in:
                         u_tome_in = u_tome_dict_in[tom_id_in]
                         u_tome = emdb.ultramicrotomyType()
                         set_ultramicrotomy_type(u_tome)
-                        if u_tome.hasContent_():
+                        if u_tome._hasContent():
                             tom_prep.set_sectioning(emdb.sectioningType(ultramicrotomy=u_tome))
                     elif sec_in == "FOCUSED ION BEAM" and tom_id_in in fib_dict_in:
                         fib_in = fib_dict_in[tom_id_in]
                         fib = emdb.focused_ion_beamType()
                         set_focused_ion_beam_type(fib)
-                        if fib.hasContent_():
+                        if fib._hasContent():
                             tom_prep.set_sectioning(emdb.sectioningType(focused_ion_beam=fib))
                     elif sec_in == "NO SECTIONING":
                         # XSD: choice 3: <xs:element name="other_sectioning" type="xs:string"/>
                         tom_prep.set_sectioning(emdb.sectioningType(other_sectioning=sec_in))
 
             # Create dictionaries where the tomography preparation id is key
             tom_prep_dict_in = make_dict(const.EM_TOMOGRAPHY_SPECIMEN, const.K_SPECIMEN_ID)
@@ -6813,15 +6816,15 @@
 
             cryst_dict_in = make_dict(const.EM_CRYSTAL_FORMATION, const.K_SPECIMEN_ID)
 
             if sp_id_in in cryst_dict_in:
                 cryst_in = cryst_dict_in[sp_id_in]
                 cryst = emdb.crystal_formationType()
                 set_crystal_formation_type(cryst)
-                if cryst.hasContent_():
+                if cryst._hasContent():
                     cryst_prep.set_crystal_formation(cryst)
 
         def set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in):
             """
             Classification for image processing
 
             @param ip_id_in: image processing id
@@ -7192,15 +7195,15 @@
                                 # element 3
                                 set_el_lower_energy_threshold(eng_flt, sp_op_in)
                                 # element 3
                                 set_el_upper_energy_threshold(eng_flt, sp_op_in)
 
                             eng_flt = emdb.energy_filterType()
                             set_energy_filter_type(eng_flt, sp_op_in)
-                            if eng_flt.hasContent_():
+                            if eng_flt._hasContent():
                                 sp_op.set_energy_filter(eng_flt)
 
                         def set_el_details(sp_op, sp_op_in):
                             """
                             XSD: <xs:element name="detals" type="xs:string" minOccurs="0"/>
                             CIF: _em_imaging_optics.details - NOT YET IMPLEMENTED IN mmcif dictionary
                             """
@@ -7469,18 +7472,18 @@
                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                     else:
                         im_rec_list_in = im_rec_dict_in[mic_id]
                         im_rec_list = emdb.image_recording_listType()
                         for im_rec_in in im_rec_list_in:
                             im_rec = emdb.image_recordingType()
                             set_image_recording_type(im_rec, im_rec_in, im_dig_dict_in)
-                            if im_rec.hasContent_():
+                            if im_rec._hasContent():
                                 im_rec_list.add_image_recording(im_rec)
 
-                        if im_rec_list.hasContent_():
+                        if im_rec_list._hasContent():
                             mic.set_image_recording_list(im_rec_list)
 
                 def set_base_microscopy(mic_in, mic, mic_id):
                     """
                     Set all elements for base microscopy
 
                     Parameters:
@@ -7861,26 +7864,26 @@
 
                         def set_el_axis1(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis1" type="axis_type"/>
                             CIF:
                             """
                             axis1 = get_tilt_axis(ts_in, axis1=True)
-                            if axis1.hasContent_():
+                            if axis1._hasContent():
                                 set_cif_value(tilt_ser.set_axis1, axis1)
 
                         def set_el_axis2(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis2" minOccurs="0"> has
                             .. a base of axis_type and
                             .. 1 element <xs:element name="axis_rotation" minOccurs="0">???
                             CIF:
                             """
                             axis2 = get_tilt_axis(ts_in, axis1=False)
-                            if axis2.hasContent_():
+                            if axis2._hasContent():
                                 set_cif_value(tilt_ser.set_axis2, axis2)
 
                         def set_el_axis_rotation(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis_rotation" fixed="90" minOccurs="0">
                             CIF: _em_tomography.dual_tilt_axis_rotation
                             """
@@ -7903,15 +7906,15 @@
                     # Create list of tomography tilt series that has microscopy id as a key.
                     tilt_dict_in = make_list_of_dicts(const.EM_TOMOGRAPHY, const.K_IMAGING_ID)
                     if mic_id in tilt_dict_in:
                         tilt_list_in = tilt_dict_in[mic_id]
                         for ts_in in tilt_list_in:
                             tilt_ser = emdb.tilt_series_type()
                             set_tilt_series_type(tilt_ser, ts_in)
-                            if tilt_ser.hasContent_():
+                            if tilt_ser._hasContent():
                                 mic.add_tilt_series(tilt_ser)
 
                 def set_cryst_mic_specifics(mic_id, cryst_mic):
                     """
                     Method that sets the crystalograhy specific microscopy elements
 
                     Parameters:
@@ -7947,15 +7950,15 @@
                         tilt_str_in = get_cif_value("tilt_angle_list", const.EM_DIFFRACTION, cry_mic_in)
                         if tilt_str_in is not None:
                             tilt_list_in = tilt_str_in.strip().split(",")
                             tilt_list = emdb.tilt_listType()
                             for tilt_in in tilt_list_in:
                                 # XSD: <xs:element name="tilt_list" minOccurs="1">
                                 tilt_list.add_angle(float(tilt_in))
-                            if tilt_list.hasContent_():
+                            if tilt_list._hasContent():
                                 cryst_mic.set_tilt_list(tilt_list)
                                 # choice 2 (IS THIS NECESSARY ????????????)
                                 # XSD: <xs:element name="tilt_series"
                                 #      type="tilt_series_type" maxOccurs="unbounded" minOccurs="1">
 
                 mic_list_in = self.cif.get(const.EM_IMAGING, None)
                 if mic_list_in != []:
@@ -8101,15 +8104,15 @@
                         # element 4
                         set_el_software_list(part_sel)
                         # element 5
                         set_el_details(part_sel, ps_in)
 
                     part_sel = emdb.particle_selection_type()
                     set_particle_selection_type(part_sel)
-                    if part_sel.hasContent_():
+                    if part_sel._hasContent():
                         im_proc.add_particle_selection(part_sel)
 
                 def set_ctfcorrection(ip_id_in, im_proc, ctf_corr_dict_in):
                     """
                     Sets CTF correction
 
                     @param ip_id_in: image processing id
@@ -8237,15 +8240,15 @@
                         # element 4
                         set_el_software_list(ctf_corr, cat_soft_dict_in)
                         # element 5
                         set_el_details(ctf_corr, ctf_corr_in)
 
                     ctf_corr = emdb.ctf_correction_type()
                     set_ctf_correction_type(ctf_corr)
-                    if ctf_corr.hasContent_():
+                    if ctf_corr._hasContent():
                         im_proc.set_ctf_correction(ctf_corr)
 
                 def set_startup_model(ip_id_in, im_proc, st_mod_dict_in):
                     """
                     Sets startup model
 
                     @param ip_id_in: image processing id
@@ -8427,15 +8430,15 @@
                                     # element 1
                                     set_el_chain_id_list()
 
                                 el_pdb_id = get_cif_value("pdb_id", const.EM_START_MODEL, cif_list=sm_in)
                                 if el_pdb_id is not None:
                                     pdb_mt = emdb.pdb_model_type()
                                     set_pdb_model_type(pdb_mt)
-                                    if pdb_mt.hasContent_():
+                                    if pdb_mt._hasContent():
                                         st_map.set_pdb_model(pdb_mt)
 
                             def set_choice_insilico_model(st_map, sm_in):
                                 """
                                 XSD: <xs:element name="insilico_model" type="xs:token" minOccurs="0"/>
                                 CIF: _em_start_model.insilico_model
                                 """
@@ -8448,20 +8451,20 @@
                                 """
                                 set_cif_value(st_map.set_other, "other", const.EM_START_MODEL, cif_list=sm_in)
 
                             t_of_m = get_cif_value("type", const.EM_START_MODEL, sm_in)
                             if t_of_m == "RANDOM CONICAL TILT":
                                 rct = emdb.random_conical_tiltType()
                                 set_choice_random_conical_tilt(rct, sm_in)
-                                if rct.hasContent_():
+                                if rct._hasContent():
                                     st_map.set_random_conical_tilt(rct)
                             elif t_of_m == "ORTHOGONAL TILT":
                                 orth_tilt = emdb.orthogonal_tiltType()
                                 set_choice_orthogonal_tilt(orth_tilt, sm_in)
-                                if orth_tilt.hasContent_():
+                                if orth_tilt._hasContent():
                                     st_map.set_orthogonal_tilt(orth_tilt)
                             elif t_of_m == "EMDB MAP":
                                 set_choice_emdb_id(st_map, sm_in)
                             elif t_of_m == "PDB ENTRY":
                                 set_choice_pdb_model(st_map, sm_in)
                             elif t_of_m == "INSILICO MODEL":
                                 set_choice_insilico_model(st_map, sm_in)
@@ -8582,15 +8585,15 @@
                                     # element 3
                                     set_el_axial_symmetry(h_sym, h_sym_in)
                                     # element 4 - REMOVED
                                     # set_el_hand(h_sym)
 
                                 h_sym = emdb.helical_parameters_type()
                                 set_helical_parameters_type(h_sym, h_sym_in)
-                                if h_sym.hasContent_():
+                                if h_sym._hasContent():
                                     app_sym.set_helical_parameters(h_sym)
 
                             p_sym_dict_in = final_dicts["p_sym_dict_in"]
                             h_sym_dict_in = final_dicts["h_sym_dict_in"]
                             if sym_type_in in ["2D CRYSTAL" "3D CRYSTAL"]:  # pylint: disable=implicit-str-concat
                                 # choice 1
                                 set_choice_space_group()
@@ -8604,15 +8607,15 @@
                                     # choice 3
                                     set_choice_helical_parameters(h_sym_in)
 
                         sym_type_in = get_cif_value("symmetry_type", const.EM_3D_RECONSTRUCTION, final_rec_in)
                         if sym_type_in is not None:
                             app_sym = emdb.applied_symmetry_type()
                             set_applied_symmetry_type(app_sym, final_dicts)
-                            if app_sym.hasContent_():
+                            if app_sym._hasContent():
                                 final_rec.set_applied_symmetry(app_sym)
 
                     def set_el_algorithm(final_rec, final_rec_in):
                         """
                         XSD: <xs:element name="algorithm" type="reconstruction_algorithm_type"  minOccurs="0">
                         CIF: _em_3d_reconstruction.algorithm
                             {ALGEBRAIC (ARTS),BACK PROJECTION,EXACT BACK PROJECTION,
@@ -8786,19 +8789,19 @@
                             """
                             XSD: <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
                             CIF: _em_euler_angle_assignment.order {FINAL,INITIAL}
                             """
                             order = get_cif_value("order", const.EM_EULER_ANGLE_ASSIGNMENT, ang_in)
                             if order == "INITIAL" and em_method == const.EMM_SP:
                                 set_software_list(const.SOFT_INITIAL_EULER_ASSIGNMENT, cat_soft_dict_in, ang.set_software_list)
-                                if ang.hasContent_():
+                                if ang._hasContent():
                                     im_proc.set_initial_angle_assignment(ang)
                             elif order == "FINAL":
                                 set_software_list(const.SOFT_FINAL_EULER_ASSIGNMENT, cat_soft_dict_in, ang.set_software_list)
-                                if ang.hasContent_():
+                                if ang._hasContent():
                                     im_proc.set_final_angle_assignment(ang)
 
                         def set_el_details(ang, ang_in):
                             """
                             XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                             CIF: _em_euler_angle_assignment.details
                             """
@@ -8924,15 +8927,15 @@
                                 # element 6
                                 set_el_alpha(u_cell, cryst_in, dict_category)
                                 # element 7
                                 set_el_beta(u_cell, cryst_in, dict_category)
 
                             u_cell = emdb.unit_cell_type()
                             set_unit_cell_type(u_cell, cryst_in, dict_category, parent_req)
-                            if u_cell.hasContent_():
+                            if u_cell._hasContent():
                                 cryst.set_unit_cell(u_cell)
 
                         def set_choice_plane_group():
                             """
                             XSD: <xs:element name="plane_group">
                             CIF:????
                             """
@@ -8968,15 +8971,15 @@
                         el_choice_space_group = get_cif_value("space_group", const.EM_3D_CRYSTAL_ENTITY, cif_list=cryst_in)
                     elif dict_category == const.EM_2D_CRYSTAL_ENTITY:
                         el_choice_space_group = get_cif_value("plane_group", const.EM_2D_CRYSTAL_ENTITY, cif_list=cryst_in)
                     crystal_parameters_type_list = [el_a, el_b, el_c, el_c_sampling_length, el_gamma, el_alpha, el_beta, el_choice_space_group]
                     if any(x is not None for x in crystal_parameters_type_list):
                         cryst = emdb.crystal_parameters_type()
                         set_crystal_parameters_type(cryst, cryst_in, dict_category, parent_req)
-                        if cryst.hasContent_():
+                        if cryst._hasContent():
                             im_proc.set_crystal_parameters(cryst)
 
                 def set_non_sub_tom_final_recon(ip_id_in, im_proc, non_st_dicts):
                     """
                     Final reconstruction for non-subtomographs
 
                     @param ip_id_in: image processing id
@@ -9091,26 +9094,26 @@
                         """
                         XSD: <xs:element name="final_two_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_2d_class_dict_in = sp_dict_list["final_2d_class_dict_in"]
                         cat_soft_dict_in = sp_dict_list["cat_soft_dict_in"]
                         if ip_id_in in final_2d_class_dict_in:
                             f2dc = set_classification(ip_id_in, final_2d_class_dict_in, cat_soft_dict_in)
-                            if f2dc.hasContent_():
+                            if f2dc._hasContent():
                                 im_proc.set_final_two_d_classification(f2dc)
 
                     def set_el_final_three_d_class(ip_id_in, im_proc, sp_dict_list):
                         """
                         XSD: <xs:element name="final_three_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_class_dict_in = sp_dict_list["final_class_dict_in"]
                         cat_soft_dict_in = sp_dict_list["cat_soft_dict_in"]
                         if ip_id_in in final_class_dict_in:
                             f3dc = set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in)
-                            if f3dc.hasContent_():
+                            if f3dc._hasContent():
                                 im_proc.set_final_three_d_classification(f3dc)
 
                     # element 1
                     set_el_particle_selection(ip_id_in, im_proc, sp_dict_list)
                     # element 2
                     set_el_ctf_correction(ip_id_in, im_proc, sp_dict_list)
                     # element 3
@@ -9248,15 +9251,15 @@
                             set_el_details(extraction, vs_in)
 
                         vol_sel_dict_in = subtom_dicts["vol_sel_dict_in"]
                         if ip_id_in in vol_sel_dict_in:
                             vs_in = vol_sel_dict_in[ip_id_in]
                             extraction = emdb.extractionType()
                             set_extraction_type(extraction, vs_in, subtom_dicts)
-                            if extraction.hasContent_():
+                            if extraction._hasContent():
                                 im_proc.set_extraction(extraction)
 
                     def set_el_ctf_correction(im_proc, ip_id_in, subtom_dicts):
                         """
                         XSD: <xs:element name="ctf_correction" type="ctf_correction_type"/>
                         """
                         ctf_corr_dict_in = subtom_dicts["ctf_corr_dict_in"]
@@ -9273,15 +9276,15 @@
                         """
                         XSD: <xs:element name="final_three_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_class_dict_in = subtom_dicts["final_class_dict_in"]
                         cat_soft_dict_in = subtom_dicts["cat_soft_dict_in"]
                         if ip_id_in in final_class_dict_in:
                             f3dc = set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in)
-                            if f3dc.hasContent_():
+                            if f3dc._hasContent():
                                 im_proc.set_final_three_d_classification(f3dc)
 
                     def set_el_final_angle_assignment(im_proc, subtom_dicts, em_method):
                         """
                         XSD: <xs:element name="final_angle_assignment" type="angle_assignment_type" minOccurs="0"/>
                         """
                         ang_dict_in = subtom_dicts["ang_dict_in"]
@@ -9437,15 +9440,15 @@
 
                         part_sel_dict_in = hel_dict_list["part_sel_dict_in"]
                         if ip_id_in in part_sel_dict_in:
                             ps_list_in = part_sel_dict_in[ip_id_in]
                             for ps_in in ps_list_in:
                                 seg_sel = emdb.segment_selection_type()
                                 set_segment_selection_type(seg_sel, ps_in)
-                                if seg_sel.hasContent_():
+                                if seg_sel._hasContent():
                                     im_proc.add_segment_selection(seg_sel)
 
                     def set_el_refinement(im_proc):
                         """
                         XSD: <xs:element name="refinement" type="refinement_type"/>
                         """
 
@@ -9458,15 +9461,15 @@
                             XSD: <xs:element name="starting_symmetry" maxOccurs="unbounded">
                             XSD: <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
                             XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                             """
 
                         refinement = emdb.refinement_type()
                         set_refinement_type()
-                        if refinement.hasContent_():
+                        if refinement._hasContent():
                             im_proc.set_refinement(refinement)
 
                     def set_el_startup_model(im_proc, ip_id_in, hel_dict_list):
                         """
                         XSD: <xs:element name="startup_model" type="starting_map_type" maxOccurs="unbounded" minOccurs="0">
                         """
                         st_mod_dict_in = hel_dict_list["st_mod_dict_in"]
@@ -9486,15 +9489,15 @@
                             XSD: <xs:element name="helix_length">
                             XSD: <xs:element name="straightening" type="xs:boolean" minOccurs="0"/>
                             XSD: <xs:element name="indexing">
                             """
 
                         lay_lines = emdb.layer_lines_type()
                         set_layer_lines_type()
-                        if lay_lines.hasContent_():
+                        if lay_lines._hasContent():
                             im_proc.set_helical_layer_lines(lay_lines)
 
                     def set_el_initial_angle_assignment():
                         """
                         XSD: <xs:element name="initial_angle_assignment" type="angle_assignment_type" minOccurs="0"/>
                         """
 
@@ -9635,15 +9638,15 @@
                             # element 2
                             set_el_resolution_range()
                             # element 3
                             set_el_software_list(mol_repl, cryst_dicts)
 
                         mol_repl = emdb.molecular_replacement_type()
                         set_molecular_replacement_type(mol_repl, cryst_dicts)
-                        if mol_repl.hasContent_():
+                        if mol_repl._hasContent():
                             im_proc.set_molecular_replacement(mol_repl)
 
                     def set_el_lat_dist_corr_soft_list(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="lattice_distortion_correction_software_list" type="software_list_type" minOccurs="0"/>
                         """
                         set_software_list(const.LATTICE_DISTORTION_CORRECTION, cryst_dicts["cat_soft_dict_in"], im_proc.set_lattice_distortion_correction_software_list)
@@ -9893,17 +9896,17 @@
                                                 el_phase_residual,
                                                 el_fourier_space_coverage,
                                                 el_multiplicity,
                                             ]
                                             if any(x is not None for x in shell_type_list):
                                                 shell = emdb.shellType()
                                                 set_shell_type(shell, cs_in)
-                                                if shell.hasContent_():
+                                                if shell._hasContent():
                                                     cry_shell_list.add_shell(shell)
-                                        if cry_shell_list.hasContent_():
+                                        if cry_shell_list._hasContent():
                                             cry_stats.set_shell_list(cry_shell_list)
 
                             def set_el_details(cry_stats, cry_stats_in):
                                 """
                                 XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                                 CIF: _em_diffraction_stats.details
                                 """
@@ -9933,15 +9936,15 @@
                             set_el_details(cry_stats, cry_stats_in)
 
                         cry_stats_dict_in = cryst_dicts["cry_stats_dict_in"]
                         if ip_id_in in cry_stats_dict_in:
                             cry_stats_in = cry_stats_dict_in[ip_id_in]
                             cry_stats = emdb.crystallography_statistics_type()
                             set_cryst_statistics_type(cry_stats, cry_stats_in)
-                            if cry_stats.hasContent_():
+                            if cry_stats._hasContent():
                                 im_proc.set_crystallography_statistics(cry_stats)
 
                     # element 1
                     set_el_final_reconstruction(im_proc, ip_id_in)
                     # element 2
                     set_el_crystal_parameters(im_proc, ip_id_in, cryst_dicts)
                     # element 3
@@ -10235,15 +10238,15 @@
                         Only space_group choice has mmCIF value
                         CIF: _em_map.symmetry_space_group 1
                         """
                         set_cif_value(app_sym.set_space_group, "symmetry_space_group", const.EM_MAP, cif_list=map_in, fmt=int)
 
                     app_sym = emdb.applied_symmetry_type()
                     set_applied_symmetry_type(app_sym)
-                    if app_sym.hasContent_():
+                    if app_sym._hasContent():
                         em_map.set_symmetry(app_sym)
 
                 def set_el_data_type(em_map, map_in):
                     """
                     XSD: <xs:element name="data_type" type="map_data_type"/>
                     CIF: _em_map.data_type 'Image stored as signed byte'
                     """
@@ -10286,15 +10289,15 @@
                         # element 2
                         set_el_row(dim, map_in)
                         # element 3
                         set_el_sec(dim, map_in)
 
                     dim = emdb.integer_vector_map_type()
                     set_integer_vector_map_type(dim, map_in)
-                    if dim.hasContent_():
+                    if dim._hasContent():
                         em_map.set_dimensions(dim)
 
                 def set_el_origin(em_map, map_in):
                     """
                     XSD: <xs:element name="origin">
                     """
 
@@ -10671,17 +10674,17 @@
                         set_el_contour_level(cntr, map_in)
                         # element 2
                         set_el_source(cntr, map_in)
 
                     cntr_list = emdb.contour_listType()
                     cntr = emdb.contourType()
                     set_contour_type(cntr, map_in)
-                    if cntr.hasContent_():
+                    if cntr._hasContent():
                         cntr_list.add_contour(cntr)
-                    if cntr_list.hasContent_():
+                    if cntr_list._hasContent():
                         em_map.set_contour_list(cntr_list)
 
                 def set_el_label(em_map, map_in):
                     """
                     XSD: <xs:element name="label" type="xs:token" minOccurs="0"/>
                     CIF: _em_map.label
                     """
@@ -10883,15 +10886,15 @@
                 len_pr_map_list_in = len(pr_map_list_in)
                 if len_pr_map_list_in != 1:
                     txt = u"There should be one and only one primary map. (%d) map(s) found." % len_pr_map_list_in
                     self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                     self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                 else:
                     em_map = make_map(pr_map_list_in[0], get_canonical_map_name(pr_map_list_in[0], "PRIMARY"))
-                    if em_map.hasContent_():
+                    if em_map._hasContent():
                         self.xml_out.set_map(em_map)
                     else:
                         txt = u"No information given for the primary map."
                         self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
             def set_el_interpretation():
@@ -11025,15 +11028,15 @@
                                         # element 2
                                         chain = emdb.chainType()
                                         set_el_id(chain, model_in)
                                         set_el_residue_range(chain, model_in)
                                         set_el_numofcps_in_final_model(chain, model_in)
                                         set_el_source_name(chain, model_in)
                                         set_el_initial_model_type(chain, model_in)
-                                        if chain.hasContent_():
+                                        if chain._hasContent():
                                             model.set_chain(chain)
 
                                     def set_el_details(model, model_in):
                                         """
                                         XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                                         CIF: _em_3d_fitting_list.details
                                         """
@@ -11044,15 +11047,15 @@
                                     set_el_chain(model, model_in)
                                     # element 3
                                     set_el_details(model, model_in)
                                 if modelling_id_in in model_dict_in:
                                     for model_in in model_dict_in[modelling_id_in]:
                                         model = emdb.initial_modelType()
                                         set_initial_model_type(model, model_in)
-                                        if model.hasContent_():
+                                        if model._hasContent():
                                             modelling.add_initial_model(model)
 
                             def set_el_final_model():
                                 """
                                 XSD: <xs:element name="final_model" minOccurs="0"> has
                                 .. 3 elements
                                 CIF: there is no _emd_modelling_final_model !!!
@@ -11128,17 +11131,17 @@
                         modelling_list = emdb.modelling_listType()
                         modelling_list_in = self.cif.get(const.EM_3D_FITTING)
                         model_dict_in = make_list_of_dicts(const.EM_3D_FITTING_LIST, const.K_3D_FITTING_ID)
                         for modelling_in in modelling_list_in:
                             modelling_id_in = get_cif_value(const.K_ID, const.EM_3D_FITTING, modelling_in)
                             modelling = emdb.modelling_type()
                             set_modelling_type(modelling, modelling_in, cat_soft_dict_in)
-                            if modelling.hasContent_():
+                            if modelling._hasContent():
                                 modelling_list.add_modelling(modelling)
-                        if modelling_list.hasContent_():
+                        if modelling_list._hasContent():
                             intrp.set_modelling_list(modelling_list)
 
                     def set_el_figure_list():
                         """
                         XSD: <xs:element name="figure_list" minOccurs="0">
                         CIF: ??
                         """
@@ -11182,19 +11185,19 @@
                             # element 3
                             set_el_mask_details()
 
                         mask_list_in = map_dict_in[const.MAP_MASK] if const.MAP_MASK in map_dict_in else []
                         seg_list = emdb.segmentation_listType()
                         for msk_in in mask_list_in:
                             msk = make_map(msk_in, get_canonical_map_name(msk_in, "MASK"))
-                            if msk.hasContent_():
+                            if msk._hasContent():
                                 seg = emdb.segmentationType()
                                 set_segmentation_type(seg, msk)
                                 seg_list.add_segmentation(seg)
-                        if seg_list.hasContent_():
+                        if seg_list._hasContent():
                             intrp.set_segmentation_list(seg_list)
 
                     def set_el_slices_list():
                         """
                         XSD: <xs:element name="slices_list" minOccurs="0">
                         CIF: Deprecated (2014-10-21)
                         """
@@ -11203,30 +11206,30 @@
                         """
                         XSD: <xs:element name="additional_map_list" minOccurs="0">
                         """
                         add_map_list_in = map_dict_in[const.MAP_ADD] if const.MAP_ADD in map_dict_in else []
                         add_map_list = emdb.additional_map_listType()
                         for add_map_in in add_map_list_in:
                             add_map = make_map(add_map_in, get_canonical_map_name(add_map_in, "ADDMAP"))
-                            if add_map.hasContent_():
+                            if add_map._hasContent():
                                 add_map_list.add_additional_map(add_map)
-                        if add_map_list.hasContent_():
+                        if add_map_list._hasContent():
                             intrp.set_additional_map_list(add_map_list)
 
                     def set_el_half_map_list(intrp, map_dict_in):
                         """
                         XSD: <xs:element name="half_map_list" minOccurs="0">
                         """
                         hf_map_list_in = map_dict_in[const.MAP_HALF] if const.MAP_HALF in map_dict_in else []
                         hf_map_list = emdb.half_map_listType()
                         for hf_map_in in hf_map_list_in:
                             hf_map = make_map(hf_map_in, get_canonical_map_name(hf_map_in, "HALFMAP"))
-                            if hf_map.hasContent_():
+                            if hf_map._hasContent():
                                 hf_map_list.add_half_map(hf_map)
-                        if hf_map_list.hasContent_():
+                        if hf_map_list._hasContent():
                             intrp.set_half_map_list(hf_map_list)
 
                     # element 1
                     set_el_modelling_list(intrp)
                     # element 2
                     set_el_figure_list()
                     # element 3
@@ -11237,15 +11240,15 @@
                     set_el_additional_map_list(intrp, map_dict_in)
                     # element 6
                     set_el_half_map_list(intrp, map_dict_in)
 
                 map_dict_in = make_list_of_dicts(const.EM_MAP, "type")
                 intrp = emdb.interpretation_type()
                 set_interpretation_type(intrp, map_dict_in)
-                if intrp.hasContent_():
+                if intrp._hasContent():
                     self.xml_out.set_interpretation(intrp)
 
             def set_el_validation():
                 """
                 XSD: <xs:element name="validation" minOccurs="0">
                 There should be 4 validation methods:
                 1. crystallography validation
@@ -11282,17 +11285,17 @@
 
                 validation = emdb.validationType()
                 fsc_list_in = self.cif.get(const.EM_FSC_CURVE, None)
                 for fsc_in in fsc_list_in:
                     fsc = emdb.fsc_curve_validation_type()
                     fsc.original_tagname_ = "fsc_curve"
                     set_fsc_curve(fsc, fsc_in)
-                    if fsc.hasContent_():
+                    if fsc._hasContent():
                         validation.add_validation_method(fsc)
-                if validation.hasContent_():
+                if validation._hasContent():
                     self.xml_out.set_validation(validation)
 
             # attribute 1
             set_attr_emdb_id()
             # attribute 2
             set_attr_version()
             # element 1
```

### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 0% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.3.2"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.3.3"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -2558,15 +2558,15 @@
       <xs:enumeration value="GENERIC TVIPS (2k x 2k)"/>
       <xs:enumeration value="GENERIC TVIPS (4k x 4k)"/>
       <xs:enumeration value="KODAK 4489 FILM"/>
       <xs:enumeration value="KODAK SO-163 FILM"/>
       <xs:enumeration value="OTHER"/>
       <xs:enumeration value="PROSCAN TEM-PIV (2k x 2k)"/>
       <xs:enumeration value="SIA 15C (3k x 3k)"/>
-      <xs:enumeration value="TFS FALCON 4i (4k x 4x)"/>
+      <xs:enumeration value="TFS FALCON 4i (4k x 4k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F216 (2k x 2k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F224 (2k x 2k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F415 (4k x 4k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F416 (4k x 4k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F816 (8k x 8k)"/>
     </xs:restriction>
   </xs:simpleType>
```

### Comparing `wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.2
+Version: 1.3
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

