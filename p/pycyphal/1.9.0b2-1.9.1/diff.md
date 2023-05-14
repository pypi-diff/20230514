# Comparing `tmp/pycyphal-1.9.0b2.tar.gz` & `tmp/pycyphal-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyphal-1.9.0b2.tar", last modified: Thu Jul  7 18:59:31 2022, max compression
+gzip compressed data, was "pycyphal-1.9.1.tar", last modified: Fri Aug 19 13:33:04 2022, max compression
```

## Comparing `pycyphal-1.9.0b2.tar` & `pycyphal-1.9.1.tar`

### file list

```diff
@@ -1,178 +1,183 @@
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.365580 pycyphal-1.9.0b2/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1077 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3721 2022-07-07 18:59:31.365580 pycyphal-1.9.0b2/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2563 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/README.md
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.273579 pycyphal-1.9.0b2/pycyphal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       12 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/VERSION
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2295 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/__init__.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.281580 pycyphal-1.9.0b2/pycyphal/application/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13407 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14342 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_node.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9744 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_node_factory.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6696 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_port_list_publisher.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6111 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_register_server.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4586 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_registry_factory.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13162 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/_transport_factory.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8731 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/diagnostic.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19285 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/file.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9312 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/heartbeat_publisher.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12554 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/node_tracker.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22238 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/plug_and_play.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.281580 pycyphal-1.9.0b2/pycyphal/application/register/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1866 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14717 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/_registry.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15508 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/_value.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.285580 pycyphal-1.9.0b2/pycyphal/application/register/backend/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2658 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/backend/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6552 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/backend/dynamic.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8177 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/application/register/backend/static.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.285580 pycyphal-1.9.0b2/pycyphal/dsdl/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2103 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10792 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_builtin_form.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16249 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_compiler.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8011 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_composite_object.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.289579 pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1084 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_common.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28621 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_deserializer.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    23809 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_serializer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.289579 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      194 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/DelimitedType.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      810 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/Namespace.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      805 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/ServiceType.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      270 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/StructureType.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      194 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/UnionType.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17732 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/base.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7463 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/deserialization.j2
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9287 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/dsdl/_templates/serialization.j2
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.293580 pycyphal-1.9.0b2/pycyphal/presentation/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9230 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/__init__.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.293580 pycyphal-1.9.0b2/pycyphal/presentation/_port/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1403 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4918 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17756 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_client.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      980 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_error.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10117 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_publisher.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13754 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_server.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17273 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_port/_subscriber.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21040 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/_presentation.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.297580 pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      575 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6119 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/_common.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16391 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/monotonic_clustering.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9814 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/transfer_id.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.305580 pycyphal-1.9.0b2/pycyphal/transport/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12228 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1417 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_data_specifier.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1840 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_error.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1915 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_payload_metadata.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16490 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_session.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5287 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_timestamp.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7855 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_tracer.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2917 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_transfer.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13952 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/_transport.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.313580 pycyphal-1.9.0b2/pycyphal/transport/can/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2525 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20708 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_can.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_frame.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16597 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_identifier.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5244 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_input_dispatch_table.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.317580 pycyphal-1.9.0b2/pycyphal/transport/can/_session/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      839 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      887 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8977 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/_input.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10632 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/_output.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16524 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/_transfer_reassembler.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6213 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_session/_transfer_sender.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11753 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/_tracer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.317580 pycyphal-1.9.0b2/pycyphal/transport/can/media/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7500 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/_filter.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3235 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/_frame.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8227 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/_media.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.317580 pycyphal-1.9.0b2/pycyphal/transport/can/media/pythoncan/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      205 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/pythoncan/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24294 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/pythoncan/_pythoncan.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.321580 pycyphal-1.9.0b2/pycyphal/transport/can/media/socketcan/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      880 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/socketcan/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15843 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/can/media/socketcan/_socketcan.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.321580 pycyphal-1.9.0b2/pycyphal/transport/commons/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      688 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6770 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/_refragment.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.329580 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      571 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1452 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3640 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc16_ccitt.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5139 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc32c.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7312 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc64we.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.333580 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      930 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2585 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_alien_transfer_reassembler.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      230 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_common.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3740 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_frame.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30978 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_transfer_reassembler.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4537 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_transfer_serializer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.333580 pycyphal-1.9.0b2/pycyphal/transport/loopback/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      538 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/loopback/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3495 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/loopback/_input_session.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9514 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/loopback/_loopback.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4871 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/loopback/_output_session.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1151 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/loopback/_tracer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.337580 pycyphal-1.9.0b2/pycyphal/transport/redundant/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20333 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/__init__.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.345580 pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      331 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2525 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2671 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_cyclic.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2341 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_monotonic.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_error.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16612 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_redundant_transport.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.345580 pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      546 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3287 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12974 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_input.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17574 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_output.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6497 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/redundant/_tracer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.349580 pycyphal-1.9.0b2/pycyphal/transport/serial/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11744 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18976 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_frame.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21283 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_serial.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.349580 pycyphal-1.9.0b2/pycyphal/transport/serial/_session/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      460 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_session/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      830 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_base.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6098 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_input.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5694 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_output.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6886 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_stream_parser.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10785 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/serial/_tracer.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.353580 pycyphal-1.9.0b2/pycyphal/transport/udp/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19237 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8760 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_frame.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.357581 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1220 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9514 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_endpoint_mapping.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    23878 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_link_layer.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5559 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_socket_factory.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8168 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_v4.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.361580 pycyphal-1.9.0b2/pycyphal/transport/udp/_session/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      726 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_session/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13522 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_session/_input.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9216 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_session/_output.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13354 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_socket_reader.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13037 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_tracer.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19422 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/transport/udp/_udp.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.365580 pycyphal-1.9.0b2/pycyphal/util/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/util/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1711 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/util/_broadcast.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3494 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/util/_introspect.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      927 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/util/_mark_last.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2037 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pycyphal/util/_repr.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-07-07 18:59:31.273579 pycyphal-1.9.0b2/pycyphal.egg-info/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3721 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5963 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/SOURCES.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/dependency_links.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/not-zip-safe
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/requires.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        9 2022-07-07 18:59:31.000000 pycyphal-1.9.0b2/pycyphal.egg-info/top_level.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      130 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/pyproject.toml
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4192 2022-07-07 18:59:31.373581 pycyphal-1.9.0b2/setup.cfg
--rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      211 2022-07-07 18:58:54.000000 pycyphal-1.9.0b2/setup.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.875632 pycyphal-1.9.1/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1077 2022-08-19 13:32:47.000000 pycyphal-1.9.1/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3719 2022-08-19 13:33:04.875632 pycyphal-1.9.1/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2563 2022-08-19 13:32:47.000000 pycyphal-1.9.1/README.md
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.839633 pycyphal-1.9.1/pycyphal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2218 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/__init__.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.839633 pycyphal-1.9.1/pycyphal/__pycache__/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      167 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       22 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/_version.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.843633 pycyphal-1.9.1/pycyphal/application/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13407 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14342 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_node.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9744 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_node_factory.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6696 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_port_list_publisher.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6111 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_register_server.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4586 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_registry_factory.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13752 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/_transport_factory.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8731 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/diagnostic.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19285 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/file.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9312 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/heartbeat_publisher.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12554 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/node_tracker.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22238 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/plug_and_play.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.843633 pycyphal-1.9.1/pycyphal/application/register/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1866 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14717 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/_registry.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15508 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/_value.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.843633 pycyphal-1.9.1/pycyphal/application/register/backend/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2658 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/backend/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6552 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/backend/dynamic.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8177 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/application/register/backend/static.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.847633 pycyphal-1.9.1/pycyphal/dsdl/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2103 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10792 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_builtin_form.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16249 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_compiler.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8011 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_composite_object.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.847633 pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1084 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_common.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28621 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_deserializer.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    23809 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_serializer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.851632 pycyphal-1.9.1/pycyphal/dsdl/_templates/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      194 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/DelimitedType.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      810 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/Namespace.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      805 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/ServiceType.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      270 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/StructureType.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      194 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/UnionType.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17732 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/base.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7463 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/deserialization.j2
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9287 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/dsdl/_templates/serialization.j2
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.851632 pycyphal-1.9.1/pycyphal/presentation/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9230 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/__init__.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.851632 pycyphal-1.9.1/pycyphal/presentation/_port/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1403 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4918 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17756 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_client.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      980 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_error.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10117 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_publisher.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13754 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_server.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17273 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_port/_subscriber.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21040 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/_presentation.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.855632 pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      575 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6119 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/_common.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16442 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/monotonic_clustering.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9814 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/transfer_id.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.855632 pycyphal-1.9.1/pycyphal/transport/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12228 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1417 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_data_specifier.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1840 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_error.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1915 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_payload_metadata.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16490 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_session.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5287 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_timestamp.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7855 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_tracer.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2917 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_transfer.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13952 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/_transport.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.859632 pycyphal-1.9.1/pycyphal/transport/can/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2525 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20708 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_can.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_frame.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16597 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_identifier.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5244 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_input_dispatch_table.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.859632 pycyphal-1.9.1/pycyphal/transport/can/_session/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      839 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      887 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8977 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/_input.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10632 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/_output.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16524 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/_transfer_reassembler.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6213 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_session/_transfer_sender.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11753 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/_tracer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.859632 pycyphal-1.9.1/pycyphal/transport/can/media/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7500 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/_filter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3235 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/_frame.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8227 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/_media.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.859632 pycyphal-1.9.1/pycyphal/transport/can/media/candump/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      199 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/candump/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12743 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/candump/_candump.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.859632 pycyphal-1.9.1/pycyphal/transport/can/media/pythoncan/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      205 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/pythoncan/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24311 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/pythoncan/_pythoncan.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.863632 pycyphal-1.9.1/pycyphal/transport/can/media/socketcan/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      880 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/socketcan/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15837 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/can/media/socketcan/_socketcan.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.863632 pycyphal-1.9.1/pycyphal/transport/commons/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      688 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6770 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/_refragment.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.863632 pycyphal-1.9.1/pycyphal/transport/commons/crc/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      571 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/crc/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1452 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/crc/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3640 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc16_ccitt.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5139 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc32c.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7312 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc64we.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.867632 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      930 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2585 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_alien_transfer_reassembler.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      230 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_common.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3740 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_frame.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30978 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_transfer_reassembler.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4537 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_transfer_serializer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.867632 pycyphal-1.9.1/pycyphal/transport/loopback/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      538 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/loopback/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3495 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/loopback/_input_session.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9514 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/loopback/_loopback.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4871 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/loopback/_output_session.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1151 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/loopback/_tracer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.867632 pycyphal-1.9.1/pycyphal/transport/redundant/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20333 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/__init__.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.867632 pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      331 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2525 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2671 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_cyclic.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2341 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_monotonic.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_error.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16612 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_redundant_transport.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.871632 pycyphal-1.9.1/pycyphal/transport/redundant/_session/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      546 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_session/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3287 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_session/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12974 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_session/_input.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17574 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_session/_output.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6497 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/redundant/_tracer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.871632 pycyphal-1.9.1/pycyphal/transport/serial/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11744 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18976 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_frame.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21283 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_serial.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.871632 pycyphal-1.9.1/pycyphal/transport/serial/_session/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      460 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_session/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      830 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_session/_base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6098 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_session/_input.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5694 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_session/_output.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6886 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_stream_parser.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10785 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/serial/_tracer.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.875632 pycyphal-1.9.1/pycyphal/transport/udp/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19237 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8760 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_frame.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.875632 pycyphal-1.9.1/pycyphal/transport/udp/_ip/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1220 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_ip/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9514 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_ip/_endpoint_mapping.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    23878 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_ip/_link_layer.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5559 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_ip/_socket_factory.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8168 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_ip/_v4.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.875632 pycyphal-1.9.1/pycyphal/transport/udp/_session/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      726 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_session/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13522 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_session/_input.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9216 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_session/_output.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13354 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_socket_reader.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13037 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_tracer.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19422 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/transport/udp/_udp.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.875632 pycyphal-1.9.1/pycyphal/util/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/util/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1711 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/util/_broadcast.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3494 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/util/_introspect.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      927 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/util/_mark_last.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2037 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pycyphal/util/_repr.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2022-08-19 13:33:04.839633 pycyphal-1.9.1/pycyphal.egg-info/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3719 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6111 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/SOURCES.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/dependency_links.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/not-zip-safe
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/requires.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        9 2022-08-19 13:33:04.000000 pycyphal-1.9.1/pycyphal.egg-info/top_level.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      130 2022-08-19 13:32:47.000000 pycyphal-1.9.1/pyproject.toml
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4205 2022-08-19 13:33:04.879632 pycyphal-1.9.1/setup.cfg
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      211 2022-08-19 13:32:47.000000 pycyphal-1.9.1/setup.py
```

### Comparing `pycyphal-1.9.0b2/LICENSE` & `pycyphal-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/PKG-INFO` & `pycyphal-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyphal
-Version: 1.9.0b2
+Version: 1.9.1
 Summary: A full-featured implementation of the Cyphal protocol stack in Python.
 Home-page: https://opencyphal.org
 Author: OpenCyphal
 Author-email: consortium@opencyphal.org
 License: MIT
 Keywords: cyphal,opencyphal,uavcan,pub-sub,publish-subscribe,data-bus,can-bus,ethernet,vehicular,onboard-networking,avionics,communication-protocol,broker
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycyphal Version: 1.9.0b2 Summary: A full-featured
+Metadata-Version: 2.1 Name: pycyphal Version: 1.9.1 Summary: A full-featured
 implementation of the Cyphal protocol stack in Python. Home-page: https://
 opencyphal.org Author: OpenCyphal Author-email: consortium@opencyphal.org
 License: MIT Keywords: cyphal,opencyphal,uavcan,pub-sub,publish-subscribe,data-
 bus,can-bus,ethernet,vehicular,onboard-networking,avionics,communication-
 protocol,broker Classifier: Intended Audience :: Developers Classifier: Topic
 :: Scientific/Engineering Classifier: Topic :: Software Development :: Embedded
 Systems Classifier: Topic :: Software Development :: Libraries :: Python
