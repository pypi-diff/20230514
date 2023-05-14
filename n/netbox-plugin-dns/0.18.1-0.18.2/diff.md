# Comparing `tmp/netbox_plugin_dns-0.18.1.tar.gz` & `tmp/netbox_plugin_dns-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-0.18.1.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-0.18.2.tar", max compression
```

## Comparing `netbox_plugin_dns-0.18.1.tar` & `netbox_plugin_dns-0.18.2.tar`

### file list

```diff
@@ -1,155 +1,85 @@
--rw-r--r--   0        0        0     1076 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/LICENSE
--rw-r--r--   0        0        0     3096 2023-05-09 20:30:41.000000 netbox_plugin_dns-0.18.1/README.md
--rw-r--r--   0        0        0      903 2023-05-10 18:58:38.000000 netbox_plugin_dns-0.18.1/netbox_dns/__init__.py
--rw-r--r--   0        0        0      512 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/admin.py
--rw-r--r--   0        0        0     2502 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/__pycache__/nested_serializers.cpython-38.pyc
--rw-r--r--   0        0        0     3812 2023-04-02 12:40:19.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0        0        0      512 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0        0        0     3776 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0        0        0     1951 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0     4555 2022-12-22 08:12:50.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0      441 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3060 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2022-10-24 11:40:31.000000 netbox_plugin_dns-0.18.1/netbox_dns/apps.py
--rw-r--r--   0        0        0       46 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0      183 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2432 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/__pycache__/address.cpython-38.pyc
--rw-r--r--   0        0        0     3985 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/__pycache__/network.cpython-38.pyc
--rw-r--r--   0        0        0     1530 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3023 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/fields/network.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__init__.py
--rw-r--r--   0        0        0      218 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1024 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__pycache__/nameserver.cpython-38.pyc
--rw-r--r--   0        0        0     1681 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0      988 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__pycache__/view.cpython-38.pyc
--rw-r--r--   0        0        0     1437 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/__pycache__/zone.cpython-38.pyc
--rwxr-xr-x   0        0        0      596 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/nameserver.py
--rwxr-xr-x   0        0        0     1609 2022-08-18 09:11:58.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/record.py
--rw-r--r--   0        0        0      572 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/view.py
--rwxr-xr-x   0        0        0     1179 2022-10-24 11:43:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/filters/zone.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__init__.py
--rw-r--r--   0        0        0      216 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2205 2023-05-10 10:14:26.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__pycache__/nameserver.cpython-38.pyc
--rw-r--r--   0        0        0     4485 2023-05-10 10:14:26.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0     1812 2023-05-10 10:14:26.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__pycache__/view.cpython-38.pyc
--rw-r--r--   0        0        0     9595 2023-05-10 10:14:26.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/__pycache__/zone.cpython-38.pyc
--rwxr-xr-x   0        0        0     1308 2023-05-03 10:29:35.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     5083 2023-05-03 10:29:35.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/record.py
--rw-r--r--   0        0        0      961 2023-05-03 10:29:35.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    14198 2023-05-03 10:29:35.000000 netbox_plugin_dns-0.18.1/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      604 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0      758 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1020 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/nameserver.cpython-38.pyc
--rw-r--r--   0        0        0      988 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0      481 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/schema.cpython-38.pyc
--rw-r--r--   0        0        0      972 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/view.cpython-38.pyc
--rw-r--r--   0        0        0      972 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/__pycache__/zone.cpython-38.pyc
--rw-r--r--   0        0        0      527 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/nameserver.py
--rw-r--r--   0        0        0      487 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/record.py
--rw-r--r--   0        0        0      221 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0      467 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/view.py
--rw-r--r--   0        0        0      467 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/graphql/zone.py
--rw-r--r--   0        0        0     1073 2022-08-04 17:32:21.000000 netbox_plugin_dns-0.18.1/netbox_dns/management/commands/__pycache__/update_soa.cpython-38.pyc
--rw-r--r--   0        0        0     6035 2023-05-03 09:25:42.000000 netbox_plugin_dns-0.18.1/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0      661 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0     4153 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0001_initial.py
--rw-r--r--   0        0        0    11513 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0      437 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0002_zone_default_ttl.py
--rw-r--r--   0        0        0     3716 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0003_soa_managed_records.py
--rw-r--r--   0        0        0     2287 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
--rw-r--r--   0        0        0     1156 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0005_update_ns_records.py
--rw-r--r--   0        0        0      861 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0006_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      399 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      527 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0008_zone_status_names.py
--rw-r--r--   0        0        0     2176 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0009_netbox32.py
--rw-r--r--   0        0        0     1543 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0010_update_soa_records.py
--rw-r--r--   0        0        0     2201 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0011_add_view_model.py
--rw-r--r--   0        0        0      402 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0012_adjust_zone_and_record.py
--rw-r--r--   0        0        0      733 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
--rw-r--r--   0        0        0      428 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0014_add_view_description.py
--rw-r--r--   0        0        0      393 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0015_add_record_status.py
--rw-r--r--   0        0        0     1053 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0016_cleanup_ptr_records.py
--rw-r--r--   0        0        0      405 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0017_alter_record_ttl.py
--rw-r--r--   0        0        0     1553 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0018_zone_arpa_network.py
--rw-r--r--   0        0        0      433 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0019_update_ns_ttl.py
--rw-r--r--   0        0        0     1260 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3304 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      891 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0        0 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0     1992 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0        0        0     4592 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0001_squashed_netbox_dns_0_15.cpython-38.pyc
--rw-r--r--   0        0        0      615 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0002_zone_default_ttl.cpython-38.pyc
--rw-r--r--   0        0        0     1901 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0003_soa_managed_records.cpython-38.pyc
--rw-r--r--   0        0        0     1842 2023-04-02 12:40:22.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0004_create_ptr_for_a_aaaa_records.cpython-38.pyc
--rw-r--r--   0        0        0     1339 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0005_update_ns_records.cpython-38.pyc
--rw-r--r--   0        0        0      890 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0006_zone_soa_serial_auto.cpython-38.pyc
--rw-r--r--   0        0        0      599 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0007_alter_zone_soa_serial_auto.cpython-38.pyc
--rw-r--r--   0        0        0      825 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0008_zone_status_names.cpython-38.pyc
--rw-r--r--   0        0        0     1150 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0009_netbox32.cpython-38.pyc
--rw-r--r--   0        0        0     1609 2022-07-17 16:26:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0010_update_soa_records.cpython-38.pyc
--rw-r--r--   0        0        0     1620 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0011_add_view_model.cpython-38.pyc
--rw-r--r--   0        0        0      577 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0012_adjust_zone_and_record.cpython-38.pyc
--rw-r--r--   0        0        0      711 2022-07-17 18:30:30.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0013_add_description.cpython-38.pyc
--rw-r--r--   0        0        0      694 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0013_add_nameserver_zone_record_description.cpython-38.pyc
--rw-r--r--   0        0        0      761 2022-07-17 17:41:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0013_nameserver_description_record_description_and_more.cpython-38.pyc
--rw-r--r--   0        0        0      659 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0014_add_view_description.cpython-38.pyc
--rw-r--r--   0        0        0      451 2022-07-17 19:23:49.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0014_converge.cpython-38.pyc
--rw-r--r--   0        0        0      591 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0015_add_record_status.cpython-38.pyc
--rw-r--r--   0        0        0      731 2022-07-28 15:48:59.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0015_alter_record_options_record_status.cpython-38.pyc
--rw-r--r--   0        0        0      676 2022-07-17 22:05:12.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0015_nameserver_status_record_status.cpython-38.pyc
--rw-r--r--   0        0        0      597 2022-07-17 22:08:34.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0015_record_status.cpython-38.pyc
--rw-r--r--   0        0        0     1242 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0016_cleanup_ptr_records.cpython-38.pyc
--rw-r--r--   0        0        0     1024 2022-07-28 19:28:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0016_consolidate_record.cpython-38.pyc
--rw-r--r--   0        0        0      649 2022-07-17 22:08:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0016_nameserver_status.cpython-38.pyc
--rw-r--r--   0        0        0      562 2022-07-28 19:49:15.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0017_alter_record_options.cpython-38.pyc
--rw-r--r--   0        0        0      727 2022-07-28 18:32:52.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0017_alter_record_options_alter_record_status.cpython-38.pyc
--rw-r--r--   0        0        0      592 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0017_alter_record_ttl.cpython-38.pyc
--rw-r--r--   0        0        0     1619 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0018_zone_arpa_network.cpython-38.pyc
--rw-r--r--   0        0        0      723 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0019_update_ns_ttl.cpython-38.pyc
--rw-r--r--   0        0        0      855 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0020_netbox_3_4.cpython-38.pyc
--rw-r--r--   0        0        0     2373 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0021_record_ip_address.cpython-38.pyc
--rw-r--r--   0        0        0     1047 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/0022_search.cpython-38.pyc
--rw-r--r--   0        0        0      144 2022-07-17 16:26:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    28247 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/models.py
--rw-r--r--   0        0        0     3158 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/navigation.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      217 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1056 2023-04-02 13:56:12.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__pycache__/nameserver.cpython-38.pyc
--rw-r--r--   0        0        0     2992 2023-04-02 13:56:12.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0      700 2022-07-28 15:47:45.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__pycache__/view.cpython-38.pyc
--rw-r--r--   0        0        0     1725 2023-04-02 13:56:12.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/__pycache__/zone.cpython-38.pyc
--rw-r--r--   0        0        0      701 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3064 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      325 2022-07-28 12:40:17.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1660 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     1980 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/template_content.py
--rw-r--r--   0        0        0     1192 2023-04-02 13:34:21.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      378 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     4136 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0      919 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      460 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2171 2023-05-10 18:57:32.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      524 2023-05-10 18:57:32.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2218 2023-05-10 18:57:32.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0      215 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/related.html
--rw-r--r--   0        0        0     5480 2023-05-10 15:29:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0        0 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/templatetags/__init__.py
--rw-r--r--   0        0        0      146 2022-07-17 16:26:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      475 2022-07-17 16:26:46.000000 netbox_plugin_dns-0.18.1/netbox_dns/templatetags/__pycache__/view_helpers.cpython-38.pyc
--rw-r--r--   0        0        0      271 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/templatetags/view_helpers.py
--rw-r--r--   0        0        0     5202 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/urls.py
--rw-r--r--   0        0        0     1537 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/utilities.py
--rw-r--r--   0        0        0     1969 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/validators.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0      216 2022-07-17 16:26:44.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3959 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__pycache__/nameserver.cpython-38.pyc
--rw-r--r--   0        0        0     3233 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0     2999 2023-04-02 12:30:27.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__pycache__/view.cpython-38.pyc
--rw-r--r--   0        0        0     4528 2023-04-02 13:56:13.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/__pycache__/zone.cpython-38.pyc
--rw-r--r--   0        0        0     2991 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     2554 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/record.py
--rw-r--r--   0        0        0     1895 2022-12-22 08:12:55.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/view.py
--rw-r--r--   0        0        0     3600 2023-04-02 13:35:16.000000 netbox_plugin_dns-0.18.1/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      690 2023-05-10 18:58:48.000000 netbox_plugin_dns-0.18.1/pyproject.toml
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-14 13:07:16.080783 netbox_plugin_dns-0.18.2/LICENSE
+-rw-r--r--   0        0        0     3096 2023-05-14 13:07:16.080783 netbox_plugin_dns-0.18.2/README.md
+-rw-r--r--   0        0        0      903 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/admin.py
+-rw-r--r--   0        0        0     1951 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0     4555 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0      441 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3060 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/apps.py
+-rw-r--r--   0        0        0       46 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3023 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/__init__.py
+-rwxr-xr-x   0        0        0      601 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/nameserver.py
+-rwxr-xr-x   0        0        0     1615 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/record.py
+-rw-r--r--   0        0        0      577 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/view.py
+-rwxr-xr-x   0        0        0     1185 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/zone.py
+-rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/__init__.py
+-rwxr-xr-x   0        0        0     1308 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     5083 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0      961 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    14198 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      604 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/nameserver.py
+-rw-r--r--   0        0        0      487 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/record.py
+-rw-r--r--   0        0        0      221 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0      467 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/view.py
+-rw-r--r--   0        0        0      467 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/zone.py
+-rw-r--r--   0        0        0     6035 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0      661 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0     4153 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_initial.py
+-rw-r--r--   0        0        0    11513 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0      437 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0002_zone_default_ttl.py
+-rw-r--r--   0        0        0     3716 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0003_soa_managed_records.py
+-rw-r--r--   0        0        0     2287 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
+-rw-r--r--   0        0        0     1156 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0005_update_ns_records.py
+-rw-r--r--   0        0        0      861 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0006_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      399 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      527 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0008_zone_status_names.py
+-rw-r--r--   0        0        0     2176 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0009_netbox32.py
+-rw-r--r--   0        0        0     1543 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0010_update_soa_records.py
+-rw-r--r--   0        0        0     2201 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0011_add_view_model.py
+-rw-r--r--   0        0        0      402 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0012_adjust_zone_and_record.py
+-rw-r--r--   0        0        0      733 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
+-rw-r--r--   0        0        0      428 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0014_add_view_description.py
+-rw-r--r--   0        0        0      393 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0015_add_record_status.py
+-rw-r--r--   0        0        0     1053 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0016_cleanup_ptr_records.py
+-rw-r--r--   0        0        0      405 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0017_alter_record_ttl.py
+-rw-r--r--   0        0        0     1553 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0018_zone_arpa_network.py
+-rw-r--r--   0        0        0      433 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0019_update_ns_ttl.py
+-rw-r--r--   0        0        0     1260 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3304 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      891 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0    28247 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/models.py
+-rw-r--r--   0        0        0     3158 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/navigation.py
+-rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3064 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      325 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1660 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     1980 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     1192 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      378 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     4136 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0      919 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      460 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2171 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      524 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2218 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0      215 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/related.html
+-rw-r--r--   0        0        0     5480 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0        0 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templatetags/__init__.py
+-rw-r--r--   0        0        0      271 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templatetags/view_helpers.py
+-rw-r--r--   0        0        0     5202 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1537 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/utilities.py
+-rw-r--r--   0        0        0     1969 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/validators.py
+-rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2991 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     2554 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     1895 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     3600 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      690 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/pyproject.toml
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.2/PKG-INFO
```

### Comparing `netbox_plugin_dns-0.18.1/LICENSE` & `netbox_plugin_dns-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/README.md` & `netbox_plugin_dns-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/__init__.py` & `netbox_plugin_dns-0.18.2/netbox_dns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.18.1"
+__version__ = "0.18.2"
 
 
 class DNSConfig(PluginConfig):
     name = "netbox_dns"
     verbose_name = "Netbox DNS"
     description = "Netbox DNS"
     min_version = "3.5"
