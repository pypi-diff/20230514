# Comparing `tmp/pypcapkit-1.0.0rc1.tar.gz` & `tmp/pypcapkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypcapkit-1.0.0rc1.tar", last modified: Thu May  4 06:22:14 2023, max compression
+gzip compressed data, was "pypcapkit-1.0.1.tar", last modified: Sun May 14 15:40:28 2023, max compression
```

## Comparing `pypcapkit-1.0.0rc1.tar` & `pypcapkit-1.0.1.tar`

### file list

```diff
@@ -1,527 +1,527 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/return_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.475485 pypcapkit-1.0.0rc1/pcapkit/const/hip/
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/di.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_low_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/eddsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/esp_transform_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/hi_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/hit_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/nat_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/notify_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/registration_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.479485 pypcapkit-1.0.0rc1/pcapkit/const/http/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.479485 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/classification_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/protection_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_rel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_thr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/ts_flag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/extension_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/seed_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/smf_dpd_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/tagger_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/ipx/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.491485 pypcapkit-1.0.0rc1/pcapkit/const/mh/
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/ack_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/ani_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/auth_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_update_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dhcp_support_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dns_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmip6_tls_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmipv6_home_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/enumerating_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_indication_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handoff_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/home_address_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/lma_mag_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_group_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_id_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/operator_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/qos_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/traffic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/upa_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/upn_reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.491485 pypcapkit-1.0.0rc1/pcapkit/const/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/block_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/filter_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/hash_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/option_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/record_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/secrets_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/verdict_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/reg/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25954 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/ethertype.py
--rw-r--r--   0 runner    (1001) docker     (123)    37247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/linktype.py
--rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/transtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/mp_tcp_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/vlan/priority_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/corekit/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/infoclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/multidict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/protochain.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/dumpkit/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/pcap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/foundation/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/dpkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pyshark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/scapy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27578 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/reassembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/traceflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/protocols/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dhcpv6.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/imap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/nntp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/onc_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/rip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/rtp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/sip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/smtp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/telnet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    49557 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)    28229 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.519486 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.519486 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/esp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/icmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/icmpv6.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/igmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/shim6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    76152 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/internet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipsec.py
--rw-r--r--   0 runner    (1001) docker     (123)    70654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    76974 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29634 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/eapol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/fddi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/isdn.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/ndp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/ppp.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/rarp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)   237556 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    43495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)    42392 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    62017 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/dccp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/rsvp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/sctp.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113821 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/dpkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pyshark.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/scapy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.543485 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/return_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.547485 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/di.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_low_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/eddsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/esp_transform_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hi_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hit_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/nat_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/notify_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.547485 pypcapkit-1.0.0rc1/pcapkit/vendor/http/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/classification_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/protection_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_rel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_thr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/ts_flag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/extension_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/seed_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/smf_dpd_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/tagger_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.559486 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ack_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ani_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/auth_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_update_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dhcp_support_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dns_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmip6_tls_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmipv6_home_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/enumerating_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_indication_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handoff_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/home_address_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/lma_mag_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_group_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_id_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/operator_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/qos_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/traffic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upa_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upn_reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/block_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/filter_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/hash_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/option_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/record_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/secrets_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/verdict_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/ethertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/linktype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/transtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/mp_tcp_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/priority_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/pypcapkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16319 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/util/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.569771 pypcapkit-1.0.1/pcapkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.573771 pypcapkit-1.0.1/pcapkit/const/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.573771 pypcapkit-1.0.1/pcapkit/const/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/arp/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/arp/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.573771 pypcapkit-1.0.1/pcapkit/const/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ftp/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ftp/return_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.573771 pypcapkit-1.0.1/pcapkit/const/hip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/ecdsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/ecdsa_low_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/eddsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/esp_transform_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/hi_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/hit_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/nat_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/notify_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/registration_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/hip/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.573771 pypcapkit-1.0.1/pcapkit/const/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/http/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.577771 pypcapkit-1.0.1/pcapkit/const/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/classification_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/option_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/option_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/protection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/tos_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/tos_ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/tos_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/tos_rel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/tos_thr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv4/ts_flag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.577771 pypcapkit-1.0.1/pcapkit/const/ipv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/extension_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/option_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/seed_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipv6/tagger_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.577771 pypcapkit-1.0.1/pcapkit/const/ipx/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipx/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ipx/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.577771 pypcapkit-1.0.1/pcapkit/const/l2tp/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/l2tp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/l2tp/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.581771 pypcapkit-1.0.1/pcapkit/const/mh/
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/ack_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/ani_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/auth_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/binding_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/binding_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/binding_update_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/dhcp_support_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/dns_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/dsmipv6_home_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/enumerating_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/fb_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/fb_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/fb_indication_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/fb_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/flow_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/flow_id_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/handoff_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/handover_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/handover_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/handover_initiate_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/handover_initiate_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/home_address_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/lma_mag_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/mn_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/mn_id_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/operator_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/qos_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/revocation_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/revocation_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/traffic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/upa_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/mh/upn_reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.581771 pypcapkit-1.0.1/pcapkit/const/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ospf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ospf/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/ospf/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/const/pcapng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/block_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/hash_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/secrets_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/pcapng/verdict_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/const/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/reg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25954 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/reg/ethertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37247 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/reg/linktype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/reg/transtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/const/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/tcp/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/tcp/mp_tcp_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/tcp/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/const/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/const/vlan/priority_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/corekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/corekit/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/fields/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/infoclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/protochain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/corekit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/dumpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/dumpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/dumpkit/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/dumpkit/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/dumpkit/pcap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.585771 pypcapkit-1.0.1/pcapkit/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/foundation/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/dpkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/engines/scapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27578 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/foundation/reassembly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/reassembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/reassembly/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/foundation/traceflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/traceflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/foundation/traceflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/traceflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/traceflow/data/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/traceflow/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/foundation/traceflow/traceflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/interface/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/interface/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.589771 pypcapkit-1.0.1/pcapkit/protocols/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.593771 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/dhcpv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/imap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/nntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/onc_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/rip.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/rtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/sip.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/smtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/NotImplemented/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49557 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/application/httpv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.593771 pypcapkit-1.0.1/pcapkit/protocols/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.593771 pypcapkit-1.0.1/pcapkit/protocols/data/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/application/httpv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.593771 pypcapkit-1.0.1/pcapkit/protocols/data/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.593771 pypcapkit-1.0.1/pcapkit/protocols/data/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.597771 pypcapkit-1.0.1/pcapkit/protocols/data/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.597771 pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27252 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.597771 pypcapkit-1.0.1/pcapkit/protocols/data/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/data/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.597771 pypcapkit-1.0.1/pcapkit/protocols/internet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.597771 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/esp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/icmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/icmpv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/igmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/shim6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/internet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70654 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76974 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29634 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/eapol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/fddi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/isdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/ndp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/NotImplemented/ppp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/rarp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237556 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43495 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.601771 pypcapkit-1.0.1/pcapkit/protocols/schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/application/httpv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43176 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/schema/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62857 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21072 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/schema/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/schema/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/transport/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/protocols/transport/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/NotImplemented/dccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/NotImplemented/rsvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/NotImplemented/sctp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113821 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/protocols/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.605771 pypcapkit-1.0.1/pcapkit/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/dpkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/toolkit/scapy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.609771 pypcapkit-1.0.1/pcapkit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.609771 pypcapkit-1.0.1/pcapkit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.609771 pypcapkit-1.0.1/pcapkit/vendor/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/arp/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/arp/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.609771 pypcapkit-1.0.1/pcapkit/vendor/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ftp/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ftp/return_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.609771 pypcapkit-1.0.1/pcapkit/vendor/hip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/ecdsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/ecdsa_low_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/eddsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/esp_transform_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/hi_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/hit_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/nat_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/notify_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/registration_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/hip/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.613771 pypcapkit-1.0.1/pcapkit/vendor/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/http/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.613771 pypcapkit-1.0.1/pcapkit/vendor/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/classification_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/option_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/option_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/protection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_rel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_thr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv4/ts_flag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.613771 pypcapkit-1.0.1/pcapkit/vendor/ipv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/extension_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/option_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/seed_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipv6/tagger_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.613771 pypcapkit-1.0.1/pcapkit/vendor/ipx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipx/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ipx/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.613771 pypcapkit-1.0.1/pcapkit/vendor/l2tp/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/l2tp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/l2tp/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.617771 pypcapkit-1.0.1/pcapkit/vendor/mh/
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/ack_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/ani_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/auth_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/binding_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/binding_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/binding_update_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/dhcp_support_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/dns_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/dsmipv6_home_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/enumerating_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/fb_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/fb_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/fb_indication_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/fb_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/flow_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/flow_id_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/handoff_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/handover_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/handover_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/handover_initiate_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/handover_initiate_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/home_address_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/lma_mag_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/mn_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/mn_id_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/operator_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/qos_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/revocation_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/revocation_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/traffic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/upa_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/mh/upn_reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pcapkit/vendor/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ospf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ospf/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/ospf/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pcapkit/vendor/pcapng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/block_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/hash_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/secrets_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/pcapng/verdict_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pcapkit/vendor/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/reg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/reg/ethertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/reg/linktype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/reg/transtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pcapkit/vendor/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/tcp/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/tcp/mp_tcp_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/tcp/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pcapkit/vendor/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pcapkit/vendor/vlan/priority_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/pypcapkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16319 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 15:40:28.000000 pypcapkit-1.0.1/pypcapkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:40:28.621771 pypcapkit-1.0.1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-14 15:40:16.000000 pypcapkit-1.0.1/util/bump_version.py
```

### Comparing `pypcapkit-1.0.0rc1/LICENSE` & `pypcapkit-1.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2022, Jarry Shaw
+Copyright (c) 2018-2023, Jarry Shaw
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pypcapkit-1.0.0rc1/PKG-INFO` & `pypcapkit-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypcapkit
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: PyPCAPKit: comprehensive network packet analysis library
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: documentation, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: repository, https://github.com/JarryShaw/PyPCAPKit
@@ -156,18 +156,18 @@
 
 Test Results
 ~~~~~~~~~~~~
 
 ============= ===========================
 Engine        Performance (ms per packet)
 ============= ===========================
-``dpkt``      0.048088_922256
-``scapy``     0.127444_444444
-``pcapkit``   0.964180_847514
-``pyshark``   23.665003_003003
+``dpkt``       0.010694_027361
+``scapy``      0.093399_399399
+``pcapkit``    0.199796_296296
+``pyshark``   25.066692_025359
 ============= ===========================
 
 ------------
 Installation
 ------------
 
 .. note::
```

### Comparing `pypcapkit-1.0.0rc1/README.rst` & `pypcapkit-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,18 @@
 
 Test Results
 ~~~~~~~~~~~~
 
 ============= ===========================
 Engine        Performance (ms per packet)
 ============= ===========================
-``dpkt``      0.048088_922256
-``scapy``     0.127444_444444
-``pcapkit``   0.964180_847514
-``pyshark``   23.665003_003003
+``dpkt``       0.010694_027361
+``scapy``      0.093399_399399
+``pcapkit``    0.199796_296296
+``pyshark``   25.066692_025359
 ============= ===========================
 
 ------------
 Installation
 ------------
 
 .. note::
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/__init__.py` & `pypcapkit-1.0.1/pcapkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,8 +109,8 @@
     'TCP', 'UDP',                                           # Transport Layer
 
     'FTP', 'FTP_DATA',                                      # Application Layer
     'HTTP',
 ]
 
 #: version number
-__version__ = '1.0.0rc1'
+__version__ = '1.0.1'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/__main__.py` & `pypcapkit-1.0.1/pcapkit/__main__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/all.py` & `pypcapkit-1.0.1/pcapkit/all.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/arp/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/arp/hardware.py` & `pypcapkit-1.0.1/pcapkit/const/arp/hardware.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/arp/operation.py` & `pypcapkit-1.0.1/pcapkit/const/arp/operation.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ftp/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ftp/command.py` & `pypcapkit-1.0.1/pcapkit/const/ftp/command.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ftp/return_code.py` & `pypcapkit-1.0.1/pcapkit/const/ftp/return_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/hip/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/certificate.py` & `pypcapkit-1.0.1/pcapkit/const/hip/certificate.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/cipher.py` & `pypcapkit-1.0.1/pcapkit/const/hip/cipher.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/di.py` & `pypcapkit-1.0.1/pcapkit/const/hip/di.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_curve.py` & `pypcapkit-1.0.1/pcapkit/const/hip/ecdsa_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_low_curve.py` & `pypcapkit-1.0.1/pcapkit/const/hip/ecdsa_low_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/eddsa_curve.py` & `pypcapkit-1.0.1/pcapkit/const/hip/eddsa_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/esp_transform_suite.py` & `pypcapkit-1.0.1/pcapkit/const/hip/esp_transform_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/group.py` & `pypcapkit-1.0.1/pcapkit/const/hip/group.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/hi_algorithm.py` & `pypcapkit-1.0.1/pcapkit/const/hip/hi_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/hit_suite.py` & `pypcapkit-1.0.1/pcapkit/const/hip/hit_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/nat_traversal.py` & `pypcapkit-1.0.1/pcapkit/const/hip/nat_traversal.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/notify_message.py` & `pypcapkit-1.0.1/pcapkit/const/hip/notify_message.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/packet.py` & `pypcapkit-1.0.1/pcapkit/const/hip/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/parameter.py` & `pypcapkit-1.0.1/pcapkit/const/hip/parameter.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/registration.py` & `pypcapkit-1.0.1/pcapkit/const/hip/registration.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/registration_failure.py` & `pypcapkit-1.0.1/pcapkit/const/hip/registration_failure.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/suite.py` & `pypcapkit-1.0.1/pcapkit/const/hip/suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/hip/transport.py` & `pypcapkit-1.0.1/pcapkit/const/hip/transport.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/error_code.py` & `pypcapkit-1.0.1/pcapkit/const/http/error_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/frame.py` & `pypcapkit-1.0.1/pcapkit/const/http/frame.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/method.py` & `pypcapkit-1.0.1/pcapkit/const/http/method.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/setting.py` & `pypcapkit-1.0.1/pcapkit/const/http/setting.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/http/status_code.py` & `pypcapkit-1.0.1/pcapkit/const/http/status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/classification_level.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/classification_level.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_class.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/option_class.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_number.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/option_number.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/protection_authority.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/protection_authority.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/qs_function.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/qs_function.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/router_alert.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/router_alert.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_del.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/tos_del.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_ecn.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/tos_ecn.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_pre.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/tos_pre.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_rel.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/tos_rel.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_thr.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/tos_thr.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/ts_flag.py` & `pypcapkit-1.0.1/pcapkit/const/ipv4/ts_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/extension_header.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/extension_header.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option_action.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/option_action.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/qs_function.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/qs_function.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/router_alert.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/router_alert.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/routing.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/routing.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/seed_id.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/seed_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/smf_dpd_mode.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/smf_dpd_mode.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/tagger_id.py` & `pypcapkit-1.0.1/pcapkit/const/ipv6/tagger_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipx/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/ipx/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipx/packet.py` & `pypcapkit-1.0.1/pcapkit/const/ipx/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ipx/socket.py` & `pypcapkit-1.0.1/pcapkit/const/ipx/socket.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/l2tp/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/l2tp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/l2tp/type.py` & `pypcapkit-1.0.1/pcapkit/const/l2tp/type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/access_type.py` & `pypcapkit-1.0.1/pcapkit/const/mh/access_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/ack_status_code.py` & `pypcapkit-1.0.1/pcapkit/const/mh/ack_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/ani_suboption.py` & `pypcapkit-1.0.1/pcapkit/const/mh/ani_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/auth_subtype.py` & `pypcapkit-1.0.1/pcapkit/const/mh/auth_subtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_ack_flag.py` & `pypcapkit-1.0.1/pcapkit/const/mh/binding_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_revocation.py` & `pypcapkit-1.0.1/pcapkit/const/mh/binding_revocation.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_update_flag.py` & `pypcapkit-1.0.1/pcapkit/const/mh/binding_update_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/dhcp_support_mode.py` & `pypcapkit-1.0.1/pcapkit/const/mh/dhcp_support_mode.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/dns_status_code.py` & `pypcapkit-1.0.1/pcapkit/const/mh/dns_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmip6_tls_packet.py` & `pypcapkit-1.0.1/pcapkit/const/mh/dsmip6_tls_packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmipv6_home_address.py` & `pypcapkit-1.0.1/pcapkit/const/mh/dsmipv6_home_address.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/enumerating_algorithm.py` & `pypcapkit-1.0.1/pcapkit/const/mh/enumerating_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_ack_status.py` & `pypcapkit-1.0.1/pcapkit/const/mh/fb_ack_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_action.py` & `pypcapkit-1.0.1/pcapkit/const/mh/fb_action.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_indication_trigger.py` & `pypcapkit-1.0.1/pcapkit/const/mh/fb_indication_trigger.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_type.py` & `pypcapkit-1.0.1/pcapkit/const/mh/fb_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_status.py` & `pypcapkit-1.0.1/pcapkit/const/mh/flow_id_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_suboption.py` & `pypcapkit-1.0.1/pcapkit/const/mh/flow_id_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/handoff_type.py` & `pypcapkit-1.0.1/pcapkit/const/mh/handoff_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_flag.py` & `pypcapkit-1.0.1/pcapkit/const/mh/handover_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_status.py` & `pypcapkit-1.0.1/pcapkit/const/mh/handover_ack_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_flag.py` & `pypcapkit-1.0.1/pcapkit/const/mh/handover_initiate_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_status.py` & `pypcapkit-1.0.1/pcapkit/const/mh/handover_initiate_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/home_address_reply.py` & `pypcapkit-1.0.1/pcapkit/const/mh/home_address_reply.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/lma_mag_suboption.py` & `pypcapkit-1.0.1/pcapkit/const/mh/lma_mag_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_group_id.py` & `pypcapkit-1.0.1/pcapkit/const/mh/mn_group_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_id_subtype.py` & `pypcapkit-1.0.1/pcapkit/const/mh/mn_id_subtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/operator_id.py` & `pypcapkit-1.0.1/pcapkit/const/mh/operator_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/option.py` & `pypcapkit-1.0.1/pcapkit/const/mh/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/packet.py` & `pypcapkit-1.0.1/pcapkit/const/mh/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/qos_attribute.py` & `pypcapkit-1.0.1/pcapkit/const/mh/qos_attribute.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_status_code.py` & `pypcapkit-1.0.1/pcapkit/const/mh/revocation_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_trigger.py` & `pypcapkit-1.0.1/pcapkit/const/mh/revocation_trigger.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/status_code.py` & `pypcapkit-1.0.1/pcapkit/const/mh/status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/traffic_selector.py` & `pypcapkit-1.0.1/pcapkit/const/mh/traffic_selector.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/upa_status.py` & `pypcapkit-1.0.1/pcapkit/const/mh/upa_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/mh/upn_reason.py` & `pypcapkit-1.0.1/pcapkit/const/mh/upn_reason.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ospf/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/ospf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ospf/authentication.py` & `pypcapkit-1.0.1/pcapkit/const/ospf/authentication.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/ospf/packet.py` & `pypcapkit-1.0.1/pcapkit/const/ospf/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/block_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/block_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/filter_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/filter_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/hash_algorithm.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/hash_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/option_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/option_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/record_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/record_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/secrets_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/secrets_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/verdict_type.py` & `pypcapkit-1.0.1/pcapkit/const/pcapng/verdict_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/reg/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/reg/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/reg/ethertype.py` & `pypcapkit-1.0.1/pcapkit/const/reg/ethertype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/reg/linktype.py` & `pypcapkit-1.0.1/pcapkit/const/reg/linktype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/reg/transtype.py` & `pypcapkit-1.0.1/pcapkit/const/reg/transtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/tcp/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/tcp/checksum.py` & `pypcapkit-1.0.1/pcapkit/const/tcp/checksum.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/tcp/mp_tcp_option.py` & `pypcapkit-1.0.1/pcapkit/const/tcp/mp_tcp_option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/tcp/option.py` & `pypcapkit-1.0.1/pcapkit/const/tcp/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/vlan/__init__.py` & `pypcapkit-1.0.1/pcapkit/const/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/const/vlan/priority_level.py` & `pypcapkit-1.0.1/pcapkit/const/vlan/priority_level.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/__init__.py` & `pypcapkit-1.0.1/pcapkit/corekit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 protocol collection class :class:`~pcapkit.corekit.protochain.ProtoChain`,
 and :class:`~pcapkit.corekit.multidict.MultiDict` family inspired from
 :mod:`Werkzeug` for multientry :obj:`dict` data mapping, the
 :class:`~pcapkit.corekit.fields.field.Field` family for data parsing.
 
 """
 from pcapkit.corekit.fields import *
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.corekit.multidict import MultiDict, OrderedMultiDict
 from pcapkit.corekit.protochain import ProtoChain
 from pcapkit.corekit.version import VersionInfo
 
 __all__ = [
-    'Info',
+    'Info', 'info_final',
 
     'ProtoChain',
 
     'VersionInfo',
 
     'MultiDict', 'OrderedMultiDict',
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/__init__.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/collections.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,17 +236,17 @@
             packet: Packet data.
 
         Returns:
             Unpacked field value.
 
         Important:
             If the option list ended before the specified size limit,
-            set :attr:`self.option_padding <OptionField.option_padding>` as the remaining length to
-            the ``packet`` argument such that the next fields can be
-            aware of such informations.
+            set :attr:`self.option_padding <OptionField.option_padding>`
+            as the remaining length to the ``packet`` argument such that
+            the next fields can be aware of such informations.
 
         """
         length = self._length
         if isinstance(buffer, bytes):
             file = io.BytesIO(buffer)  # type: IO[bytes]
         else:
             file = buffer
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/field.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,21 @@
             updating the current instance.
 
         """
         new_self = copy.copy(self)
         new_self._callback(new_self, packet)
         return new_self
 
+    # NOTE: This method is created as a placeholder for the necessary attributes.
+    def __init__(self, *args: 'Any', **kwargs: 'Any') -> 'None':
+        self._name = f'<{type(self).__name__[:-5].lower()}>'
+        self._default = NoValue
+        self._template = '0s'
+        self._callback = lambda *_: None
+
     def __repr__(self) -> 'str':
         if not self.name.isidentifier():
             return f'<{self.__class__.__name__}>'
         return f'<{self.__class__.__name__} {self.name}>'
 
     def pre_process(self, value: '_T', packet: 'dict[str, Any]') -> 'Any':  # pylint: disable=unused-argument
         """Process field value before construction (packing).
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/ipaddress.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/misc.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/misc.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/numbers.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/numbers.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/strings.py` & `pypcapkit-1.0.1/pcapkit/corekit/fields/strings.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/infoclass.py` & `pypcapkit-1.0.1/pcapkit/corekit/infoclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,120 @@
 :class:`~pcapkit.corekit.infoclass.Info` only, which is originally
 designed to work alike :func:`dataclasses.dataclass` as introduced
 in :pep:`557`.
 
 """
 import collections.abc
 import itertools
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, TypeVar, cast, final
 
 from pcapkit.utilities.compat import Mapping
-from pcapkit.utilities.exceptions import UnsupportedCall
+from pcapkit.utilities.exceptions import UnsupportedCall, stacklevel
+from pcapkit.utilities.warnings import InfoWarning, warn
 
 if TYPE_CHECKING:
-    from typing import Any, Iterable, Iterator, NoReturn, Optional
+    from typing import Any, Iterable, Iterator, NoReturn, Optional, Type
 
     from typing_extensions import Self
 
-__all__ = ['Info']
+__all__ = ['Info', 'info_final']
 
 VT = TypeVar('VT')
 
 
+def info_final(cls: 'Type[Info[VT]]') -> 'Type[Info[VT]]':
+    """Finalise info class.
+
+    Args:
+        cls: Info class.
+
+    Returns:
+        Finalised info class.
+
+    Notes:
+        This decorator function is used to generate necessary
+        attributes and methods for the decorated :class:`Info`
+        class. It can be useful to reduce runtime generation
+        time as well as caching already generated attributes.
+
+    :meta decorator:
+    """
+    if cls.__finalised__:
+        warn(f'{cls.__name__}: info class has been finalised; now skipping',
+             InfoWarning, stacklevel=stacklevel())
+        return cls
+
+    temp = ['__map__', '__map_reverse__', '__builtin__', '__finalised__']
+    temp.extend(cls.__additional__)
+    for obj in cls.mro():
+        temp.extend(dir(obj))
+    cls.__builtin__ = set(temp)
+    cls.__excluded__.extend(cls.__builtin__)
+
+    # NOTE: We only generate ``__init__`` method for subclasses of the
+    # ``Info`` class, rather than itself, plus that such class does not
+    # override the ``__init__`` method of the meta class.
+    if '__init__' not in cls.__dict__ and cls is not Info:
+        args_ = []  # type: list[str]
+        dict_ = []  # type: list[str]
+
+        for cls_ in cls.mro():
+            # NOTE: We skip the ``Info`` class itself, to avoid superclass
+            # type annotations being considered.
+            if cls_ is Info:
+                break
+
+            # NOTE: We iterate in reversed order to ensure that the type
+            # annotations of the superclasses are considered first.
+            for key in reversed(cls_.__annotations__):
+                # NOTE: We skip duplicated annotations to avoid duplicate
+                # argument in function definition.
+                if key in args_:
+                    continue
+
+                args_.append(key)
+                dict_.append(f'{key}={key}')
+
+        # NOTE: We reverse the two lists such that the order of the
+        # arguments is the same as the order of the type annotations, i.e.,
+        # from the most base class to the most derived class.
+        args_.reverse()
+        dict_.reverse()
+
+        # NOTE: We only generate typed ``__init__`` method if only the class
+        # has type annotations from any of itself and its base classes.
+        if args_:
+            # NOTE: The following code is to make the ``__init__`` method work.
+            # It is inspired from the :func:`dataclasses._create_fn` function.
+            init_ = (
+                f'def __create_fn__():\n'
+                f'    def __init__(self, {", ".join(args_)}):\n'
+                f'        self.__update__({", ".join(dict_)})\n'
+                f'        self.__post_init__()\n'
+                f'    return __init__\n'
+            )
+        else:
+            init_ = (
+                'def __create_fn__():\n'
+                '    def __init__(self, dict_=None, **kwargs):\n'
+                '        self.__update__(dict_, **kwargs)\n'
+                '        self.__post_init__()\n'
+                '    return __init__\n'
+            )
+
+        ns = {}  # type: dict[str, Any]
+        exec(init_, None, ns)  # pylint: disable=exec-used # nosec
+
+        cls.__init__ = ns['__create_fn__']()
+        cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
+
+    cls.__finalised__ = True
+    return final(cls)
+
+
 class Info(Mapping[str, VT], Generic[VT]):
     """Turn dictionaries into :obj:`object` like instances.
 
     * :class:`Info` objects inherit from :obj:`dict` type
     * :class:`Info` objects are *iterable*, and support all functions as
       :obj:`dict` type
     * :class:`Info` objects are **immutable**, thus cannot set or delete
@@ -51,14 +142,17 @@
         __map__: 'dict[str, str]'
         #: Mapping of name conflicts with builtin methods (transformed names to
         #: original names).
         __map_reverse__: 'dict[str, str]'
         #: List of builtin methods.
         __builtin__: 'set[str]'
 
+    #: Flag for finalised class initialisation.
+    __finalised__ = False
+
     #: List of additional built-in names.
     __additional__: 'list[str]' = []
     #: List of names to be excluded from :obj:`dict` conversion.
     __excluded__: 'list[str]' = []
 
     def __new__(cls, *args: 'VT', **kwargs: 'VT') -> 'Self':  # pylint: disable=unused-argument
         """Create a new instance.
@@ -68,77 +162,16 @@
         which is inspired by :pep:`557` (:mod:`dataclasses`).
 
         Args:
             *args: Arbitrary positional arguments.
             **kwargs: Arbitrary keyword arguments.
 
         """
