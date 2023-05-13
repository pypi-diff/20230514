# Comparing `tmp/dr_import-0.2.8-py3-none-any.whl.zip` & `tmp/dr_import-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 76129 bytes, number of entries: 23
+Zip file size: 76515 bytes, number of entries: 23
 -rwxrwxrwx  2.0 unx        0 b- defN 21-Mar-16 19:06 dr_import/__init__.py
 -rwxrwxrwx  2.0 unx     2678 b- defN 21-Aug-10 19:40 dr_import/analyze_gps.py
 -rwxrwxrwx  2.0 unx     3046 b- defN 21-Aug-11 18:56 dr_import/analyze_trip.py
--rwxrwxrwx  2.0 unx    20207 b- defN 21-Apr-16 13:42 dr_import/clone_mrem_section.py
+-rwxrwxrwx  2.0 unx    21872 b- defN 21-Oct-08 12:46 dr_import/clone_mrem_section.py
 -rwxrwxrwx  2.0 unx     2359 b- defN 21-Jul-30 18:19 dr_import/clone_mrem_trip.py
 -rwxrwxrwx  2.0 unx     2377 b- defN 21-Jul-30 18:19 dr_import/clone_mrem_trips_to_noaa.py
 -rwxrwxrwx  2.0 unx     4637 b- defN 21-Mar-16 19:06 dr_import/clone_trip.py
 -rwxrwxrwx  2.0 unx    18989 b- defN 21-Mar-16 19:06 dr_import/clone_trip2.py
 -rwxrwxrwx  2.0 unx     7231 b- defN 21-Aug-10 19:39 dr_import/import_gps.py
--rwxrwxrwx  2.0 unx    10536 b- defN 21-Aug-10 19:38 dr_import/import_media.py
+-rwxrwxrwx  2.0 unx    10675 b- defN 21-Oct-08 13:09 dr_import/import_media.py
 -rwxrwxrwx  2.0 unx     5208 b- defN 21-Jul-30 18:19 dr_import/import_poll_gps.py
 -rwxrwxrwx  2.0 unx     7025 b- defN 21-Mar-16 19:06 dr_import/legacy_import.py
 -rwxrwxrwx  2.0 unx     1924 b- defN 21-Mar-29 18:36 dr_import/local_gaps.py
 -rwxrwxrwx  2.0 unx     5373 b- defN 21-Apr-07 18:54 dr_import/make_management_report.py
 -rwxrwxrwx  2.0 unx     6204 b- defN 21-Apr-07 18:54 dr_import/make_trip.py
 -rwxrwxrwx  2.0 unx     7659 b- defN 21-Jul-30 18:19 dr_import/nvr_import.py
 -rwxrwxrwx  2.0 unx     3130 b- defN 21-Apr-08 23:32 dr_import/trim_trip.py
 -rwxrwxrwx  2.0 unx    51441 b- defN 21-Mar-16 19:06 dr_import/trip_summary.png
 -rwxrwxrwx  2.0 unx     5122 b- defN 21-Mar-16 19:06 dr_import/update_media.py
--rwxrwxrwx  2.0 unx      430 b- defN 21-Aug-13 19:27 dr_import-0.2.8.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 21-Aug-13 19:27 dr_import-0.2.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       10 b- defN 21-Aug-13 19:27 dr_import-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1880 b- defN 21-Aug-13 19:27 dr_import-0.2.8.dist-info/RECORD
-23 files, 167558 bytes uncompressed, 73105 bytes compressed:  56.4%
+-rwxrwxrwx  2.0 unx      430 b- defN 21-Oct-08 13:10 dr_import-0.2.9.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 21-Oct-08 13:10 dr_import-0.2.9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       10 b- defN 21-Oct-08 13:10 dr_import-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1880 b- defN 21-Oct-08 13:10 dr_import-0.2.9.dist-info/RECORD
+23 files, 169362 bytes uncompressed, 73491 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: dr_import/trip_summary.png
 Comment: 
 
 Filename: dr_import/update_media.py
 Comment: 
 