```

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/admin.py` & `netbox_plugin_dns-0.18.2/netbox_dns/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-0.18.2/netbox_dns/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/api/serializers.py` & `netbox_plugin_dns-0.18.2/netbox_dns/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/api/views.py` & `netbox_plugin_dns-0.18.2/netbox_dns/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/fields/address.py` & `netbox_plugin_dns-0.18.2/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/fields/network.py` & `netbox_plugin_dns-0.18.2/netbox_dns/fields/network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/filters/nameserver.py` & `netbox_plugin_dns-0.18.2/netbox_dns/filters/nameserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class NameServerFilter(NetBoxModelFilterSet):
     """Filter capabilities for NameServer instances."""
 
     name = django_filters.CharFilter()
 
     class Meta:
         model = NameServer
-        fields = ("name",)
+        fields = ("id", "name")
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = Q(name__icontains=value)
         return queryset.filter(qs_filter)
```

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/filters/record.py` & `netbox_plugin_dns-0.18.2/netbox_dns/filters/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         to_field_name="name",
         label="View the Parent Zone belongs to",
     )
     managed = django_filters.BooleanFilter()
 
     class Meta:
         model = Record
-        fields = ("type", "name", "value", "status", "zone", "managed")
+        fields = ("id", "type", "name", "value", "status", "zone", "managed")
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = (
             Q(name__icontains=value)
```

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/filters/view.py` & `netbox_plugin_dns-0.18.2/netbox_dns/filters/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class ViewFilter(NetBoxModelFilterSet):
     """Filter capabilities for View instances."""
 
     name = django_filters.CharFilter()
 
     class Meta:
         model = View
-        fields = ("name",)
+        fields = ("id", "name")
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = Q(name__icontains=value)
         return queryset.filter(qs_filter)
```

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/filters/zone.py` & `netbox_plugin_dns-0.18.2/netbox_dns/filters/zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     )
     active = django_filters.BooleanFilter(
         label="Zone is active",
     )
 
     class Meta:
         model = Zone