-        temp = ['__map__', '__map_reverse__', '__builtin__']
-        temp.extend(cls.__additional__)
-        for obj in cls.mro():
-            temp.extend(dir(obj))
-        cls.__builtin__ = set(temp)
-        cls.__excluded__.extend(cls.__builtin__)
-
-        # NOTE: We only generate ``__init__`` method for subclasses of the
-        # ``Info`` class, rather than itself, plus that such class does not
-        # override the ``__init__`` method of the meta class.
-        if '__init__' not in cls.__dict__ and cls is not Info:
-            args_ = []  # type: list[str]
-            dict_ = []  # type: list[str]
-
-            for cls_ in cls.mro():
-                # NOTE: We skip the ``Info`` class itself, to avoid superclass
-                # type annotations being considered.
-                if cls_ is Info:
-                    break
-
-                # NOTE: We iterate in reversed order to ensure that the type
-                # annotations of the superclasses are considered first.
-                for key in reversed(cls_.__annotations__):
-                    # NOTE: We skip duplicated annotations to avoid duplicate
-                    # argument in function definition.
-                    if key in args_:
-                        continue
-
-                    args_.append(key)
-                    dict_.append(f'{key}={key}')
-
-            # NOTE: We reverse the two lists such that the order of the
-            # arguments is the same as the order of the type annotations, i.e.,
-            # from the most base class to the most derived class.
-            args_.reverse()
-            dict_.reverse()
-
-            # NOTE: We only generate typed ``__init__`` method if only the class
-            # has type annotations from any of itself and its base classes.
-            if args_:
-                # NOTE: The following code is to make the ``__init__`` method work.
-                # It is inspired from the :func:`dataclasses._create_fn` function.
-                init_ = (
-                    f'def __create_fn__():\n'
-                    f'    def __init__(self, {", ".join(args_)}):\n'
-                    f'        self.__update__({", ".join(dict_)})\n'
-                    f'        self.__post_init__()\n'
-                    f'    return __init__\n'
-                )
-            else:
-                init_ = (
-                    'def __create_fn__():\n'
-                    '    def __init__(self, dict_=None, **kwargs):\n'
-                    '        self.__update__(dict_, **kwargs)\n'
-                    '        self.__post_init__()\n'
-                    '    return __init__\n'
-                )
-
-            ns = {}  # type: dict[str, Any]
-            exec(init_, None, ns)  # pylint: disable=exec-used # nosec
-            cls.__init__ = ns['__create_fn__']()
-            cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
-
+        if not cls.__finalised__:
+            cls = cast('Type[Self]', info_final(cls))
         self = super().__new__(cls)
 
         # NOTE: We define the ``__map__`` and ``__map_reverse__`` attributes
         # here under ``self`` to avoid them being considered as class variables
         # and thus being shared by all instances.
         super().__setattr__(self, '__map__', {})
         super().__setattr__(self, '__map_reverse__', {})
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/multidict.py` & `pypcapkit-1.0.1/pcapkit/corekit/multidict.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/corekit/protochain.py` & `pypcapkit-1.0.1/pcapkit/corekit/protochain.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/dumpkit/common.py` & `pypcapkit-1.0.1/pcapkit/dumpkit/common.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/dumpkit/null.py` & `pypcapkit-1.0.1/pcapkit/dumpkit/null.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/dumpkit/pcap.py` & `pypcapkit-1.0.1/pcapkit/dumpkit/pcap.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/dpkt.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/dpkt.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/engine.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/engine.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcap.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/pcap.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcapng.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/pcapng.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 support, as is used by :class:`pcapkit.foundation.extraction.Extractor`.
 
 """
 from logging import warn
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.pcapng.block_type import BlockType as Enum_BlockType
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.foundation.engines.engine import Engine
 from pcapkit.protocols.misc.pcapng import PCAPNG as P_PCAPNG
 from pcapkit.utilities.exceptions import FormatError, stacklevel
 from pcapkit.utilities.warnings import DeprecatedFormatWarning
 
 __all__ = ['PCAPNG']
 
@@ -35,14 +35,15 @@
     from pcapkit.protocols.data.misc.pcapng import PacketBlock as Data_PacketBlock
     from pcapkit.protocols.data.misc.pcapng import SectionHeaderBlock as Data_SectionHeaderBlock
     from pcapkit.protocols.data.misc.pcapng import \
         SystemdJournalExportBlock as Data_SystemdJournalExportBlock
     from pcapkit.protocols.data.misc.pcapng import UnknownBlock as Data_UnknownBlock
 
 
+@info_final
 class Context(Info):
     """Context manager for PCAP-NG file format."""
 
     #: Section header.
     section: 'Data_SectionHeaderBlock'
 
     def __post_init__(self) -> None:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pyshark.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/pyshark.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/scapy.py` & `pypcapkit-1.0.1/pcapkit/foundation/engines/scapy.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,24 +42,24 @@
     def name(cls) -> 'str':
         """Engine name."""
         return 'Scapy'
 
     @classmethod
     def module(cls) -> 'str':
         """Engine module name."""
-        return 'scapy.all'
+        return 'scapy'
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
     def __init__(self, extractor: 'Extractor') -> 'None':
-        from scapy import all as scapy_all  # isort:skip
+        from scapy import sendrecv as scapy  # isort:skip
 
-        self._expkg = scapy_all
+        self._expkg = scapy
         self._extmp = cast('Iterator[ScapyPacket]', None)
 
         super().__init__(extractor)
 
     ##########################################################################
     # Methods.
     ##########################################################################
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/extraction.py` & `pypcapkit-1.0.1/pcapkit/foundation/extraction.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 __all__ = [
     'IPv4_Reassembly', 'IPv6_Reassembly',   # IP Reassembly
     'TCP_Reassembly',                       # TCP Reassembly
 ]
 
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 
 if TYPE_CHECKING:
     from typing import Optional
 
 
+@info_final
 class ReassemblyManager(Info):
     """Reassembly Manager."""
 
     #: IPv4 reassembly.
     ipv4: 'IPv4_Reassembly'
     #: IPv6 reassembly.
     ipv6: 'IPv6_Reassembly'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 
     'TCP_Packet', 'TCP_DatagramID', 'TCP_Datagram', 'TCP_Buffer',
     'TCP_Fragment', 'TCP_HoleDiscriptor', 'TCP_BufferID',
 ]
 
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 
 if TYPE_CHECKING:
     from typing import Optional
 
 
+@info_final
 class ReassemblyData(Info):
     """Data storage for reassembly."""
 
     #: IPv4 reassembled data.
     ipv4: 'tuple[IP_Datagram, ...]'
     #: IPv6 reassembled data.
     ipv6: 'tuple[IP_Datagram, ...]'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/ip.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """data models for IP reassembly"""
 
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.utilities.compat import Tuple
 
 __all__ = [
     'Packet', 'DatagramID', 'Datagram', 'Buffer', 'BufferID',
 ]
 
 if TYPE_CHECKING:
@@ -21,14 +21,15 @@
 
 AT = TypeVar('AT', 'IPv4Address', 'IPv6Address')
 
 #: Buffer ID.
 BufferID = Tuple[AT, AT, int, 'TransType']
 
 
+@info_final
 class Packet(Info, Generic[AT]):
     """Data model for :term:`reasm.ipv4.packet` / :term:`reasm.ipv6.packet`."""
 
     #: Buffer ID.
     bufid: 'BufferID'
     #: Original packet range number.
     num: 'int'
@@ -45,14 +46,15 @@
     #: Raw :obj:`bytearray` type payload.
     payload: 'bytearray'
 
     if TYPE_CHECKING:
         def __init__(self, bufid: 'tuple[AT, AT, int, TransType]', num: 'int', fo: 'int', ihl: 'int', mf: 'bool', tl: 'int', header: 'bytes', payload: 'bytearray') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class DatagramID(Info, Generic[AT]):
     """Data model for :term:`reasm.ipv4.datagram` / :term:`reasm.ipv6.datagram` original packet identifier."""
 
     #: Source address.
     src: 'AT'
     #: Destination address.
     dst: 'AT'
@@ -61,14 +63,15 @@
     #: Payload protocol type.
     proto: 'TransType'
 
     if TYPE_CHECKING:
         def __init__(self, src: 'AT', dst: 'AT', id: 'int', proto: 'TransType') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Datagram(Info, Generic[AT]):
     """Data model for :term:`reasm.ipv4.datagram` / :term:`reasm.ipv6.datagram`."""
 
     #: Completed flag.
     completed: 'bool'
     #: Original packet identifier.
     id: 'DatagramID[AT]'
@@ -87,14 +90,15 @@
 
         @overload
         def __init__(self, completed: 'Literal[False]', id: 'DatagramID[AT]', index: 'tuple[int, ...]', header: 'bytes', payload: 'tuple[bytes, ...]', packet: 'None') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
         def __init__(self, completed: 'bool', id: 'DatagramID[AT]', index: 'tuple[int, ...]', header: 'bytes', payload: 'bytes | tuple[bytes, ...]', packet: 'Optional[Protocol]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Buffer(Info, Generic[AT]):
     """Data model for :term:`reasm.ipv4.buffer` / :term:`reasm.ipv6.buffer`."""
 
     #: Total data length.
     TDL: 'int'
     #: Fragment received bit table.
     RCVBT: 'bytearray'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/tcp.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/data/tcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """data models for TCP reassembly"""
 
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.utilities.compat import Tuple
 
 __all__ = [
     'Packet', 'DatagramID', 'Datagram', 'HoleDiscriptor',
     'Fragment', 'Buffer', 'BufferID',
 ]
 
@@ -21,14 +21,15 @@
 
 IPAddress = TypeVar('IPAddress', 'IPv4Address', 'IPv6Address')
 
 #: Buffer ID.
 BufferID = Tuple[IPAddress, int, IPAddress, int]
 
 
+@info_final
 class Packet(Info):
     """Data model for :term:`reasm.tcp.packet`."""
 
     #: Buffer ID.
     bufid: 'BufferID'
     #: Data sequence number.
     dsn: 'int'
@@ -53,28 +54,30 @@
     #: Raw :obj:`bytearray` type payload.
     payload: 'bytearray'
 
     if TYPE_CHECKING:
         def __init__(self, bufid: 'BufferID', dsn: 'int', ack: 'int', num: 'int', syn: 'bool', fin: 'bool', rst: 'bool', len: 'int', first: 'int', last: 'int', header: 'bytes', payload: 'bytearray') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class DatagramID(Info, Generic[IPAddress]):
     """Data model for :term:`reasm.tcp.datagram` original packet identifier."""
 
     #: Source address.
     src: 'tuple[IPAddress, int]'
     #: Destination address.
     dst: 'tuple[IPAddress, int]'
     #: Original packet ACK number.
     ack: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, src: 'tuple[IPAddress, int]', dst: 'tuple[IPAddress, int]', ack: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Datagram(Info, Generic[IPAddress]):
     """Data model for :term:`reasm.tcp.datagram`."""
 
     #: Completed flag.
     completed: 'bool'
     #: Original packet identifier.
     id: 'DatagramID[IPAddress]'
@@ -93,26 +96,28 @@
 
         @overload
         def __init__(self, completed: 'Literal[False]', id: 'DatagramID[IPAddress]', index: 'tuple[int, ...]', header: 'bytes', payload: 'tuple[bytes, ...]', packet: 'None') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
         def __init__(self, completed: 'bool', id: 'DatagramID[IPAddress]', index: 'tuple[int, ...]', header: 'bytes', payload: 'bytes | tuple[bytes, ...]', packet: 'Optional[Protocol]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class HoleDiscriptor(Info):
     """Data model for :term:`reasm.tcp.buffer` hole descriptor."""
 
     #: Start of hole.
     first: 'int'
     #: Stop of hole.
     last: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, first: 'int', last: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Fragment(Info):
     """Data model for :term:`reasm.tcp.buffer` ACK list fragment item."""
 
     #: List of reassembled packets.
     ind: 'list[int]'
     #: ISN of payload buffer.
     isn: 'int'
@@ -121,14 +126,15 @@
     #: Reassembled payload holes set to b'\x00'.
     raw: 'bytearray'
 
     if TYPE_CHECKING:
         def __init__(self, ind: 'list[int]', isn: 'int', len: 'int', raw: 'bytearray') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Buffer(Info):
     """Data model for :term:`reasm.tcp.buffer`."""
 
     #: Hole descriptor list.
     hdl: 'list[HoleDiscriptor]'
     #: Initial TCP header.
     hdr: 'bytes'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ip.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/ip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv4.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/ipv4.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv6.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/ipv6.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/reassembly.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/reassembly.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/tcp.py` & `pypcapkit-1.0.1/pcapkit/foundation/reassembly/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/registry.py` & `pypcapkit-1.0.1/pcapkit/foundation/registry.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/traceflow/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 __all__ = [
     'TCP_TraceFlow',
 ]
 
 
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 
 if TYPE_CHECKING:
     from typing import Optional
 
 
+@info_final
 class TraceFlowManager(Info):
     """TraceFlow Manager."""
 
     #: TCP reassembly.
     tcp: 'TCP_TraceFlow'
 
     if TYPE_CHECKING:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/__init__.py` & `pypcapkit-1.0.1/pcapkit/foundation/traceflow/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 __all__ = [
     'TCP_Buffer', 'TCP_BufferID', 'TCP_Index', 'TCP_Packet',
 ]
 
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 
 if TYPE_CHECKING:
     from typing import Optional
 
 
+@info_final
 class TraceFlowData(Info):
     """Data storage for flow tracing."""
 
     #: TCP traced flows.
     tcp: 'tuple[TCP_Index, ...]'
 
     if TYPE_CHECKING:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/tcp.py` & `pypcapkit-1.0.1/pcapkit/foundation/traceflow/data/tcp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """data models for TCP flow tracing"""
 
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.utilities.compat import Tuple
 
 __all__ = ['BufferID', 'Packet', 'Buffer', 'Index']
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address, IPv6Address
     from typing import Any, Optional
@@ -19,14 +19,15 @@
 
 IPAddress = TypeVar('IPAddress', 'IPv4Address', 'IPv6Address')
 
 #: Buffer ID.
 BufferID = Tuple[IPAddress, int, IPAddress, int]
 
 
+@info_final
 class Packet(Info, Generic[IPAddress]):
     """Data structure for **TCP flow tracing**.
 
     See Also:
         * :meth:`pcapkit.foundation.traceflow.TraceFlow.dump`
         * :term:`trace.tcp.packet`
 
@@ -54,14 +55,15 @@
     timestamp: 'float'
 
     if TYPE_CHECKING:
         def __init__(self, protocol: 'Enum_LinkType', index: 'int', frame: 'Data_Frame | dict[str, Any]', syn: 'bool', fin: 'bool', src: 'IPAddress', dst: 'IPAddress',
                      srcport: 'int', dstport: 'int', timestamp: 'float') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long
 
 
+@info_final
 class Buffer(Info):
     """Data structure for **TCP flow tracing**.
 
     See Also:
         * :attr:`pcapkit.foundation.traceflow.TraceFlow.index`
         * :term:`trace.tcp.buffer`
 
@@ -75,14 +77,15 @@
     label: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, fpout: 'Dumper',
                      index: 'list[int]', label: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
 
 
+@info_final
 class Index(Info):
     """Data structure for **TCP flow tracing**.
 
     See Also:
         * element from :attr:`pcapkit.foundation.traceflow.TraceFlow.index`
           *tuple*
         * :term:`trace.tcp.index`
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/tcp.py` & `pypcapkit-1.0.1/pcapkit/foundation/traceflow/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/traceflow.py` & `pypcapkit-1.0.1/pcapkit/foundation/traceflow/traceflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 import abc
 import collections
 import importlib
 import os
 import sys
 from typing import TYPE_CHECKING, Generic, TypeVar, overload
 
-from pcapkit.corekit.infoclass import Info
 from pcapkit.dumpkit.common import make_dumper
 from pcapkit.utilities.exceptions import FileExists, stacklevel
 from pcapkit.utilities.warnings import FileWarning, FormatWarning, warn
 
 __all__ = ['TraceFlow']
 
 if TYPE_CHECKING:
     from typing import Any, DefaultDict, Optional, Type
 
     from dictdumper.dumper import Dumper
     from typing_extensions import Literal, Self
 
+    from pcapkit.corekit.infoclass import Info
     from pcapkit.protocols.protocol import Protocol
 
 BufferID = TypeVar('BufferID')
 Buffer = TypeVar('Buffer', bound='Info')
 Index = TypeVar('Index', bound='Info')
 Packet = TypeVar('Packet', bound='Info')
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/interface/__init__.py` & `pypcapkit-1.0.1/pcapkit/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/interface/core.py` & `pypcapkit-1.0.1/pcapkit/interface/core.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/interface/misc.py` & `pypcapkit-1.0.1/pcapkit/interface/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 user interface functions, classes, etc., which are
 generally provided per user's requests.
 
 """
 import sys
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.infoclass import Info
+from pcapkit.corekit.infoclass import Info, info_final
 from pcapkit.foundation.extraction import Extractor
 from pcapkit.foundation.reassembly.tcp import TCP as TCP_Reassembly
 from pcapkit.utilities.exceptions import stacklevel
 from pcapkit.utilities.warnings import EngineWarning, warn
 
 if TYPE_CHECKING:
     from typing import Optional
@@ -32,14 +32,15 @@
 __all__ = ['follow_tcp_stream']
 
 ###############################################################################
 # Follow TCP Stream
 ###############################################################################
 
 
+@info_final
 class Stream(Info):
     """Data model for TCP streams."""
 
     #: Output filename.
     filename: 'Optional[str]'
     #: Packet list.
     packets: 'tuple[Packet, ...]'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/application.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/application.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/ftp.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/ftp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/http.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/http.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv1.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/httpv1.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv2.py` & `pypcapkit-1.0.1/pcapkit/protocols/application/httpv2.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/ftp.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/application/ftp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """data models for FTP protocol"""
 
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
     from pcapkit.const.ftp.command import Command
     from pcapkit.const.ftp.return_code import ReturnCode
@@ -22,28 +23,30 @@
 class FTP(Data):
     """Data model for FTP protocol."""
 
     #: Type.
     type: 'FTP_Type'
 
 
+@info_final
 class Request(FTP):
     """Data model for FTP request."""
 
     #: Type.
     type: 'Literal[FTP_Type.REQUEST]'
     #: Command.
     cmmd: 'Command'
     #: Arguments.
     args: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Literal[FTP_Type.REQUEST]', cmmd: 'Command', args: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Response(FTP):
     """Data model for FTP response."""
 
     #: Type.
     type: 'Literal[FTP_Type.RESPONSE]'
     #: Return code.
     code: 'ReturnCode'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv1.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/application/httpv1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 """data model for HTTP/1.* protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing import Any
 
-    from typing_extensions import Literal
-
     from pcapkit.const.http.method import Method as Enum_Method
     from pcapkit.const.http.status_code import StatusCode as Enum_StatusCode
     from pcapkit.corekit.multidict import OrderedMultiDict
     from pcapkit.protocols.application.httpv1 import Type as HTTP_Type
 
 __all__ = [
     'HTTP',
 
     'Header',
     'RequestHeader', 'ResponseHeader',
 ]
 
 
+@info_final
 class HTTP(Data):
     """Data model for HTTP/1.* protocol."""
 
     #: HTTP receipt.
     receipt: 'Header'
     #: HTTP header.
     header: 'OrderedMultiDict[str, str]'
@@ -40,37 +40,39 @@
 class Header(Data):
     """Data model for HTTP/1.* header line."""
 
     #: Receipt type.
     type: 'HTTP_Type'
 
 
+@info_final
 class RequestHeader(Header):
     """Data model for HTTP/1.* request header line."""
 
     #: HTTP request header line.