```

### Comparing `pycyphal-1.9.0b2/README.md` & `pycyphal-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/__init__.py` & `pycyphal-1.9.1/pycyphal/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 - ``ERROR``
 - ``WARNING``
 - ``INFO``
 - ``DEBUG``
 """
 
 import os as _os
-from importlib.resources import read_text as _read_text
 
 
-__version__ = _read_text(__name__, "VERSION", encoding="utf8").strip()
+from ._version import __version__ as __version__
+
 __version_info__ = tuple(map(int, __version__.split(".")[:3]))
 __author__ = "OpenCyphal"
 __copyright__ = "Copyright (c) 2019 OpenCyphal"
 __email__ = "consortium@opencyphal.org"
 __license__ = "MIT"
```

### Comparing `pycyphal-1.9.0b2/pycyphal/application/__init__.py` & `pycyphal-1.9.1/pycyphal/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_node.py` & `pycyphal-1.9.1/pycyphal/application/_node.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_node_factory.py` & `pycyphal-1.9.1/pycyphal/application/_node_factory.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_port_list_publisher.py` & `pycyphal-1.9.1/pycyphal/application/_port_list_publisher.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_register_server.py` & `pycyphal-1.9.1/pycyphal/application/_register_server.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_registry_factory.py` & `pycyphal-1.9.1/pycyphal/application/_registry_factory.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/_transport_factory.py` & `pycyphal-1.9.1/pycyphal/application/_transport_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,21 @@
         * - Register name
           - Register type
           - Register semantics
 
         * - ``uavcan.can.iface``
           - ``string``
           - Whitespace-separated list of CAN iface names.
-            Each iface name shall follow the format defined in :class:`pycyphal.transport.can.media.pythoncan`.
+            Each iface name shall follow the format defined in :mod:`pycyphal.transport.can.media.pythoncan`.
             E.g.: ``socketcan:vcan0``.
+            On GNU/Linux, the ``socketcan:`` prefix selects :mod:`pycyphal.transport.can.media.socketcan`
+            instead of PythonCAN.
+            All platforms support the ``candump:`` prefix, which selects :mod:`pycyphal.transport.can.media.candump`;
+            the text after colon is the path of the log file;
+            e.g., ``candump:/home/pavel/candump-2022-07-14_150815.log``.
 
         * - ``uavcan.can.mtu``
           - ``natural16[1]``
           - The MTU value to use with all constructed CAN transports.
             Values other than 8 and 64 should not be used.
 
         * - ``uavcan.can.bitrate``
@@ -283,15 +288,19 @@
         from pycyphal.transport.can import CANTransport
 
         for iface in iface_list:
             media: pycyphal.transport.can.media.Media
             if iface.lower().startswith("socketcan:"):
                 from pycyphal.transport.can.media.socketcan import SocketCANMedia
 
-                media = SocketCANMedia(iface.split(":")[-1], mtu=mtu)
+                media = SocketCANMedia(iface.split(":", 1)[-1], mtu=mtu)
+            elif iface.lower().startswith("candump:"):
+                from pycyphal.transport.can.media.candump import CandumpMedia
+
+                media = CandumpMedia(iface.split(":", 1)[-1])
             else:
                 from pycyphal.transport.can.media.pythoncan import PythonCANMedia
 
                 media = PythonCANMedia(iface, br_arb if br_arb == br_data else (br_arb, br_data), mtu)
             yield CANTransport(media, node_id)
```

### Comparing `pycyphal-1.9.0b2/pycyphal/application/diagnostic.py` & `pycyphal-1.9.1/pycyphal/application/diagnostic.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/file.py` & `pycyphal-1.9.1/pycyphal/application/file.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/heartbeat_publisher.py` & `pycyphal-1.9.1/pycyphal/application/heartbeat_publisher.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/node_tracker.py` & `pycyphal-1.9.1/pycyphal/application/node_tracker.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/plug_and_play.py` & `pycyphal-1.9.1/pycyphal/application/plug_and_play.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/__init__.py` & `pycyphal-1.9.1/pycyphal/application/register/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/_registry.py` & `pycyphal-1.9.1/pycyphal/application/register/_registry.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/_value.py` & `pycyphal-1.9.1/pycyphal/application/register/_value.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/backend/__init__.py` & `pycyphal-1.9.1/pycyphal/application/register/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/backend/dynamic.py` & `pycyphal-1.9.1/pycyphal/application/register/backend/dynamic.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/application/register/backend/static.py` & `pycyphal-1.9.1/pycyphal/application/register/backend/static.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/__init__.py` & `pycyphal-1.9.1/pycyphal/dsdl/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_builtin_form.py` & `pycyphal-1.9.1/pycyphal/dsdl/_builtin_form.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_compiler.py` & `pycyphal-1.9.1/pycyphal/dsdl/_compiler.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_composite_object.py` & `pycyphal-1.9.1/pycyphal/dsdl/_composite_object.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/__init__.py` & `pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_common.py` & `pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_common.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_deserializer.py` & `pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_deserializer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_serialized_representation/_serializer.py` & `pycyphal-1.9.1/pycyphal/dsdl/_serialized_representation/_serializer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_templates/Namespace.j2` & `pycyphal-1.9.1/pycyphal/dsdl/_templates/Namespace.j2`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_templates/ServiceType.j2` & `pycyphal-1.9.1/pycyphal/dsdl/_templates/ServiceType.j2`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_templates/base.j2` & `pycyphal-1.9.1/pycyphal/dsdl/_templates/base.j2`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_templates/deserialization.j2` & `pycyphal-1.9.1/pycyphal/dsdl/_templates/deserialization.j2`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/dsdl/_templates/serialization.j2` & `pycyphal-1.9.1/pycyphal/dsdl/_templates/serialization.j2`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/__init__.py` & `pycyphal-1.9.1/pycyphal/presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/__init__.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_base.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_client.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_client.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_error.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_error.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_publisher.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_publisher.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_server.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_server.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_port/_subscriber.py` & `pycyphal-1.9.1/pycyphal/presentation/_port/_subscriber.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/_presentation.py` & `pycyphal-1.9.1/pycyphal/presentation/_presentation.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/__init__.py` & `pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/_common.py` & `pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/_common.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/monotonic_clustering.py` & `pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/monotonic_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) 2022 OpenCyphal
 # This software is distributed under the terms of the MIT License.
 # Author: Pavel Kirienko <pavel@opencyphal.org>
 
+# mypy: warn_unused_ignores=False
+
 from __future__ import annotations
 import bisect
 import asyncio
 import logging
 import functools
 import typing
 from typing import Iterable, Any, Callable
@@ -269,15 +271,15 @@
         self._clusters: list[_Cluster[T]] = []
         self._depth = int(depth)
         self._seq_counter = 0
 
     def update(self, key: float, tolerance: float, index: int, item: T) -> tuple[T, ...] | None:
         clust: _Cluster[T] | None = None
         # noinspection PyTypeChecker
-        ni = bisect.bisect_left(self._clusters, key)
+        ni = bisect.bisect_left(self._clusters, key)  # type: ignore
         assert 0 <= ni <= len(self._clusters)
         neigh: list[tuple[float, int]] = []
         if 0 < ni:
             neigh.append((self._clusters[ni - 1].delta(key), ni - 1))
         if ni < len(self._clusters):
             neigh.append((self._clusters[ni].delta(key), ni))
         if ni < (len(self._clusters) - 1):
```

### Comparing `pycyphal-1.9.0b2/pycyphal/presentation/subscription_synchronizer/transfer_id.py` & `pycyphal-1.9.1/pycyphal/presentation/subscription_synchronizer/transfer_id.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_data_specifier.py` & `pycyphal-1.9.1/pycyphal/transport/_data_specifier.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_error.py` & `pycyphal-1.9.1/pycyphal/transport/_error.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_payload_metadata.py` & `pycyphal-1.9.1/pycyphal/transport/_payload_metadata.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_session.py` & `pycyphal-1.9.1/pycyphal/transport/_session.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_timestamp.py` & `pycyphal-1.9.1/pycyphal/transport/_timestamp.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_transfer.py` & `pycyphal-1.9.1/pycyphal/transport/_transfer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/_transport.py` & `pycyphal-1.9.1/pycyphal/transport/_transport.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/can/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_can.py` & `pycyphal-1.9.1/pycyphal/transport/can/_can.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_frame.py` & `pycyphal-1.9.1/pycyphal/transport/can/_frame.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_identifier.py` & `pycyphal-1.9.1/pycyphal/transport/can/_identifier.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_input_dispatch_table.py` & `pycyphal-1.9.1/pycyphal/transport/can/_input_dispatch_table.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/_base.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/_input.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/_input.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/_output.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/_output.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/_transfer_reassembler.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/_transfer_reassembler.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_session/_transfer_sender.py` & `pycyphal-1.9.1/pycyphal/transport/can/_session/_transfer_sender.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/can/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/_filter.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/_filter.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/_frame.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/_frame.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/_media.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/_media.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/pythoncan/_pythoncan.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/pythoncan/_pythoncan.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,27 +528,27 @@
 
 
 def _construct_gs_usb(parameters: _InterfaceParameters) -> can.ThreadSafeBus:
     if isinstance(parameters, _ClassicInterfaceParameters):
         try:
             index = int(parameters.channel_name)
         except ValueError:
-            raise InvalidMediaConfigurationError("Channel name must be an integer interface index")
+            raise InvalidMediaConfigurationError("Channel name must be an integer interface index") from None
 
         try:
             bus = can.ThreadSafeBus(
                 interface=parameters.interface_name,
                 channel=parameters.channel_name,
                 index=index,
                 bitrate=parameters.bitrate,
             )
         except TypeError as e:
             raise InvalidMediaConfigurationError(
                 f"Interface error: {e}.\nNote: gs_usb currently requires unreleased python-can version from git."
-            )
+            ) from e
 
         return (PythonCANBusOptions(hardware_loopback=True, hardware_timestamp=True), bus)
     if isinstance(parameters, _FDInterfaceParameters):
         raise InvalidMediaConfigurationError(f"Interface does not support CAN FD: {parameters.interface_name}")
     assert False, "Internal error"
```

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/socketcan/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/socketcan/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/can/media/socketcan/_socketcan.py` & `pycyphal-1.9.1/pycyphal/transport/can/media/socketcan/_socketcan.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         self._sock = _make_socket(iface_name, can_fd=self._is_fd, native_frame_size=self._native_frame_size)
         self._ctl_main, self._ctl_worker = socket.socketpair()  # This is used for controlling the worker thread.
         self._closed = False
         self._maybe_thread: typing.Optional[threading.Thread] = None
         self._loopback_enabled = False
 
-        self._ancillary_data_buffer_size = socket.CMSG_SPACE(_TIMEVAL_STRUCT.size)  # Used for recvmsg()
+        self._ancillary_data_buffer_size = socket.CMSG_SPACE(_TIMEVAL_STRUCT.size)  # type: ignore
 
         super().__init__()
 
     @property
     def interface_name(self) -> str:
         return self._iface_name
```

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/_refragment.py` & `pycyphal-1.9.1/pycyphal/transport/commons/_refragment.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/crc/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/commons/crc/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_base.py` & `pycyphal-1.9.1/pycyphal/transport/commons/crc/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc16_ccitt.py` & `pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc32c.py` & `pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc32c.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/crc/_crc64we.py` & `pycyphal-1.9.1/pycyphal/transport/commons/crc/_crc64we.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_alien_transfer_reassembler.py` & `pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_alien_transfer_reassembler.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_frame.py` & `pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_frame.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_transfer_reassembler.py` & `pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_transfer_reassembler.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/commons/high_overhead_transport/_transfer_serializer.py` & `pycyphal-1.9.1/pycyphal/transport/commons/high_overhead_transport/_transfer_serializer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/loopback/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/loopback/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/loopback/_input_session.py` & `pycyphal-1.9.1/pycyphal/transport/loopback/_input_session.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/loopback/_loopback.py` & `pycyphal-1.9.1/pycyphal/transport/loopback/_loopback.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/loopback/_output_session.py` & `pycyphal-1.9.1/pycyphal/transport/loopback/_output_session.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/loopback/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/loopback/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_base.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_cyclic.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_cyclic.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_deduplicator/_monotonic.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_deduplicator/_monotonic.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_redundant_transport.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_redundant_transport.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_session/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_base.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_session/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_input.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_session/_input.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_session/_output.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_session/_output.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/redundant/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/redundant/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_frame.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_frame.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_serial.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_serial.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_base.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_session/_base.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_input.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_session/_input.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_session/_output.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_session/_output.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_stream_parser.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_stream_parser.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/serial/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/serial/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_frame.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_frame.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_ip/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_endpoint_mapping.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_ip/_endpoint_mapping.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_link_layer.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_ip/_link_layer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_socket_factory.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_ip/_socket_factory.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_ip/_v4.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_ip/_v4.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_session/__init__.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_session/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_session/_input.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_session/_input.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_session/_output.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_session/_output.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_socket_reader.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_socket_reader.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_tracer.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_tracer.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/transport/udp/_udp.py` & `pycyphal-1.9.1/pycyphal/transport/udp/_udp.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/util/__init__.py` & `pycyphal-1.9.1/pycyphal/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/util/_broadcast.py` & `pycyphal-1.9.1/pycyphal/util/_broadcast.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/util/_introspect.py` & `pycyphal-1.9.1/pycyphal/util/_introspect.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/util/_mark_last.py` & `pycyphal-1.9.1/pycyphal/util/_mark_last.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal/util/_repr.py` & `pycyphal-1.9.1/pycyphal/util/_repr.py`

 * *Files identical despite different names*

### Comparing `pycyphal-1.9.0b2/pycyphal.egg-info/PKG-INFO` & `pycyphal-1.9.1/pycyphal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyphal
-Version: 1.9.0b2
+Version: 1.9.1
 Summary: A full-featured implementation of the Cyphal protocol stack in Python.
 Home-page: https://opencyphal.org
 Author: OpenCyphal
 Author-email: consortium@opencyphal.org
 License: MIT
 Keywords: cyphal,opencyphal,uavcan,pub-sub,publish-subscribe,data-bus,can-bus,ethernet,vehicular,onboard-networking,avionics,communication-protocol,broker
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycyphal Version: 1.9.0b2 Summary: A full-featured
+Metadata-Version: 2.1 Name: pycyphal Version: 1.9.1 Summary: A full-featured
 implementation of the Cyphal protocol stack in Python. Home-page: https://
 opencyphal.org Author: OpenCyphal Author-email: consortium@opencyphal.org
 License: MIT Keywords: cyphal,opencyphal,uavcan,pub-sub,publish-subscribe,data-
 bus,can-bus,ethernet,vehicular,onboard-networking,avionics,communication-
 protocol,broker Classifier: Intended Audience :: Developers Classifier: Topic
 :: Scientific/Engineering Classifier: Topic :: Software Development :: Embedded
 Systems Classifier: Topic :: Software Development :: Libraries :: Python
```

### Comparing `pycyphal-1.9.0b2/pycyphal.egg-info/SOURCES.txt` & `pycyphal-1.9.1/pycyphal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-pycyphal/VERSION
 pycyphal/__init__.py
+pycyphal/_version.py
 pycyphal.egg-info/PKG-INFO
 pycyphal.egg-info/SOURCES.txt
 pycyphal.egg-info/dependency_links.txt
 pycyphal.egg-info/not-zip-safe
 pycyphal.egg-info/requires.txt
 pycyphal.egg-info/top_level.txt
+pycyphal/__pycache__/_version.cpython-310.pyc
 pycyphal/application/__init__.py
 pycyphal/application/_node.py
 pycyphal/application/_node_factory.py
 pycyphal/application/_port_list_publisher.py
 pycyphal/application/_register_server.py
 pycyphal/application/_registry_factory.py
 pycyphal/application/_transport_factory.py
@@ -79,14 +80,16 @@
 pycyphal/transport/can/_session/_output.py
 pycyphal/transport/can/_session/_transfer_reassembler.py
 pycyphal/transport/can/_session/_transfer_sender.py
 pycyphal/transport/can/media/__init__.py
 pycyphal/transport/can/media/_filter.py
 pycyphal/transport/can/media/_frame.py
 pycyphal/transport/can/media/_media.py
+pycyphal/transport/can/media/candump/__init__.py
+pycyphal/transport/can/media/candump/_candump.py
 pycyphal/transport/can/media/pythoncan/__init__.py
 pycyphal/transport/can/media/pythoncan/_pythoncan.py
 pycyphal/transport/can/media/socketcan/__init__.py
 pycyphal/transport/can/media/socketcan/_socketcan.py
 pycyphal/transport/commons/__init__.py
 pycyphal/transport/commons/_refragment.py
 pycyphal/transport/commons/crc/__init__.py
```

### Comparing `pycyphal-1.9.0b2/setup.cfg` & `pycyphal-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pycyphal
-version = file: pycyphal/VERSION
+version = attr: pycyphal._version.__version__
 author = OpenCyphal
 author_email = consortium@opencyphal.org
 url = https://opencyphal.org
 description = A full-featured implementation of the Cyphal protocol stack in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