-        fields = ("name", "view", "status", "nameservers", "active")
+        fields = ("id", "name", "view", "status", "nameservers", "active")
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = (
             Q(name__icontains=value)
```

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-0.18.2/netbox_dns/forms/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/forms/record.py` & `netbox_plugin_dns-0.18.2/netbox_dns/forms/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/forms/view.py` & `netbox_plugin_dns-0.18.2/netbox_dns/forms/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/forms/zone.py` & `netbox_plugin_dns-0.18.2/netbox_dns/forms/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/graphql/__init__.py` & `netbox_plugin_dns-0.18.2/netbox_dns/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/graphql/nameserver.py` & `netbox_plugin_dns-0.18.2/netbox_dns/graphql/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-0.18.2/netbox_dns/management/commands/cleanup_database.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-0.18.2/netbox_dns/management/commands/update_soa.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0001_initial.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0003_soa_managed_records.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0003_soa_managed_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0005_update_ns_records.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0005_update_ns_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0006_zone_soa_serial_auto.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0006_zone_soa_serial_auto.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0008_zone_status_names.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0008_zone_status_names.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0009_netbox32.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0009_netbox32.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0010_update_soa_records.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0010_update_soa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0011_add_view_model.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0011_add_view_model.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0016_cleanup_ptr_records.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0016_cleanup_ptr_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0018_zone_arpa_network.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0018_zone_arpa_network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0021_record_ip_address.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/migrations/0022_search.py` & `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0022_search.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/models.py` & `netbox_plugin_dns-0.18.2/netbox_dns/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/navigation.py` & `netbox_plugin_dns-0.18.2/netbox_dns/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-0.18.2/netbox_dns/tables/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/tables/record.py` & `netbox_plugin_dns-0.18.2/netbox_dns/tables/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/tables/zone.py` & `netbox_plugin_dns-0.18.2/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/template_content.py` & `netbox_plugin_dns-0.18.2/netbox_dns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/view.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/managed_record.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/managed_record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/urls.py` & `netbox_plugin_dns-0.18.2/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/utilities.py` & `netbox_plugin_dns-0.18.2/netbox_dns/utilities.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/validators.py` & `netbox_plugin_dns-0.18.2/netbox_dns/validators.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-0.18.2/netbox_dns/views/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/views/record.py` & `netbox_plugin_dns-0.18.2/netbox_dns/views/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/views/view.py` & `netbox_plugin_dns-0.18.2/netbox_dns/views/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/netbox_dns/views/zone.py` & `netbox_plugin_dns-0.18.2/netbox_dns/views/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.1/pyproject.toml` & `netbox_plugin_dns-0.18.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-plugin-dns"
-version = "0.18.1"
+version = "0.18.2"
 description = "Netbox DNS is a NetBox plugin for managing DNS data."
 authors = ["Peter Eckel <pe-netbox-dns@hindenburgring.com>"]
 homepage = "https://github.com/peteeckel/netbox-plugin-dns"
 repository = "https://github.com/peteeckel/netbox-plugin-dns"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_dns"}]
```

### Comparing `netbox_plugin_dns-0.18.1/PKG-INFO` & `netbox_plugin_dns-0.18.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-dns
-Version: 0.18.1
+Version: 0.18.2
 Summary: Netbox DNS is a NetBox plugin for managing DNS data.
 Home-page: https://github.com/peteeckel/netbox-plugin-dns
 License: MIT
 Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel
 Author-email: pe-netbox-dns@hindenburgring.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.1 Summary: Netbox
+Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.2 Summary: Netbox
 DNS is a NetBox plugin for managing DNS data. Home-page: https://github.com/
 peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel Author-email: pe-netbox-dns@hindenburgring.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