-    type: 'Literal[HTTP_Type.REQUEST]'
+    type: 'HTTP_Type'
     #: HTTP method.
     method: 'Enum_Method'
     #: HTTP request URI.
     uri: 'str'
     #: HTTP request version.
     version: 'str'
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Literal[HTTP_Type.REQUEST]', method: 'Enum_Method', uri: 'str', version: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
+        def __init__(self, type: 'HTTP_Type', method: 'Enum_Method', uri: 'str', version: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class ResponseHeader(Header):
     """Data model for HTTP/1.* response header line."""
 
     #: HTTP response header line.
-    type: 'Literal[HTTP_Type.RESPONSE]'
+    type: 'HTTP_Type'
     #: HTTP response version.
     version: 'str'
     #: HTTP response status.
     status: 'Enum_StatusCode'
     #: HTTP response status message.
     message: 'str'
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Literal[HTTP_Type.RESPONSE]', version: 'str', status: 'Enum_StatusCode', message: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
+        def __init__(self, type: 'HTTP_Type', version: 'str', status: 'Enum_StatusCode', message: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv2.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/application/httpv2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for HTTP/2 protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from typing_extensions import Literal
 
@@ -46,52 +47,56 @@
     type: 'Frame'
     #: Flags.
     flags: 'Optional[Flags]'
     #: Stream ID.
     sid: 'int'
 
 
+@info_final
 class UnassignedFrame(HTTP):
     """Data model for HTTP/2 unassigned frame."""
 
     #: Flags.
     flags: 'Literal[None]'
     #: Frame payload.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Literal[None]', sid: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class DataFrameFlags(Flags):
     """Data model for HTTP/2 ``DATA`` frame flags."""
 
     #: ``END_STREAM`` flag.
     END_STREAM: 'bool'  # bit 0
     #: ``PADDED`` flag.
     PADDED: 'bool'      # bit 3
 
     if TYPE_CHECKING:
         def __init__(self, END_STREAM: 'bool', PADDED: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class DataFrame(HTTP):
     """Data model for HTTP/2 ``DATA`` frame."""
 
     #: Flags.
     flags: 'DataFrameFlags'
     #: Padded length.
     pad_len: 'int'
     #: Frame payload.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'DataFrameFlags', pad_len: 'int', sid: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class HeadersFrameFlags(Flags):
     """Data model for HTTP/2 ``HEADERS`` frame flags."""
 
     #: ``END_STREAM`` flag.
     END_STREAM: 'bool'   # bit 0
     #: ``END_HEADERS`` flag.
     END_HEADERS: 'bool'  # bit 2
@@ -100,14 +105,15 @@
     #: ``PRIORITY`` flag.
     PRIORITY: 'bool'     # bit 5
 
     if TYPE_CHECKING:
         def __init__(self, END_STREAM: 'bool', END_HEADERS: 'bool', PADDED: 'bool', PRIORITY: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class HeadersFrame(HTTP):
     """Data model for HTTP/2 ``HEADERS`` frame."""
 
     #: Flags.
     flags: 'HeadersFrameFlags'
     #: Padded length.
     pad_len: 'int'
@@ -120,14 +126,15 @@
     #: Header block fragment.
     fragment: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'HeadersFrameFlags', pad_len: 'int', sid: 'int', excl_dependency: 'bool', stream_dependency: 'int', weight: 'int', fragment: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PriorityFrame(HTTP):
     """Data model for HTTP/2 ``PRIORITY`` frame."""
 
     #: Flags.
     flags: 'Literal[None]'
     #: Exclusive dependency.
     excl_dependency: 'bool'
@@ -136,60 +143,65 @@
     #: Weight.
     weight: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Literal[None]', sid: 'int', excl_dependency: 'bool', stream_dependency: 'int', weight: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class RSTStreamFrame(HTTP):
     """Data model for HTTP/2 ``RST_STREAM`` frame."""
 
     #: Flags.
     flags: 'Literal[None]'
     #: Error code.
     error: 'ErrorCode'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Literal[None]', sid: 'int', error: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SettingsFrameFlags(Flags):
     """Data model for HTTP/2 ``SETTINGS`` frame flags."""
 
     #: ``ACK`` flag.
     ACK: 'bool'  # bit 0
 
     if TYPE_CHECKING:
         def __init__(self, ACK: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SettingsFrame(HTTP):
     """Data model for HTTP/2 ``SETTINGS`` frame."""
 
     #: Flags.
     flags: 'SettingsFrameFlags'
     #: Settings.
     settings: 'OrderedMultiDict[Setting, int]'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Optional[Flags]', sid: 'int', settings: 'OrderedMultiDict[Setting, int]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PushPromiseFrameFlags(Flags):
     """Data model for HTTP/2 ``PUSH_PROMISE`` frame flags."""
 
     #: ``END_HEADERS`` flag.
     END_HEADERS: 'bool'  # bit 2
     #: ``PADDED`` flag.
     PADDED: 'bool'       # bit 3
 
     if TYPE_CHECKING:
         def __init__(self, END_HEADERS: 'bool', PADDED: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PushPromiseFrame(HTTP):
     """Data model for HTTP/2 ``PUSH_PROMISE`` frame."""
 
     #: Flags.
     flags: 'PushPromiseFrameFlags'
     #: Padded length.
     pad_len: 'int'
@@ -198,36 +210,39 @@
     #: Header block fragment.
     fragment: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Optional[Flags]', pad_len: 'int', sid: 'int', promised_sid: 'int', fragment: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PingFrameFlags(Flags):
     """Data model for HTTP/2 ``PING`` frame flags."""
 
     #: ``ACK`` flag.
     ACK: 'bool'  # bit 0
 
     if TYPE_CHECKING:
         def __init__(self, ACK: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PingFrame(HTTP):
     """Data model for HTTP/2 ``PING`` frame."""
 
     #: Flags.
     flags: 'PingFrameFlags'
     #: Opaque data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Optional[Flags]', sid: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class GoawayFrame(HTTP):
     """Data model for HTTP/2 ``GOAWAY`` frame."""
 
     #: Flags.
     flags: 'Literal[None]'
     #: Last stream ID.
     last_sid: 'int'
@@ -236,36 +251,39 @@
     #: Additional debug data.
     debug_data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Optional[Flags]', sid: 'int', last_sid: 'int', error: 'int', debug_data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class WindowUpdateFrame(HTTP):
     """Data moddel for HTTP/2 ``WINDOW_UPDATE`` frame."""
 
     #: Flags.
     flags: 'Literal[None]'
     #: Window size increment.
     increment: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Frame', flags: 'Optional[Flags]', sid: 'int', increment: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class ContinuationFrameFlags(Flags):
     """Data model for HTTP/2 ``CONTINUATION`` frame flags."""
 
     #: ``END_HEADERS`` flag.
     END_HEADERS: 'bool'  # bit 2
 
     if TYPE_CHECKING:
         def __init__(self, END_HEADERS: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class ContinuationFrame(HTTP):
     """Data model for HTTP/2 ``CONTINUATION`` frame."""
 
     #: Flags.
     flags: 'ContinuationFrameFlags'
     #: Header block fragment.
     fragment: 'bytes'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/data.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/data.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ah.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ah.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """data model for AH protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from pcapkit.const.reg.transtype import TransType
 
 __all__ = ['AH']
 
 
+@info_final
 class AH(Data):
     """Data model for AH protocol."""
 
     #: Next header.
     next: 'TransType'
     #: Payload length.
     length: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hip.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/hip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for HIP protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from ipaddress import IPv6Address
     from typing import Optional
 
@@ -54,14 +55,15 @@
     'HIPMAC2Parameter', 'HIPSignature2Parameter', 'HIPSignatureParameter',
     'EchoRequestUnsignedParameter', 'EchoResponseUnsignedParameter', 'RelayFromParameter',
     'RelayToParameter', 'RouteViaParameter', 'FromParameter',
     'RVSHMACParameter', 'RelayHMACParameter',
 ]
 
 
+@info_final
 class Control(Data):
     """Data model for HIP controls."""
 
     #: Anonymous flag.
     anonymous: 'bool'
 
     if TYPE_CHECKING:
@@ -75,14 +77,15 @@
     type: 'Enum_Parameter'
     #: Critical flag.
     critical: 'bool'
     #: Content length.
     length: 'int'
 
 
+@info_final
 class HIP(Data):
     """Data model for HIP header."""
 
     #: Next header.
     next: 'TransType'
     #: Header length.
     length: 'int'
@@ -102,60 +105,65 @@
     if TYPE_CHECKING:
         #: HIP parameters.
         parameters: 'OrderedMultiDict[Enum_Parameter, Parameter]'
 
         def __init__(self, next: 'TransType', length: 'int', type: 'Packet', version: 'int', chksum: 'bytes', control: 'Control', shit: 'int', rhit: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class UnassignedParameter(Parameter):
     """Data model for unassigned parameter."""
 
     #: Content.
     contents: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', contents: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class ESPInfoParameter(Parameter):
     """Data model for HIP ``ESP_INFO`` parameter."""
 
     #: KEYMAT index.
     index: 'int'
     #: Old SDI.
     old_spi: 'int'
     #: New SDI.
     new_spi: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', index: 'int', old_spi: 'int', new_spi: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class R1CounterParameter(Parameter):
     """Data model for HIP ``R1_COUNTER`` parameter."""
 
     #: R1 counter.
     counter: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', counter: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class LocatorData(Data):
     """Data model for HIP locator data."""
 
     #: SPI.
     spi: 'int'
     #: IP address.
     ip: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, spi: 'int', ip: 'IPv6Address') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,multiple-statements
 
 
+@info_final
 class Locator(Data):
     """Data model for HIP locator."""
 
     #: Traffic.
     traffic: 'int'
     #: Locator type.
     type: 'int'
@@ -168,24 +176,26 @@
     #: Locator data.
     locator: 'LocatorData | IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, traffic: 'int', type: 'int', length: 'int', preferred: 'bool', lifetime: 'timedelta', locator: 'LocatorData | IPv6Address') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,multiple-statements,redefined-builtin,line-too-long
 
 
+@info_final
 class LocatorSetParameter(Parameter):
     """Data model for HIP ``LOCATOR_SET`` parameter."""
 
     #: Locator set.
     locator_set: 'tuple[Locator, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', locator_set: 'tuple[Locator, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class PuzzleParameter(Parameter):
     """Data model for HIP ``PUZZLE`` parameter."""
 
     #: Numeric index.
     index: 'int'
     #: Lifetime.
     lifetime: 'timedelta'
@@ -194,14 +204,15 @@
     #: Random number.
     random: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', index: 'int', lifetime: 'timedelta', opaque: 'bytes', random: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class SolutionParameter(Parameter):
     """Data model for HIP ``SOLUTION`` parameter."""
 
     #: Numeric index.
     index: 'int'
     #: Lifetime.
     lifetime: 'timedelta'
@@ -212,98 +223,107 @@
     #: Puzzle solution.
     solution: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', index: 'int', lifetime: 'timedelta', opaque: 'bytes', random: 'int', solution: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class SEQParameter(Parameter):
     """Data model for HIP ``SEQ`` parameter."""
 
     #: Unique ID.
     id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', id: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class ACKParameter(Parameter):
     """Data model for HIP ``ACK`` parameter."""
 
     #: Peer update IDs.
     update_id: 'tuple[int, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', update_id: 'tuple[int, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class DHGroupListParameter(Parameter):
     """Data model for HIP ``DH_GROUP_LIST`` parameter."""
 
     #: DH group list.
     group_id: 'tuple[Group, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', group_id: 'tuple[Group, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class DiffieHellmanParameter(Parameter):
     """Data model for HIP ``DIFFIE_HELLMAN`` parameter."""
 
     #: Group ID.
     group_id: 'Group'
     #: Public value length.
     pub_len: 'int'
     #: Public value.
     pub_val: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', group_id: 'Group', pub_len: 'int', pub_val: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPTransformParameter(Parameter):
     """Data model for HIP ``HIP_TRANSFORM`` parameter."""
 
     #: Suite IDs.
     suite_id: 'tuple[Suite, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', suite_id: 'tuple[Suite, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPCipherParameter(Parameter):
     """Data model for HIP ``HIP_CIPHER`` parameter."""
 
     #: Cipher IDs.
     cipher_id: 'tuple[Cipher, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', cipher_id: 'tuple[Cipher, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class NATTraversalModeParameter(Parameter):
     """Data model for HIP ``NAT_TRAVERSAL_MODE`` parameter."""
 
     #: Mode IDs
     mode_id: 'tuple[NATTraversal, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', mode_id: 'tuple[NATTraversal, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class TransactionPacingParameter(Parameter):
     """Data model for HIP ``TRANSACTION_PACING`` parameter."""
 
     #: Min TA.
     min_ta: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', min_ta: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class EncryptedParameter(Parameter):
     """Data model for HIP ``ENCRYPTED`` parameter."""
 
     #: Cipher ID.
     cipher: 'Cipher'
     #: Initialization vector.
     iv: 'Optional[bytes]'
@@ -311,27 +331,29 @@
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int',
                      cipher: 'Cipher', iv: 'Optional[bytes]', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HostIdentity(Data):
     """Data model for host identity."""
 
     #: Curve type.
     curve: 'ECDSACurve | ECDSALowCurve | EdDSACurve'
     #: Public key.
     pubkey: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, curve: 'ECDSACurve | ECDSALowCurve | EdDSACurve',
                      pubkey: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HostIDParameter(Parameter):
     """Data model for HIP ``HOST_ID`` parameter."""
 
     #: Host identity length.
     hi_len: 'int'
     #: Domain identifier type.
     di_type: 'DITypes'
@@ -344,24 +366,26 @@
     #: Domain identifier.
     di: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', hi_len: 'int', di_type: 'DITypes', di_len: 'int', algorithm: 'HIAlgorithm', hi: 'HostIdentity | bytes', di: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HITSuiteListParameter(Parameter):
     """Data model for HIP ``HIST_SUITE_LIST`` parameter."""
 
     #: Suite IDs.
     suite_id: 'tuple[HITSuite, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', suite_id: 'tuple[HITSuite, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class CertParameter(Parameter):
     """Data model for HIP ``CERT`` parameter."""
 
     #: Certificate group.
     cert_group: 'Group'
     #: Certificate count.
     cert_count: 'int'
@@ -372,374 +396,407 @@
     #: Certificate.
     cert: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', cert_group: 'Group', cert_count: 'int', cert_id: 'int', cert_type: 'Certificate', cert: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class NotificationParameter(Parameter):
     """Data model for HIP ``NOTIFICATION`` parameter."""
 
     #: Notify message type.
     msg_type: 'NotifyMessage'
     #: Notification data.
     msg: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', msg_type: 'NotifyMessage', msg: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class EchoRequestSignedParameter(Parameter):
     """Data model for HIP ``ECHO_REQUEST_SIGNED`` parameter."""
 
     #: Opaque data.
     opaque: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', opaque: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class Lifetime(Data):
     """Data model for registration lifetime."""
 
     #: Minimum lifetime.
     min: 'timedelta'
     #: Maximum lifetime.
     max: 'timedelta'
 
     if TYPE_CHECKING:
         def __init__(self, min: 'timedelta', max: 'timedelta') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RegInfoParameter(Parameter):
     """Data model for HIP ``REG_INFO`` parameter."""
 
     #: Registration lifetime.
     lifetime: 'Lifetime'
     #: Registration type.
     reg_type: 'tuple[Registration, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', lifetime: 'Lifetime', reg_type: 'tuple[Registration, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RegRequestParameter(Parameter):
     """Data model for HIP ``REG_REQUEST`` parameter."""
 
     #: Registration lifetime.
     lifetime: 'timedelta'
     #: Registration type.
     reg_type: 'tuple[Registration, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', lifetime: 'timedelta', reg_type: 'tuple[Registration, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RegResponseParameter(Parameter):
     """Data model for HIP ``REG_RESPONSE`` parameter."""
 
     #: Registration lifetime.
     lifetime: 'timedelta'
     #: Registration type.
     reg_type: 'tuple[Registration, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', lifetime: 'timedelta', reg_type: 'tuple[Registration, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RegFailedParameter(Parameter):
     """Data model for HIP ``REG_FAILED`` parameter."""
 
     #: Registration lifetime.
     lifetime: 'timedelta'
     #: Registration failure type.
     reg_type: 'tuple[RegistrationFailure, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', lifetime: 'timedelta', reg_type: 'tuple[RegistrationFailure, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RegFromParameter(Parameter):
     """Data model for HIP ``REG_FROM`` parameter."""
 
     #: Port.
     port: 'int'
     #: Protocol.
     protocol: 'TransType'
     #: Address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', port: 'int', protocol: 'TransType', address: 'IPv6Address') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class EchoResponseSignedParameter(Parameter):
     """Data model for HIP ``ECHO_RESPONSE_SIGNED`` parameter."""
 
     #: Opaque data.
     opaque: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', opaque: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class TransportFormatListParameter(Parameter):
     """Data model for HIP ``TRANSPORT_FORMAT_LIST`` parameter."""
 
     #: Transport format list.
     tf_type: 'tuple[Enum_Parameter, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', tf_type: 'tuple[Enum_Parameter, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class ESPTransformParameter(Parameter):
     """Data model for HIP ``ESP_TRANSFORM`` parameter."""
 
     #: ESP transform.
     suite_id: 'tuple[ESPTransformSuite, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', suite_id: 'tuple[ESPTransformSuite, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class SeqDataParameter(Parameter):
     """Data model for HIP ``SEQ_DATA`` parameter."""
 
     #: Sequence number.
     seq: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', seq: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class AckDataParameter(Parameter):
     """Data model for HIP ``ACK_DATA`` parameter."""
 
     #: Acknowledged sequence number.
     ack: 'tuple[int, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', ack: 'tuple[int, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class PayloadMICParameter(Parameter):
     """Data model for HIP ``PAYLOAD_MIC`` parameter."""
 
     #: Next header
     next: 'TransType'
     #: Payload data.
     payload: 'bytes'
     #: MIC value.
     mic: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', next: 'TransType', payload: 'bytes', mic: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class TransactionIDParameter(Parameter):
     """Data model for HIP ``TRANSACTION_ID`` parameter."""
 
     #: Identifier.
     id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', id: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class OverlayIDParameter(Parameter):
     """Data mode HIP ``OVERLAY_ID`` parameter."""
 
     #: Identifier.
     id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', id: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class Flags(Data):
     """Data model for flags in HIP ``HIP_PARAMETER_FLAGS`` parameter."""
 
     #: Symmetric flag.
     symmetric: 'bool'
     #: Must follow flag.
     must_follow: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, symmetric: 'bool', must_follow: 'bool') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RouteDstParameter(Parameter):
     """Data model for HIP ``ROUTE_DST`` parameter."""
 
     #: Flags.
     flags: 'Flags'
     #: Destination address.
     hit: 'tuple[IPv6Address, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', flags: 'Flags', hit: 'tuple[IPv6Address, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPTransportModeParameter(Parameter):
     """Data model for HIP ``HIP_TRANSPORT_MODE`` parameter."""
 
     #: Port.
     port: 'int'
     #: Mode IDs.
     mode_id: 'tuple[Transport, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', port: 'int', mode_id: 'tuple[Transport, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPMACParameter(Parameter):
     """Data model for HIP ``HIP_MAC`` parameter."""
 
     #: HMAC value.
     hmac: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', hmac: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPMAC2Parameter(Parameter):
     """Data model for HIP ``HIP_MAC_2`` parameter."""
 
     #: HMAC value.
     hmac: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', hmac: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPSignature2Parameter(Parameter):
     """Data model for HIP ``HIP_SIGNATURE_2`` parameter."""
 
     #: Signature algorithm.
     algorithm: 'HIAlgorithm'
     #: Signature value.
     signature: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', algorithm: 'HIAlgorithm', signature: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class HIPSignatureParameter(Parameter):
     """Data model for HIP ``HIP_SIGNATURE`` parameter."""
 
     #: Signature algorithm.
     algorithm: 'HIAlgorithm'
     #: Signature value.
     signature: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', algorithm: 'HIAlgorithm', signature: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class EchoRequestUnsignedParameter(Parameter):
     """Data model for HIP ``ECHO_REQUEST_UNSIGNED`` parameter."""
 
     #: Opaque data.
     opaque: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', opaque: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class EchoResponseUnsignedParameter(Parameter):
     """Data model for HIP ``ECHO_RESPONSE_UNSIGNED`` parameter."""
 
     #: Opaque data.
     opaque: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', opaque: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RelayFromParameter(Parameter):
     """Data model for HIP ``RELAY_FROM`` parameter."""
 
     #: Port.
     port: 'int'
     #: Protocol.
     protocol: 'TransType'
     #: Address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', port: 'int', protocol: 'TransType', address: 'IPv6Address') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RelayToParameter(Parameter):
     """Data model for HIP ``RELAY_TO`` parameter."""
 
     #: Port.
     port: 'int'
     #: Protocol.
     protocol: 'TransType'
     #: Address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', port: 'int', protocol: 'TransType', address: 'IPv6Address') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class OverlayTTLParameter(Parameter):
     """Data model for HIP ``OVERLAY_TTL`` parameter."""
 
     #: TTL value.
     ttl: 'timedelta'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', ttl: 'timedelta') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RouteViaParameter(Parameter):
     """Data model for HIP ``ROUTE_VIA`` parameter."""
 
     #: Flags.
     flags: 'Flags'
     #: HIT addresses.
     hit: 'tuple[IPv6Address, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', flags: 'Flags', hit: 'tuple[IPv6Address, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class FromParameter(Parameter):
     """Data model for HIP ``FROM`` parameter."""
 
     #: HIT address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', address: 'IPv6Address') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RVSHMACParameter(Parameter):
     """Data model for HIP ``RVS_HMAC`` parameter."""
 
     #: HMAC value.
     hmac: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', hmac: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class ViaRVSParameter(Parameter):
     """Data model for HIP ``VIA_RVS`` parameter."""
 
     #: Addresses.
     address: 'tuple[IPv6Address, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', critical: 'bool', length: 'int', address: 'tuple[IPv6Address, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,redefined-builtin,super-init-not-called,line-too-long
 
 
+@info_final
 class RelayHMACParameter(Parameter):
     """Data model for HIP ``RELAY_HMAC`` parameter."""
 
     #: HMAC value.
     hmac: 'bytes'
 
     if TYPE_CHECKING:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hopopt.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/hopopt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for HOPOPT protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from ipaddress import IPv4Address, IPv6Address
     from typing import Optional
 
@@ -44,65 +45,71 @@
     action: 'OptionAction'
     #: Change flag.
     change: 'bool'
     #: Content length.
     length: 'int'
 
 
+@info_final
 class HOPOPT(Data):
     """Data model for HOPOPT protocol."""
 
     #: Next header.
     next: 'TransType'
     #: Header extension length.
     length: 'int'
     #: HOPOPT options.
     options: 'OrderedMultiDict[Enum_Option, Option]'
 
     if TYPE_CHECKING:
         def __init__(self, next: 'TransType', length: 'int', options: 'OrderedMultiDict[Enum_Option, Option]') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class UnassignedOption(Option):
     """Data model for HOPOPT unassigned option."""
 
     #: Option data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class PadOption(Option):
     """Data model for HOPOPT padding options."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class TunnelEncapsulationLimitOption(Option):
     """Data model for HOPOPT tunnel encapsulation limit option."""
 
     #: Tunnel encapsulation limit.
     limit: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', limit: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class RouterAlertOption(Option):
     """Data model for HOPOPT router alter option."""
 
     #: Router alter value.
     value: 'RouterAlert'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', value: 'RouterAlert') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class CALIPSOOption(Option):
     """Data model for HOPOPT Common Architecture Label IPv6 Security Option (CALIPSO) option."""
 
     #: CALIPSO domain of interpretation.
     domain: 'int'
     #: Compartment length.
     cmpt_len: 'int'
@@ -121,15 +128,15 @@
 class SMFDPDOption(Option):
     """Data model for HOPOPT Simplified Multicast Forwarding Duplicate Packet Detection (``SMF_DPD``) option."""
 
     #: DPD type.
     dpd_type: 'SMFDPDMode'
 
 
-
+@info_final
 class SMFIdentificationBasedDPDOption(SMFDPDOption):
     """Data model for HOPOPT **I-DPD** (Identification-Based DPD) option."""
 
     #: TaggerID type.
     tid_type: 'TaggerID'
     #: TaggerID length.
     tid_len: 'int'
@@ -138,24 +145,26 @@
     #: Identifier.
     id: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', dpd_type: 'SMFDPDMode', tid_type: 'TaggerID', tid_len: 'int', tid: 'Optional[bytes | IPv4Address | IPv6Address]', id: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class SMFHashBasedDPDOption(SMFDPDOption):
     """Data model for HOPOPT **H-DPD** (Hash-Based DPD) option."""
 
     #: Hash assist value.
     hav: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', dpd_type: 'SMFDPDMode', hav: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class PDMOption(Option):
     """Data model for HOPOPT Performance Diagnostic Metrics (PDM) option."""
 
     #: Scale delta time last received.
     scaledtlr: 'int'
     #: Scale delta time last sent.
     scaledtls: 'int'
@@ -177,77 +186,83 @@
 
     #: QS function.
     func: 'QSFunction'
     #: Rate request/report.
     rate: 'int'
 
 
+@info_final
 class QuickStartRequestOption(QuickStartOption):
     """Data model for HOPOPT Quick Start request option."""
 
     #: TTL.
     ttl: 'timedelta'
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', func: 'QSFunction', rate: 'int', ttl: 'timedelta',
                      nonce: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class QuickStartReportOption(QuickStartOption):
     """Data model for HOPOPT Quick Start report of approved rate option."""
 
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', func: 'QSFunction', rate: 'int', nonce: 'int') -> 'None': ...
 
 
+@info_final
 class RPLFlags(Data):
     """Data model for HOPOPT RPL option flags fields."""
 
     #: Down flag.
     down: 'bool'
     #: Rank error flag.
     rank_err: 'bool'
     #: Forwarding error flag.
     fwd_err: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, down: 'bool', rank_err: 'bool', fwd_err: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class RPLOption(Option):
     """Data model for HOPOPT Routing Protocol for Low-Power and Lossy Networks (RPL) option."""
 
     #: Flags.
     flags: 'RPLFlags'
     #: RPL instance ID.
     id: 'int'
     #: Sender rank.
     rank:' int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', flags: 'RPLFlags', id: 'int', rank: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class MPLFlags(Data):
     """Data model for HOPOPT MPL option flags fields."""
 
     #: Max flag.
     max: 'bool'
     #: Non-conformation flag.
     drop: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, max: 'bool', drop: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class MPLOption(Option):
     """Data model for HOPOPT Multicast Protocol for Low-Power and Lossy Networks (MPL) option."""
 
     #: Seed length.
     seed_type: 'SeedID'
     #: Flags.
     flags: 'MPLFlags'
@@ -256,69 +271,75 @@
     #: Seed ID.
     seed_id: 'Optional[int]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', seed_type: 'int', flags: 'MPLFlags', seq: 'int', seed_id: 'Optional[int]') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class ILNPOption(Option):
     """Data model for HOPOPT Identifier-Locator Network Protocol (ILNP) Nonce option."""
 
     #: Nonce value.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', nonce: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class LineIdentificationOption(Option):
     """Data model for HOPOPT Line-Identification option."""
 
     #: Line ID length.
     line_id_len: 'int'
     #: Line ID.
     line_id: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', line_id_len: 'int', line_id: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class JumboPayloadOption(Option):
     """Data model for Jumbo Payload option."""
 
     #: Jumbo payload length.
     jumbo_len: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      jumbo_len: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class HomeAddressOption(Option):
     """Data model for HOPOPT Home Address option."""
 
     #: Home address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', address: 'IPv6Address') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class DFFFlags(Data):
     """Data model for HOPOPT ``IP_DFF`` option flags."""
 
     #: Duplicate flag.
     dup: 'bool'
     #: Return flag.
     ret: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, dup: 'bool', ret: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class IPDFFOption(Option):
     """Data model for HOPOPT Depth-First Forwarding (``IP_DFF``) option."""
 
     #: Version.
     version: 'int'
     #:Flags.
     flags: 'DFFFlags'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv4.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv4.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """data model for IPv4 protocol"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.ipv4.option_class import OptionClass
 from pcapkit.const.ipv4.tos_del import ToSDelay
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from ipaddress import IPv4Address
     from typing import Any, Optional
 
@@ -38,14 +39,15 @@
     'ESECOption', 'RROption', 'SIDOption',
     'SSROption', 'MTUPOption', 'MTUROption',
     'TROption', 'RTRALTOption', 'QSOption',
     'QuickStartRequestOption', 'QuickStartReportOption',
 ]
 
 
+@info_final
 class ToSField(Data):
     """Data model for IPv4 ToS fields.
 
     Important:
         Due to the preserved keyword conflict, please use :meth:`from_dict`
         to create an instance of this data model.
 
@@ -65,29 +67,31 @@
     def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'ToSField':
         self = super().__new__(cls, *args, **kwargs)
 
         # NOTE: We cannot define ``del`` due to preserved keyword conflict.
         # Thus, we directly inject the information into the annotations.
         self.__annotations__['del'] = ToSDelay  # pylint: disable=no-member
 
-        return self  # type: ignore[return-value]
+        return self
 
 
+@info_final
 class Flags(Data):
     """Data model for IPv4 Flags."""
 
     #: Don't fragment.
     df: 'bool'
     #: More fragments.
     mf: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, df: 'bool', mf: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class IPv4(Data):
     """Data model for IPv4 packet."""
 
     #: Version.
     version: 'Literal[4]'
     #: Internet header length.
     hdr_len: 'int'
@@ -114,14 +118,15 @@
 
     if TYPE_CHECKING:
         options: 'OrderedMultiDict[OptionNumber, Option]'
 
         def __init__(self, version: 'Literal[4]', hdr_len: 'int', tos: 'ToSField', len: 'int', id: 'int', flags: 'Flags', offset: 'int', ttl: 'timedelta', protocol: 'TransType', checksum: 'bytes', src: 'IPv4Address', dst: 'IPv4Address') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class OptionType(Data):
     """Data model for IPv4 option type data."""
 
     #: Change flag.
     change: 'bool'
     #: Option class.
     #class: 'int'
@@ -131,76 +136,82 @@
     def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'OptionType':
         self = super().__new__(cls, *args, **kwargs)
 
         # NOTE: We cannot define ``class`` due to preserved keyword conflict.
         # Thus, we directly inject the information into the annotations.
         self.__annotations__['class'] = OptionClass  # pylint: disable=no-member
 
-        return self  # type: ignore[return-value]
+        return self
 
 
 class Option(Data):
     """Data model for IPv4 options."""
 
     #: Option code.
     code: 'OptionNumber'
     #: Option length.
     length: 'int'
     #: Option type.
     type: 'OptionType'
 
 
+@info_final
 class UnassignedOption(Option):
     """Data model for IPv4 unassigned option."""
 
     #: Option data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class EOOLOption(Option):
     """Data model for IPv4 End of Option List (``EOOL``) option."""
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class NOPOption(Option):
     """Data model for IPv4 No Operation (``NOP``) option."""
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SECOption(Option):
     """Data model for IPv4 Security (``SEC``) option."""
 
     #: Classification level.
     level: 'ClassificationLevel'
     #: Protection authority flags.
     flags: 'tuple[ProtectionAuthority, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', level: 'ClassificationLevel', flags: 'tuple[ProtectionAuthority, ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class LSROption(Option):
     """Data model for IPv4 Loose Source Route (``LSR``) option."""
 
     #: Pointer.
     pointer: 'int'
     #: Route.
     route: 'tuple[IPv4Address, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', pointer: 'int', route: 'tuple[IPv4Address, ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class TSOption(Option):
     """Data model for IPv4 Time Stamp (``TS``) option."""
 
     #: Pointer.
     pointer: 'int'
     #: Overflow.
     overflow: 'int'
@@ -209,80 +220,87 @@
     #: Timestamp data.
     timestamp: 'tuple[timedelta | int, ...] | OrderedMultiDict[IPv4Address, timedelta | int]'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', pointer: 'int', overflow: 'int', flag: 'TSFlag', timestamp: 'tuple[timedelta | int, ...] | OrderedMultiDict[IPv4Address, timedelta | int]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class ESECOption(Option):
     """Data model for IPv4 Extended Security (``ESEC``) option."""
 
     #: Additional security information format code.
     format: 'int'
     #: Additional security information.
     info: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', format: 'int', info: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class RROption(Option):
     """Data model for IPv4 Record Route (``RR``) option."""
 
     #: Pointer.
     pointer: 'int'
     #: Route.
     route: 'Optional[tuple[IPv4Address, ...]]'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', pointer: 'int', route: 'Optional[tuple[IPv4Address, ...]]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SIDOption(Option):
     """Data model for IPv4 Stream ID (``SID``) option."""
 
     #: Stream ID.
     sid: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', sid: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SSROption(Option):
     """Data model for IPv4 Strict Source Route (``SSR``) option."""
 
     #: Pointer.
     pointer: 'int'
     #: Route.
     route: 'Optional[tuple[IPv4Address, ...]]'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', pointer: 'int', route: 'Optional[tuple[IPv4Address, ...]]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MTUPOption(Option):
     """Data model for IPv4 MTU Probe (``MTUP``) option."""
 
     #: MTU.
     mtu: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', mtu: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MTUROption(Option):
     """Data model for IPv4 MTU Reply (``MTUR``) option."""
 
     #: MTU.
     mtu: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', mtu: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class TROption(Option):
     """Data model for IPv4 Traceroute (``TR``) option.
 
     Important:
         Due to the preserved keyword conflict, please use :meth:`from_dict`
         to create an instance of this data model.
 
@@ -299,17 +317,18 @@
     def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'TROption':
         self = super().__new__(cls, *args, **kwargs)
 
         # NOTE: We cannot define ``return`` due to preserved keyword conflict.
         # Thus, we directly inject the information into the annotations.
         self.__annotations__['return'] = int  # pylint: disable=no-member
 
-        return self  # type: ignore[return-value]
+        return self
 
 
+@info_final
 class RTRALTOption(Option):
     """Data model for IPv4 Router Alert (``RTRALT``) option."""
 
     #: Router alert.
     alert: 'RouterAlert'
 
     if TYPE_CHECKING:
@@ -321,26 +340,28 @@
 
     #: QS function.
     func: 'QSFunction'
     #: Rate request/report.
     rate: 'int'
 
 
+@info_final
 class QuickStartRequestOption(QSOption):
     """Data model for IPv4 Quick Start request option."""
 
     #: TTL.
     ttl: 'timedelta'
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
          def __init__(self, code: 'OptionNumber', length: 'int', type: 'OptionType', func: 'QSFunction', rate: 'int', ttl: 'timedelta', nonce: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class QuickStartReportOption(QSOption):
     """Data model for IPv4 Quick Start report of approved rate option."""
 
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 """data model for Internet Protocol version 6"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from ipaddress import IPv6Address
     from typing import Any
 
     from typing_extensions import Literal
 
     from pcapkit.const.reg.transtype import TransType
     from pcapkit.protocols.data.protocol import Packet
 
 __all__ = [
     'IPv6',
-
 ]
 
 
+@info_final
 class IPv6(Data):
     """Data model for Internet Protocol version 6.
 
     Important:
         Due to the preserved keyword conflict, please use :meth:`from_dict`
         to create an instance of this data model.
 
@@ -59,8 +60,8 @@
     def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'IPv6':
         self = super().__new__(cls, *args, **kwargs)
 
         # NOTE: We cannot define ``class`` due to preserved keyword conflict.
         # Thus, we directly inject the information into the annotations.
         self.__annotations__['class'] = int  # pylint: disable=no-member
 
-        return self  # type: ignore[return-value]
+        return self
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_frag.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_frag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """data models for IPv6 Fragment Header"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from pcapkit.const.reg.transtype import TransType
 
 __all__ = ['IPv6_Frag']
 
 
+@info_final
 class IPv6_Frag(Data):
     """Data model for IPv6 fragment header."""
 
     #: Next header.
     next: 'TransType'
     #: Fragment offset.
     offset: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_opts.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_opts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for IPv6 Destination Options protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from ipaddress import IPv4Address, IPv6Address
     from typing import Optional
 
@@ -44,14 +45,15 @@
     action: 'OptionAction'
     #: Change flag.
     change: 'bool'
     #: Content length.
     length: 'int'
 
 
+@info_final
 class IPv6_Opts(Data):
     """Data model for IPv6-Opts protocol."""
 
     #: Next header.
     next: 'TransType'
     #: Header extension length.
     length: 'int'
@@ -59,55 +61,60 @@
     options: 'OrderedMultiDict[Enum_Option, Option]'
 
     if TYPE_CHECKING:
         def __init__(self, next: 'TransType', length: 'int',
                      options: 'OrderedMultiDict[Enum_Option, Option]') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class UnassignedOption(Option):
     """Data model for IPv6-Opts unassigned option."""
 
     #: Option data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      data: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class PadOption(Option):
     """Data model for IPv6-Opts padding options."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool',
                      length: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class TunnelEncapsulationLimitOption(Option):
     """Data model for IPv6-Opts tunnel encapsulation limit option."""
 
     #: Tunnel encapsulation limit.
     limit: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      limit: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class RouterAlertOption(Option):
     """Data model for IPv6-Opts router alter option."""
 
     #: Router alter value.
     value: 'RouterAlert'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      value: 'RouterAlert') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class CALIPSOOption(Option):
     """Data model for IPv6-Opts Common Architecture Label IPv6 Security Option (CALIPSO) option."""
 
     #: CALIPSO domain of interpretation.
     domain: 'int'
     #: Compartment length.
     cmpt_len: 'int'
@@ -127,14 +134,15 @@
 class SMFDPDOption(Option):
     """Data model for IPv6-Opts Simplified Multicast Forwarding Duplicate Packet Detection (``SMF_DPD``) option."""
 
     #: DPD type.
     dpd_type: 'SMFDPDMode'
 
 
+@info_final
 class SMFIdentificationBasedDPDOption(SMFDPDOption):
     """Data model for IPv6-Opts **I-DPD** (Identification-Based DPD) option."""
 
     #: TaggerID type.
     tid_type: 'TaggerID'
     #: TaggerID length.
     tid_len: 'int'
@@ -144,25 +152,27 @@
     id: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', dpd_type: 'SMFDPDMode', tid_type: 'TaggerID', tid_len: 'int',
                      tid: 'Optional[bytes | IPv4Address | IPv6Address]', id: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class SMFHashBasedDPDOption(SMFDPDOption):
     """Data model for IPv6-Opts **H-DPD** (Hash-Based DPD) option."""
 
     #: Hash assist value.
     hav: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', dpd_type: 'SMFDPDMode',
                      hav: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class PDMOption(Option):
     """Data model for IPv6-Opts Performance Diagnostic Metrics (PDM) option."""
 
     #: Scale delta time last received.
     scaledtlr: 'int'
     #: Scale delta time last sent.
     scaledtls: 'int'
@@ -185,38 +195,41 @@
 
     #: QS function.
     func: 'QSFunction'
     #: Rate request/report.
     rate: 'int'
 
 
+@info_final
 class QuickStartRequestOption(QuickStartOption):
     """Data model for IPv6-Opts Quick Start request option."""
 
     #: TTL.
     ttl: 'timedelta'
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', func: 'QSFunction', rate: 'int', ttl: 'timedelta',
                      nonce: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class QuickStartReportOption(QuickStartOption):
     """Data model for IPv6-Opts Quick Start report of approved rate option."""
 
     #: Nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', func: 'QSFunction', rate: 'int', nonce: 'int') -> 'None':
             ...
 
 
+@info_final
 class RPLFlags(Data):
     """Data model for IPv6-Opts RPL option flags fields."""
 
     #: Down flag.
     down: 'bool'
     #: Rank error flag.
     rank_err: 'bool'
@@ -224,14 +237,15 @@
     fwd_err: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, down: 'bool', rank_err: 'bool',
                      fwd_err: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class RPLOption(Option):
     """Data model for IPv6-Opts Routing Protocol for Low-Power and Lossy Networks (RPL) option."""
 
     #: Flags.
     flags: 'RPLFlags'
     #: RPL instance ID.
     id: 'int'
@@ -239,26 +253,28 @@
     rank: ' int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', flags: 'RPLFlags', id: 'int',
                      rank: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class MPLFlags(Data):
     """Data model for IPv6-Opts MPL option flags fields."""
 
     #: Max flag.
     max: 'bool'
     #: Non-conformation flag.
     drop: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, max: 'bool', drop: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class MPLOption(Option):
     """Data model for IPv6-Opts Multicast Protocol for Low-Power and Lossy Networks (MPL) option."""
 
     #: Seed length.
     seed_type: 'SeedID'
     #: Flags.
     flags: 'MPLFlags'
@@ -268,72 +284,78 @@
     seed_id: 'Optional[int]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', seed_type: 'int', flags: 'MPLFlags', seq: 'int',
                      seed_id: 'Optional[int]') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class ILNPOption(Option):
     """Data model for IPv6-Opts Identifier-Locator Network Protocol (ILNP) Nonce option."""
 
     #: Nonce value.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      nonce: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class LineIdentificationOption(Option):
     """Data model for IPv6-Opts Line-Identification option."""
 
     #: Line ID length.
     line_id_len: 'int'
     #: Line ID.
     line_id: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int', line_id_len: 'int',
                      line_id: 'bytes') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class JumboPayloadOption(Option):
     """Data model for Jumbo Payload option."""
 
     #: Jumbo payload length.
     jumbo_len: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      jumbo_len: 'int') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class HomeAddressOption(Option):
     """Data model for IPv6-Opts Home Address option."""
 
     #: Home address.
     address: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', action: 'int', change: 'bool', length: 'int',
                      address: 'IPv6Address') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class DFFFlags(Data):
     """Data model for IPv6-Opts ``IP_DFF`` option flags."""
 
     #: Duplicate flag.
     dup: 'bool'
     #: Return flag.
     ret: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, dup: 'bool', ret: 'bool') -> 'None': ...  # pylint: disable=super-init-not-called,unused-argument,redefined-builtin,multiple-statements,line-too-long
 
 
+@info_final
 class IPDFFOption(Option):
     """Data model for IPv6-Opts Depth-First Forwarding (``IP_DFF``) option."""
 
     #: Version.
     version: 'int'
     # :Flags.
     flags: 'DFFFlags'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_route.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipv6_route.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for IPv6 Routing Header"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from ipaddress import IPv6Address
 
     from pcapkit.const.ipv6.routing import Routing
     from pcapkit.const.reg.transtype import TransType
@@ -27,47 +28,51 @@
     length: 'int'
     #: Routing type.
     type: 'Routing'
     #: Segments left.
     seg_left: 'int'
 
 
+@info_final
 class UnknownType(IPv6_Route):
     """Data model for IPv6-Route unknown type."""
 
     #: Data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, next: 'TransType', length: 'int', type: 'Routing', seg_left: 'int',
                      data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,super-init-not-called,redefined-builtin,line-too-long
 
 
+@info_final
 class SourceRoute(IPv6_Route):
     """Data model for IPv6-Route Source Route data type."""
 
     #: Source addresses.
     ip: 'tuple[IPv6Address, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, next: 'TransType', length: 'int', type: 'Routing', seg_left: 'int',
                      ip: 'tuple[IPv6Address, ...]') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,super-init-not-called,redefined-builtin,line-too-long
 
 
+@info_final
 class Type2(IPv6_Route):
     """Data model for IPv6-Route Type 2 data type."""
 
     #: Address.
     ip: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, next: 'TransType', length: 'int', type: 'Routing', seg_left: 'int',
                      ip: 'IPv6Address') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,super-init-not-called,redefined-builtin,line-too-long
 
 
+@info_final
 class RPL(IPv6_Route):
     """Data model for RPL Source data type."""
 
     #: CmprI.
     cmpr_i: 'int'
     #: CmprE.
     cmpr_e: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipx.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/internet/ipx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 """data model for internetwork packet exchange"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from pcapkit.const.ipx.packet import Packet
     from pcapkit.const.ipx.socket import Socket
 
 __all__ = [
     'IPX',
 
     'Address',
 ]
 
 
+@info_final
 class Address(Data):
     """Data model for IPX address."""
 
     #: Network number (``:`` separated).
     network: 'str'
     #: Node number (``-`` separated).
     node: 'str'
@@ -28,14 +30,15 @@
     #: Full address (``:`` separated).
     addr: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, network: 'str', node: 'str', socket: 'Socket', addr: 'str') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
 
 
+@info_final
 class IPX(Data):
     """Data model for Internetwork Packet Exchange."""
 
     #: Checksum.
     chksum: 'bytes'
     #: Packet length (header includes).
     len: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/mh.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/protocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # -*- coding: utf-8 -*-
-"""data model for MH protocol"""
+"""data models for root protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
-if TYPE_CHECKING:
-    from pcapkit.const.mh.packet import Packet
-    from pcapkit.const.reg.transtype import TransType
-
-__all__ = ['MH']
-
-
-class MH(Data):
-    """Data model for MH protocol."""
-
-    #: Next header.
-    next: 'TransType'
-    #: Header length.
-    length: 'int'
-    #: Mobility header type.
-    type: 'Packet'
-    #: Checksum.
-    chksum: 'bytes'
-    #: Message data.
-    data: 'bytes'
+__all__ = [
+    'Packet',
+]
+
+
+@info_final
+class Packet(Data):
+    """Header and payload data."""
+
+    #: packet header
+    header: 'bytes'
+    #: packet payload
+    payload: 'bytes'
 
     if TYPE_CHECKING:
-        def __init__(self, next: 'TransType', length: 'int', type: 'Packet', chksum: 'bytes', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,redefined-builtin,line-too-long
+        def __init__(self, header: 'bytes', payload: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/arp.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/arp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 # -*- coding: utf-8 -*-
 """data models for address resolution protocol family"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address, IPv6Address
 
     from pcapkit.const.arp.hardware import Hardware
     from pcapkit.const.arp.operation import Operation
     from pcapkit.const.reg.ethertype import EtherType
 
 __all__ = ['Address', 'Type', 'ARP']
 
 
+@info_final
 class Address(Data):
     """Data model for ARP addresses."""
 
     #: Hardware address.
     hardware: 'str'
     #: Protocol address.
     protocol: 'str | IPv4Address | IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, hardware: 'str', protocol: 'str | IPv4Address | IPv6Address') -> 'None': ...  # pylint: disable=line-too-long,super-init-not-called,unused-argument,multiple-statements
 
 
+@info_final
 class Type(Data):
     """Data model for ARP type."""
 
     #: Hardware type.
     hardware: 'Hardware'
     #: Protocol type.
     protocol: 'EtherType | str'
 
     if TYPE_CHECKING:
         def __init__(self, hardware: 'Hardware', protocol: 'EtherType | str') -> 'None': ...  # pylint: disable=line-too-long,super-init-not-called,unused-argument,multiple-statements
 
 
+@info_final
 class ARP(Data):
     """Data model for ARP packet."""
 
     #: Hardware type.
     htype: 'Hardware'
     #: Protocol type.
     ptype: 'EtherType'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ethernet.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/ethernet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """data models for ethernet protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from pcapkit.const.reg.ethertype import EtherType
 
 __all__ = ['Ethernet']
 
 
+@info_final
 class Ethernet(Data):
     """Data model for ethernet packet."""
 
     #: Destination MAC address.
     dst: 'str'
     #: Source MAC address.
     src: 'str'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/l2tp.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/l2tp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 """data models for L2TP protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from pcapkit.const.l2tp.type import Type
 
 __all__ = ['L2TP']
 
 
+@info_final
 class Flags(Data):
     """Data model for L2TP flags and version info."""
 
     #: Type.
     type: 'Type'
     #: Length.
     len: 'bool'
@@ -26,14 +28,16 @@
     offset: 'bool'
     #: Priority.
     prio: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Type', len: 'bool', seq: 'bool', offset: 'bool', prio: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,redefined-builtin,multiple-statements
 
+
+@info_final
 class L2TP(Data):
     """Data model for L2TP packet."""
 
     #: Flags and version info.
     flags: 'Flags'
     #: Version.
     version: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ospf.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/ospf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*-
 """data models for OSPF protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address
 
     from pcapkit.const.ospf.authentication import Authentication
     from pcapkit.const.ospf.packet import Packet
 
 __all__ = ['OSPF', 'CrytographicAuthentication']
 
 
+@info_final
 class CrytographicAuthentication(Data):
     """Data model for OSPF crytographic authentication."""
 
     #: Key ID.
     key_id: 'int'
     #: Authentication data length.
     len: 'int'
     #: Cryptographic sequence number.
     seq: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, key_id: 'int', len: 'int', seq: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,redefined-builtin
 
 
+@info_final
 class OSPF(Data):
     """Data model for OSPF packet."""
 
     #: Version number.
     version: 'int'
     #: Type.
     type: 'Packet'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/vlan.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/link/vlan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # -*- coding: utf-8 -*-
 """data models for 802.1Q customer VLAN tag type"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from pcapkit.const.reg.ethertype import EtherType
     from pcapkit.const.vlan.priority_level import PriorityLevel
 
 __all__ = ['VLAN', 'TCI']
 
 
+@info_final
 class TCI(Data):
     """Data model for tag control information."""
 
     #: Priority code point.
     pcp: 'PriorityLevel'
     #: Drop eligible indicator.
     dei: 'bool'
     #: VLAN identifier.
     vid: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, pcp: 'PriorityLevel', dei: 'bool', vid: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
 
 
+@info_final
 class VLAN(Data):
     """Data model for 802.1Q customer VLAN tag type."""
 
     #: Tag control information.
     tci: 'TCI'
     #: Protocol (Internet Layer).
     type: 'EtherType'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/frame.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/frame.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 """data models for frame header of PCAP file"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import datetime
     from decimal import Decimal
 
 __all__ = ['Frame', 'FrameInfo']
 
 
+@info_final
 class FrameInfo(Data):
     """Frame metadata information."""
 
     #: Timestamp seconds.
     ts_sec: 'int'
     #: Timestamp microseconds.
     ts_usec: 'int'
@@ -24,14 +26,15 @@
     #: Actual length of packet.
     orig_len: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, ts_sec: 'int', ts_usec: 'int', incl_len: 'int', orig_len: 'int') -> 'None': ...  # pylint: disable=unused-argument,multiple-statements,super-init-not-called
 
 
+@info_final
 class Frame(Data):
     """Frame header of PCAP file."""
 
     #: Metadata information.
     frame_info: 'FrameInfo'
     #: Timestamp instance.
     time: 'datetime'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/header.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcap/header.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*-
 """data models for global header of PCAP file"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
     from pcapkit.const.reg.linktype import LinkType
     from pcapkit.corekit.version import VersionInfo
 
 __all__ = ['Header', 'MagicNumber']
 
 
+@info_final
 class MagicNumber(Data):
     """Magic number of PCAP file."""
 
     #: Magic number sequence.
     data: 'bytes'
     #: Byte order.
     byteorder: 'Literal["big", "little"]'
     #: Nanosecond-timestamp resolution flag.
     nanosecond: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes', byteorder: 'Literal["big", "little"]', nanosecond: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
 
 
+@info_final
 class Header(Data):
     """Global header of PCAP file."""
 
     #: Magic number.
     magic_number: 'MagicNumber'
     #: Version number.
     version: 'VersionInfo'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcapng.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/pcapng.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """data models for PCAP-NG file format"""
 
 import datetime
 import decimal
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.corekit.multidict import MultiDict
 from pcapkit.protocols.data.data import Data
 
 __all__ = [
     'PCAPNG',
 
     'Option', 'UnknownOption',
@@ -62,14 +63,15 @@
 
     #: Block type.
     type: 'Enum_BlockType'
     #: Block total length.
     length: 'int'
 
 
+@info_final
 class UnknownBlock(PCAPNG):
     """Data model for unknown PCAP-NG file blocks."""
 
     #: Block body.
     body: 'bytes'
 
     if TYPE_CHECKING:
@@ -81,53 +83,58 @@
 
     #: Option type.
     type: 'Enum_OptionType'
     #: Option data length.
     length: 'int'
 
 
+@info_final
 class UnknownOption(Option):
     """Data model for unknown PCAP-NG file options."""
 
     #: Option data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', data: 'bytes') -> None: ...
 
 
+@info_final
 class EndOfOption(Option):
     """Data model for PCAP-NG file ``opt_endofopt`` options."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int') -> None: ...
 
 
+@info_final
 class CommentOption(Option):
     """Data model for PCAP-NG file ``opt_comment`` options."""
 
     #: Comment text.
     comment: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', comment: 'str') -> None: ...
 
 
+@info_final
 class CustomOption(Option):
     """Data model for PCAP-NG file ``opt_custom`` options."""
 
     #: Private enterprise number (PEN).
     pen: 'int'
     #: Custom data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', pen: 'int', data: 'bytes') -> None: ...
 
 
+@info_final
 class SectionHeaderBlock(PCAPNG):
     """Data model for PCAP-NG Section Header Block (SHB)."""
 
     #: Byte order.
     byteorder: 'Literal["big", "little"]'
     #: Version number.
     version: 'VersionInfo'
@@ -137,173 +144,190 @@
     options: 'OrderedMultiDict[Enum_OptionType, Option]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', byteorder: 'Literal["big", "little"]', version: 'VersionInfo',  # pylint: disable=unused-argument
                      section_length: 'int', options: 'OrderedMultiDict[Enum_OptionType, Option]') -> None: ...
 
 
+@info_final
 class IF_NameOption(Option):
     """Data model for PCAP-NG file ``if_name`` options."""
 
     #: Interface name.
     name: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', name: 'str') -> None: ...
 
 
+@info_final
 class IF_DescriptionOption(Option):
     """Data model for PCAP-NG file ``if_description`` options."""
 
     #: Interface description.
     description: 'str'
 
 
+@info_final
 class IF_IPv4AddrOption(Option):
     """Data model for PCAP-NG file ``if_IPv4addr`` options."""
 
     #: IPv4 interface.
     interface: 'IPv4Interface'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'IPv4Interface') -> None: ...
 
 
+@info_final
 class IF_IPv6AddrOption(Option):
     """Data model for PCAP-NG file ``if_IPv6addr`` options."""
 
     #: IPv6 interface.
     interface: 'IPv6Interface'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'IPv6Interface') -> None: ...
 
 
+@info_final
 class IF_MACAddrOption(Option):
     """Data model for PCAP-NG file ``if_MACaddr`` options."""
 
     #: MAC address.
     interface: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'str') -> None: ...
 
 
+@info_final
 class IF_EUIAddrOption(Option):
     """Data model for PCAP-NG file ``if_EUIaddr`` options."""
 
     #: EUI address.
     interface: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'str') -> None: ...
 
 
+@info_final
 class IF_SpeedOption(Option):
     """Data model for PCAP-NG file ``if_speed`` options."""
 
     #: Interface speed, in bits per second.
     speed: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', speed: 'int') -> None: ...
 
 
+@info_final
 class IF_TSResolOption(Option):
     """Data model for PCAP-NG file ``if_tsresol`` options."""
 
     #: Time stamp resolution, in units per second.
     resolution: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', resolution: 'int') -> None: ...
 
 
+@info_final
 class IF_TZoneOption(Option):
     """Data model for PCAP-NG file ``if_tzone`` options."""
 
     #: Time zone.
     timezone: 'dt_timezone'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', timezone: 'dt_timezone') -> None: ...
 
 
+@info_final
 class IF_FilterOption(Option):
     """Data model for PCAP-NG file ``if_filter`` options."""
 
     #: Filter code.
     code: 'Enum_FilterType'
     #: Filter expression.
     expression: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', code: 'Enum_FilterType', expression: 'bytes') -> None: ...
 
 
+@info_final
 class IF_OSOption(Option):
     """Data model for PCAP-NG file ``if_os`` options."""
 
     #: Operating system.
     os: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', os: 'str') -> None: ...
 
 
+@info_final
 class IF_FCSLenOption(Option):
     """Data model for PCAP-NG file ``if_fcslen`` options."""
 
     #: FCS length.
     fcs_length: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', fcs_length: 'int') -> None: ...
 
 
+@info_final
 class IF_TSOffsetOption(Option):
     """Data model for PCAP-NG file ``if_tsoffset`` options."""
 
     #: Timestamp offset (in seconds).
     offset: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', offset: 'int') -> None: ...
 
 
+@info_final
 class IF_HardwareOption(Option):
     """Data model for PCAP-NG file ``if_hardware`` options."""
 
     #: Hardware information.
     hardware: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', hardware: 'str') -> None: ...
 
 
+@info_final
 class IF_TxSpeedOption(Option):
     """Data model for PCAP-NG file ``if_txspeed`` options."""
 
     #: Interface transmit speed (in bits per second).
     speed: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', speed: 'int') -> None: ...
 
 
+@info_final
 class IF_RxSpeedOption(Option):
     """Data model for PCAP-NG file ``if_rxspeed`` options."""
 
     #: Interface receive speed (in bits per second).
     speed: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', speed: 'int') -> None: ...
 
 
+@info_final
 class InterfaceDescriptionBlock(PCAPNG):
     """Data model for PCAP-NG Interface Description Block (IDB)."""
 
     #: Link type.
     linktype: 'Enum_LinkType'
     #: Snap length.
     snaplen: 'int'
@@ -311,14 +335,15 @@
     options: 'OrderedMultiDict[Enum_OptionType, Option]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', linktype: 'Enum_LinkType',
                      snaplen: 'int', options: 'OrderedMultiDict[Enum_OptionType, Option]') -> None: ...
 
 
+@info_final
 class EPB_FlagsOption(Option):
     """Data model for PCAP-NG file ``epb_flags`` options."""
 
     #: Inbound / Outbound packet.
     direction: 'PacketDirection'
     #: Reception type.
     reception: 'PacketReception'
@@ -344,68 +369,74 @@
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', direction: 'PacketDirection',
                      reception: 'PacketReception', fcs_len: 'int', crc_error: 'bool',
                      too_long: 'bool', too_short: 'bool', gap_error: 'bool', unaligned_error: 'bool',
                      delimiter_error: 'bool', preamble_error: 'bool', symbol_error: 'bool') -> 'None': ...
 
 
+@info_final
 class EPB_HashOption(Option):
     """Data model for PCAP-NG ``epb_hash`` options."""
 
     #: Hash algorithm.
     algorithm: 'Enum_HashAlgorithm'
     #: Hash value.
     hash: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', algorithm: 'Enum_HashAlgorithm', hash: 'bytes') -> 'None': ...
 
 
+@info_final
 class EPB_DropCountOption(Option):
     """Data model for PCAP-NG ``epb_dropcount`` options."""
 
     #: Number of packets dropped by the interface.
     drop_count: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', drop_count: 'int') -> 'None': ...
 
 
+@info_final
 class EPB_PacketIDOption(Option):
     """Data model for PCAP-NG ``epb_packetid`` options."""
 
     #: Packet ID.
     packet_id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packet_id: 'int') -> 'None': ...
 
 
+@info_final
 class EPB_QueueOption(Option):
     """Data model for PCAP-NG ``epb_queue`` options."""
 
     #: Queue ID.
     queue_id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', queue_id: 'int') -> 'None': ...
 
 
+@info_final
 class EPB_VerdictOption(Option):
     """Data model for PCAP-NG ``epb_verdict`` options."""
 
     #: Verdict type.
     verdict: 'Enum_VerdictType'
     #: Verdict value.
     value: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', verdict: 'Enum_VerdictType', value: 'bytes') -> 'None': ...
 
 
+@info_final
 class EnhancedPacketBlock(PCAPNG):
     """Data model for PCAP-NG Enhanced Packet Block (EPB)."""
 
     #: Section index.
     section_number: 'int'
     #: Frame index.
     number: 'int'
@@ -429,14 +460,15 @@
 
         def __init__(self, type: 'Enum_BlockType', length: 'int', section_number: 'int',
                      number: 'int', interface_id: 'int', timestamp: 'dt_type',
                      timestamp_epoch: 'Decimal', captured_len: 'int', original_len: 'int',
                      options: 'OrderedMultiDict[Enum_OptionType, Option]') -> 'None': ...
 
 
+@info_final
 class SimplePacketBlock(PCAPNG):
     """Data model for PCAP-NG Simple Packet Block (SPB)."""
 
     #: Section index.
     section_number: 'int'
     #: Frame index.
     number: 'int'
@@ -475,87 +507,95 @@
 
     #: Record type.
     type: 'Enum_RecordType'
     #: Record value length.
     length: 'int'
 
 
+@info_final
 class UnknownRecord(NameResolutionRecord):
     """Data model for PCAP-NG NRB unknown records."""
 
     #: Unknown record value.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@info_final
 class EndRecord(NameResolutionRecord):
     """Data model for PCAP-NG ``nrb_record_end`` records."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int') -> 'None': ...
 
 
+@info_final
 class IPv4Record(NameResolutionRecord):
     """Data model for PCAP-NG ``nrb_record_ipv4`` records."""
 
     #: IPv4 address.
     ip: 'IPv4Address'
     #: Name resolution data.
     records: 'tuple[str, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int', ip: 'IPv4Address',
                      records: 'tuple[str, ...]') -> 'None': ...
 
 
+@info_final
 class IPv6Record(NameResolutionRecord):
     """Data model for PCAP-NG ``nrb_record_ipv6`` records."""
 
     #: IPv6 address.
     ip: 'IPv6Address'
     #: Name resolution data.
     records: 'tuple[str, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int', ip: 'IPv6Address',
                      records: 'tuple[str, ...]') -> 'None': ...
 
 
+@info_final
 class NS_DNSNameOption(Option):
     """Data model for PCAP-NG ``ns_dnsname`` option."""
 
     #: DNS name.
     name: 'str'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', name: 'str') -> 'None': ...
 
 
+@info_final
 class NS_DNSIP4AddrOption(Option):
     """Data model for PCAP-NG ``ns_dnsip4addr`` option."""
 
     #: IPv4 address.
     ip: 'IPv4Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', ip: 'IPv4Address') -> 'None': ...
 
 
+@info_final
 class NS_DNSIP6AddrOption(Option):
     """Data model for PCAP-NG ``ns_dnsip6addr`` option."""
 
     #: IPv6 address.
     ip: 'IPv6Address'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', ip: 'IPv6Address') -> 'None': ...
 
 
+@info_final
 class NameResolutionBlock(PCAPNG):
     """Data model for PCAP-NG Name Resolution Block (NRB)."""
 
     #: Records.
     records: 'OrderedMultiDict[Enum_RecordType, NameResolutionRecord]'
     #: Options.
     options: 'OrderedMultiDict[Enum_OptionType, Option]'
@@ -582,90 +622,98 @@
         #: Name resolution mapping (name -> IP address).
         reverse_mapping: 'MultiDict[str, IPv4Address | IPv6Address]'
 
         def __init__(self, type: 'Enum_BlockType', length: 'int', records: 'OrderedMultiDict[Enum_RecordType, NameResolutionRecord]',
                      options: 'OrderedMultiDict[Enum_OptionType, Option]') -> 'None': ...
 
 
+@info_final
 class ISB_StartTimeOption(Option):
     """Data model for PCAP-NG ``isb_starttime`` option."""
 
     #: Start time.
     timestamp: 'dt_type'
     #: Start time as in UNIX epoch (in seconds).
     timestamp_epoch: 'Decimal'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', timestamp: 'dt_type',
                      timestamp_epoch: 'Decimal') -> 'None': ...
 
 
+@info_final
 class ISB_EndTimeOption(Option):
     """Data model for PCAP-NG ``isb_endtime`` option."""
 
     #: End time.
     timestamp: 'dt_type'
     #: End time as in UNIX epoch (in seconds).
     timestamp_epoch: 'Decimal'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', timestamp: 'dt_type',
                      timestamp_epoch: 'Decimal') -> 'None': ...
 
 
+@info_final
 class ISB_IFRecvOption(Option):
     """Data model for PCAP-NG ``isb_ifrecv`` option."""
 
     #: Number of packets received.
     packets: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@info_final
 class ISB_IFDropOption(Option):
     """Data model for PCAP-NG ``isb_ifdrop`` option."""
 
     #: Number of packets dropped.
     packets: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@info_final
 class ISB_FilterAcceptOption(Option):
     """Data model for PCAP-NG ``isb_filteraccept`` option."""
 
     #: Number of packets accepted by the filter.
     packets: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@info_final
 class ISB_OSDropOption(Option):
     """Data model for PCAP-NG ``isb_osdrop`` option."""
 
     #: Number of packets dropped by the operating system.
     packets: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@info_final
 class ISB_UsrDelivOption(Option):
     """Data model for PCAP-NG ``isb_usrdeliv`` option."""
 
     #: Number of packets delivered to the user.
     packets: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@info_final
 class InterfaceStatisticsBlock(PCAPNG):
     """Data model for PCAP-NG Interface Statistics Block (ISB)."""
 
     #: Interface ID.
     interface_id: 'int'
     #: Timestamp.
     timestamp: 'dt_type'
@@ -675,84 +723,91 @@
     options: 'OrderedMultiDict[Enum_OptionType, Option]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', interface_id: 'int', timestamp: 'dt_type',
                      timestamp_epoch: 'Decimal', options: 'OrderedMultiDict[Enum_OptionType, Option]') -> 'None': ...
 
 
+@info_final
 class SystemdJournalExportBlock(PCAPNG):
     """Data model for PCAP-NG :manpage:`systemd(1)` Journal Export Block."""
 
     #: Journal entry.
     data: 'tuple[OrderedMultiDict[str, str | bytes], ...]'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', data: 'tuple[OrderedMultiDict[str, str | bytes], ...]') -> 'None': ...
 
 
 class DSBSecrets(Data):
     """Data model for DSB secrets data."""
 
 
+@info_final
 class UnknownSecrets(DSBSecrets):
     """Data model for unknown DSB secrets."""
 
     #: Secrets data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
+@info_final
 class TLSKeyLog(DSBSecrets):
     """Data model for TLS key log DSB secrets."""
 
     #: TLS key log entries.
     entries: 'dict[TLSKeyLabel, OrderedMultiDict[bytes, bytes]]'
 
     if TYPE_CHECKING:
         def __init__(self, entries: 'dict[TLSKeyLabel, OrderedMultiDict[bytes, bytes]]') -> 'None': ...
 
 
+@info_final
 class WireGuardKeyLog(DSBSecrets):
     """Data model for WireGuard key DSB secrets."""
 
     #: WireGuard Key Log entries.
     entries: 'OrderedMultiDict[WireGuardKeyLabel, bytes]'
 
     if TYPE_CHECKING:
         def __init__(self, entries: 'OrderedMultiDict[WireGuardKeyLabel, bytes]') -> 'None': ...
 
 
+@info_final
 class ZigBeeNWKKey(DSBSecrets):
     """Data model for ZigBEE NWK Key and ZigBee PANID secrets data."""
 
     #: AES-128 NKW key.
     nwk_key: 'bytes'
     #: PAN ID.
     pan_id: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, nwk_key: 'bytes', pan_id: 'int') -> 'None': ...
 
 