-Filename: dr_import-0.2.8.dist-info/METADATA
+Filename: dr_import-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: dr_import-0.2.8.dist-info/WHEEL
+Filename: dr_import-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: dr_import-0.2.8.dist-info/top_level.txt
+Filename: dr_import-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dr_import-0.2.8.dist-info/RECORD
+Filename: dr_import-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dr_import/clone_mrem_section.py

```diff
@@ -1,26 +1,30 @@
 """ Clones a MREM trip/section to another project/section
 Assumptions:
 - Types are the same in the source/destination projects
 - Assumes using Baseline version
 """
 
 import argparse
+import datetime
+import dateutil
 import os
 
 import tator
 
 def main(
         in_host: str,
         in_token: str,
         in_src_project: int,
         in_dest_project: int,
         in_src_section_name: str,
         in_dest_section_name: str,
-        in_copy_annotations: bool) -> None:
+        in_copy_annotations: bool,
+        in_start_time: datetime.datetime,
+        in_end_time: datetime.datetime) -> None:
     """ Clones the section (including GPS)
 
     :param in_host: Tator URL
     :param in_token: Tator API token
     :param in_src_project: Project ID that includes the section name to be cloned
     :param in_dest_project: Destination project ID
     :param in_src_section_name: Section to clone
@@ -122,18 +126,18 @@
                 src_em_specific_type = state_type.id
 
             elif state_type.name == "Fishing Op. Event":
                 if src_fishing_op_type != None:
                     raise ValueError(f"Invalid amount of Fishing Op. Event types in project {in_src_project}!")
                 src_fishing_op_type = state_type.id
 
-            elif state_type.name == "Video Qual. Event":
-                if src_video_qual_type != None:
-                    raise ValueError(f"Invalid amount of Video Qual. Event types in project {in_src_project}!")
-                src_video_qual_type = state_type.id
+            #elif state_type.name == "Video Qual. Event":
+            #    if src_video_qual_type != None:
+            #        raise ValueError(f"Invalid amount of Video Qual. Event types in project {in_src_project}!")
+            #    src_video_qual_type = state_type.id
 
     # Get the corresponding section ID
     src_section = tator_api.get_section_list(
         project=in_src_project, name=in_src_section_name)[0].id
 
     if in_dest_project == in_src_project:
         dest_multi_type = src_multi_type
@@ -242,18 +246,18 @@
                     dest_em_specific_type = state_type.id
 
                 elif state_type.name == "Fishing Op. Event":
                     if dest_fishing_op_type != None:
                         raise ValueError(f"Invalid amount of Fishing Op. Event types in project {in_dest_project}!")
                     dest_fishing_op_type = state_type.id
 
-                elif state_type.name == "Video Qual. Event":
-                    if dest_video_qual_type != None:
-                        raise ValueError(f"Invalid amount of Video Qual. Event types in project {in_dest_project}!")
-                    dest_video_qual_type = state_type.id
+                #elif state_type.name == "Video Qual. Event":
+                #    if dest_video_qual_type != None:
+                #        raise ValueError(f"Invalid amount of Video Qual. Event types in project {in_dest_project}!")
+                #    dest_video_qual_type = state_type.id
 
     # Create the new trip/section in the target project
     #response = tator_api.create_section_list(project=dest_project, name=in_dest_section_name)
     #dest_section = tator_api.get_section_list(id=response.id)
 
     # Create the new single-view trip/section in the target project
     #response = tator_api.create_section_list(project=dest_project, name=in_dest_single_view_section)
@@ -261,16 +265,28 @@
 
     # Grab the multviews we care about
     src_multis = tator_api.get_media_list(
         project=in_src_project, type=src_multi_type, section=src_section)
 
     # Clone the new multi-view media
     media_ids = []
+    filtered_src_multis = []
     for multi in src_multis:
-        media_ids.append(multi.id)
+
+        if in_start_time is not None and in_end_time is not None:
+            current_multi_date = dateutil.parser.parse(multi.name.split(".multi")[0])
+            if in_start_time <= current_multi_date <= in_end_time:
+                media_ids.append(multi.id)
+                filtered_src_multis.append(multi)
+        else:
+            media_ids.append(multi.id)
+            filtered_src_multis(multi)
+
+    print(f"Cloning media: {len(media_ids)} of {len(src_multis)}")
+    src_multis = filtered_src_multis
 
     spec = {
       "dest_project": in_dest_project,
       "dest_type": dest_multi_type,
       "dest_section": in_dest_section_name
     }
     response = tator_api.clone_media_list(
@@ -402,39 +418,46 @@
 
         if len(states) > 0:
             response = tator_api.create_state_list(project=in_dest_project, state_spec=dest_state_specs)
             print(response)
 
     if in_copy_annotations:
         # Copy over the other states if requested
-        src_state_types = [src_haul_type, src_crew_type, src_em_specific_type, src_video_qual_type, src_fishing_op_type]
-        dest_state_types = [dest_haul_type, dest_crew_type, dest_em_specific_type, dest_video_qual_type, dest_fishing_op_type]
-
-        for src_video_id, dest_video_ids in prime_video_mapping.items():
-            for src_type, dest_type in zip(src_state_types, dest_state_types):
-                states = tator_api.get_state_list(
-                    project=in_src_project, media_id=[src_video_id], type=src_type)
-
-                # #TODO look into tator.util.clone_state_list to do this
-                dest_state_specs = []
-                for state in states:
-                    spec = {
-                        "type": dest_type,
-                        "media_ids": dest_video_ids,
-                        "localization_ids": [],
-                        "version": dest_baseline_version,
-                        **state.attributes
-                    }
-                    if state.frame is not None:
-                        spec["frame"] = state.frame
-                    dest_state_specs.append(spec)
-
-                if len(states) > 0:
-                    response = tator_api.create_state_list(project=in_dest_project, state_spec=dest_state_specs)
-                    print(response)
+        if src_video_qual_type is not None:
+            src_state_types = [src_haul_type, src_crew_type, src_em_specific_type, src_video_qual_type, src_fishing_op_type]
+            dest_state_types = [dest_haul_type, dest_crew_type, dest_em_specific_type, dest_video_qual_type, dest_fishing_op_type]
+        else:
+            src_state_types = [src_haul_type, src_crew_type, src_em_specific_type, src_fishing_op_type]
+            dest_state_types = [dest_haul_type, dest_crew_type, dest_em_specific_type, dest_fishing_op_type]
+
+        try:
+            for src_video_id, dest_video_ids in prime_video_mapping.items():
+                for src_type, dest_type in zip(src_state_types, dest_state_types):
+                    states = tator_api.get_state_list(
+                        project=in_src_project, media_id=[src_video_id], type=src_type)
+
+                    # #TODO look into tator.util.clone_state_list to do this
+                    dest_state_specs = []
+                    for state in states:
+                        spec = {
+                            "type": dest_type,
+                            "media_ids": dest_video_ids,
+                            "localization_ids": [],
+                            "version": dest_baseline_version,
+                            **state.attributes
+                        }
+                        if state.frame is not None:
+                            spec["frame"] = state.frame
+                        dest_state_specs.append(spec)
+
+                    if len(states) > 0:
+                        response = tator_api.create_state_list(project=in_dest_project, state_spec=dest_state_specs)
+                        print(response)
+        except Exception as exc:
+            print(exc)
 
         # Copy over the other localizations if requested
         for src_video_id, dest_video_id in single_video_mapping.items():
             locs = tator_api.get_localization_list(
                 project=in_src_project, media_id=[src_video_id], type=src_discard_type)
 
             dest_loc_specs = []
@@ -465,25 +488,38 @@
     parser.add_argument('--host', type=str, required=True)
     parser.add_argument('--token', type=str, required=True)
     parser.add_argument('--src-project', type=int, required=True)
     parser.add_argument('--src-section-name', type=str, required=True)
     parser.add_argument('--dest-project', type=int, required=True)
     parser.add_argument('--dest-section-name', type=str, required=True)
     parser.add_argument('--copy-annotations', action='store_true')
+    parser.add_argument('--start-time', type=str, default="Use in conjunction with end-time argument. Omit to copy entire trip. Example: 2021-08-02T16:11:53")
+    parser.add_argument('--end-time', type=str, default="Use in conjunction with end-time argument. Omit to copy entire trip. Example: 2021-08-02T16:11:53")
     args = parser.parse_args()
     return args
 
 def script_main() -> None:
     """ Script's entry point
     """
     args = parse_args()
+
+    start_time = None
+    if args.start_time is not None:
+        start_time = dateutil.parser.parse(args.start_time)
+
+    end_time = None
+    if args.end_time is not None:
+        end_time = dateutil.parser.parse(args.end_time)
+
     main(
         in_host=args.host,
         in_token=args.token,
         in_src_project=args.src_project,
         in_src_section_name=args.src_section_name,
         in_dest_project=args.dest_project,
         in_dest_section_name=args.dest_section_name,
-        in_copy_annotations=args.copy_annotations)
+        in_copy_annotations=args.copy_annotations,
+        in_start_time=start_time,
+        in_end_time=end_time)
 
 if __name__ == "__main__":
     script_main()
```