+@info_final
 class ZigBeeAPSKey(DSBSecrets):
     """Data model for ZigBEE APS Key secrets data."""
 
     #: AES-128 APS key.
     aps_key: 'bytes'
     #: PAN ID.
     pan_id: 'int'
     #: Node short address.
     short_address: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, aps_key: 'bytes', pan_id: 'int', short_address: 'int') -> 'None': ...
 
 
+@info_final
 class DecryptionSecretsBlock(PCAPNG):
     """Data model for PCAP-NG Decryption Secrets Block (DSB)."""
 
     #: Secrets type.
     secrets_type: 'Enum_SecretsType'
     #: Secrets length.
     secrets_length: 'int'
@@ -763,26 +818,28 @@
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', secrets_type: 'Enum_SecretsType',
                      secrets_length: 'int', secrets_data: 'DSBSecrets',
                      options: 'OrderedMultiDict[Enum_OptionType, Option]') -> 'None': ...
 
 
+@info_final
 class CustomBlock(PCAPNG):
     """Data model for PCAP-NG Custom Block (CB)."""
 
     #: Private enterprise number.
     pen: 'int'
     #: Custom block data (incl. data, options and padding).
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_BlockType', length: 'int', pen: 'int', data: 'bytes') -> 'None': ...
 
 
+@info_final
 class PACK_FlagsOption(Option):
     """Data model for PCAP-NG file ``pack_flags`` options."""
 
     #: Inbound / Outbound packet.
     direction: 'PacketDirection'
     #: Reception type.
     reception: 'PacketReception'
@@ -808,26 +865,28 @@
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', direction: 'PacketDirection',
                      reception: 'PacketReception', fcs_len: 'int', crc_error: 'bool',
                      too_long: 'bool', too_short: 'bool', gap_error: 'bool', unaligned_error: 'bool',
                      delimiter_error: 'bool', preamble_error: 'bool', symbol_error: 'bool') -> 'None': ...
 
 
+@info_final
 class PACK_HashOption(Option):
     """Data model for PCAP-NG ``pack_hash`` options."""
 
     #: Hash algorithm.
     algorithm: 'Enum_HashAlgorithm'
     #: Hash value.
     hash: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', algorithm: 'Enum_HashAlgorithm', hash: 'bytes') -> 'None': ...
 
 
+@info_final
 class PacketBlock(PCAPNG):
     """Data model for PCAP-NG Packet Block (obsolete)."""
 
     #: Section index.
     section_number: 'int'
     #: Frame index.
     number: 'int'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/raw.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/misc/raw.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """data models for raw protocol data"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing import Optional
 
 __all__ = ['Raw']
 
 
+@info_final
 class Raw(Data):
     """Raw packet is an unknown protocol."""
 
     #: Original enumeration of this protocol.
     protocol: 'Optional[int]'
     #: packet data
     packet: 'bytes'
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/tcp.py` & `pypcapkit-1.0.1/pcapkit/protocols/data/transport/tcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """data model for TCP protocol"""
 
 from typing import TYPE_CHECKING
 
+from pcapkit.corekit.infoclass import info_final
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from ipaddress import IPv4Address, IPv6Address
     from typing import Optional, Union
 
@@ -37,14 +38,15 @@
     'MPTCPPriority', 'MPTCPFallback', 'MPTCPFastclose',
 
     'MPTCPJoin',
     'MPTCPJoinSYN', 'MPTCPJoinSYNACK', 'MPTCPJoinACK',
 ]
 
 
+@info_final
 class Flags(Data):
     """Data model for TCP flags."""
 
     #: ECN-nonce concealment protection.
     ns: 'bool'
     #: Congestion window reduced.
     cwr: 'bool'
@@ -63,14 +65,15 @@
     #: Last packet from sender.
     fin: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, ns: 'bool', cwr: 'bool', ece: 'bool', urg: 'bool', ack: 'bool', psh: 'bool', rst: 'bool', syn: 'bool', fin: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class TCP(Data):
     """Data model for TCP packet."""
 
     #: Source port.
     srcport: 'int'
     #: Destination port.
     dstport: 'int'
@@ -103,236 +106,259 @@
 
     #: Option kind.
     kind: 'OptionNumber'
     #: Option length.
     length: 'int'
 
 
+@info_final
 class UnassignedOption(Option):
     """Data model for unassigned TCP option."""
 
     #: Option data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class EndOfOptionList(Option):
     """Data model for TCP end of option list option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class NoOperation(Option):
     """Data model for TCP no operation option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MaximumSegmentSize(Option):
     """Data model for TCP maximum segment size option."""
 
     #: Maximum segment size.
     mss: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', mss: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class WindowScale(Option):
     """Data model for TCP window scale option."""
 
     #: Window scale.
     shift: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', shift: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SACKPermitted(Option):
     """Data model for TCP SACK permitted option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SACKBlock(Data):
     """Data model for TCP SACK block."""
 
     #: Left edge.
     left: 'int'
     #: Right edge.
     right: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, left: 'int', right: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class SACK(Option):
     """Data model for TCP SACK option."""
 
     #: SACK blocks.
     sack: 'tuple[SACKBlock, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', sack: 'tuple[SACKBlock, ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Echo(Option):
     """Data model for TCP echo option."""
 
     #: Echo data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class EchoReply(Option):
     """Data model for TCP echo reply option."""
 
     #: Echo data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Timestamp(Option):
     """Data model for TCP timestamp option."""
 
     #: Timestamp .
     timestamp: 'int'
     #: Echo data.
     echo: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', timestamp: 'int', echo: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PartialOrderConnectionPermitted(Option):
     """Data model for TCP partial order connection permitted option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class PartialOrderConnectionProfile(Option):
     """Data model for TCP partial order connection profile option."""
 
     #: Start flag.
     start: 'bool'
     #: End flag.
     end: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', start: 'bool', end: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class CC(Option):
     """Data model for TCP CC option."""
 
     #: Connection count.
     cc: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', cc: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class CCNew(Option):
     """Data model for TCP CC.NEW option."""
 
     #: Connection count.
     cc: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', cc: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class CCEcho(Option):
     """Data model for TCP CC.ECHO option."""
 
     #: Connection count.
     cc: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', cc: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class AlternateChecksumRequest(Option):
     """Data model for TCP alternate checksum request option."""
 
     #: Checksum algorithm.
     chksum: 'Checksum'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', chksum: 'Checksum') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class AlternateChecksumData(Option):
     """Data model for TCP alternate checksum data option."""
 
     #: Checksum data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MD5Signature(Option):
     """Data model for TCP MD5 signature option."""
 
     #: MD5 signature.
     digest: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', digest: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class QuickStartResponse(Option):
     """Data model for TCP quick start response option."""
 
     #: Rate request.
     req_rate: 'int'
     #: TTL difference.
     ttl_diff: 'int'
     #: QS nonce.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', req_rate: 'int', ttl_diff: 'int', nonce: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class UserTimeout(Option):
     """Data model for TCP user timeout option."""
 
     #: User timeout.
     timeout: 'timedelta'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', timeout: 'timedelta') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class Authentication(Option):
     """Data model for TCP authentication option."""
 
     #: Key ID.
     key_id: 'int'
     #: Receive next key ID.
     next_key_id: 'int'
     #: MAC.
     mac: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', key_id: 'int', next_key_id: 'int', mac: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class FastOpenCookie(Option):
     """Data model for TCP fast open cookie option."""
 
     #: Cookie.
     cookie: 'bytes'
 
     if TYPE_CHECKING:
@@ -342,38 +368,41 @@
 class MPTCP(Option):
     """Data model for TCP MPTCP option."""
 
     #: Subtype.
     subtype: 'MPTCPOption'
 
 
+@info_final
 class MPTCPUnknown(MPTCP):
     """Data model for TCP unknown MPTCP option."""
 
     #: Data.
     data: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', data: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPCapableFlag(Data):
     """Data model for TCP MPTCP capable option flags."""
 
     #: Checksum require flag.
     req: 'bool'
     #: Extensibility flag.
     ext: 'bool'
     #: HMAC-SHA1 flag.
     hsa: 'bool'
 
     if TYPE_CHECKING:
         def __init__(self, req: 'bool', ext: 'bool', hsa: 'bool') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPCapable(MPTCP):
     """Data model for TCP ``MP_CAPABLE`` option."""
 
     #: Version.
     version: 'int'
     #: Flags.
     flags: 'MPTCPCapableFlag'
@@ -389,14 +418,15 @@
 class MPTCPJoin(MPTCP):
     """Data model for TCP ``MP_JOIN`` option."""
 
     #: Connection type.
     connection: 'TCP_Flags'
 
 
+@info_final
 class MPTCPJoinSYN(MPTCPJoin):
     """Data model for TCP ``MP_JOIN-SYN`` option."""
 
     #: Backup path flag.
     backup: 'bool'
     #: Address ID.
     addr_id: 'int'
@@ -405,14 +435,15 @@
     #: Sendder's random number.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', connection: 'TCP_Flags', backup: 'bool', addr_id: 'int', token: 'int', nonce: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPJoinSYNACK(MPTCPJoin):
     """Data model for TCP ``MP_JOIN-SYNACK`` option."""
 
     #: Backup path flag.
     backup: 'bool'
     #: Address ID.
     addr_id: 'int'
@@ -421,24 +452,26 @@
     #: Sendder's random number.
     nonce: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', connection: 'TCP_Flags', backup: 'bool', addr_id: 'int', hmac: 'bytes', nonce: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPJoinACK(MPTCPJoin):
     """Data model for TCP ``MP_JOIN-ACK`` option."""
 
     #: HMAC value.
     hmac: 'bytes'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', connection: 'TCP_Flags', hmac: 'bytes') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPDSS(MPTCP):
     """Data model for TCP ``DSS`` option."""
 
     #: ``DATA_FIN`` flag.
     data_fin: 'bool'
     #: Data ACK.
     ack: 'Optional[int]'
@@ -451,14 +484,15 @@
     #: Checksum.
     checksum: 'Optional[bytes]'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', data_fin: 'bool', ack: 'Optional[int]', dsn: 'Optional[int]', ssn: 'Optional[int]', dl_len: 'Optional[int]', checksum: 'Optional[bytes]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPAddAddress(MPTCP):
     """Data model for TCP ``ADD_ADDR`` option."""
 
     #: IP version.
     version: 'int'
     #: Address ID.
     addr_id: 'int'
@@ -467,46 +501,50 @@
     #: Port number.
     port: 'Optional[int]'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', version: 'int', addr_id: 'int', addr: 'IPAddress', port: 'Optional[int]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPRemoveAddress(MPTCP):
     """Data model for TCP ``REMOVE_ADDR`` option."""
 
     #: Address ID.
     addr_id: 'tuple[int, ...]'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', addr_id: 'tuple[int, ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPPriority(MPTCP):
     """Data model for TCP ``MP_PRIO`` option."""
 
     #: Backup path flag.
     backup: 'bool'
     #: Address ID.
     addr_id: 'Optional[int]'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', backup: 'bool', addr_id: 'Optional[int]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPFallback(MPTCP):
     """Data model for TCP ``MP_FAIL`` option."""
 
     #: Data sequence number.
     dsn: 'int'
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'OptionNumber', length: 'int', subtype: 'MPTCPOption', dsn: 'int') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long,redefined-builtin
 
 
+@info_final
 class MPTCPFastclose(MPTCP):
     """Data model for TCP ``MP_FASTCLOSE`` option."""
 
     #: Option receiver's key.
     rkey: 'int'
 
     if TYPE_CHECKING:
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/esp.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/NotImplemented/esp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ah.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ah.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hip.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/hip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hopopt.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/hopopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     ##########################################################################
     # Defaults.
     ##########################################################################
 
     #: DefaultDict[Enum_Option, str | tuple[OptionParser, OptionConstructor]]:
     #: Option code to method mapping, c.f. :meth:`_read_hopopt_options` and/or
     #: :meth:`_make_hopopt_options`. Method names are expected to be referred
-    #: to the class by ``_read_opt_${name}`` and/or ``_make_opt_${name}, and
+    #: to the class by ``_read_opt_${name}`` and/or ``_make_opt_${name}``, and
     #: if such name not found, the value should then be a method that can parse
     #: the option by itself.
     __option__ = collections.defaultdict(
         lambda: 'none',
         {
             Enum_Option.Pad1:                       'pad',      # [RFC 8200] 0
             Enum_Option.PadN:                       'pad',      # [RFC 8200]
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/internet.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/internet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ip.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipsec.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipsec.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv4.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipv4.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_frag.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_frag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_opts.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_opts.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_route.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipv6_route.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipx.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/ipx.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     ##########################################################################
     # Methods.
     ##########################################################################
 
     def read(self, length: 'Optional[int]' = None, **kwargs: 'Any') -> 'Data_IPX':
         """Read Internetwork Packet Exchange.
 
-         Args:
+        Args:
             length: Length of packet data.
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Parsed packet data.
 
         """
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/mh.py` & `pypcapkit-1.0.1/pcapkit/protocols/internet/mh.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/arp.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/arp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/ethernet.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/ethernet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/l2tp.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/l2tp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/link.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/link.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/ospf.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/ospf.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/rarp.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/rarp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/link/vlan.py` & `pypcapkit-1.0.1/pcapkit/protocols/link/vlan.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/null.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/null.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/frame.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/frame.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/header.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/pcap/header.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcapng.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/pcapng.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/raw.py` & `pypcapkit-1.0.1/pcapkit/protocols/misc/raw.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/protocol.py` & `pypcapkit-1.0.1/pcapkit/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv2.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/application/httpv2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pcapkit.const.http.error_code import ErrorCode as Enum_ErrorCode
 from pcapkit.const.http.frame import Frame as Enum_Frame
 from pcapkit.const.http.setting import Setting as Enum_Setting
 from pcapkit.corekit.fields.collections import ListField
 from pcapkit.corekit.fields.misc import ConditionalField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import EnumField, NumberField, UInt8Field, UInt32Field
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
     'HTTP',
 
     'FrameType',
     'UnassignedFrame', 'DataFrame', 'HeadersFrame', 'PriorityFrame',
@@ -97,14 +97,15 @@
     if type == Enum_Frame.WINDOW_UPDATE:
         return SchemaField(length=pkt['__length__'], schema=WindowUpdateFrame)
     if type == Enum_Frame.CONTINUATION:
         return SchemaField(length=pkt['__length__'], schema=ContinuationFrame)
     return SchemaField(length=pkt['__length__'], schema=UnassignedFrame)
 
 
+@schema_final
 class HTTP(Schema):
     """Header schema for HTTP/2 packet."""
 
     #: Length.
     length: 'int' = NumberField(length=3, signed=False)
     #: Frame type.
     type: 'Enum_Frame' = EnumField(length=1, namespace=Enum_Frame)
@@ -159,24 +160,26 @@
             if packet['flags'][name]:
                 flags |= val
 
         self.__flags__ = flags
         return self
 
 
+@schema_final
 class UnassignedFrame(FrameType):
     """Header schema for unassigned HTTP/2 frame payload."""
 
     #: Frame payload.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class DataFrame(FrameType):
     """Header schema for HTTP/2 ``DATA`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``DATA`` frames."""
 
         END_STREAM = BIT_0 = 0x1
@@ -195,14 +198,15 @@
         lambda pkt: pkt['flags']['bit_3'],  # PADDED
     )
 
     if TYPE_CHECKING:
         def __init__(self, pad_len: 'Optional[int]', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HeadersFrame(FrameType):
     """Header schema for HTTP/2 ``HEADERS`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``DATA`` frames."""
 
         END_STREAM  = BIT_0 = 0x1
@@ -238,14 +242,15 @@
         lambda pkt: pkt['flags']['bit_3'],  # PADDED
     )
 
     if TYPE_CHECKING:
         def __init__(self, pad_len: 'Optional[int]', stream_dep: 'Optional[StreamDependency]', weight: 'Optional[int]', fragment: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PriorityFrame(FrameType):
     """Header schema for HTTP/2 ``PRIORITY`` frames."""
 
     #: Stream dependency (exclusive, stream ID).
     stream: 'StreamDependency' = BitField(length=4, namespace={
         'exclusive': (0, 1),
         'sid': (1, 31),
@@ -253,36 +258,39 @@
     #: Weight.
     weight: 'int' = UInt8Field()
 
     if TYPE_CHECKING:
         def __init__(self, stream: 'StreamDependency', weight: 'int') -> 'None': ...
 
 
+@schema_final
 class RSTStreamFrame(FrameType):
     """Header schema for HTTP/2 ``RST_STREAM`` frames."""
 
     #: Error code.
     error: 'Enum_ErrorCode' = EnumField(length=4, namespace=Enum_ErrorCode)
 
     if TYPE_CHECKING:
         def __init__(self, error: 'Enum_ErrorCode') -> 'None': ...
 
 
+@schema_final
 class SettingPair(Schema):
     """Header schema for HTTP/2 ``SETTINGS`` frame setting pairs."""
 
     #: Identifier.
     id: 'Enum_Setting' = EnumField(length=2, namespace=Enum_Setting)
     #: Value.
     value: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, id: 'Enum_Setting', value: 'int') -> 'None': ...
 
 
+@schema_final
 class SettingsFrame(FrameType):
     """Header schema for HTTP/2 ``SETTINGS`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``SETTINGS`` frames."""
 
         ACK = BIT_0 = 0x1
@@ -293,14 +301,15 @@
         item_type=SettingPair,  # type: ignore[arg-type]
     )
 
     if TYPE_CHECKING:
         def __init__(self, settings: 'list[SettingPair] | bytes') -> 'None': ...
 
 
+@schema_final
 class PushPromiseFrame(FrameType):
     """Header schema for HTTP/2 ``PUSH_PROMISE`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``PUSH_PROMISE`` frames."""
 
         END_HEADERS = BIT_2 = 0x4
@@ -325,14 +334,15 @@
         lambda pkt: pkt['flags']['bit_3'],  # PADDED
     )
 
     if TYPE_CHECKING:
         def __init__(self, pad_len: 'Optional[int]', stream: 'StreamID', fragment: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PingFrame(FrameType):
     """Header schema for HTTP/2 ``PING`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``PING`` frames."""
 
         ACK = BIT_0 = 0x1
@@ -340,14 +350,15 @@
     #: Opaque data.
     data: 'bytes' = BytesField(length=8)
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class GoawayFrame(FrameType):
     """Header schema for HTTP/2 ``GOAWAY`` frames."""
 
     #: Last stream ID.
     stream: 'StreamID' = BitField(length=4, namespace={
         'sid': (1, 31),
     })
@@ -356,26 +367,28 @@
     #: Additional debug data.
     debug: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, stream: 'StreamID', error: 'Enum_ErrorCode', debug: 'bytes') -> 'None': ...
 
 
+@schema_final
 class WindowUpdateFrame(FrameType):
     """Header schema for HTTP/2 ``WINDOW_UPDATE`` frames."""
 
     #: Window size increment.
     size: 'WindowSize' = BitField(length=4, namespace={
         'incr': (1, 31),
     })
 
     if TYPE_CHECKING:
         def __init__(self, size: 'WindowSize') -> 'None': ...
 
 
+@schema_final
 class ContinuationFrame(FrameType):
     """Header schema for HTTP/2 ``CONTINUATION`` frames."""
 
     class Flags(FrameType.Flags):
         """Flags enumeration for HTTP/2 ``CONTINUATION`` frames."""
 
         END_HEADERS = BIT_2 = 0x4
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ah.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ah.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt32Field
 from pcapkit.corekit.fields.strings import BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['AH']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
 
+@schema_final
 class AH(Schema):
     """Header schema for AH packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Payload length.
     len: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hip.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/hip.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import ListField, OptionField
 from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import ConditionalField, PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 from pcapkit.utilities.warnings import ProtocolWarning, warn
 
 __all__ = [
     'HIP',
 
@@ -171,26 +171,28 @@
 
     #: Parameter type.
     type: 'Enum_Parameter' = EnumField(length=2, namespace=Enum_Parameter)
     #: Parameter length.
     len: 'int' = UInt16Field()
 
 
+@schema_final
 class UnassignedParameter(Parameter):
     """Header schema for HIP unsigned parameters."""
 
     #: Parameter value.
     value: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', value: 'bytes') -> 'None': ...
 
 
+@schema_final
 class ESPInfoParameter(Parameter):
     """Header schema for HIP ``ESP_INFO`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: Key management index.
     index: 'int' = UInt16Field()
@@ -202,28 +204,30 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', index: 'int',
                      old_spi: 'int', new_spi: 'int') -> 'None': ...
 
 
+@schema_final
 class R1CounterParameter(Parameter):
     """Header schema for HIP ``R1_COUNTER`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: R1 counter.
     counter: 'int' = UInt32Field()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', counter: 'int') -> 'None': ...
 
 
+@schema_final
 class Locator(Schema):
     """Header schema for HIP locators."""
 
     #: Traffic type.
     traffic: 'int' = UInt8Field()
     #: Locator type.
     type: 'int' = UInt8Field()
@@ -243,14 +247,15 @@
     )
 
     if TYPE_CHECKING:
         def __init__(self, traffic: 'int', type: 'int', len: 'int', flags: 'LocatorFlags',
                      lifetime: 'int', value: 'bytes | LocatorData') -> 'None': ...
 
 
+@schema_final
 class LocatorSetParameter(Parameter):
     """Header schema for HIP ``LOCATOR_SET`` parameters."""
 
     #: List of locators.
     locators: 'list[Locator]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=SchemaField(schema=Locator),
@@ -258,26 +263,28 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', locators: 'list[Locator]') -> 'None': ...
 
 
+@schema_final
 class LocatorData(Schema):
     """Header schema for HIP locator data."""
 
     #: SPI.
     spi: 'int' = UInt32Field()
     #: Locator.
     ip: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, spi: 'int', ip: 'IPv6Address | int | bytes | str') -> 'None': ...
 
 
+@schema_final
 class PuzzleParameter(Parameter):
     """Header schema for HIP ``PUZZLE`` parameters."""
 
     #: Numeric index.
     index: 'int' = UInt8Field()
     #: Lifetime.
     lifetime: 'int' = UInt8Field()
@@ -289,14 +296,15 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', index: 'int', lifetime: 'int',
                      opaque: 'bytes', random: 'int') -> 'None': ...
 
 
+@schema_final
 class SolutionParameter(Parameter):
     """Header schema for HIP ``SOLUTION`` parameters."""
 
     #: Numeric index.
     index: 'int' = UInt8Field()
     #: Lifetime.
     lifetime: 'int' = UInt8Field()
@@ -310,26 +318,28 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', index: 'int', lifetime: 'int',
                      opaque: 'bytes', random: 'int', solution: 'int') -> 'None': ...
 
 
+@schema_final
 class SEQParameter(Parameter):
     """Header schema for HIP ``SEQ`` parameters."""
 
     #: Update ID.
     update_id: 'int' = UInt32Field()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', update_id: 'int') -> 'None': ...
 
 
+@schema_final
 class ACKParameter(Parameter):
     """Header schema for HIP ``ACK`` parameters."""
 
     #: Update ID.
     update_id: 'list[int]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=UInt32Field(),
@@ -337,14 +347,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', update_id: 'bytes | list[int]') -> 'None': ...
 
 
+@schema_final
 class DHGroupListParameter(Parameter):
     """Header schema for HIP ``DH_GROUP_LIST`` parameters."""
 
     #: List of DH groups.
     groups: 'list[Enum_Group]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=EnumField(length=1, namespace=Enum_Group),
@@ -352,14 +363,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', groups: 'list[Enum_Group]') -> 'None': ...
 
 
+@schema_final
 class DiffieHellmanParameter(Parameter):
     """Header schema for HIP ``DIFFIE_HELLMAN`` parameters."""
 
     #: Diffie-Hellman group.
     group: 'Enum_Group' = EnumField(length=1, namespace=Enum_Group)
     #: Public value length.
     pub_len: 'int' = UInt16Field()
@@ -369,14 +381,15 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', group: 'Enum_Group', pub_len: 'int',
                      pub_val: 'int') -> 'None': ...
 
 
+@schema_final
 class HIPTransformParameter(Parameter):
     """Header schema for HIP ``TRANSFORM`` parameters."""
 
     #: Suite IDs.
     suites: 'list[Enum_Suite]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=EnumField(length=2, namespace=Enum_Suite),
@@ -384,14 +397,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', suites: 'list[Enum_Suite]') -> 'None': ...
 
 
+@schema_final
 class HIPCipherParameter(Parameter):
     """Header schema for HIP ``CIPHER`` parameters."""
 
     #: Cipher IDs.
     ciphers: 'list[Enum_Cipher]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=EnumField(length=2, namespace=Enum_Cipher),
@@ -399,14 +413,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', ciphers: 'list[Enum_Cipher]') -> 'None': ...
 
 
+@schema_final
 class NATTraversalModeParameter(Parameter):
     """Header schema for HIP ``NAT_TRAVERSAL_MODE`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: NAT traversal modes.
     modes: 'list[Enum_NATTraversal]' = ListField(
@@ -416,26 +431,28 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', modes: 'list[Enum_NATTraversal]') -> 'None': ...
 
 
+@schema_final
 class TransactionPacingParameter(Parameter):
     """Header schema for HIP ``TRANSACTION_PACING`` parameters."""
 
     #: Transaction pacing.
     min_ta: 'int' = UInt32Field()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', min_ta: 'int') -> 'None': ...
 
 
+@schema_final
 class EncryptedParameter(Parameter):
     """Header schema for HIP ``ENCRYPTED`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: Initialization vector.
     iv: 'bytes' = ConditionalField(
@@ -507,14 +524,15 @@
         #: Cipher ID.
         cipher: 'Enum_Cipher'
 
         def __init__(self, type: 'Enum_Parameter', len: 'int', cipher: 'Enum_Cipher',
                      iv: 'Optional[bytes]', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HostIDParameter(Parameter):
     """Header schema for HIP ``HOST_ID`` parameters."""
 
     #: Host ID length.
     hi_len: 'int' = UInt16Field()
     #: Domain ID type and length.
     di_data: 'DIData' = BitField(
@@ -539,50 +557,54 @@
                      di: 'bytes') -> 'None': ...
 
 
 class HostIdentity(Schema):
     """Host identity schema."""
 
 
+@schema_final
 class ECDSACurveHostIdentity(HostIdentity):
     """Host identity schema with ECDSA curve."""
 
     #: Algorithm curve type.
     curve: 'Enum_ECDSACurve' = EnumField(length=2, namespace=Enum_ECDSACurve)
     #: Public key.
     pub_key: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, curve: 'Enum_ECDSACurve', pub_key: 'bytes') -> 'None': ...
 
 
+@schema_final
 class ECDSALowCurveHostIdentity(HostIdentity):
     """Host identity schema with ECDSA_LOW curve."""
 
     #: Algorithm curve type.
     curve: 'Enum_ECDSALowCurve' = EnumField(length=2, namespace=Enum_ECDSALowCurve)
     #: Public key.
     pub_key: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, curve: 'Enum_ECDSALowCurve', pub_key: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EdDSACurveHostIdentity(HostIdentity):
     """Host identity schema with EdDSA curve."""
 
     #: Algorithm curve type.
     curve: 'Enum_EdDSACurve' = EnumField(length=2, namespace=Enum_EdDSACurve)
     #: Public key.
     pub_key: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, curve: 'Enum_EdDSACurve', pub_key: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HITSuiteListParameter(Parameter):
     """Header schema for HIP ``HIT_SUITE_LIST`` parameters."""
 
     #: HIT suite IDs.
     suites: 'list[Enum_HITSuite]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=EnumField(length=1, namespace=Enum_HITSuite),
@@ -590,14 +612,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', suites: 'list[Enum_HITSuite]') -> 'None': ...
 
 
+@schema_final
 class CertParameter(Parameter):
     """Header schema for HIP ``CERT`` parameters."""
 
     #: Certificate group.
     cert_group: 'Enum_Group' = EnumField(length=1, namespace=Enum_Group)
     #: Certificate count.
     cert_count: 'int' = UInt8Field()
@@ -611,14 +634,15 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', cert_group: 'Enum_Group', cert_count: 'int',
                      cert_id: 'int', cert_type: 'Enum_Certificate', cert: 'bytes') -> 'None': ...
 
 