## dr_import/import_media.py

```diff
@@ -32,32 +32,32 @@
     path = os.path.basename(full_path)
     file_type = os.path.splitext(path)[0]
     if file_type == "archival":
         if args.skip_archival is True:
             return True
         filename = os.path.basename(path)
         for _, upload_info in _upload_file(api, project, full_path,
-                                           media_id=media_id, filename=filename):
+                                           media_id=media_id, filename=filename, chunk_size=0xa0000000):
             pass
         media_def = {**make_video_definition(full_path),
                      'path': upload_info.key}
         # Patch in video file with the api.
         response = api.create_video_file(media_id, role='archival',
                                          video_definition=media_def)
     else:
         filename = os.path.basename(path)
         for _, upload_info in _upload_file(api, project, full_path,
-                                           media_id=media_id, filename=filename):
+                                           media_id=media_id, filename=filename, chunk_size=0xa0000000):
             pass
         with tempfile.TemporaryDirectory() as td:
             filename = f"{uuid.uuid4()}.json"
             segments_path = os.path.join(td, filename)
             make_fragment_info(full_path, segments_path)
             for _, segment_info in _upload_file(api, project, segments_path,
-                                                media_id=media_id, filename=filename):
+                                                media_id=media_id, filename=filename, chunk_size=0xa0000000):
                 pass
         # Construct create video file spec.
         media_def = {**make_video_definition(full_path),
                      'path': upload_info.key,
                      'segment_info': segment_info.key}
         response = api.create_video_file(media_id, role='streaming',
                                          video_definition=media_def)
@@ -193,15 +193,16 @@
                                                         'type': args.type_id,
                                                         'md5': tator.util.md5sum(video_fp)})
             media_id = media_response.id
             for p,_ in tator.util.upload_media(api,
                                                args.type_id,
                                                video_fp,
                                                upload_gid=upload_gid,
-                                               media_id=media_id):
+                                               media_id=media_id,
+                                               chunk_size=0xa0000000):
                 print(f"\r{p}%",end='')
             print("\rComplete")
         else:
             # This path is deprecated because it assumes we did client side recording
             # that is compatible with the web player.
             md5sum = tator.util.md5sum(media_path)
             spec ={
```

## Comparing `dr_import-0.2.8.dist-info/RECORD` & `dr_import-0.2.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 dr_import/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dr_import/analyze_gps.py,sha256=ngtjB2NBv3dIf0jf2ctQlwEW58NryhmEuZOfDsU0v4c,2678
 dr_import/analyze_trip.py,sha256=3hc1YSlNtkHQwGS9vI1lYt1YBFg5x0w8SRcAeO1_xbQ,3046
-dr_import/clone_mrem_section.py,sha256=qITnCclrxYj3RR_F3RXlhhnFuXvWZQphJtPMDVpa3fY,20207
+dr_import/clone_mrem_section.py,sha256=XaszHEs0bRQcRV0r9cJSkXq2F7Dvf3_lt-rwtZ0bces,21872
 dr_import/clone_mrem_trip.py,sha256=Q9OfG34QkqcUYcP1ErzFv7rnOShDgCiOdoghvmNkEyM,2359
 dr_import/clone_mrem_trips_to_noaa.py,sha256=Fp2NssYDIPbEtGlUgLu_GoLTriDdY7IcFR4o8IGqDvo,2377
 dr_import/clone_trip.py,sha256=EISu6jv_2E-iOrd4o6xeL9S-GVSYwxBgVZjYP9adf54,4637
 dr_import/clone_trip2.py,sha256=fA8DgsCy5zTTDC3tNjJeo2MtaOp4OG0EqF-0sUxEMyM,18989
 dr_import/import_gps.py,sha256=UYStSa5rNaQqYWLjEH2tilqmn-esqFCKfu1Sin6dFy0,7231