+@schema_final
 class NotificationParameter(Parameter):
     """Header schema for HIP ``NOTIFICATION`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: Notify message type.
     msg_type: 'Enum_NotifyMessage' = EnumField(length=2, namespace=Enum_NotifyMessage)
@@ -627,26 +651,28 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', msg_type: 'Enum_NotifyMessage', msg: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EchoRequestSignedParameter(Parameter):
     """Header schema for HIP ``ECHO_REQUEST_SIGNED`` parameters."""
 
     #: Opaque data.
     opaque: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', opaque: 'bytes') -> 'None': ...
 
 
+@schema_final
 class RegInfoParameter(Parameter):
     """Header schema for HIP ``REG_INFO`` parameters."""
 
     #: Minimum lifetime.
     min_lifetime: 'int' = UInt8Field()
     #: Maximum lifetime.
     max_lifetime: 'int' = UInt8Field()
@@ -659,14 +685,15 @@
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', min_lifetime: 'int', max_lifetime: 'int',
                      reg_info: 'list[Enum_Registration]') -> 'None': ...
 
 
+@schema_final
 class RegRequestParameter(Parameter):
     """Header schema for HIP ``REG_REQUEST`` parameters."""
 
     #: Lifetime.
     lifetime: 'int' = UInt8Field()
     #: Registration types.
     reg_request: 'list[Enum_Registration]' = ListField(
@@ -676,14 +703,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', lifetime: 'int', reg_request: 'list[Enum_Registration]') -> 'None': ...
 
 
+@schema_final
 class RegResponseParameter(Parameter):
     """Header schema for HIP ``REG_RESPONSE`` parameters."""
 
     #: Lifetime.
     lifetime: 'int' = UInt8Field()
     #: Registration types.
     reg_response: 'list[Enum_Registration]' = ListField(
@@ -693,14 +721,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', lifetime: 'int', reg_response: 'list[Enum_Registration]') -> 'None': ...
 
 
+@schema_final
 class RegFailedParameter(Parameter):
     """Header schema for HIP ``REG_FAILED`` parameters."""
 
     #: Lifetime.
     lifetime: 'int' = UInt8Field()
     #: Registration types.
     reg_failed: 'list[Enum_RegistrationFailure]' = ListField(
@@ -710,14 +739,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', lifetime: 'int', reg_failed: 'list[Enum_RegistrationFailure]') -> 'None': ...
 
 
+@schema_final
 class RegFromParameter(Parameter):
     """Header schema for HIP ``REG_FROM`` parameters."""
 
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
@@ -726,26 +756,28 @@
     #: Address.
     address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'IPv6Address | bytes | int | str') -> 'None': ...
 
 
+@schema_final
 class EchoResponseSignedParameter(Parameter):
     """Header schema for HIP ``ECHO_RESPONSE_SIGNED`` parameters."""
 
     #: Opaque data.
     opaque: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', opaque: 'bytes') -> 'None': ...
 
 
+@schema_final
 class TransportFormatListParameter(Parameter):
     """Header schema for HIP ``TRANSPORT_FORMAT_LIST`` parameters."""
 
     #: Transport formats.
     formats: 'list[Enum_Parameter]' = ListField(
         length=lambda pkt: pkt['len'] - 2,
         item_type=EnumField(length=1, namespace=Enum_Parameter),
@@ -753,14 +785,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', formats: 'list[Enum_Parameter]') -> 'None': ...
 
 
+@schema_final
 class ESPTransformParameter(Parameter):
     """Header schema for HIP ``ESP_TRANSFORM`` parameters."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: Suite IDs.
     suites: 'list[Enum_ESPTransformSuite]' = ListField(
@@ -770,26 +803,28 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', suites: 'list[Enum_ESPTransformSuite]') -> 'None': ...
 
 
+@schema_final
 class SeqDataParameter(Parameter):
     """Header schema for HIP ``SEQ_DATA`` parameters."""
 
     #: Sequence number.
     seq: 'int' = UInt32Field()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', seq: 'int') -> 'None': ...
 
 
+@schema_final
 class AckDataParameter(Parameter):
     """Header schema for HIP ``ACK_DATA`` parameters."""
 
     #: Acked sequence number.
     ack: 'list[int]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=UInt32Field(),
@@ -797,14 +832,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', ack: 'list[int]') -> 'None': ...
 
 
+@schema_final
 class PayloadMICParameter(Parameter):
     """Header schema for HIP ``PAYLOAD_MIC`` parameters."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Reversed.
     reserved: 'bytes' = PaddingField(length=3)
@@ -815,38 +851,41 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', next: 'Enum_TransType', payload: 'bytes', mic: 'bytes') -> 'None': ...
 
 
+@schema_final
 class TransactionIDParameter(Parameter):
     """Header schema for HIP ``TRANSACTION_ID`` parameters."""
 
     #: Transaction ID.
     id: 'int' = NumberField(length=lambda pkt: pkt['len'], signed=False)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', id: 'int') -> 'None': ...
 
 
+@schema_final
 class OverlayIDParameter(Parameter):
     """Header schema for HIP ``OVERLAY_ID`` parameters."""
 
     #: Overlay ID.
     id: 'int' = NumberField(length=lambda pkt: pkt['len'], signed=False)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', id: 'int') -> 'None': ...
 
 
+@schema_final
 class RouteDstParameter(Parameter):
     """Header schema for HIP ``ROUTE_DST`` parameters."""
 
     #: Flags.
     flags: 'RouteFlags' = BitField(length=2, namespace={
             'symmetric': (0, 1),
             'must_follow': (1, 1),
@@ -861,14 +900,15 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', flags: 'RouteFlags', hit: 'list[str | int | bytes | IPv6Address]') -> 'None': ...
 
 
+@schema_final
 class HIPTransportModeParameter(Parameter):
     """Header schema for HIP ``HIP_TRANSPORT_MODE`` parameters."""
 
     #: Port.
     port: 'int' = UInt16Field()
     #: Mode IDs.
     mode: 'list[Enum_Transport]' = ListField(
@@ -878,90 +918,97 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', mode: 'list[Enum_Transport]') -> 'None': ...
 
 
+@schema_final
 class HIPMACParameter(Parameter):
     """Header schema for HIP ``HIP_MAC`` parameters."""
 
     #: HMAC value.
     hmac: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', hmac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HIPMAC2Parameter(Parameter):
     """Header schema for HIP ``HIP_MAC_2`` parameters."""
 
     #: HMAC value.
     hmac: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', hmac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HIPSignature2Parameter(Parameter):
     """Header schema for HIP ``HIP_SIGNATURE_2`` parameters."""
 
     #: Signature algorithm.
     algorithm: 'Enum_HIAlgorithm' = EnumField(length=2, namespace=Enum_HIAlgorithm)
     #: Signature value.
     signature: 'bytes' = BytesField(length=lambda pkt: pkt['len'] - 2)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', algorithm: 'Enum_HIAlgorithm', signature: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HIPSignatureParameter(Parameter):
     """Header schema for HIP ``HIP_SIGNATURE`` parameters."""
 
     #: Signature algorithm.
     algorithm: 'Enum_HIAlgorithm' = EnumField(length=2, namespace=Enum_HIAlgorithm)
     #: Signature value.
     signature: 'bytes' = BytesField(length=lambda pkt: pkt['len'] - 2)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', algorithm: 'Enum_HIAlgorithm', signature: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EchoRequestUnsignedParameter(Parameter):
     """Header schema for HIP ``ECHO_REQUEST_UNSIGNED`` parameters."""
 
     #: Opaque data.
     opaque: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', opaque: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EchoResponseUnsignedParameter(Parameter):
     """Header schema for HIP ``ECHO_RESPONSE_UNSIGNED`` parameters."""
 
     #: Opaque data.
     opaque: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', opaque: 'bytes') -> 'None': ...
 
 
+@schema_final
 class RelayFromParameter(Parameter):
     """Header schema for HIP ``RELAY_FROM`` parameters."""
 
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
@@ -970,14 +1017,15 @@
     #: Address.
     address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
+@schema_final
 class RelayToParameter(Parameter):
     """Header schema for HIP ``RELAY_TO`` parameters."""
 
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
@@ -986,28 +1034,30 @@
     #: Address.
     address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
+@schema_final
 class OverlayTTLParameter(Parameter):
     """Header schema for HIP ``OVERLAY_TTL`` parameters."""
 
     #: TTL value.
     ttl: 'int' = UInt16Field()
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', ttl: 'int') -> 'None': ...
 
 
+@schema_final
 class RouteViaParameter(Parameter):
     """Header schema for HIP ``ROUTE_VIA`` parameters."""
 
     #: Flags.
     flags: 'RouteFlags' = BitField(length=2, namespace={
         'symmetric': (0, 1),
         'must_follow': (1, 1),
@@ -1022,38 +1072,41 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', flags: 'RouteFlags', hit: 'list[str | bytes | int | IPv6Address]') -> 'None': ...
 
 
+@schema_final
 class FromParameter(Parameter):
     """Header schema for HIP ``FROM`` parameters."""
 
     #: Address.
     address: 'IPv6Address' = IPv6AddressField()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
+@schema_final
 class RVSHMACParameter(Parameter):
     """Header schema for HIP ``RVS_HMAC`` parameters."""
 
     #: HMAC value.
     hmac: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', hmac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class ViaRVSParameter(Parameter):
     """Header schema for HIP ``VIA_RVS`` parameters."""
 
     #: Address.
     address: 'list[IPv6Address]' = ListField(
         length=lambda pkt: pkt['len'],
         item_type=IPv6AddressField(),
@@ -1061,26 +1114,28 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', address: 'list[str | bytes | int | IPv6Address]') -> 'None': ...
 
 
+@schema_final
 class RelayHMACParameter(Parameter):
     """Header schema for HIP ``RELAY_HMAC`` parameters."""
 
     #: HMAC value.
     hmac: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', hmac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class HIP(Schema):
     """Header schema for HIP packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Header length.
     len: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hopopt.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/hopopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pcapkit.corekit.fields.field import NoValue
 from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, NoValueField,
                                          PayloadField, SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
     'HOPOPT',
 
     'SMFDPDOption', 'QuickStartOption',
@@ -249,54 +249,59 @@
         """
         # for Pad1 option, length is always 0
         if self.type == Enum_Option.Pad1:
             self.len = 0
         return self
 
 
+@schema_final
 class UnassignedOption(Option):
     """Header schema for HOPOPT unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PadOption(Option):
     """Header schema for HOPOPT padding options."""
 
     #: Padding.
     pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int') -> 'None': ...
 
 
+@schema_final
 class TunnelEncapsulationLimitOption(Option):
     """Header schema for HOPOPT tunnel encapsulation limit options."""
 
     #: Tunnel encapsulation limit.
     limit: 'int' = UInt8Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', limit: 'int') -> 'None': ...
 
 
+@schema_final
 class RouterAlertOption(Option):
     """Header schema for HOPOPT router alert options."""
 
     #: Router alert.
     alert: 'Enum_RouterAlert' = EnumField(length=2, namespace=Enum_RouterAlert)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', alert: 'Enum_RouterAlert') -> 'None': ...
 
 
+@schema_final
 class CALIPSOOption(Option):
     """Header schema for HOPOPT common architecture label IPv6 security options."""
 
     #: CALIPSO domain of interpretation.
     domain: 'int' = UInt32Field()
     #: Compartment length.
     cmpt_len: 'int' = UInt8Field()
@@ -313,14 +318,15 @@
     pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'] - 8 - pkt['cmpt_len'] * 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', domain: 'int', cmpt_len: 'int',
                      level: 'int', checksum: 'bytes', bitmap: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class _SMFDPDOption(Schema):
     """Header schema for HOPOPT SMF DPD options with generic representation."""
 
     #: SMF DPD mode.
     test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=3, namespace={
         'len': (1, 8),
         'mode': (16, 1),
@@ -348,14 +354,15 @@
     """Header schema for HOPOPT simplified multicast forwarding duplicate packet
     detection (``SMF_DPD``) options."""
 
     if TYPE_CHECKING:
         mode: 'Enum_SMFDPDMode'
 
 
+@schema_final
 class SMFIdentificationBasedDPDOption(SMFDPDOption):
     """Header schema for HOPOPT SMF identification-based DPD options."""
 
     #: TaggerID information.
     info: 'TaggerIDInfo' = BitField(length=1, namespace={
         'mode': (0, 1),
         'type': (1, 3),
@@ -386,14 +393,15 @@
         return ret
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', info: 'TaggerIDInfo',
                      tid: 'Optional[bytes]', id: 'bytes') -> 'None': ...
 
 
+@schema_final
 class SMFHashBasedDPDOption(SMFDPDOption):
     """Header schema for HOPOPT SMF hash-based DPD options."""
 
     #: Hash assist value (HAV).
     hav: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
     def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
@@ -410,14 +418,15 @@
         ret.mode = Enum_SMFDPDMode.H_DPD
         return ret
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', hav: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PDMOption(Option):
     """Header schema for HOPOPT performance and diagnostic metrics (PDM) options."""
 
     #: Scale delta time last received (DTLR).
     scaledtlr: 'int' = UInt8Field()
     #: Scale delta time last sent (DTLS).
     scaledtls: 'int' = UInt8Field()
@@ -431,14 +440,15 @@
     deltatls: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', scaledtlr: 'int', scaledtls: 'int',
                      psntp: 'int', psnlr: 'int', deltatlr: 'int', deltatls: 'int') -> 'None': ...
 
 
+@schema_final
 class _QuickStartOption(Schema):
     """Header schema for HOPOPT quick start options in generic representation."""
 
     #: Flags.
     flags: 'QSTestFlags' = ForwardMatchField(BitField(length=3, namespace={
         'func': (16, 4),
     }))
@@ -471,14 +481,15 @@
         'rate': (4, 4),
     })
 
     if TYPE_CHECKING:
         func: 'Enum_QSFunction'
 
 