-dr_import/import_media.py,sha256=nEqTcbp9g8vswllSlCbhUT34AQmkaTpdWjK2MXQG1Po,10536
+dr_import/import_media.py,sha256=QVtikblIHoK6xNjeJC8Qg4Wx9wkuUbcMYNrLZ5oVr3E,10675
 dr_import/import_poll_gps.py,sha256=mk7hRMkQCgJWk4nz7noJMXRopKZBuay5VVwQL1giH08,5208
 dr_import/legacy_import.py,sha256=rMIUaMTRDu88AUTZmiPKFOA0va7ebRnOe0MymAcfAbE,7025
 dr_import/local_gaps.py,sha256=rcu4MmI-W24jnFMCYV6mTpbJaeKTwEfuFn-kaFkqdkQ,1924
 dr_import/make_management_report.py,sha256=y16LhSIcODSvdzROZeayUgpEuE5Cfqy6PR0JYjvEXKk,5373
 dr_import/make_trip.py,sha256=UQO0xZZ1RF1KXKFdzJN6uTCGLTEiw--okWAH_GY75uU,6204
 dr_import/nvr_import.py,sha256=sULItA29GzVPWRdEWJkX-FeFHbqe9j-siiE-AMDA2KY,7659
 dr_import/trim_trip.py,sha256=npjVDTelQFUU0oaRE86hvJZMRXJsuwgG5EqSbaGom0M,3130
 dr_import/trip_summary.png,sha256=3syHLe2mkdih3UK5iwAMxE2T5-NdAKspuoTP8uZl9dg,51441
 dr_import/update_media.py,sha256=gieap6APvvgJuQH9asSTcLs3WW1jykhkhh6Tyo06xZs,5122
-dr_import-0.2.8.dist-info/METADATA,sha256=BoCRHMROGaPuf0-ee0ClLjtoAyDjFEd4tv5h_ydKuiM,430
-dr_import-0.2.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-dr_import-0.2.8.dist-info/top_level.txt,sha256=LQ21Hy3KJ3iQ1Z3-DH-HQk93yklm20zDjY8giTxswJ0,10
-dr_import-0.2.8.dist-info/RECORD,,
+dr_import-0.2.9.dist-info/METADATA,sha256=UMcYAVLiH5VoPWVlE-4GNzN9GuvSPoG-cT8uVL1yULM,430
+dr_import-0.2.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+dr_import-0.2.9.dist-info/top_level.txt,sha256=LQ21Hy3KJ3iQ1Z3-DH-HQk93yklm20zDjY8giTxswJ0,10
+dr_import-0.2.9.dist-info/RECORD,,
```