+@schema_final
 class QuickStartRequestOption(QuickStartOption):
     """Header schema for HOPOPT quick start request options."""
 
     #: QS time-to-live (TTL).
     ttl: 'int' = UInt8Field()
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
@@ -486,14 +497,15 @@
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      ttl: 'int', nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class QuickStartReportOption(QuickStartOption):
     """Header schema for HOPOPT quick start report of approved rate options."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
@@ -501,14 +513,15 @@
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class RPLOption(Option):
     """Header schema for HOPOPT routing protocol for low-power and lossy networks (RPL) options."""
 
     #: Flags.
     flags: 'RPLFlags' = BitField(length=1, namespace={
         'down': (0, 1),
         'rank_err': (1, 1),
@@ -520,14 +533,15 @@
     rank: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'RPLFlags', id: 'int',
                      rank: 'int') -> 'None': ...
 
 
+@schema_final
 class MPLOption(Option):
     """Header schema for HOPOPT multicast protocol for low-power and lossy networks (MPL) options."""
 
     #: Flags.
     flags: 'MPLFlags' = BitField(length=1, namespace={
         'type': (0, 2),
         'max': (2, 1),
@@ -560,56 +574,61 @@
         return self
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'MPLFlags', seq: 'int',
                      seed: 'Optional[int]') -> 'None': ...
 
 
+@schema_final
 class ILNPOption(Option):
     """Header schema for HOPOPT identifier-locator network protocol (ILNP) options."""
 
     #: Nonce value.
     nonce: 'int' = NumberField(length=lambda pkt: pkt['len'], signed=False)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', nonce: 'int') -> 'None': ...
 
 
+@schema_final
 class LineIdentificationOption(Option):
     """Header schema for HOPOPT line-identification options."""
 
     #: Line ID length.
     id_len: 'int' = UInt8Field()
     #: Line ID.
     id: 'bytes' = BytesField(length=lambda pkt: pkt['id_len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', id_len: 'int', id: 'bytes') -> 'None': ...
 
 
+@schema_final
 class JumboPayloadOption(Option):
     """Header schema for HOPOPT jumbo payload options."""
 
     #: Jumbo payload length.
     jumbo_len: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', jumbo_len: 'int') -> 'None': ...
 
 
+@schema_final
 class HomeAddressOption(Option):
     """Header schema for HOPOPT home address options."""
 
     #: Home address.
     addr: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', addr: 'IPv6Address | int | str | bytes') -> 'None': ...
 
 
+@schema_final
 class IPDFFOption(Option):
     """Header schema for HOPOPT depth-first forwarding (``IP_DFF``) options."""
 
     #: Flags.
     flags: 'DFFFlags' = BitField(length=1, namespace={
         'ver': (0, 2),
         'dup': (2, 1),
@@ -618,14 +637,15 @@
     #: Sequence number.
     seq: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'DFFFlags', seq: 'int') -> 'None': ...
 
 
+@schema_final
 class HOPOPT(Schema):
     """Header schema for HOPOPT packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Header length.
     len: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv4.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv4.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import ListField, OptionField
 from pcapkit.corekit.fields.ipaddress import IPv4AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, PayloadField,
                                          SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field, UInt32Field
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 from pcapkit.utilities.warnings import ProtocolWarning, warn
 
 __all__ = [
     'IPv4',
 
@@ -152,38 +152,42 @@
         """
         # for EOOL/NOP option, length is always 1
         if self.type in (Enum_OptionNumber.EOOL, Enum_OptionNumber.NOP):
             self.length = 1
         return self
 
 
+@schema_final
 class UnassignedOption(Option):
     """Header schema for IPv4 unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EOOLOption(Option):
     """Header schema for IPv4 end of option list (``EOOL``) option."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int') -> 'None': ...
 
 
+@schema_final
 class NOPOption(Option):
     """Header schema for IPv4 no operation (``NOP``) option."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int') -> 'None': ...
 
 
+@schema_final
 class SECOption(Option):
     """Header schema for IPv4 security (``SEC``) option."""
 
     #: Classification level.
     level: 'Enum_ClassificationLevel' = EnumField(length=1, namespace=Enum_ClassificationLevel)
     #: Protection authority flags.
     data: 'bytes' = ConditionalField(
@@ -191,14 +195,15 @@
         lambda pkt: pkt['length'] > 3,
     )
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', level: 'int', data: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class LSROption(Option):
     """Header schema for IPv4 loose source route (``LSR``) option."""
 
     #: Pointer.
     pointer: 'int' = UInt8Field()
     #: Route.
     route: 'list[IPv4Address]' = ListField(
@@ -211,14 +216,15 @@
         default=bytes(36),  # a reasonable default
     )
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
 
 
+@schema_final
 class TSOption(Option):
     """Header schema for IPv4 timestamp (``TS``) option."""
 
     #: Pointer.
     pointer: 'int' = UInt8Field()
     #: Overflow and flags.
     flags: 'TSFlags' = BitField(length=1, namespace={
@@ -312,14 +318,15 @@
         ts_flag: 'Enum_TSFlag'
         data: 'list[int] | OrderedMultiDict[IPv4Address, int]'
         timestamp: 'tuple[int | timedelta] | OrderedMultiDict[IPv4Address, int | timedelta]'
 
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', flags: 'TSFlags', data: 'list[int]') -> 'None': ...
 
 
+@schema_final
 class ESECOption(Option):
     """Header schema for IPv4 extended security (``ESEC``) option."""
 
     #: Additional security information format code.
     format: 'int' = UInt8Field()
     #: Additional security information.
     info: 'bytes' = ConditionalField(
@@ -327,14 +334,15 @@
         lambda pkt: pkt['length'] > 3,
     )
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', format: 'int', info: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class RROption(Option):
     """Header schema for IPv4 record route (``RR``) option."""
 
     #: Pointer.
     pointer: 'int' = UInt8Field()
     #: Route.
     route: 'list[IPv4Address]' = ListField(
@@ -347,24 +355,26 @@
         default=bytes(36),  # a reasonable default
     )
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
 
 
+@schema_final
 class SIDOption(Option):
     """Header schema for IPv4 stream identifier (``SID``) option."""
 
     #: Stream identifier.
     sid: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', sid: 'int') -> 'None': ...
 
 
+@schema_final
 class SSROption(Option):
     """Header schema for IPv4 strict source route (``SSR``) option."""
 
     #: Pointer.
     pointer: 'int' = UInt8Field()
     #: Route.
     route: 'list[IPv4Address]' = ListField(
@@ -377,34 +387,37 @@
         default=bytes(36),  # a reasonable default
     )
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
 
 
+@schema_final
 class MTUPOption(Option):
     """Header schema for IPv4 MTU probe (``MTUP``) option."""
 
     #: MTU.
     mtu: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', mtu: 'int') -> 'None': ...
 
 
+@schema_final
 class MTUROption(Option):
     """Header schema for IPv4 MTU reply (``MTUR``) option."""
 
     #: MTU.
     mtu: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', mtu: 'int') -> 'None': ...
 
 
+@schema_final
 class TROption(Option):
     """Header schema for IPv4 traceroute (``TR``) option."""
 
     #: ID number.
     id: 'int' = UInt16Field()
     #: Outbound hop count.
     out: 'int' = UInt16Field()
@@ -413,24 +426,26 @@
     #: Originator IP address.
     origin: 'IPv4Address' = IPv4AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', id: 'int', out: 'int', ret: 'int', origin: 'IPv4Address | str | bytes | int') -> 'None': ...
 
 
+@schema_final
 class RTRALTOption(Option):
     """Header schema for IPv4 router alert (``RTRALT``) option."""
 
     #: Router alert value.
     alert: 'Enum_RouterAlert' = EnumField(length=2, namespace=Enum_RouterAlert)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', alert: 'Enum_RouterAlert') -> 'None': ...
 
 
+@schema_final
 class _QSOption(Schema):
     """Header schema for IPv4 quick start (``QS``) options in generic representation."""
 
     #: Flags.
     flags: 'QSTestFlags' = ForwardMatchField(BitField(length=3, namespace={
         'func': (16, 4),
     }))
@@ -463,14 +478,15 @@
         'rate': (4, 4),
     })
 
     if TYPE_CHECKING:
         func: 'Enum_QSFunction'
 
 
+@schema_final
 class QuickStartRequestOption(QSOption):
     """Header schema for IPV4 quick start request options."""
 
     #: QS time-to-live (TTL).
     ttl: 'int' = UInt8Field()
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
@@ -478,27 +494,29 @@
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', flags: 'QuickStartFlags',
                      ttl: 'int', nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class QuickStartReportOption(QSOption):
     """Header schema for IPV4 quick start report of approved rate options."""
 
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
         'nonce': (0, 30),
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionNumber', length: 'int', flags: 'QuickStartFlags',
                      nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class IPv4(Schema):
     """Header schema for IPv4 packet."""
 
     #: Version and header length.
     vihl: 'VerIHLField' = BitField(length=1, namespace={
         'version': (0, 4),
         'ihl': (4, 8),
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field
 from pcapkit.corekit.fields.strings import BitField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = ['IPv6']
 
 if TYPE_CHECKING:
     from ipaddress import IPv6Address
 
@@ -29,14 +29,15 @@
         #: Traffic class.
         'class': int,
         #: Flow label.
         'label': int,
     })
 
 
+@schema_final
 class IPv6(Schema):
     """Header schema for IPv6 packet."""
 
     #: Version, traffic class and flow label.
     hextet: 'IPv6Hextet' = BitField(length=4, namespace={
         'version': (0, 4),
         'class': (4, 8),
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_frag.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_frag.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt32Field
 from pcapkit.corekit.fields.strings import BitField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['IPv6_Frag']
 
 if TYPE_CHECKING:
     from typing_extensions import TypedDict
 
     from pcapkit.protocols.protocol import Protocol
@@ -22,14 +22,15 @@
 
         #: Fragment offset.
         offset: int
         #: More fragments flag.
         mf: int
 
 
+@schema_final
 class IPv6_Frag(Schema):
     """Header schema for IPv6-Frag packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_opts.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_opts.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pcapkit.corekit.fields.field import NoValue
 from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, NoValueField,
                                          PayloadField, SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
     'IPv6_Opts',
 
     'SMFDPDOption', 'QuickStartOption',
@@ -249,54 +249,59 @@
         """
         # for Pad1 option, length is always 0
         if self.type == Enum_Option.Pad1:
             self.len = 0
         return self
 
 
+@schema_final
 class UnassignedOption(Option):
     """Header schema for IPv6-Opts unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PadOption(Option):
     """Header schema for IPv6-Opts padding options."""
 
     #: Padding.
     pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int') -> 'None': ...
 
 
+@schema_final
 class TunnelEncapsulationLimitOption(Option):
     """Header schema for IPv6-Opts tunnel encapsulation limit options."""
 
     #: Tunnel encapsulation limit.
     limit: 'int' = UInt8Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', limit: 'int') -> 'None': ...
 
 
+@schema_final
 class RouterAlertOption(Option):
     """Header schema for IPv6-Opts router alert options."""
 
     #: Router alert.
     alert: 'Enum_RouterAlert' = EnumField(length=2, namespace=Enum_RouterAlert)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', alert: 'Enum_RouterAlert') -> 'None': ...
 
 
+@schema_final
 class CALIPSOOption(Option):
     """Header schema for IPv6-Opts common architecture label IPv6 security options."""
 
     #: CALIPSO domain of interpretation.
     domain: 'int' = UInt32Field()
     #: Compartment length.
     cmpt_len: 'int' = UInt8Field()
@@ -313,14 +318,15 @@
     pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'] - 8 - pkt['cmpt_len'] * 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', domain: 'int', cmpt_len: 'int',
                      level: 'int', checksum: 'bytes', bitmap: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class _SMFDPDOption(Schema):
     """Header schema for IPv6-Opts SMF DPD options with generic representation."""
 
     #: SMF DPD mode.
     test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=3, namespace={
         'len': (1, 8),
         'mode': (16, 1),
@@ -348,14 +354,15 @@
     """Header schema for IPv6-Opts simplified multicast forwarding duplicate packet
     detection (``SMF_DPD``) options."""
 
     if TYPE_CHECKING:
         mode: 'Enum_SMFDPDMode'
 
 
+@schema_final
 class SMFIdentificationBasedDPDOption(SMFDPDOption):
     """Header schema for IPv6-Opts SMF identification-based DPD options."""
 
     test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=1, namespace={
         'mode': (0, 1),
     }))
     #: TaggerID information.
@@ -389,14 +396,15 @@
         return ret
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', info: 'TaggerIDInfo',
                      tid: 'Optional[bytes]', id: 'bytes') -> 'None': ...
 
 
+@schema_final
 class SMFHashBasedDPDOption(SMFDPDOption):
     """Header schema for IPv6-Opts SMF hash-based DPD options."""
 
     #: Hash assist value (HAV).
     hav: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
     def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
@@ -413,14 +421,15 @@
         ret.mode = Enum_SMFDPDMode.H_DPD
         return ret
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', hav: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PDMOption(Option):
     """Header schema for IPv6-Opts performance and diagnostic metrics (PDM) options."""
 
     #: Scale delta time last received (DTLR).
     scaledtlr: 'int' = UInt8Field()
     #: Scale delta time last sent (DTLS).
     scaledtls: 'int' = UInt8Field()
@@ -434,14 +443,15 @@
     deltatls: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', scaledtlr: 'int', scaledtls: 'int',
                      psntp: 'int', psnlr: 'int', deltatlr: 'int', deltatls: 'int') -> 'None': ...
 
 
+@schema_final
 class _QuickStartOption(Schema):
     """Header schema for IPv6-Opts quick start options in generic representation."""
 
     #: Flags.
     flags: 'QSTestFlags' = ForwardMatchField(BitField(length=3, namespace={
         'func': (16, 4),
     }))
@@ -474,14 +484,15 @@
         'rate': (4, 4),
     })
 
     if TYPE_CHECKING:
         func: 'Enum_QSFunction'
 
 
+@schema_final
 class QuickStartRequestOption(QuickStartOption):
     """Header schema for IPv6-Opts quick start request options."""
 
     #: QS time-to-live (TTL).
     ttl: 'int' = UInt8Field()
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
@@ -489,14 +500,15 @@
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      ttl: 'int', nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class QuickStartReportOption(QuickStartOption):
     """Header schema for IPv6-Opts quick start report of approved rate options."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
@@ -504,14 +516,15 @@
     })
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      nonce: 'QSNonce') -> 'None': ...
 
 
+@schema_final
 class RPLOption(Option):
     """Header schema for IPv6-Opts routing protocol for low-power and lossy networks (RPL) options."""
 
     #: Flags.
     flags: 'RPLFlags' = BitField(length=1, namespace={
         'down': (0, 1),
         'rank_err': (1, 1),
@@ -523,14 +536,15 @@
     rank: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'RPLFlags', id: 'int',
                      rank: 'int') -> 'None': ...
 
 
+@schema_final
 class MPLOption(Option):
     """Header schema for IPv6-Opts multicast protocol for low-power and lossy networks (MPL) options."""
 
     #: Flags.
     flags: 'MPLFlags' = BitField(length=1, namespace={
         'type': (0, 2),
         'max': (2, 1),
@@ -563,56 +577,61 @@
         return self
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'MPLFlags', seq: 'int',
                      seed: 'Optional[int]') -> 'None': ...
 
 
+@schema_final
 class ILNPOption(Option):
     """Header schema for IPv6-Opts identifier-locator network protocol (ILNP) options."""
 
     #: Nonce value.
     nonce: 'int' = NumberField(length=lambda pkt: pkt['len'], signed=False)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', nonce: 'int') -> 'None': ...
 
 
+@schema_final
 class LineIdentificationOption(Option):
     """Header schema for IPv6-Opts line-identification options."""
 
     #: Line ID length.
     id_len: 'int' = UInt8Field()
     #: Line ID.
     id: 'bytes' = BytesField(length=lambda pkt: pkt['id_len'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', id_len: 'int', id: 'bytes') -> 'None': ...
 
 
+@schema_final
 class JumboPayloadOption(Option):
     """Header schema for IPv6-Opts jumbo payload options."""
 
     #: Jumbo payload length.
     jumbo_len: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', jumbo_len: 'int') -> 'None': ...
 
 
+@schema_final
 class HomeAddressOption(Option):
     """Header schema for IPv6-Opts home address options."""
 
     #: Home address.
     addr: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', addr: 'IPv6Address | int | str | bytes') -> 'None': ...
 
 
+@schema_final
 class IPDFFOption(Option):
     """Header schema for IPv6-Opts depth-first forwarding (``IP_DFF``) options."""
 
     #: Flags.
     flags: 'DFFFlags' = BitField(length=1, namespace={
         'ver': (0, 2),
         'dup': (2, 1),
@@ -621,14 +640,15 @@
     #: Sequence number.
     seq: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'DFFFlags', seq: 'int') -> 'None': ...
 
 
+@schema_final
 class IPv6_Opts(Schema):
     """Header schema for IPv6-Opts packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Header length.
     len: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_route.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipv6_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pcapkit.const.ipv6.routing import Routing as Enum_Routing
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import ListField
 from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
     'IPv6_Route',
 
     'RoutingType',
     'UnknownType', 'SourceRoute', 'Type2', 'RPL',
@@ -62,14 +62,15 @@
     if type == Enum_Routing.Type_2_Routing_Header:
         return SchemaField(length=pkt['length'] * 8 - 4, schema=Type2)
     if type == Enum_Routing.RPL_Source_Route_Header:
         return SchemaField(length=pkt['length'] * 8 - 4, schema=RPL)
     return SchemaField(length=pkt['length'] * 8 - 4, schema=UnknownType)
 
 
+@schema_final
 class IPv6_Route(Schema):
     """Header schema for IPv6-Route packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Header extension length.
     length: 'int' = UInt8Field()
@@ -89,24 +90,26 @@
                      seg_left: 'int', data: 'bytes | RoutingType', payload: 'Protocol | Schema | bytes') -> 'None': ...
 
 
 class RoutingType(Schema):
     """Header schema for IPv6-Route type-specific routing data."""
 
 
+@schema_final
 class UnknownType(RoutingType):
     """Header schema for IPv6-Route unknown type routing data."""
 
     #: Type-specific data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class SourceRoute(RoutingType):
     """Header schema for IPv6-Route source route routing data."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: Addresses.
     ip: 'list[IPv6Address]' = ListField(
@@ -114,26 +117,28 @@
         item_type=IPv6AddressField(),
     )
 
     if TYPE_CHECKING:
         def __init__(self, ip: 'list[IPv6Address | str | int | bytes]') -> 'None': ...
 
 
+@schema_final
 class Type2(RoutingType):
     """Header schema for IPv6-Route type 2 routing data."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: Addresses.
     ip: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, ip: 'IPv6Address | str | int | bytes') -> 'None': ...
 
 
+@schema_final
 class RPL(RoutingType):
     """Header schema for IPv6-Route RPL routing data."""
 
     #: CmprI.
     cmpr_i: 'int' = UInt8Field()
     #: CmprE.
     cmpr_e: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipx.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/ipx.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.ipx.packet import Packet as Enum_Packet
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field
 from pcapkit.corekit.fields.strings import BytesField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['IPX']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
 
+@schema_final
 class IPX(Schema):
     """Header schema for IPX packet."""
 
     #: Checksum.
     chksum: 'bytes' = BytesField(length=2)
     #: Packet length (header includes).
     len: 'int' = UInt16Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/mh.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/internet/mh.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from typing import TYPE_CHECKING
 
 from pcapkit.const.mh.packet import Packet as Enum_Packet
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field
 from pcapkit.corekit.fields.strings import BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['MH']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
 
+@schema_final
 class MH(Schema):
     """Header schema for MH packets."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Header length.
     length: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/arp.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/arp.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from pcapkit.const.arp.hardware import Hardware as Enum_Hardware
 from pcapkit.const.arp.operation import Operation as Enum_Operation
 from pcapkit.const.reg.ethertype import EtherType as Enum_EtherType
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field
 from pcapkit.corekit.fields.strings import BytesField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['ARP']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
 
+@schema_final
 class ARP(Schema):
     """Header schema for ARP packet."""
 
     htype: 'Enum_Hardware' = EnumField(length=2, namespace=Enum_Hardware)
     ptype: 'Enum_EtherType' = EnumField(length=2, namespace=Enum_EtherType)
     hlen: 'int' = UInt8Field()
     plen: 'int' = UInt8Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ethernet.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/ethernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.reg.ethertype import EtherType as Enum_EtherType
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField
 from pcapkit.corekit.fields.strings import BytesField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['Ethernet']
 
 if TYPE_CHECKING:
     from typing import Any, Type
 
     from pcapkit.protocols.protocol import Protocol
@@ -25,14 +25,15 @@
 
     type_ = packet['type']
     module, name = Ethernet.__proto__[type_]
     protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
     self.protocol = protocol
 
 
+@schema_final
 class Ethernet(Schema):
     """Header schema for ethernet packet."""
 
     #: Destination MAC address.
     dst: 'bytes' = BytesField(length=6)
     #: Source MAC address.
     src: 'bytes' = BytesField(length=6)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/l2tp.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/l2tp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """header schema for L2TP protocol"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.corekit.fields.misc import ConditionalField, PayloadField
 from pcapkit.corekit.fields.numbers import UInt16Field
 from pcapkit.corekit.fields.strings import BitField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = ['L2TP']
 
 if TYPE_CHECKING:
     from typing import Optional
 
@@ -33,14 +33,15 @@
         offset: int
         #: Priority of L2TP packet.
         prio: int
         #: Version of L2TP packet.
         version: Literal[2]
 
 
+@schema_final
 class L2TP(Schema):
     """Header schema for L2TP packet."""
 
     #: Flags and version of L2TP packet.
     flags: 'FlagsType' = BitField(length=2, namespace={
         'type': (0, 1),
         'len': (1, 1),
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ospf.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/ospf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pcapkit.const.ospf.authentication import Authentication as Enum_Authentication
 from pcapkit.const.ospf.packet import Packet as Enum_Packet
 from pcapkit.corekit.fields.ipaddress import IPv4AddressField
 from pcapkit.corekit.fields.misc import PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field, UInt32Field
 from pcapkit.corekit.fields.strings import BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['OSPF', 'CrytographicAuthentication']
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address
     from typing import Any
 
@@ -35,14 +35,15 @@
 
     """
     if pkt['auth_type'] == Enum_Authentication.Cryptographic_authentication:
         return SchemaField(length=8, schema=CrytographicAuthentication)
     return BytesField(length=8)
 
 
+@schema_final
 class CrytographicAuthentication(Schema):
     """Header schema for OSPF cryptographic authentication."""
 
     #: Reserved bytes.
     reserved: 'bytes' = PaddingField(length=2)
     #: Key ID.
     key_id: 'int' = UInt8Field()
@@ -51,14 +52,15 @@
     #: Sequence number.
     seq: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, key_id: 'int', len: 'int', seq: 'int') -> 'None': ...
 
 
+@schema_final
 class OSPF(Schema):
     """Header schema for OSPF packet."""
 
     #: Version.
     version: 'int' = UInt8Field()
     #: Type.
     type: 'Enum_Packet' = EnumField(length=1, namespace=Enum_Packet)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/vlan.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/link/vlan.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.ethertype import EtherType as Enum_EtherType
 from pcapkit.const.vlan.priority_level import PriorityLevel as Enum_PriorityLevel
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field
 from pcapkit.corekit.fields.strings import BitField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = ['VLAN', 'TCI']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
@@ -27,28 +27,30 @@
         pcp: int
         #: Drop eligible indicator.
         dei: int
         #: VLAN identifier.
         vid: int
 
 
-class TCI(Schema[int]):
+@schema_final
+class TCI(Schema):
     """Header schema for 802.1Q Customer VLAN Tag Type tag control information."""
 
     #: Priority code point.
     pcp: 'Enum_PriorityLevel' = EnumField(length=1, bit_length=3, namespace=Enum_PriorityLevel)
     #: Drop eligible indicator.
-    dei: 'bool' = UInt8Field(bit_length=1)
+    dei: 'int' = UInt8Field(bit_length=1)
     #: VLAN identifier.
     vid: 'int' = UInt16Field(bit_length=12)
 
     if TYPE_CHECKING:
-        def __init__(self, pcp: 'Enum_PriorityLevel', dei: 'bool', vid: 'int') -> 'None': ...
+        def __init__(self, pcp: 'Enum_PriorityLevel', dei: 'int', vid: 'int') -> 'None': ...
 
 
+@schema_final
 class VLAN(Schema):
     """Header schema for 802.1Q Customer VLAN Tag Type packet."""
 
     #: Tag control information.
     tci: 'TCIType' = BitField(
         length=2,
         namespace={
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/null.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/misc/null.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
 """header schema for empty payload"""
 
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['NoPayload']
 
 
+@schema_final
 class NoPayload(Schema):
     """Schema for empty payload."""
 
     # NOTE: We add this method for both type annotation and to mark that this
     # class accepts no arguments at runtime, since :class:`Schema` explicitly
     # skipped those whose :attr:`__dict__` is empty :obj:`dict`.
     def __init__(self) -> 'None':  # pylint: disable=super-init-not-called
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/frame.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """header schema for frame header of PCAP file format"""
 
 import sys
 from typing import TYPE_CHECKING
 
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import UInt32Field
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['Frame']
 
 if TYPE_CHECKING:
     from typing import Any
 
     from pcapkit.corekit.fields.numbers import NumberField as Field
@@ -25,14 +25,15 @@
         field: Field instance.
         packet: Packet data.
 
     """
     field._byteorder = packet.get('byteorder', sys.byteorder)
 
 
+@schema_final
 class Frame(Schema):
     """Frame header of PCAP file format."""
 
     __payload__ = 'packet'
 
     #: Timestamp seconds.
     ts_sec: 'int' = UInt32Field(callback=byteorder_callback)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/header.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcap/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """header schema for global header of PCAP file format"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.linktype import LinkType as Enum_LinkType
 from pcapkit.corekit.fields.numbers import EnumField, Int32Field, UInt16Field, UInt32Field
 from pcapkit.corekit.fields.strings import BytesField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import ProtocolError
 
 __all__ = ['Header']
 
 if TYPE_CHECKING:
     from typing import Any
 
@@ -35,14 +35,15 @@
         field._byteorder = 'little'
     elif magic_number == b'\xa1\xb2\x3c\x4d':
         field._byteorder = 'big'
     else:
         raise ProtocolError('invalid magic number')
 
 
+@schema_final
 class Header(Schema):
     """Global header of PCAP file."""
 
     #: Magic number.
     magic_number: 'bytes' = BytesField(length=4)
     #: Version number major.
     version_major: 'int' = UInt16Field(callback=magic_number_callback)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcapng.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/misc/pcapng.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pcapkit.corekit.fields.ipaddress import (IPv4AddressField, IPv4InterfaceField,
                                               IPv6AddressField, IPv6InterfaceField)
 from pcapkit.corekit.fields.misc import ForwardMatchField, PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import (EnumField, Int32Field, Int64Field, NumberField,
                                             UInt8Field, UInt16Field, UInt32Field, UInt64Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField, StringField
 from pcapkit.corekit.multidict import MultiDict, OrderedMultiDict
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldValueError, ProtocolError, stacklevel
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 from pcapkit.utilities.warnings import ProtocolWarning, warn
 
 __all__ = [
     'PCAPNG',
 
@@ -304,14 +304,15 @@
             Processed field value.
 
         """
         value = super(EnumField, self).post_process(value, packet)
         return self._namespace.get(value, namespace=self._opt_ns)
 
 
+@schema_final
 class PCAPNG(Schema):
     """Header schema for PCAP-NG file blocks."""
 
     #: Block type.
     type: 'Enum_BlockType' = EnumField(length=4, namespace=Enum_BlockType, callback=byteorder_callback)
     #: Block specific data.
     block: 'BlockType' = SwitchField(
@@ -347,14 +348,15 @@
         return self
 
     if TYPE_CHECKING:
         length: int
         length2: int
 
 
+@schema_final
 class UnknownBlock(BlockType):
     """Header schema for unknown PCAP-NG file blocks."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Block body (including padding).
     body: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 12)
@@ -380,59 +382,64 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='opt', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class UnknownOption(_OPT_Option):
     """Header schema for unknown PCAP-NG file options."""
 
     #: Option value.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EndOfOption(_OPT_Option):
     """Header schema for PCAP-NG file ``opt_endofopt`` options."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int') -> 'None': ...
 
 
+@schema_final
 class CommentOption(_OPT_Option):
     """Header schema for PCAP-NG file ``opt_comment`` options."""
 
     #: Comment text.
     comment: 'str' = StringField(length=lambda pkt: pkt['length'], encoding='utf-8')
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', comment: 'str') -> 'None': ...
 
 
+@schema_final
 class CustomOption(_OPT_Option):
     """Header schema for PCAP-NG file ``opt_custom`` options."""
 
     #: Private enterprise number (PEN).
     pen: 'int' = UInt32Field(callback=byteorder_callback)
     #: Custom data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 4)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'int', length: 'int', pen: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class SectionHeaderBlock(BlockType):
     """Header schema for PCAP-NG Section Header Block (SHB)."""
 
     #: Fast forward field to test the byteorder.
     match: 'ByteorderTest' = ForwardMatchField(BitField(length=8, namespace={
         'byteorder': (32, 32),
     }))
@@ -525,98 +532,106 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='if', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class IF_NameOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_name`` options."""
 
     #: Interface name.
     name: 'str' = StringField(length=lambda pkt: pkt['length'], encoding='utf-8')
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', name: 'str') -> 'None': ...
 
 
+@schema_final
 class IF_DescriptionOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_description`` options."""
 
     #: Interface description.
     description: 'str' = StringField(length=lambda pkt: pkt['length'], encoding='utf-8')
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', description: 'str') -> 'None': ...
 
 
+@schema_final
 class IF_IPv4AddrOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_IPv4addr`` options."""
 
     #: IPv4 interface.
     interface: 'IPv4Interface' = IPv4InterfaceField()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'IPv4Interface | str') -> 'None': ...
 
 
+@schema_final
 class IF_IPv6AddrOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_IPv6addr`` options."""
 
     #: IPv6 interface.
     interface: 'IPv6Interface' = IPv6InterfaceField()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'IPv6Interface | str') -> 'None': ...
 
 
+@schema_final
 class IF_MACAddrOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_MACaddr`` options."""
 
     #: MAC interface.
     interface: 'bytes' = BytesField(length=6)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'bytes') -> 'None': ...
 
 
+@schema_final
 class IF_EUIAddrOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_EUIaddr`` options."""
 
     #: EUI interface.
     interface: 'bytes' = BytesField(length=8)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', interface: 'bytes') -> 'None': ...
 
 
+@schema_final
 class IF_SpeedOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_speed`` options."""
 
     #: Interface speed, in bits per second.
     speed: 'int' = UInt64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', speed: 'int') -> 'None': ...
 
 
+@schema_final
 class IF_TSResolOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_tsresol`` options."""
 
     #: Interface timestamp resolution, in units per second.
     tsresol: 'ResolutionData' = BitField(length=1, namespace={
         'flag': (0, 1),
         'resolution': (1, 7),
@@ -641,112 +656,121 @@
     if TYPE_CHECKING:
         #: Interface timestamp resolution, in units per second.
         resolution: 'int'
 
         def __init__(self, type: 'Enum_OptionType', length: 'int', tsresol: 'ResolutionData') -> 'None': ...
 
 
+@schema_final
 class IF_TZoneOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_tzone`` options."""
 
     #: Interface time zone (as in seconds difference from GMT).
     tzone: 'int' = Int32Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', tzone: 'int') -> 'None': ...
 
 
+@schema_final
 class IF_FilterOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_filter`` options."""
 
     #: Filter code.
     code: 'Enum_FilterType' = EnumField(length=1, namespace=Enum_FilterType, callback=byteorder_callback)
     #: Capture filter.
     filter: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 1)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', code: 'Enum_FilterType', filter: 'bytes') -> 'None': ...
 
 
+@schema_final
 class IF_OSOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_os`` options."""
 
     #: OS information.
     os: 'str' = StringField(length=lambda pkt: pkt['length'], encoding='utf-8')
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', os: 'str') -> 'None': ...
 
 
+@schema_final
 class IF_FCSLenOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_fcslen`` options."""
 
     #: FCS length.
     fcslen: 'int' = UInt8Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', fcslen: 'int') -> 'None': ...
 
 
+@schema_final
 class IF_TSOffsetOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_tsoffset`` options."""
 
     #: Timestamp offset (in seconds).
     tsoffset: 'int' = Int64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', tsoffset: 'int') -> 'None': ...
 
 
+@schema_final
 class IF_HardwareOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_hardware`` options."""
 
     #: Hardware information.
     hardware: 'str' = StringField(length=lambda pkt: pkt['length'], encoding='utf-8')
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', hardware: 'str') -> 'None': ...
 
 
+@schema_final
 class IF_TxSpeedOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_txspeed`` options."""
 
     #: Interface transmit speed, in bits per second.
     tx_speed: 'int' = UInt64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', tx_speed: 'int') -> 'None': ...
 
 
+@schema_final
 class IF_RxSpeedOption(_IF_Option):
     """Header schema for PCAP-NG file ``if_rxspeed`` options."""
 
     #: Interface receive speed, in bits per second.
     rx_speed: 'int' = UInt64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', rx_speed: 'int') -> 'None': ...
 
 
+@schema_final
 class InterfaceDescriptionBlock(BlockType):
     """Header schema for PCAP-NG Interface Description Block (IDB)."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Link type.
     linktype: 'Enum_LinkType' = EnumField(length=2, namespace=Enum_LinkType, callback=byteorder_callback)
@@ -800,14 +824,15 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='epb', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class EPB_FlagsOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_flags`` options."""
 
     #: Flags.
     flags: 'EPBFlags' = BitField(length=4, namespace={
         'direction': (0, 2),
         'reception': (2, 3),
@@ -824,78 +849,84 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', flags: 'EPBFlags') -> 'None': ...
 
 
+@schema_final
 class EPB_HashOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_hash`` options."""
 
     #: Hash algorithm.
     func: 'Enum_HashAlgorithm' = EnumField(length=1, namespace=Enum_HashAlgorithm, callback=byteorder_callback)
     #: Hash value.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 1)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', func: 'Enum_HashAlgorithm', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EPB_DropCountOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_dropcount`` options."""
 
     #: Number of packets dropped by the interface.
     drop_count: 'int' = UInt64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', drop_count: 'int') -> 'None': ...
 
 
+@schema_final
 class EPB_PacketIDOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_packetid`` options."""
 
     #: Packet ID.
     packet_id: 'int' = UInt64Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packet_id: 'int') -> 'None': ...
 
 
+@schema_final
 class EPB_QueueOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_queue`` options."""
 
     #: Queue ID.
     queue_id: 'int' = UInt32Field(callback=byteorder_callback)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', queue_id: 'int') -> 'None': ...
 
 
+@schema_final
 class EPB_VerdictOption(_EPB_Option):
     """Header schema for PCAP-NG ``epb_verdict`` options."""
 
     #: Verdict type.
     verdict: 'Enum_VerdictType' = EnumField(length=1, namespace=Enum_VerdictType, callback=byteorder_callback)
     #: Verdict value.
     value: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 1)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', verdict: 'Enum_VerdictType', value: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EnhancedPacketBlock(BlockType):
     """Header schema for PCAP-NG Enhanced Packet Block (EPB)."""
 
     __payload__ = 'packet_data'
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
@@ -942,14 +973,15 @@
     if TYPE_CHECKING:
         def __init__(self, length: 'int', interface_id: 'int', timestamp_high: 'int',
                      timestamp_low: 'int', captured_len: 'int', original_len: 'int',
                      packet_data: 'bytes | Protocol | Schema',
                      options: 'list[Option | bytes] | bytes', length2: 'int') -> 'None': ...
 
 
+@schema_final
 class SimplePacketBlock(BlockType):
     """Header schema for PCAP-NG Simple Packet Block (SPB)."""
 
     __payload__ = 'packet_data'
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
@@ -974,33 +1006,36 @@
 
     #: Record type.
     type: 'Enum_RecordType' = EnumField(length=2, namespace=Enum_RecordType, callback=byteorder_callback)
     #: Record value length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class UnknownRecord(NameResolutionRecord):
     """Header schema for PCAP-NG NRB unknown records."""
 
     #: Unknown record data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EndRecord(NameResolutionRecord):
     """Header schema for PCAP-NG ``nrb_record_end`` records."""
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_RecordType', length: 'int') -> 'None': ...
 
 
+@schema_final
 class IPv4Record(NameResolutionRecord):
     """Header schema for PCAP-NG NRB ``nrb_record_ipv4`` records."""
 
     #: IPv4 address.
     ip: 'IPv4Address' = IPv4AddressField()
     #: Name resolution data.
     resol: 'str' = StringField(length=lambda pkt: pkt['length'] - 4)
@@ -1023,14 +1058,15 @@
     if TYPE_CHECKING:
         #: Name resolution records.
         names: 'list[str]'
 
         def __init__(self, type: 'Enum_RecordType', length: 'int', ip: 'IPv4Address | str | bytes | int', resol: 'str') -> 'None': ...
 
 
+@schema_final
 class IPv6Record(NameResolutionRecord):
     """Header schema for PCAP-NG NRB ``nrb_record_ipv4`` records."""
 
     #: IPv4 address.
     ip: 'IPv6Address' = IPv6AddressField()
     #: Name resolution data.
     resol: 'str' = StringField(length=lambda pkt: pkt['length'] - 4)
@@ -1062,44 +1098,48 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='ns', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class NS_DNSNameOption(_NS_Option):
     """Header schema for PCAP-NG ``ns_dnsname`` option."""
 
     #: DNS name.
     name: 'str' = StringField(length=lambda pkt: pkt['length'])
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', name: 'str') -> 'None': ...
 
 
+@schema_final
 class NS_DNSIP4AddrOption(_NS_Option):
     """Header schema for PCAP-NG ``ns_dnsIP4addr`` option."""
 
     #: IPv4 address.
     ip: 'IPv4Address' = IPv4AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', ip: 'IPv4Address | str | bytes | int') -> 'None': ...
 
 
+@schema_final
 class NS_DNSIP6AddrOption(_NS_Option):
     """Header schema for PCAP-NG ``ns_dnsIP6addr`` option."""
 
     #: IPv6 address.
     ip: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', ip: 'IPv6Address | bytes | str | int') -> 'None': ...
 
 
+@schema_final
 class NameResolutionBlock(BlockType):
     """Header schema for PCAP-NG Name Resolution Block (NRB)."""
 
     #: Record total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Name resolution records.
     records: 'list[NameResolutionRecord]' = OptionField(
@@ -1177,88 +1217,96 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='isb', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class ISB_StartTimeOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_starttime`` option."""
 
     #: Timestamp (higher 32 bits).
     timestamp_high: 'int' = UInt32Field(callback=byteorder_callback)
     #: Timestamp (lower 32 bits).
     timestamp_low: 'int' = UInt32Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', timestamp_high: 'int', timestamp_low: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_EndTimeOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_endtime`` option."""
 
     #: Timestamp (higher 32 bits).
     timestamp_high: 'int' = UInt32Field(callback=byteorder_callback)
     #: Timestamp (lower 32 bits).
     timestamp_low: 'int' = UInt32Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', timestamp_high: 'int', timestamp_low: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_IFRecvOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_ifrecv`` option."""
 
     #: Number of packets received.
     packets: 'int' = UInt64Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_IFDropOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_ifdrop`` option."""
 
     #: Number of packets dropped.
     packets: 'int' = UInt64Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_FilterAcceptOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_filteraccept`` option."""
 
     #: Number of packets accepted by filter.
     packets: 'int' = UInt64Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_OSDropOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_osdrop`` option."""
 
     #: Number of packets dropped by OS.
     packets: 'int' = UInt64Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@schema_final
 class ISB_UsrDelivOption(_ISB_Option):
     """Header schema for PCAP-NG ``isb_usrdeliv`` option."""
 
     #: Number of packets delivered to user.
     packets: 'int' = UInt64Field(callback=byteorder_callback)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', packets: 'int') -> 'None': ...
 
 
+@schema_final
 class InterfaceStatisticsBlock(BlockType):
     """Header schema for PCAP-NG Interface Statistics Block (ISB)."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Interface ID.
     interface_id: 'int' = UInt32Field(callback=byteorder_callback)
@@ -1295,14 +1343,15 @@
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', interface_id: 'int',
                      timestamp_high: 'int', timestamp_low: 'int',
                      options: 'list[Option | bytes] | bytes', length2: 'int') -> 'None': ...
 
 
+@schema_final
 class SystemdJournalExportBlock(BlockType):
     """Header schema for PCAP-NG :manpage:`systemd(1)` Journal Export Block."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Journal entry.
     entry: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 12)
@@ -1351,24 +1400,26 @@
         def __init__(self, length: 'int', entry: 'bytes', length2: 'int') -> 'None': ...
 
 
 class DSBSecrets(Schema):
     """Header schema for DSB secrets data."""
 
 
+@schema_final
 class UnknownSecrets(DSBSecrets):
     """Header schema for unknown DSB secrets data."""
 
     #: Secrets data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class TLSKeyLog(DSBSecrets):
     """Header schema for TLS Key Log secrets data."""
 
     #: TLS key log data.
     data: 'str' = StringField(length=lambda pkt: pkt['__length__'], encoding='ascii')
 
     def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
@@ -1399,14 +1450,15 @@
     if TYPE_CHECKING:
         #: TLS Key Log entries.
         entries: 'dict[TLSKeyLabel, OrderedMultiDict[bytes, bytes]]'
 
         def __init__(self, data: 'str') -> 'None': ...
 
 
+@schema_final
 class WireGuardKeyLog(DSBSecrets):
     """Header schema for WireGuard Key Log secrets data."""
 
     #: WireGuard key log data.
     data: 'str' = StringField(length=lambda pkt: pkt['__length__'], encoding='ascii')
 
     def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
@@ -1438,28 +1490,30 @@
     if TYPE_CHECKING:
         #: WireGuard Key Log entries.
         entries: 'OrderedMultiDict[WireGuardKeyLabel, bytes]'
 
         def __init__(self, data: 'str') -> 'None': ...
 
 
+@schema_final
 class ZigBeeNWKKey(DSBSecrets):
     """Header schema for ZigBee NWK Key and ZigBee PANID secrets data."""
 
     #: AES-128 NKW key.
     key: 'bytes' = BytesField(length=16)
     #: ZigBee PANID.
     panid: 'int' = UInt16Field(byteorder='little')
     #: Padding.
     padding: 'bytes' = BytesField(length=2)
 
     if TYPE_CHECKING:
         def __init__(self, key: 'bytes', panid: 'int') -> 'None': ...
 
 
+@schema_final
 class ZigBeeAPSKey(DSBSecrets):
     """Header schema for ZigBee APS Key secrets data."""
 
     #: AES-128 APS key.
     key: 'bytes' = BytesField(length=16)
     #: ZigBee PANID.
     panid: 'int' = UInt16Field(byteorder='little')
@@ -1479,14 +1533,15 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='dsb', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class DecryptionSecretsBlock(BlockType):
     """Header schema for PCAP-NG Decryption Secrets Block (DSB)."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Secrets type.
     secrets_type: 'Enum_SecretsType' = EnumField(length=4, namespace=Enum_SecretsType, callback=byteorder_callback)
@@ -1520,14 +1575,15 @@
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', secrets_type: 'Enum_SecretsType',
                      secrets_length: 'int', secrets_data: 'DSBSecrets | bytes',
                      options: 'list[Option | bytes] | bytes', length2: 'int') -> 'None': ...
 
 
+@schema_final
 class CustomBlock(BlockType):
     """Header schema for PCAP-NG Custom Block (CB)."""
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
     #: Private enterprise number.
     pen: 'int' = UInt32Field(callback=byteorder_callback)
@@ -1547,14 +1603,15 @@
 
     #: Option type.
     type: 'Enum_OptionType' = OptionEnumField(length=2, namespace='pack', callback=byteorder_callback)
     #: Option data length.
     length: 'int' = UInt16Field(callback=byteorder_callback)
 
 
+@schema_final
 class PACK_FlagsOption(_PACK_Option):
     """Header schema for PCAP-NG ``pack_flags`` options."""
 
     #: Flags.
     flags: 'PACKFlags' = BitField(length=4, namespace={
         'direction': (0, 2),
         'reception': (2, 3),
@@ -1571,28 +1628,30 @@
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', flags: 'EPBFlags') -> 'None': ...
 
 
+@schema_final
 class PACK_HashOption(_PACK_Option):
     """Header schema for PCAP-NG ``pack_hash`` options."""
 
     #: Hash algorithm.
     func: 'Enum_HashAlgorithm' = EnumField(length=1, namespace=Enum_HashAlgorithm, callback=byteorder_callback)
     #: Hash value.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 1)
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (4 - pkt['length'] % 4) % 4)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_OptionType', length: 'int', func: 'Enum_HashAlgorithm', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class PacketBlock(BlockType):
     """Header schema for PCAP-NG Packet Block (obsolete)."""
 
     __payload__ = 'packet_data'
 
     #: Block total length.
     length: 'int' = UInt32Field(callback=byteorder_callback)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/raw.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/application/httpv1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
-"""header schema for raw packet"""
+"""header schema for HTTP/1.* protocol"""
 
 from typing import TYPE_CHECKING
 
-from pcapkit.corekit.fields.misc import PayloadField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.corekit.fields.strings import BytesField
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
-__all__ = ['Raw']
+__all__ = ['HTTP']
 
-if TYPE_CHECKING:
-    from pcapkit.protocols.protocol import Protocol
 
-
-class Raw(Schema):
-    """Schema for raw packet."""
+@schema_final
+class HTTP(Schema):
+    """Header schema for HTTP/1.\* packet."""
 
     #: Packet data.
-    packet: 'bytes' = PayloadField(length=lambda x: x['__length__'], default=b'')
+    data: 'bytes' = BytesField(lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
-        def __init__(self, packet: 'bytes | Schema | Protocol') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
+        def __init__(self, data: 'bytes') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/schema.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,146 @@
 # -*- coding: utf-8 -*-
 """schema for protocol headers"""
 
 import collections
 import collections.abc
 import io
 import itertools
-from typing import TYPE_CHECKING, Generic, TypeVar, cast
+from typing import TYPE_CHECKING, Generic, TypeVar, cast, final
 
 from pcapkit.corekit.fields.collections import ListField, OptionField
 from pcapkit.corekit.fields.field import NoValue, _Field
 from pcapkit.corekit.fields.misc import ConditionalField, ForwardMatchField, PayloadField
 from pcapkit.corekit.fields.strings import PaddingField
 from pcapkit.utilities.compat import Mapping
 from pcapkit.utilities.decorators import prepare
 from pcapkit.utilities.exceptions import NoDefaultValue, ProtocolUnbound, stacklevel
 from pcapkit.utilities.warnings import SchemaWarning, UnknownFieldWarning, warn
 
 if TYPE_CHECKING:
     from collections import OrderedDict
-    from typing import IO, Any, Iterable, Iterator, Optional
+    from typing import IO, Any, Iterable, Iterator, Optional, Type
 
     from typing_extensions import Self
 
-__all__ = ['Schema']
+__all__ = ['Schema', 'schema_final']
 
 VT = TypeVar('VT')
 
 
+def schema_final(cls: 'Type[Schema[VT]]') -> 'Type[Schema[VT]]':
+    """Finalise schema class.
+
+    Args:
+        cls: Schema class.
+
+    Returns:
+        Finalised schema class.
+
+    Notes:
+        This decorator function is used to generate necessary
+        attributes and methods for the decorated :class:`Schema`
+        class. It can be useful to reduce runtime generation
+        time as well as caching already generated attributes.
+
+    :meta decorator:
+    """
+    if cls.__finalised__:
+        warn(f'{cls.__name__}: schema has been finalised; now skipping',
+             SchemaWarning, stacklevel=stacklevel())
+        return cls
+
+    temp = ['__map__', '__map_reverse__', '__builtin__',
+            '__fields__', '__buffer__', '__updated__',
+            '__payload__', '__finalised__']
+    temp.extend(cls.__additional__)
+    for obj in cls.mro():
+        temp.extend(dir(obj))
+    cls.__builtin__ = set(temp)
+    cls.__excluded__.extend(cls.__builtin__)
+
+    args_ = []  # type: list[str]
+    dict_ = []  # type: list[str]
+
+    cls_fields = []  # type: list[tuple[str, _Field]]
+    for cls_ in cls.mro():
+        # NOTE: We skip the ``Schema`` class itself, to avoid superclass
+        # type annotations being considered.
+        if cls_ is Schema:
+            break
+
+        # NOTE: We iterate in reversed order to ensure that the type
+        # annotations of the superclasses are considered first.
+        for key in reversed(cls_.__dict__):
+            # NOTE: We skip duplicated annotations to avoid duplicate
+            # argument in function definition.
+            if key in args_:
+                continue
+
+            # NOTE: We only consider the fields that are instances of
+            # the ``_Field`` class.
+            field = cls_.__dict__[key]
+            if not isinstance(field, _Field):
+                continue
+
+            # NOTE: We need to consider the case where the field itself
+            # is optional, i.e., the field is not required to be present
+            # in the protocol header.
+            args_.append(f'{key}=NoValue')
+            dict_.append(f'{key}={key}')
+
+            field.name = key
+            cls_fields.append((key, field))
+
+    # NOTE: We reverse the two lists such that the order of the
+    # arguments is the same as the order of the field definition,
+    # i.e., from the most base class to the most derived class.
+    args_.reverse()
+    dict_.reverse()
+
+    # NOTE: We also reverse the field list such that the order
+    # can be preserved in the :class:`~collections.OrderedDict`
+    # instance.
+    cls_fields.reverse()
+    cls.__fields__ = collections.OrderedDict(cls_fields)
+
+    # NOTE: We shall only attempt to generate ``__init__`` method
+    # if the class does not define such method.
+    if not hasattr(cls, '__init__'):
+        # NOTE: We only generate typed ``__init__`` method if only the class
+        # has field definition from any of itself and its base classes.
+        if args_:
+            # NOTE: The following code is to make the ``__init__`` method work.
+            # It is inspired from the :func:`dataclasses._create_fn` function.
+            init_ = (
+                f'def __create_fn__():\n'
+                f'    def __init__(self, {", ".join(args_)}, *, __packet__=None):\n'
+                f'        self.__update__({", ".join(dict_)})\n'
+                f'        self.__post_init__(__packet__)\n'
+                f'    return __init__\n'
+            )
+        else:
+            init_ = (
+                'def __create_fn__():\n'
+                '    def __init__(self, dict_=None, *, __packet__=None, **kwargs):\n'
+                '        self.__update__(dict_, **kwargs)\n'
+                '        self.__post_init__(__packet__)\n'
+                '    return __init__\n'
+            )
+
+        ns = {}  # type: dict[str, Any]
+        exec(init_, None, ns)  # pylint: disable=exec-used # nosec
+
+        cls.__init__ = ns['__create_fn__']()
+        cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
+
+    cls.__finalised__ = True
+    return final(cls)
+
+
 class Schema(Mapping[str, VT], Generic[VT]):
     """Schema for protocol headers."""
 
     if TYPE_CHECKING:
         #: Mapping of name conflicts with builtin methods (original names to
         #: transformed names).
         __map__: 'dict[str, str]'
@@ -42,14 +152,17 @@
         #: Mapping of fields.
         __fields__: 'OrderedDict[str, _Field]'
         #: Mapping of field names to packed values.
         __buffer__: 'dict[str, bytes]'
         #: Flag for whether the schema is recently updated.
         __updated__: 'bool'
 
+    #: Flag for finalised class initialisation.
+    __finalised__ = False
+
     #: Field name of the payload.
     __payload__: 'str' = 'payload'
     #: List of additional built-in names.
     __additional__: 'list[str]' = []
     #: List of names to be excluded from :obj:`dict` conversion.
     __excluded__: 'list[str]' = []
 
@@ -61,103 +174,28 @@
         which is inspired by :pep:`557` (:mod:`dataclasses`).
 
         Args:
             *args: Arbitrary positional arguments.
             **kwargs: Arbitrary keyword arguments.
 
         """
-        cls_fields = []
-
-        temp = ['__map__', '__map_reverse__', '__builtin__',
-                '__fields__', '__buffer__', '__updated__',
-                '__payload__']
-        temp.extend(cls.__additional__)
-        for obj in cls.mro():
-            temp.extend(dir(obj))
-        cls.__builtin__ = set(temp)
-        cls.__excluded__.extend(cls.__builtin__)
-
-        args_ = []  # type: list[str]
-        dict_ = []  # type: list[str]
-
-        for cls_ in cls.mro():
-            # NOTE: We skip the ``Schema`` class itself, to avoid superclass
-            # type annotations being considered.
-            if cls_ is Schema:
-                break
-
-            # NOTE: We iterate in reversed order to ensure that the type
-            # annotations of the superclasses are considered first.
-            for key in reversed(cls_.__dict__):
-                # NOTE: We skip duplicated annotations to avoid duplicate
-                # argument in function definition.
-                if key in args_:
-                    continue
-
-                # NOTE: We only consider the fields that are instances of
-                # the ``_Field`` class.
-                field = cls_.__dict__[key]
-                if not isinstance(field, _Field):
-                    continue
-
-                # NOTE: We need to consider the case where the field itself
-                # is optional, i.e., the field is not required to be present
-                # in the protocol header.
-                args_.append(f'{key}=NoValue')
-                dict_.append(f'{key}={key}')
-
-                field.name = key
-                cls_fields.append((key, field))
-
-        # NOTE: We reverse the two lists such that the order of the
-        # arguments is the same as the order of the type annotations, i.e.,
-        # from the most base class to the most derived class.
-        args_.reverse()
-        dict_.reverse()
-        cls_fields.reverse()
-        cls.__fields__ = collections.OrderedDict(cls_fields)
-
-        # NOTE: We only generate typed ``__init__`` method if only the class
-        # has type annotations from any of itself and its base classes.
-        if args_:
-            # NOTE: The following code is to make the ``__init__`` method work.
-            # It is inspired from the :func:`dataclasses._create_fn` function.
-            init_ = (
-                f'def __create_fn__():\n'
-                f'    def __init__(self, {", ".join(args_)}, *, __packet__=None):\n'
-                f'        self.__update__({", ".join(dict_)})\n'
-                f'        self.__post_init__(__packet__)\n'
-                f'    return __init__\n'
-            )
-        else:
-            init_ = (
-                'def __create_fn__():\n'
-                '    def __init__(self, dict_=None, **kwargs, *, __packet__=None):\n'
-                '        self.__update__(dict_, **kwargs)\n'
-                '        self.__post_init__(__packet__)\n'
-                '    return __init__\n'
-            )
-
-        ns = {}  # type: dict[str, Any]
-        exec(init_, None, ns)  # pylint: disable=exec-used # nosec
-        cls.__init__ = ns['__create_fn__']()
-        cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
-
+        if not cls.__finalised__:
+            cls = cast('Type[Self]', schema_final(cls))
         self = super().__new__(cls)
 
         # NOTE: We define the ``__map__`` and ``__map_reverse__`` attributes
         # here under ``self`` to avoid them being considered as class variables
         # and thus being shared by all instances.
         super().__setattr__(self, '__map__', {})
         super().__setattr__(self, '__map_reverse__', {})
 
         # NOTE: We only create the attributes for the instance itself,
         # to avoid creating shared attributes for the class.
-        self.__buffer__ = {name: b'' for name in self.__fields__.keys()}
-        self.__updated__ = True
+        super().__setattr__(self, '__buffer__', {name: b'' for name in self.__fields__.keys()})
+        super().__setattr__(self, '__updated__', True)
 
         return self
 
     def __post_init__(self, packet: 'Optional[dict[str, Any]]' = None) -> 'None':
         for name, field in self.__fields__.items():
             if self.__dict__[name] in (NoValue, None):
                 self.__dict__[name] = field.default
@@ -456,14 +494,20 @@
             Unpacked data as :class:`Schema`.
 
         Notes:
             We used a ``__length__`` key in ``packet`` to record the length
             of the remaining data, which is used to determine the length of
             the payload field.
 
+            And a ``__padding_length__`` key in the ``packet`` to record the
+            length of the padding field after an
+            :class:`~pcapkit.corekit.fields.collections.OptionField`, which
+            is used to potentially determine the length of the remaining
+            padding field data.
+
         """
         # force cast arg type since decorator changed their signatures
         if TYPE_CHECKING:
             data = cast('IO[bytes]', data)
             length = cast('int', length)
             packet = cast('dict[str, Any]', packet)
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/tcp.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/transport/tcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pcapkit.corekit.fields.collections import ListField, OptionField
 from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, PayloadField,
                                          SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field, UInt64Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 from pcapkit.utilities.exceptions import FieldError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
     'TCP',
 
     'Option',
@@ -268,202 +268,222 @@
         """
         # for EOOL/NOP option, length is always 1
         if self.kind in (Enum_Option.End_of_Option_List, Enum_Option.No_Operation):
             self.length = 1
         return self
 
 
+@schema_final
 class UnassignedOption(Option):
     """Header schema for TCP unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EndOfOptionList(Option):
     """Header schema for TCP end of option list."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int') -> 'None': ...
 
 
+@schema_final
 class NoOperation(Option):
     """Header schema for TCP no operation."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int') -> 'None': ...
 
 
+@schema_final
 class MaximumSegmentSize(Option):
     """Header schema for TCP max segment size option."""
 
     #: Maximum segment size.
     mss: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', mss: 'int') -> 'None': ...
 
 
+@schema_final
 class WindowScale(Option):
     """Header schema for TCP window scale option."""
 
     #: Window scale (shift count).
     shift: 'int' = UInt8Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', scale: 'int') -> 'None': ...
 
 
+@schema_final
 class SACKPermitted(Option):
     """Header schema for TCP SACK permitted option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int') -> 'None': ...
 
 
+@schema_final
 class SACKBlock(Schema):
     """Header schema for TCP SACK option data."""
 
     #: Left edge of the block.
     left: 'int' = UInt32Field()
     #: Right edge of the block.
     right: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, left: 'int', right: 'int') -> 'None': ...
 
 
+@schema_final
 class SACK(Option):
     """Header schema for TCP SACK option."""
 
     #: Selected ACK data.
     sack: 'list[SACKBlock]' = ListField(
         length=lambda pkt: pkt['length'] - 2,
         item_type=SchemaField(length=8, schema=SACKBlock),
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', sack: 'list[SACKBlock]') -> 'None': ...
 
 
+@schema_final
 class Echo(Option):
     """Header schema for TCP echo option."""
 
     #: Info to be echoed.
     data: 'bytes' = BytesField(length=4)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class EchoReply(Option):
     """Header schema for TCP echo reply option."""
 
     #: Echoed info.
     data: 'bytes' = BytesField(length=4)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class Timestamp(Option):
     """Header schema for TCP timestamps option."""
 
     #: Timestamp value.
     value: 'int' = UInt32Field()
     #: Timestamp echo reply.
     reply: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', value: 'int', reply: 'int') -> 'None': ...
 
 
+@schema_final
 class PartialOrderConnectionPermitted(Option):
     """Header schema for TCP partial order connection permitted option."""
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int') -> 'None': ...
 
 
+@schema_final
 class PartialOrderConnectionProfile(Option):
     """Header schema for TCP partial order connection service profile option."""
 
     #: Profile data.
     profile: 'POCProfile' = BitField(length=1, namespace={
         'start': (0, 1),
         'end': (1, 1),
     })
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', profile: 'POCProfile') -> 'None': ...
 
 
+@schema_final
 class CC(Option):
     """Header schema for TCP CC option."""
 
     #: Connection count.
     count: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', count: 'int') -> 'None': ...
 
 
+@schema_final
 class CCNew(Option):
     """Header schema for TCP connection count (new) option."""
 
     #: Connection count.
     count: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', count: 'int') -> 'None': ...
 
 
+@schema_final
 class CCEcho(Option):
     """Header schema for TCP connection count (echo) option."""
 
     #: Connection count.
     count: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', count: 'int') -> 'None': ...
 
 
+@schema_final
 class AlternateChecksumRequest(Option):
     """Header schema for TCP alternate checksum request option."""
 
     #: Checksum algorithm.
     algorithm: 'Enum_Checksum' = EnumField(length=1, namespace=Enum_Checksum)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', algorithm: 'Enum_Checksum') -> 'None': ...
 
 
+@schema_final
 class AlternateChecksumData(Option):
     """Header schema for TCP alternate checksum data option."""
 
     #: Checksum data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class MD5Signature(Option):
     """Header schema for TCP MD5 signature option."""
 
     #: MD5 digest.
     digest: 'bytes' = BytesField(length=16)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', digest: 'bytes') -> 'None': ...
 
 
+@schema_final
 class QuickStartResponse(Option):
     """Header schema for TCP quick start response option."""
 
     #: Flags.
     flags: 'QuickStartFlags' = BitField(length=1, namespace={
         'rate': (4, 4),
     })
@@ -474,41 +494,44 @@
         'nonce': (0, 30),
     })
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', flags: 'QuickStartFlags', diff: 'int', nonce: 'QuickStartNonce') -> 'None': ...
 
 
+@schema_final
 class UserTimeout(Option):
     """Header schema for TCP user timeout option."""
 
     #: Granularity and user timeout.
     info: 'TimeoutInfo' = BitField(length=2, namespace={
         'granularity': (0, 1),
         'timeout': (1, 15),
     })
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', info: 'TimeoutInfo') -> 'None': ...
 
 
+@schema_final
 class Authentication(Option):
     """Header schema for TCP authentication option."""
 
     #: Key ID.
     key_id: 'int' = UInt8Field()
     #: Next key ID.
     next_key_id: 'int' = UInt8Field()
     #: MAC value.
     mac: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 4)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', key_id: 'int', next_key_id: 'int', mac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class _MPTCP(Schema):
     """Header schema for Multipath TCP options in a generic representation."""
 
     #: Subtype and flags.
     test: 'MPTCPSubtypeTest' = ForwardMatchField(BitField(length=3, namespace={
         'length': (1, 8),
         'subtype': (16, 4),
@@ -537,14 +560,15 @@
     """Header schema for Multipath TCP options."""
 
     if TYPE_CHECKING:
         #: MPTCP subtype.
         subtype: 'Enum_MPTCPOption'
 
 
+@schema_final
 class MPTCPUnknown(MPTCP):
     """Header schema for unknown Multipath TCP option."""
 
     #: Subtype and data.
     test: 'MPTCPSubtypeUnknown' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'data': (4, 4),
@@ -552,14 +576,15 @@
     #: Data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypeUnknown', data: 'bytes') -> 'None': ...
 
 
+@schema_final
 class MPTCPCapable(MPTCP):
     """Header schema for Multipath TCP capable option."""
 
     #: Subtype and version.
     test: 'MPTCPSubtypeCapable' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'version': (4, 4),
@@ -582,14 +607,15 @@
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypeCapable', flags: 'MPTCPCapableFlags', skey: 'int', rkey: 'Optional[int]') -> 'None': ...
 
 
 class MPTCPJoin(MPTCP):
     """Header schema for Multipath TCP join option."""
 
 
+@schema_final
 class MPTCPJoinSYN(MPTCPJoin):
     """Header schema for Multipath TCP join option for ``SYN`` connection."""
 
     #: Subtype and flags.
     test: 'MPTCPSubtypeJoin' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'backup': (7, 1),
@@ -601,14 +627,15 @@
     #: Sender's random number.
     nonce: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypeJoin', addr_id: 'int', token: 'int', nonce: 'int') -> 'None': ...
 
 
+@schema_final
 class MPTCPJoinSYNACK(MPTCPJoin):
     """Header schema for Multipath TCP join option for ``SYN/ACK`` connection."""
 
     #: Subtype and flags.
     test: 'MPTCPSubtypeJoin' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'backup': (7, 1),
@@ -620,14 +647,15 @@
     #: Sender's random number.
     nonce: 'int' = UInt32Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypeJoin', addr_id: 'int', hmac: 'bytes', nonce: 'int') -> 'None': ...
 
 
+@schema_final
 class MPTCPJoinACK(MPTCPJoin):
     """Header schema for Multipath TCP join option for ``ACK`` connection."""
 
     #: Subtype.
     test: 'MPTCPSubtype' = BitField(length=1, namespace={
         'subtype': (0, 4),
     })
@@ -636,14 +664,15 @@
     #: Sender's HMAC.
     hmac: 'bytes' = BytesField(length=20)
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtype', hmac: 'bytes') -> 'None': ...
 
 
+@schema_final
 class MPTCPDSS(MPTCP):
     """Header schema for Multipath TCP DSS option."""
 
     #: Subtype and flags.
     test: 'MPTCPSubtype' = BitField(length=1, namespace={
         'subtype': (0, 4),
     })
@@ -681,14 +710,15 @@
         lambda pkt: pkt['flags']['M'],
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtype', flags: 'MPTCPDSSFlags', ack: 'Optional[int]', dsn: 'Optional[int]', ssn: 'Optional[int]', dl_len: 'Optional[int]', checksum: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class MPTCPAddAddress(MPTCP):
     """Header schema for Multipath TCP add address option."""
 
     #: Subtype and IP version.
     test: 'MPTCPSubtypeAddAddress' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'version': (4, 4),
@@ -705,14 +735,15 @@
         lambda pkt: pkt['length'] in (10, 22),
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypeAddAddress', addr_id: 'int', address: 'IPv4Address | IPv6Address', port: 'Optional[int]') -> 'None': ...
 
 
+@schema_final
 class MPTCPRemoveAddress(MPTCP):
     """Header schema for Multipath TCP remove address option."""
 
     #: Subtype.
     test: 'MPTCPSubtype' = BitField(length=1, namespace={
         'subtype': (0, 4),
     })
@@ -722,14 +753,15 @@
         item_type=UInt8Field(),
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtype', addr_id: 'list[int]') -> 'None': ...
 
 
+@schema_final
 class MPTCPPriority(MPTCP):
     """Header schema for Multipath TCP priority option."""
 
     #: Subtype.
     test: 'MPTCPSubtypePriority' = BitField(length=1, namespace={
         'subtype': (0, 4),
         'backup': (7, 1),
@@ -740,55 +772,59 @@
         lambda pkt: pkt['length'] == 4,
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtypePriority', addr_id: 'Optional[int]') -> 'None': ...
 
 
+@schema_final
 class MPTCPFallback(MPTCP):
     """Header schema for Multipath TCP fallback option."""
 
     #: Subtype.
     test: 'MPTCPSubtype' = BitField(length=1, namespace={
         'subtype': (0, 4),
     })
     #: Data sequence number.
     dsn: 'int' = UInt64Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtype', dsn: 'int') -> 'None': ...
 
 
+@schema_final
 class MPTCPFastclose(MPTCP):
     """Header schema for Multipath TCP fastclose option."""
 
     #: Subtype.
     test: 'MPTCPSubtype' = BitField(length=1, namespace={
         'subtype': (0, 4),
     })
     #: Option receiver's key.
     key: 'int' = UInt64Field()
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', test: 'MPTCPSubtype', key: 'int') -> 'None': ...
 
 
+@schema_final
 class FastOpenCookie(Option):
     """"Header schema for TCP Fast Open option."""
 
     #: Cookie.
     cookie: 'bytes' = ConditionalField(
         BytesField(length=lambda pkt: pkt['length'] - 2),
         lambda pkt: pkt['length'] >= 6,
     )
 
     if TYPE_CHECKING:
         def __init__(self, kind: 'Enum_Option', length: 'int', cookie: 'Optional[bytes]') -> 'None': ...
 
 
+@schema_final
 class TCP(Schema):
     """Header schema for TCP packet."""
 
     #: Source port.
     srcport: 'int' = UInt16Field()
     #: Destination port.
     dstport: 'int' = UInt16Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/udp.py` & `pypcapkit-1.0.1/pcapkit/protocols/schema/transport/udp.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 """header schema for user datagram protocol"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import UInt16Field
 from pcapkit.corekit.fields.strings import BytesField
-from pcapkit.protocols.schema.schema import Schema
+from pcapkit.protocols.schema.schema import Schema, schema_final
 
 __all__ = ['UDP']
 
 if TYPE_CHECKING:
     from pcapkit.protocols.protocol import Protocol
 
 
+@schema_final
 class UDP(Schema):
     """Header schema for UDP packet."""
 
     #: Source port.
     srcport: 'int' = UInt16Field()
     #: Destination port.
     dstport: 'int' = UInt16Field()
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/__init__.py` & `pypcapkit-1.0.1/pcapkit/protocols/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/tcp.py` & `pypcapkit-1.0.1/pcapkit/protocols/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/transport.py` & `pypcapkit-1.0.1/pcapkit/protocols/transport/transport.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/udp.py` & `pypcapkit-1.0.1/pcapkit/protocols/transport/udp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/__init__.py` & `pypcapkit-1.0.1/pcapkit/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/dpkt.py` & `pypcapkit-1.0.1/pcapkit/toolkit/dpkt.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/pcap.py` & `pypcapkit-1.0.1/pcapkit/toolkit/pcap.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/pcapng.py` & `pypcapkit-1.0.1/pcapkit/toolkit/pcapng.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/pyshark.py` & `pypcapkit-1.0.1/pcapkit/toolkit/pyshark.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/toolkit/scapy.py` & `pypcapkit-1.0.1/pcapkit/toolkit/scapy.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 from pcapkit.foundation.reassembly.data.tcp import Packet as TCP_Packet
 from pcapkit.foundation.traceflow.data.tcp import Packet as TF_TCP_Packet
 from pcapkit.utilities.compat import ModuleNotFoundError  # pylint: disable=redefined-builtin
 from pcapkit.utilities.exceptions import ModuleNotFound, stacklevel
 from pcapkit.utilities.warnings import ScapyWarning, warn
 
 try:
-    import scapy.all as scapy_all
+    import scapy
 except ModuleNotFoundError:
-    scapy_all = None
+    scapy = None
     warn("dependency package 'Scapy' not found",
          ScapyWarning, stacklevel=stacklevel())
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address, IPv6Address
     from typing import Any
 
     from scapy.layers.inet import IP, TCP
-    from scapy.layers.inet6 import IPv6, IPv6ExtHdrFragment
+    from scapy.layers.inet6 import IPv6
     from scapy.packet import Packet
 
 __all__ = [
     'packet2chain', 'packet2dict',
     'ipv4_reassembly', 'ipv6_reassembly', 'tcp_reassembly', 'tcp_traceflow'
 ]
 
@@ -59,20 +59,21 @@
     Returns:
         Colon (``:``) seperated list of protocol chain.
 
     Raises:
         ModuleNotFound: If `Scapy`_ is not installed.
 
     """
-    if scapy_all is None:
+    if scapy is None:
         raise ModuleNotFound("No module named 'scapy'", name='scapy')
+    from scapy.packet import NoPayload
 
     chain = [packet.name]
     payload = packet.payload
-    while not isinstance(payload, scapy_all.packet.NoPayload):
+    while not isinstance(payload, NoPayload):
         chain.append(payload.name)
         payload = payload.payload
     return ':'.join(chain)
 
 
 def packet2dict(packet: 'Packet') -> 'dict[str, Any]':
     """Convert Scapy packet into :obj:`dict`.
@@ -83,21 +84,22 @@
     Returns:
         A :obj:`dict` mapping of packet data.
 
     Raises:
         ModuleNotFound: If `Scapy`_ is not installed.
 
     """
-    if scapy_all is None:
+    if scapy is None:
         raise ModuleNotFound("No module named 'scapy'", name='scapy')
+    from scapy.packet import NoPayload
 
     def wrapper(packet: 'Packet') -> 'dict[str, Any]':
         dict_ = packet.fields
         payload = packet.payload
-        if not isinstance(payload, scapy_all.packet.NoPayload):
+        if not isinstance(payload, NoPayload):
             dict_[payload.name] = wrapper(payload)
         return dict_
 
     return {
         'packet': bytes(packet),
         packet.name: wrapper(packet),
     }
@@ -168,20 +170,21 @@
     Raises:
         ModuleNotFound: If `Scapy`_ is not installed.
 
     See Also:
         :class:`pcapkit.foundation.reassembly.ipv6.IPv6`
 
     """
-    if scapy_all is None:
+    if scapy is None:
         raise ModuleNotFound("No module named 'scapy'", name='scapy')
+    from scapy.layers.inet6 import IPv6ExtHdrFragment
 
     if 'IPv6' in packet:
         ipv6 = cast('IPv6', packet['IPv6'])
-        if scapy_all.IPv6ExtHdrFragment not in ipv6:  # pylint: disable=E1101
+        if IPv6ExtHdrFragment not in ipv6:  # pylint: disable=E1101
             return None                        # dismiss not fragmented packet
         ipv6_frag = cast('IPv6ExtHdrFragment', ipv6['IPv6ExtHdrFragment'])
 
         data = IP_Packet(
             bufid=(
                 cast('IPv6Address',
                      ipaddress.ip_address(ipv6.src)),     # source IP address
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/__init__.py` & `pypcapkit-1.0.1/pcapkit/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/compat.py` & `pypcapkit-1.0.1/pcapkit/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/decorators.py` & `pypcapkit-1.0.1/pcapkit/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/exceptions.py` & `pypcapkit-1.0.1/pcapkit/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/logging.py` & `pypcapkit-1.0.1/pcapkit/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/utilities/warnings.py` & `pypcapkit-1.0.1/pcapkit/utilities/warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # UserWarning
     'BaseWarning',
     # ImportWarning
     'FormatWarning', 'EngineWarning', 'InvalidVendorWarning',
     # RuntimeWarning
     'FileWarning', 'LayerWarning', 'ProtocolWarning', 'AttributeWarning',
     'DevModeWarning', 'VendorRequestWarning', 'VendorRuntimeWarning',
-    'UnknownFieldWarning', 'RegistryWarning', 'SchemaWarning',
+    'UnknownFieldWarning', 'RegistryWarning', 'SchemaWarning', 'InfoWarning',
     # ResourceWarning
     'DPKTWarning', 'ScapyWarning', 'PySharkWarning', 'EmojiWarning',
     'VendorWarning',
     # DeprecationWarning
     'DeprecatedFormatWarning',
 ]
 
@@ -131,14 +131,18 @@
     """Registry warning."""
 
 
 class SchemaWarning(BaseWarning, RuntimeWarning):
     """Schema warning."""
 
 
+class InfoWarning(BaseWarning, RuntimeWarning):
+    """Info class warning."""
+
+
 ##############################################################################
 # ResourceWarning session.
 ##############################################################################
 
 
 class DPKTWarning(BaseWarning, ResourceWarning):
     """Warnings on DPKT usage."""
```

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/__main__.py` & `pypcapkit-1.0.1/pcapkit/vendor/__main__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/hardware.py` & `pypcapkit-1.0.1/pcapkit/vendor/arp/hardware.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/operation.py` & `pypcapkit-1.0.1/pcapkit/vendor/arp/operation.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/default.py` & `pypcapkit-1.0.1/pcapkit/vendor/default.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/command.py` & `pypcapkit-1.0.1/pcapkit/vendor/ftp/command.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/return_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/ftp/return_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/certificate.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/certificate.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/cipher.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/cipher.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/di.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/di.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_curve.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/ecdsa_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_low_curve.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/ecdsa_low_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/eddsa_curve.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/eddsa_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/esp_transform_suite.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/esp_transform_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/group.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/group.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hi_algorithm.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/hi_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hit_suite.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/hit_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/nat_traversal.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/nat_traversal.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/notify_message.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/notify_message.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/packet.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/parameter.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/parameter.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/registration.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration_failure.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/registration_failure.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/suite.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/transport.py` & `pypcapkit-1.0.1/pcapkit/vendor/hip/transport.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/error_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/error_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/frame.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/frame.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/method.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/method.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/setting.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/setting.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/http/status_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/http/status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/classification_level.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/classification_level.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_class.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/option_class.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_number.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/option_number.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/protection_authority.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/protection_authority.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/qs_function.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/qs_function.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/router_alert.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/router_alert.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_del.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_del.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_ecn.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_ecn.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_pre.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_pre.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_rel.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_rel.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_thr.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/tos_thr.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/ts_flag.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv4/ts_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/extension_header.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/extension_header.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option_action.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/option_action.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/qs_function.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/qs_function.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/router_alert.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/router_alert.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/routing.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/routing.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/seed_id.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/seed_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/smf_dpd_mode.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/smf_dpd_mode.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/tagger_id.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipv6/tagger_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipx/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/packet.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipx/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/socket.py` & `pypcapkit-1.0.1/pcapkit/vendor/ipx/socket.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/l2tp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/type.py` & `pypcapkit-1.0.1/pcapkit/vendor/l2tp/type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/access_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/access_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ack_status_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/ack_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ani_suboption.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/ani_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/auth_subtype.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/auth_subtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_ack_flag.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/binding_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_revocation.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/binding_revocation.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_update_flag.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/binding_update_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dhcp_support_mode.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/dhcp_support_mode.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dns_status_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/dns_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmip6_tls_packet.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/dsmip6_tls_packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmipv6_home_address.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/dsmipv6_home_address.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/enumerating_algorithm.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/enumerating_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_ack_status.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/fb_ack_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_action.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/fb_action.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_indication_trigger.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/fb_indication_trigger.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/fb_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_status.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/flow_id_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_suboption.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/flow_id_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handoff_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/handoff_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_flag.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/handover_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_status.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/handover_ack_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_flag.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/handover_initiate_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_status.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/handover_initiate_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/home_address_reply.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/home_address_reply.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/lma_mag_suboption.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/lma_mag_suboption.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_group_id.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/mn_group_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_id_subtype.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/mn_id_subtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/operator_id.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/operator_id.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/option.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/packet.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/qos_attribute.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/qos_attribute.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_status_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/revocation_status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_trigger.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/revocation_trigger.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/status_code.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/status_code.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/traffic_selector.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/traffic_selector.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upa_status.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/upa_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upn_reason.py` & `pypcapkit-1.0.1/pcapkit/vendor/mh/upn_reason.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/ospf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/authentication.py` & `pypcapkit-1.0.1/pcapkit/vendor/ospf/authentication.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/packet.py` & `pypcapkit-1.0.1/pcapkit/vendor/ospf/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/block_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/block_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/filter_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/filter_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/hash_algorithm.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/hash_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/option_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/option_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/record_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/record_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/secrets_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/secrets_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/verdict_type.py` & `pypcapkit-1.0.1/pcapkit/vendor/pcapng/verdict_type.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/reg/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/ethertype.py` & `pypcapkit-1.0.1/pcapkit/vendor/reg/ethertype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/linktype.py` & `pypcapkit-1.0.1/pcapkit/vendor/reg/linktype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/transtype.py` & `pypcapkit-1.0.1/pcapkit/vendor/reg/transtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/checksum.py` & `pypcapkit-1.0.1/pcapkit/vendor/tcp/checksum.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/mp_tcp_option.py` & `pypcapkit-1.0.1/pcapkit/vendor/tcp/mp_tcp_option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/option.py` & `pypcapkit-1.0.1/pcapkit/vendor/tcp/option.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/__init__.py` & `pypcapkit-1.0.1/pcapkit/vendor/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/priority_level.py` & `pypcapkit-1.0.1/pcapkit/vendor/vlan/priority_level.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pypcapkit.egg-info/PKG-INFO` & `pypcapkit-1.0.1/pypcapkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypcapkit
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: PyPCAPKit: comprehensive network packet analysis library
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: documentation, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: repository, https://github.com/JarryShaw/PyPCAPKit
@@ -156,18 +156,18 @@
 
 Test Results
 ~~~~~~~~~~~~
 
 ============= ===========================
 Engine        Performance (ms per packet)
 ============= ===========================
-``dpkt``      0.048088_922256
-``scapy``     0.127444_444444
-``pcapkit``   0.964180_847514
-``pyshark``   23.665003_003003
+``dpkt``       0.010694_027361
+``scapy``      0.093399_399399
+``pcapkit``    0.199796_296296
+``pyshark``   25.066692_025359
 ============= ===========================
 
 ------------
 Installation
 ------------
 
 .. note::
```

### Comparing `pypcapkit-1.0.0rc1/pypcapkit.egg-info/SOURCES.txt` & `pypcapkit-1.0.1/pypcapkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/pyproject.toml` & `pypcapkit-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/setup.py` & `pypcapkit-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0rc1/util/bump_version.py` & `pypcapkit-1.0.1/util/bump_version.py`

 * *Files identical despite different names*

