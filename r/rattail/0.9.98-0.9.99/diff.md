# Comparing `tmp/rattail-0.9.98.tar.gz` & `tmp/rattail-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rattail-0.9.98.tar", last modified: Fri Oct  4 19:32:23 2019, max compression
+gzip compressed data, was "dist/rattail-0.9.99.tar", last modified: Mon Oct  7 16:55:27 2019, max compression
```

## Comparing `rattail-0.9.98.tar` & `rattail-0.9.99.tar`

### file list

```diff
@@ -1,517 +1,518 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/
--rw-r--r--   0 lance     (1000) lance     (1000)      210 2019-10-04 19:32:23.000000 rattail-0.9.98/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1429 2019-10-04 19:32:23.000000 rattail-0.9.98/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)    95810 2019-10-04 19:31:08.000000 rattail-0.9.98/CHANGES.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1429 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)     2417 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      290 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)    21235 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      245 2018-11-17 22:12:16.000000 rattail-0.9.98/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-11-17 22:12:16.000000 rattail-0.9.98/MANIFEST.in
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/win32/
--rw-r--r--   0 lance     (1000) lance     (1000)     2506 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/win32/registry.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3367 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/win32/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6027 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/win32/service.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4161 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/win32/users.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     2012 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/core.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/api/
--rw-r--r--   0 lance     (1000) lance     (1000)     3417 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/org.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2044 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1530 2019-09-18 15:55:44.000000 rattail-0.9.98/rattail/db/api/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7118 2019-09-18 15:55:54.000000 rattail-0.9.98/rattail/db/api/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2010 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2076 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1381 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1854 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/api/settings.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11539 2019-06-05 21:22:51.000000 rattail-0.9.98/rattail/db/changes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2997 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/diffs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5037 2018-11-28 21:35:56.000000 rattail-0.9.98/rattail/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4928 2019-07-09 00:22:39.000000 rattail-0.9.98/rattail/db/continuum.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/alembic/
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail-0.9.98/rattail/db/alembic/README
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     3693 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/9740f0dcf84b_add_tempmon.py
--rw-r--r--   0 lance     (1000) lance     (1000)      662 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/6a1ec8b93637_add_productcost_discontinued.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6542 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/1f8e3cf6b2a2_add_handheld_batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1103 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/69d924015613_add_product_inventory.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      738 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/33c3b9acc341_make_message_recips_unique.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1399 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/35b1da3be8f5_add_bouncer.py
--rw-r--r--   0 lance     (1000) lance     (1000)      774 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/9de6ffc1d2af_add_product_price_required.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2201 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/e5c3eab67b28_add_upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4183 2015-02-14 03:52:01.000000 rattail-0.9.98/rattail/db/alembic/versions/218562884128_add_vendor_invoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1124 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/7ba105af22a7_add_some_product_flags.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2655 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/b82daacc86b7_add_importer_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1320 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/017daa26c36c_add_employee_worked_shifts.py
--rw-r--r--   0 lance     (1000) lance     (1000)      740 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/471299288da9_add_product_notes.py
--rw-r--r--   0 lance     (1000) lance     (1000)      939 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/d87aeb7da072_allow_null_for_purchase_buyer.py
--rw-r--r--   0 lance     (1000) lance     (1000)      835 2019-02-06 22:42:50.000000 rattail-0.9.98/rattail/db/alembic/versions/40a4855cb22d_add_receiving_truck_dump_children_first.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2260 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/35b451f8cc27_add_product_cost_discount.py
--rw-r--r--   0 lance     (1000) lance     (1000)      807 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/8b02c6eaf318_grow_datasync_change_source_consumer.py
--rw-r--r--   0 lance     (1000) lance     (1000)      595 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/e1edeba632f8_grow_role_name.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1654 2019-04-24 03:41:44.000000 rattail-0.9.98/rattail/db/alembic/versions/90d5e8185d44_add_category_family_for_product_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1099 2019-03-08 19:47:35.000000 rattail-0.9.98/rattail/db/alembic/versions/5b393c108673_add_product_volatile.py
--rw-r--r--   0 lance     (1000) lance     (1000)      723 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/c384c65995db_make_cost_case_size_decimal.py
--rw-r--r--   0 lance     (1000) lance     (1000)      572 2015-02-05 17:33:54.000000 rattail-0.9.98/rattail/db/alembic/versions/2e3f33b8ea46_increase_vendor_name_length.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1241 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a48db300576a_add_unit_pack_products.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      622 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/d042f5e34b77_add_person_modified.py
--rw-r--r--   0 lance     (1000) lance     (1000)      866 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/6c68c814f3c2_grow_change_key_columns.py
--rw-r--r--   0 lance     (1000) lance     (1000)      705 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/1f21b32fd2a7_add_inventory_prev_on_hand.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1138 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/27bcaa3c7f5f_add_employee_x_store.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1138 2019-04-18 23:11:45.000000 rattail-0.9.98/rattail/db/alembic/versions/5dee2f796f25_add_item_codes_for_pricing_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      699 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/f5c936a4cc62_add_inventory_batch_mode.py
--rw-r--r--   0 lance     (1000) lance     (1000)      632 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/528c049eb5b7_add_role_session_timeout.py
--rw-r--r--   0 lance     (1000) lance     (1000)      730 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/139fea9de0a0_add_upgrade_status.py
--rw-r--r--   0 lance     (1000) lance     (1000)      835 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a03ee3718ff4_add_dept_exempt_from_gross_sales.py
--rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3dc08453a5d3_add_batch_pricing_row_vendor.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6774 2019-04-18 00:55:51.000000 rattail-0.9.98/rattail/db/alembic/versions/4e5526fae79e_add_newproduct_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      882 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/16a72305f72c_add_purchase_item_item_id.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1335 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/b50a59f35e3f_add_scheduled_shifts.py
--rw-r--r--   0 lance     (1000) lance     (1000)      976 2015-02-27 07:44:51.000000 rattail-0.9.98/rattail/db/alembic/versions/321f8f7b3887_add_product_special_order.py
--rw-r--r--   0 lance     (1000) lance     (1000)      996 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/0c91cf7d557b_add_invadjust_reason.py
--rw-r--r--   0 lance     (1000) lance     (1000)      615 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/c2af678f010c_make_tax_code_a_string.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1595 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/0a3dca1cd299_add_product_batch_row_item_entry.py
--rw-r--r--   0 lance     (1000) lance     (1000)      597 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/391fac830cb1_grow_category_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)      640 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/765ce0ae5bbd_add_inventory_reason_hidden.py
--rw-r--r--   0 lance     (1000) lance     (1000)      757 2018-11-18 01:25:38.000000 rattail-0.9.98/rattail/db/alembic/versions/5ef33e961026_add_customer_wholesale.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1102 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/af4c4ec011fb_add_purchase_ship_method.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1819 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/40326eb83e18_add_messages.py
--rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/eb4e965ce771_grow_inventory_total_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)      927 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/6551a4d9ff25_add_receiving_truck_dump_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4748 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3350e0220faf_add_purchases.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      653 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/14d23631733d_grow_datasyncchange_payload_type.py
--rw-r--r--   0 lance     (1000) lance     (1000)      825 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/aa32b6e51129_grow_product_description.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1812 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/b5aa18867ab3_add_purchase_batch_row_claim.py
--rw-r--r--   0 lance     (1000) lance     (1000)    35667 2015-02-10 05:51:10.000000 rattail-0.9.98/rattail/db/alembic/versions/47d30c955111_add_versioning.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2581 2019-03-01 16:57:54.000000 rattail-0.9.98/rattail/db/alembic/versions/03be1584f923_add_purchase_batch_truck_dump_status.py
--rw-r--r--   0 lance     (1000) lance     (1000)      765 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/51756b0edcdf_add_product_default_pack.py
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/9f1d111fa775_update_brand_version.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     3492 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/3df3144cec58_add_mailingaddress.py
--rw-r--r--   0 lance     (1000) lance     (1000)      706 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/8c17754a6bbf_add_purchase_batch_complete.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1421 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/064f71d774ad_add_batch_ids.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1244 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/ea9718f6e6c6_add_product_store_info.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2872 2015-02-27 00:18:56.000000 rattail-0.9.98/rattail/db/alembic/versions/ee253b66b7b_add_tax.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1012 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/de4ebbf5bbb3_add_brand_confirmed.py
--rw-r--r--   0 lance     (1000) lance     (1000)      866 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/c1bfb033050d_add_vendor_catalog_row_cost_ref.py
--rw-r--r--   0 lance     (1000) lance     (1000)      625 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/195ceb6abeb3_add_customer_number.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1048 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/c2085638f487_add_pricing_batch_true_unit_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)      652 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/2fe69ea73233_add_inventory_reason_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1996 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/123af5f6a0bc_add_purchase_damaged_expired_counts.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1290 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/687646b42fce_add_batch_complete.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1074 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/e63d53698e9f_add_department_flags.py
--rw-r--r--   0 lance     (1000) lance     (1000)    27560 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/e9fca3d787ea_remove_old_versioning.py
--rw-r--r--   0 lance     (1000) lance     (1000)      789 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/86632a7bc5b5_add_employee_full_time.py
--rw-r--r--   0 lance     (1000) lance     (1000)      576 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/37e0e46ec6fe_add_user_last_login.py
--rw-r--r--   0 lance     (1000) lance     (1000)      778 2019-05-07 22:04:59.000000 rattail-0.9.98/rattail/db/alembic/versions/abd43933c6c6_add_report_output_params.py
--rw-r--r--   0 lance     (1000) lance     (1000)      923 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a8c96f5491ae_add_purchase_po_line_number.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1237 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/fd935205655d_add_item_id_for_product_batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2627 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/043d4bafc0be_add_batch_status.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1014 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/1242c7a0e24a_add_user_events.py
--rw-r--r--   0 lance     (1000) lance     (1000)      994 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/234c79420312_add_product_image.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1313 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/ff8662bbdb53_add_email_attempt.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2567 2018-12-18 22:43:20.000000 rattail-0.9.98/rattail/db/alembic/versions/bd7acb7028da_add_product_batch_subdepartment.py
--rw-r--r--   0 lance     (1000) lance     (1000)      772 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a9b37b388e56_add_product_status.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1120 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/ccd32c44393f_add_columns_for_vendor_catalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)      731 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3f1e4a7b5268_add_catalog_suggested_retail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1576 2019-01-09 17:15:09.000000 rattail-0.9.98/rattail/db/alembic/versions/4db5dbf725f5_add_batch_extra_data.py
--rw-r--r--   0 lance     (1000) lance     (1000)      990 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/4137e9938122_add_foodstamp_and_tax_flags.py
--rw-r--r--   0 lance     (1000) lance     (1000)      688 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/5b88c82dbd8d_add_case_quantity_for_inventory_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      643 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3b5e0b87c176_add_user_active_sticky.py
--rw-r--r--   0 lance     (1000) lance     (1000)      659 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/09ed5bdc99f1_make_depositlink_code_a_string.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4013 2018-12-20 04:08:20.000000 rattail-0.9.98/rattail/db/alembic/versions/f3781f071de3_add_members.py
--rw-r--r--   0 lance     (1000) lance     (1000)      956 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/86042c0323c6_add_credit_product_discarded.py
--rw-r--r--   0 lance     (1000) lance     (1000)      801 2018-12-19 21:09:36.000000 rattail-0.9.98/rattail/db/alembic/versions/45b90e4f8ab4_grow_product_uom_abbreviation.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4353 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/d6ca20fe9452_add_custorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1303 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a47a4d73b662_use_decimal_qty_for_handheld_inventory_.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      618 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/4da3fe4a368f_add_email_invalid_flag.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5675 2019-04-19 17:56:35.000000 rattail-0.9.98/rattail/db/alembic/versions/e1685bf9f1ad_add_product_batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)      894 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/0174642e7b60_add_vendor_catalog_future.py
--rw-r--r--   0 lance     (1000) lance     (1000)      865 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/65098d24972f_add_transaction_meta.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1193 2019-04-18 21:21:23.000000 rattail-0.9.98/rattail/db/alembic/versions/727c63fcde2d_add_allowances_to_vendorcatalog_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3107 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/23600f00cda7_add_person_notes.py
--rw-r--r--   0 lance     (1000) lance     (1000)      646 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/b9658d212053_add_customer_active_in_pos.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19199 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3a500dc55e0f_add_more_versions.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      638 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/0b90d5c59fd7_add_person_middle_name.py
--rw-r--r--   0 lance     (1000) lance     (1000)      698 2015-02-12 02:00:12.000000 rattail-0.9.98/rattail/db/alembic/versions/268ff6454410_add_product_case_pack.py
--rw-r--r--   0 lance     (1000) lance     (1000)      748 2015-03-10 21:03:19.000000 rattail-0.9.98/rattail/db/alembic/versions/3623367c499f_add_product_last_sold.py
--rw-r--r--   0 lance     (1000) lance     (1000)      674 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/aa5962fb998e_add_inventory_unit_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)      706 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/d67dee1cb849_grow_inventory_row_total_cost.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1242 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/835215361bb_add_change_uuid.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1193 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/57d12767eb53_add_employee_x_department.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1536 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/539c2df56562_add_batch_description.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2208 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a5a7358ed27f_inventory_from_handheld_batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)      957 2019-03-07 21:38:03.000000 rattail-0.9.98/rattail/db/alembic/versions/6118198dc4db_add_purchase_batch_row_invoice_total_.py
--rw-r--r--   0 lance     (1000) lance     (1000)    35081 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a28c3583c8f0_add_product_versioning.py
--rw-r--r--   0 lance     (1000) lance     (1000)      691 2018-12-01 01:20:14.000000 rattail-0.9.98/rattail/db/alembic/versions/648cb088658c_add_batch_pricing_old_price_margin.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1307 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/0a5a866f2a3d_add_report_output.py
--rw-r--r--   0 lance     (1000) lance     (1000)      592 2015-02-11 08:49:31.000000 rattail-0.9.98/rattail/db/alembic/versions/f950be5601a_make_employee_person_unique.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2005 2015-02-27 06:10:01.000000 rattail-0.9.98/rattail/db/alembic/versions/3544687ae150_improve_size_fields.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1154 2015-02-24 02:04:59.000000 rattail-0.9.98/rattail/db/alembic/versions/3ef0fbcfb42e_make_invoice_quantities_decimal.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3961 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3f266c89a3d4_add_pricing_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      688 2018-11-19 01:55:07.000000 rattail-0.9.98/rattail/db/alembic/versions/e645676eb37a_add_pricing_batch_suggested_price.py
--rw-r--r--   0 lance     (1000) lance     (1000)      949 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/20ec527fad0a_add_purchase_batch_row_item.py
--rw-r--r--   0 lance     (1000) lance     (1000)      635 2018-12-19 01:04:54.000000 rattail-0.9.98/rattail/db/alembic/versions/c5f39e2dec78_add_label_batch_label_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/4a4ae7ebdae6_add_purchase_batch_mode.py
--rw-r--r--   0 lance     (1000) lance     (1000)      925 2015-02-11 04:25:39.000000 rattail-0.9.98/rattail/db/alembic/versions/1513dc6d6ca7_add_product_deleted.py
--rw-r--r--   0 lance     (1000) lance     (1000)      859 2018-11-19 03:02:50.000000 rattail-0.9.98/rattail/db/alembic/versions/d28d28bc3cd0_add_pricing_batch_margin_diff.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1902 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/d3b6e3c971b4_add_product_future_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2610 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/7f88949a7ab9_add_employee_history.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2752 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3b2859694c53_add_new_versioning.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2121 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/3e79dd89fe12_add_label_handheld_batch_es_tie.py
--rw-r--r--   0 lance     (1000) lance     (1000)      878 2019-06-07 21:44:29.000000 rattail-0.9.98/rattail/db/alembic/versions/64d163d9de3a_add_purchase_batch_po_total_calculated.py
--rw-r--r--   0 lance     (1000) lance     (1000)      678 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/be079e974a52_add_purchase_batch_order_quantities_.py
--rw-r--r--   0 lance     (1000) lance     (1000)      833 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/b3432785a839_add_inventory_total_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1727 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a809caf23cf0_grow_vendorcatalog_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)      868 2018-12-19 00:20:25.000000 rattail-0.9.98/rattail/db/alembic/versions/95a66a59d420_add_label_batch_label_profile.py
--rw-r--r--   0 lance     (1000) lance     (1000)      965 2015-02-27 06:30:24.000000 rattail-0.9.98/rattail/db/alembic/versions/3c33f288ad62_add_product_discountable.py
--rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-12-19 01:05:51.000000 rattail-0.9.98/rattail/db/alembic/versions/a7b7246e48e2_grow_label_profile_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)      823 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/92a49edc45c3_add_purchase_batch_invoice_file.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1052 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/11a9145414a9_add_product_suggested_price.py
--rw-r--r--   0 lance     (1000) lance     (1000)      835 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/6ef6db00abe8_add_product_discontinued.py
--rw-r--r--   0 lance     (1000) lance     (1000)      678 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/fb4bd12cbd37_add_label_batch_static_prices.py
--rw-r--r--   0 lance     (1000) lance     (1000)      637 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/c37154504ae1_add_receiving_truck_dump.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1384 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/3a7029aed67_fix_user_x_role_null_bug.py
--rw-r--r--   0 lance     (1000) lance     (1000)      894 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a295dee8d1e9_add_credit_total.py
--rw-r--r--   0 lance     (1000) lance     (1000)      785 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/8e965902bf93_add_product_item_id_item_type.py
--rw-r--r--   0 lance     (1000) lance     (1000)      773 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/05d1ed3a4a28_add_vendor_abbreviation.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1269 2015-02-27 07:09:00.000000 rattail-0.9.98/rattail/db/alembic/versions/3f0d2a97f12a_add_vendor_schedule_fields.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14469 2015-02-07 21:40:45.000000 rattail-0.9.98/rattail/db/alembic/versions/33b76c3cb892_rename_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)      798 2018-12-05 00:19:31.000000 rattail-0.9.98/rattail/db/alembic/versions/f7dc4e92752c_add_label_profile_sync_me.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5824 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/09976b73e96a_add_labels_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1233 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/977a76f259bd_add_purchase_shipped_counts.py
--rw-r--r--   0 lance     (1000) lance     (1000)      897 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/90a3338b187b_add_credit_vendor_item_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1053 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/adcb91f473c3_add_purchase_item_out_of_stock.py
--rw-r--r--   0 lance     (1000) lance     (1000)      672 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/a33583135905_add_inventory_variance.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1500 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/830a20917c49_add_batch_row_modified.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8310 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/193c2dcdd14d_add_purchase_credits.py
--rw-r--r--   0 lance     (1000) lance     (1000)      573 2015-03-03 01:32:46.000000 rattail-0.9.98/rattail/db/alembic/versions/6cadbeb3f82_grow_report_code_name.py
--rw-r--r--   0 lance     (1000) lance     (1000)    25068 2015-01-27 18:54:45.000000 rattail-0.9.98/rattail/db/alembic/versions/1515aa76b64a_initial_schema.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3291 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/42edf57f1ae2_prevent_null_for_batch_comlete.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1036 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/cc3de1ca0689_add_customer_active_in_pos_sticky.py
--rw-r--r--   0 lance     (1000) lance     (1000)      675 2018-11-26 01:47:31.000000 rattail-0.9.98/rattail/db/alembic/versions/7eb0903932ff_add_pricing_batch_min_diff_percent.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     1114 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/188810a5f9db_add_datasync_change.py
--rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/36ffa8b83782_make_batch_filename_nullable.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1573 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/cd23a59c5d89_add_dept_to_product_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      652 2018-12-18 04:05:26.000000 rattail-0.9.98/rattail/db/alembic/versions/c02430f167c2_add_pricing_batch_filename.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1086 2018-11-27 00:05:41.000000 rattail-0.9.98/rattail/db/alembic/versions/04f17c46b42f_grow_batch_pricing_row_margins.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1317 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/4bd528bca236_add_purchase_department.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5699 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/9a5511fdc9f5_add_purchase_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)      916 2015-02-27 01:03:56.000000 rattail-0.9.98/rattail/db/alembic/versions/3f5be78f0f18_add_product_organic.py
--rw-r--r--   0 lance     (1000) lance     (1000)      818 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/14d83595afa1_add_category_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)      741 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/45d7d92f4aa6_add_price_batch_thresholds.py
--rw-rw-r--   0 lance     (1000) lance     (1000)      645 2016-12-17 08:39:11.000000 rattail-0.9.98/rattail/db/alembic/versions/6e6d6e2ef0e_grow_change_class_name.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3163 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/4d2c5bdfecff_remove_legacy_batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)      755 2015-02-14 10:02:44.000000 rattail-0.9.98/rattail/db/alembic/versions/2dd756a44a16_add_batchrow_status_text.py
--rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/0f4cb39da3cc_add_product_scancode_uom_abbrev.py
--rw-r--r--   0 lance     (1000) lance     (1000)      861 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/6a02ca0279c9_add_manual_flag_to_price_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3148 2015-02-27 00:18:56.000000 rattail-0.9.98/rattail/db/alembic/versions/2d046576154c_add_deposit_link.py
--rw-r--r--   0 lance     (1000) lance     (1000)      738 2015-02-12 01:14:37.000000 rattail-0.9.98/rattail/db/alembic/versions/571c070b7080_enlarge_product_cost_code.py
--rw-r--r--   0 lance     (1000) lance     (1000)      700 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/19da5ebe6fb5_add_label_batch_filename.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1433 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/versions/9305c1f493b4_add_batch_notes.py
--rw-r--r--   0 lance     (1000) lance     (1000)      701 2019-01-08 18:34:55.000000 rattail-0.9.98/rattail/db/alembic/versions/fd7cf00b2918_grow_pricing_batch_row_markup.py
--rw-r--r--   0 lance     (1000) lance     (1000)      610 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/script.py.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2013 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/alembic/env.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2679 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/dump.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/sync/
--rw-r--r--   0 lance     (1000) lance     (1000)    12100 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/sync/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2052 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/sync/linux.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2423 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/sync/win32.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6462 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5797 2019-10-02 23:57:06.000000 rattail-0.9.98/rattail/db/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2041 2019-03-20 21:05:28.000000 rattail-0.9.98/rattail/db/types.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8361 2019-07-29 03:55:13.000000 rattail-0.9.98/rattail/db/cache.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     5769 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/org.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5795 2019-01-31 04:58:30.000000 rattail-0.9.98/rattail/db/model/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4357 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4592 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/bouncer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8268 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/custorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3516 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9770 2019-07-31 02:47:08.000000 rattail-0.9.98/rattail/db/model/employees.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5551 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/shifts.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20450 2019-03-07 17:44:28.000000 rattail-0.9.98/rattail/db/model/purchase.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6832 2018-12-20 19:47:13.000000 rattail-0.9.98/rattail/db/model/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2124 2019-05-07 22:12:17.000000 rattail-0.9.98/rattail/db/model/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9826 2019-10-02 23:10:32.000000 rattail-0.9.98/rattail/db/model/contact.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3650 2019-04-19 18:19:41.000000 rattail-0.9.98/rattail/db/model/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4157 2018-12-19 01:01:57.000000 rattail-0.9.98/rattail/db/model/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2876 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)    31847 2019-04-17 22:00:52.000000 rattail-0.9.98/rattail/db/model/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9243 2019-08-22 22:10:31.000000 rattail-0.9.98/rattail/db/model/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4472 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/messages.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3268 2019-07-03 01:51:01.000000 rattail-0.9.98/rattail/db/model/exports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11105 2019-08-25 20:00:52.000000 rattail-0.9.98/rattail/db/model/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6674 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8091 2019-08-04 00:57:37.000000 rattail-0.9.98/rattail/db/model/people.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/db/model/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)    15563 2019-09-17 22:17:21.000000 rattail-0.9.98/rattail/db/model/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2351 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/batch/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5276 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/batch/vendorinvoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5859 2019-04-24 03:39:32.000000 rattail-0.9.98/rattail/db/model/batch/product.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14538 2019-06-07 21:43:36.000000 rattail-0.9.98/rattail/db/model/batch/purchase.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1233 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8513 2018-12-19 01:04:14.000000 rattail-0.9.98/rattail/db/model/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6734 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7232 2019-04-18 21:20:56.000000 rattail-0.9.98/rattail/db/model/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6958 2019-04-18 23:10:58.000000 rattail-0.9.98/rattail/db/model/batch/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2324 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/batch/dynamic.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8055 2019-04-18 01:30:02.000000 rattail-0.9.98/rattail/db/model/batch/newproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4884 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/model/tempmon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6252 2019-06-11 03:17:43.000000 rattail-0.9.98/rattail/db/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5191 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/db/load.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1433 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/threads.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/contrib/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.98/rattail/contrib/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/contrib/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.98/rattail/contrib/vendors/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/
--rw-r--r--   0 lance     (1000) lance     (1000)     3590 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/dutchvalley.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3128 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/lotuslight.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5053 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/kehe.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4413 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/contrib/vendors/catalogs/unfi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/contrib/vendors/invoices/
--rw-r--r--   0 lance     (1000) lance     (1000)     2899 2019-01-24 20:04:56.000000 rattail-0.9.98/rattail/contrib/vendors/invoices/alberts.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.98/rattail/contrib/vendors/invoices/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3270 2019-01-21 22:06:17.000000 rattail-0.9.98/rattail/contrib/vendors/invoices/kehe.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5079 2019-01-22 19:45:32.000000 rattail-0.9.98/rattail/contrib/vendors/invoices/unfi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1949 2018-12-03 03:25:44.000000 rattail-0.9.98/rattail/core.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/config/
--rw-r--r--   0 lance     (1000) lance     (1000)      653 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/datasync.conf
--rw-r--r--   0 lance     (1000) lance     (1000)     2733 2018-12-01 23:55:42.000000 rattail-0.9.98/rattail/data/config/rattail.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      200 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/without-versioning.conf
--rw-r--r--   0 lance     (1000) lance     (1000)     1740 2018-12-01 22:37:08.000000 rattail-0.9.98/rattail/data/config/web.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      393 2018-07-05 07:17:19.000000 rattail-0.9.98/rattail/data/config/silent.conf~
--rw-r--r--   0 lance     (1000) lance     (1000)      196 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/with-versioning.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      379 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/silent.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      852 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/filemon.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      393 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/config/quiet.conf
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/images/
--rw-r--r--   0 lance     (1000) lance     (1000)     7770 2013-07-22 19:33:54.000000 rattail-0.9.98/rattail/data/images/rattail_avatar.png
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/new-batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     2519 2019-09-17 21:49:43.000000 rattail-0.9.98/rattail/data/new-batch/webview.py
--rw-r--r--   0 lance     (1000) lance     (1000)      702 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/new-batch/handler.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2750 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/new-batch/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/
--rw-r--r--   0 lance     (1000) lance     (1000)     3143 2019-08-17 07:08:35.000000 rattail-0.9.98/rattail/data/project/setup.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      182 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/MANIFEST.in_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)       28 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+dot+gitignore_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      177 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/README.rst_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/db/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/README
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/versions/.keepme
--rw-r--r--   0 lance     (1000) lance     (1000)      640 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/script.py.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2017 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/alembic/env.py_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     1184 2018-12-01 22:06:48.000000 rattail-0.9.98/rattail/data/project/+package+/db/model/core.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      288 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/db/model/__init__.py_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/web/
--rw-r--r--   0 lance     (1000) lance     (1000)     1133 2019-03-22 19:34:56.000000 rattail-0.9.98/rattail/data/project/+package+/web/app.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)     4353 2018-12-01 22:17:32.000000 rattail-0.9.98/rattail/data/project/+package+/web/menus.py~
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/
--rw-r--r--   0 lance     (1000) lance     (1000)      711 2018-12-01 22:32:49.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl~
--rw-r--r--   0 lance     (1000) lance     (1000)      810 2019-04-17 19:47:58.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/mobile/
--rw-r--r--   0 lance     (1000) lance     (1000)      398 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/mobile/home.mako_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)     1171 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/templates/mobile/base.mako_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)     2386 2018-12-01 22:18:11.000000 rattail-0.9.98/rattail/data/project/+package+/web/menus.py_tmpl~
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/web/views/
--rw-r--r--   0 lance     (1000) lance     (1000)      371 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/views/common.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)     1349 2019-03-23 00:41:04.000000 rattail-0.9.98/rattail/data/project/+package+/web/views/__init__.py_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/project/+package+/web/static/
--rw-r--r--   0 lance     (1000) lance     (1000)      211 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/static/__init__.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)     5142 2019-03-22 04:59:12.000000 rattail-0.9.98/rattail/data/project/+package+/web/menus.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      423 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/web/subscribers.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      527 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/emails.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      829 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/commands.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)      157 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/__init__.py_tmpl
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/project/+package+/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)      526 2018-12-01 22:25:25.000000 rattail-0.9.98/rattail/data/project/+package+/config.py_tmpl
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/data/sample/
--rw-r--r--   0 lance     (1000) lance     (1000)       51 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Brand.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      241 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/CustomerPerson.csv
--rw-r--r--   0 lance     (1000) lance     (1000)       69 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Store.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      418 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Product.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      124 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Vendor.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      141 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/VendorContact.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      281 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Subdepartment.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      228 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/EmployeeStore.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      306 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/User.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      253 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Employee.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      245 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Person.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      308 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/ProductCost.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      149 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Department.csv
--rw-r--r--   0 lance     (1000) lance     (1000)      201 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/data/sample/Customer.csv
--rw-r--r--   0 lance     (1000) lance     (1000)     4838 2019-02-06 20:28:07.000000 rattail-0.9.98/rattail/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3979 2019-04-19 22:19:26.000000 rattail-0.9.98/rattail/progress.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/bouncer/
--rw-r--r--   0 lance     (1000) lance     (1000)     1015 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/bouncer/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5135 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/bouncer/handler.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4732 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/bouncer/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6644 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/bouncer/daemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1774 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/poddoc.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4960 2019-04-18 01:27:15.000000 rattail-0.9.98/rattail/gpc.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1439 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2691 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_core.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    17920 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_changes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7273 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5191 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1288 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2878 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/test_init.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     2252 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/model/test_people.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/model/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1483 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/model/test_users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1463 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/model/test_customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)      696 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/db/model/test_datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1600 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_logging.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2006 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_util.py
--rw-r--r--   0 lance     (1000) lance     (1000)      341 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1178 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_csvutil.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3249 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      700 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_exceptions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2849 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_time.py
--rw-r--r--   0 lance     (1000) lance     (1000)      696 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_mail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7680 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_daemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6884 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/sil/
--rw-r--r--   0 lance     (1000) lance     (1000)      456 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/sil/test_columns.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/sil/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      753 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_files.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/filemon/
--rw-r--r--   0 lance     (1000) lance     (1000)     1804 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/filemon/test_util.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/filemon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6594 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/filemon/test_actions.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12154 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/filemon/test_config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3731 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/filemon/test_linux.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/tests/commands/
--rw-r--r--   0 lance     (1000) lance     (1000)     7514 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/commands/test_core.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/commands/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5082 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/tests/test_barcodes.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/templates/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/templates/mail/
--rw-r--r--   0 lance     (1000) lance     (1000)     5859 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/rattail_import_updates.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1292 2019-02-13 20:23:35.000000 rattail-0.9.98/rattail/templates/mail/datasync_error_consumer_process_changes.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      770 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/user_feedback.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      957 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/upgrade_failure.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1888 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/filemon_action_error.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      906 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/upgrade_success.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      459 2019-09-30 19:34:16.000000 rattail-0.9.98/rattail/templates/mail/run_n_mail.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1698 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/templates/mail/datasync_error_watcher_get_changes.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5187 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/exceptions.py
--rw-r--r--   0 lance     (1000) lance     (1000)    17301 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/enum.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3807 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/logging.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/reporting/
--rw-r--r--   0 lance     (1000) lance     (1000)     4963 2019-05-09 19:47:38.000000 rattail-0.9.98/rattail/reporting/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3404 2019-05-07 21:58:29.000000 rattail-0.9.98/rattail/reporting/handlers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1150 2019-05-07 22:19:10.000000 rattail-0.9.98/rattail/reporting/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3575 2019-05-07 22:47:45.000000 rattail-0.9.98/rattail/reporting/excel.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     6249 2019-07-29 18:09:48.000000 rattail-0.9.98/rattail/importing/sqlalchemy.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12568 2019-10-04 03:49:37.000000 rattail-0.9.98/rattail/importing/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7472 2019-08-16 01:06:00.000000 rattail-0.9.98/rattail/importing/csv.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7771 2019-02-19 01:32:29.000000 rattail-0.9.98/rattail/importing/rattail_bulk.py
--rw-r--r--   0 lance     (1000) lance     (1000)    26596 2019-09-17 19:11:09.000000 rattail-0.9.98/rattail/importing/handlers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1391 2019-07-29 17:44:14.000000 rattail-0.9.98/rattail/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5580 2019-07-29 17:40:49.000000 rattail-0.9.98/rattail/importing/exporters.py
--rw-r--r--   0 lance     (1000) lance     (1000)    30229 2019-07-29 16:39:05.000000 rattail-0.9.98/rattail/importing/importers.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10519 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/importing/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3243 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/importing/postgresql.py
--rw-r--r--   0 lance     (1000) lance     (1000)    87284 2019-03-08 19:29:31.000000 rattail-0.9.98/rattail/importing/model.py
--rw-------   0 lance     (1000) lance     (1000)     7719 2019-06-05 19:14:09.000000 rattail-0.9.98/rattail/importing/sample.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1836 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/pod.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1427 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11328 2019-01-21 22:23:06.000000 rattail-0.9.98/rattail/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8426 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/palm.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4265 2019-06-05 19:29:18.000000 rattail-0.9.98/rattail/wince.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.98/rattail/vendors/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4467 2019-04-18 22:01:11.000000 rattail-0.9.98/rattail/vendors/catalogs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4131 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/vendors/invoices.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/trainwreck/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/trainwreck/db/
--rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/trainwreck/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11489 2019-09-10 18:37:33.000000 rattail-0.9.98/rattail/trainwreck/db/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/trainwreck/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2019-07-25 22:29:00.000000 rattail-0.9.98/rattail/trainwreck/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2416 2019-07-26 04:11:10.000000 rattail-0.9.98/rattail/trainwreck/importing/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2342 2019-07-26 04:09:39.000000 rattail-0.9.98/rattail/trainwreck/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4159 2019-07-28 19:48:28.000000 rattail-0.9.98/rattail/trainwreck/importing/trainwreck.py
--rw-r--r--   0 lance     (1000) lance     (1000)      131 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6569 2019-09-10 21:56:17.000000 rattail-0.9.98/rattail/trainwreck/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1680 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/trainwreck/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1889 2019-03-08 20:02:01.000000 rattail-0.9.98/rattail/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8304 2019-09-20 01:07:44.000000 rattail-0.9.98/rattail/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/sil/
--rw-r--r--   0 lance     (1000) lance     (1000)    11136 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/sil/writer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1208 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/sil/exceptions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1289 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/sil/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6029 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/sil/columns.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2039 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/sil/batches.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7210 2019-02-13 20:22:58.000000 rattail-0.9.98/rattail/emails.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7563 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/files.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6358 2019-02-11 19:58:11.000000 rattail-0.9.98/rattail/time.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/filemon/
--rw-r--r--   0 lance     (1000) lance     (1000)      999 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/filemon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2237 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/filemon/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4818 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/filemon/linux.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14326 2019-07-09 00:08:18.000000 rattail-0.9.98/rattail/filemon/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7586 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/filemon/actions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8765 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/filemon/win32.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/commands/
--rw-r--r--   0 lance     (1000) lance     (1000)    52530 2019-09-30 19:34:23.000000 rattail-0.9.98/rattail/commands/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19257 2019-07-29 17:32:46.000000 rattail-0.9.98/rattail/commands/importing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1198 2019-07-29 17:21:34.000000 rattail-0.9.98/rattail/commands/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2984 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/commands/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)    22945 2019-09-26 00:25:36.000000 rattail-0.9.98/rattail/commands/backup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2765 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/commands/dev.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6580 2019-04-29 14:24:13.000000 rattail-0.9.98/rattail/commands/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)    30360 2019-09-10 21:48:46.000000 rattail-0.9.98/rattail/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7049 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/csvutil.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20931 2019-09-30 18:56:08.000000 rattail-0.9.98/rattail/mail.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/datasync/
--rw-r--r--   0 lance     (1000) lance     (1000)    14670 2019-09-14 20:07:36.000000 rattail-0.9.98/rattail/datasync/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1215 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/datasync/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3885 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/datasync/watchers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4082 2018-11-24 21:50:56.000000 rattail-0.9.98/rattail/datasync/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9124 2019-09-20 20:07:17.000000 rattail-0.9.98/rattail/datasync/consumers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4942 2019-02-13 20:26:24.000000 rattail-0.9.98/rattail/datasync/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13968 2019-02-13 20:27:32.000000 rattail-0.9.98/rattail/datasync/daemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)       49 2019-10-04 19:31:11.000000 rattail-0.9.98/rattail/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6480 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/barcodes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4471 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/daemon.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-04 19:32:23.000000 rattail-0.9.98/rattail/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     7884 2019-04-19 17:06:36.000000 rattail-0.9.98/rattail/batch/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6529 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/batch/vendorinvoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5511 2019-04-24 03:50:21.000000 rattail-0.9.98/rattail/batch/product.py
--rw-r--r--   0 lance     (1000) lance     (1000)    99334 2019-06-08 18:16:30.000000 rattail-0.9.98/rattail/batch/purchase.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29941 2019-09-18 15:55:02.000000 rattail-0.9.98/rattail/batch/handlers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1103 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13152 2019-04-19 18:20:53.000000 rattail-0.9.98/rattail/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4561 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/batch/importer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6478 2019-09-04 16:09:16.000000 rattail-0.9.98/rattail/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3779 2018-12-11 19:53:49.000000 rattail-0.9.98/rattail/batch/filemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7373 2019-05-03 16:49:53.000000 rattail-0.9.98/rattail/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6885 2019-05-30 18:16:49.000000 rattail-0.9.98/rattail/batch/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1601 2018-11-17 22:12:16.000000 rattail-0.9.98/rattail/batch/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4919 2019-04-18 01:31:02.000000 rattail-0.9.98/rattail/batch/newproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7476 2019-09-20 22:24:25.000000 rattail-0.9.98/rattail/excel.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6735 2019-02-20 02:51:21.000000 rattail-0.9.98/rattail/settings.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3007 2019-09-30 18:27:02.000000 rattail-0.9.98/rattail/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8934 2019-09-13 01:54:41.000000 rattail-0.9.98/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)      505 2018-11-17 22:12:16.000000 rattail-0.9.98/covered.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-11-17 22:12:16.000000 rattail-0.9.98/COPYING.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/
+-rw-r--r--   0 lance     (1000) lance     (1000)      210 2019-10-07 16:55:27.000000 rattail-0.9.99/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1429 2019-10-07 16:55:27.000000 rattail-0.9.99/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)    95992 2019-10-07 16:54:13.000000 rattail-0.9.99/CHANGES.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1429 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)     2417 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      290 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)    21299 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      245 2018-11-17 22:12:16.000000 rattail-0.9.99/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-11-17 22:12:16.000000 rattail-0.9.99/MANIFEST.in
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/win32/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2506 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/win32/registry.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3367 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/win32/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6027 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/win32/service.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4161 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/win32/users.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2012 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/core.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/api/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3417 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/org.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2044 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1530 2019-09-18 15:55:44.000000 rattail-0.9.99/rattail/db/api/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7118 2019-09-18 15:55:54.000000 rattail-0.9.99/rattail/db/api/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2010 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2076 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1381 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1854 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/api/settings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11539 2019-06-05 21:22:51.000000 rattail-0.9.99/rattail/db/changes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2997 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/diffs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5037 2018-11-28 21:35:56.000000 rattail-0.9.99/rattail/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4928 2019-07-09 00:22:39.000000 rattail-0.9.99/rattail/db/continuum.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/alembic/
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail-0.9.99/rattail/db/alembic/README
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3693 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/9740f0dcf84b_add_tempmon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      662 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/6a1ec8b93637_add_productcost_discontinued.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6542 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/1f8e3cf6b2a2_add_handheld_batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1103 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/69d924015613_add_product_inventory.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      738 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/33c3b9acc341_make_message_recips_unique.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1399 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/35b1da3be8f5_add_bouncer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      774 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/9de6ffc1d2af_add_product_price_required.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2201 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/e5c3eab67b28_add_upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4183 2015-02-14 03:52:01.000000 rattail-0.9.99/rattail/db/alembic/versions/218562884128_add_vendor_invoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1124 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/7ba105af22a7_add_some_product_flags.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2655 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/b82daacc86b7_add_importer_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1320 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/017daa26c36c_add_employee_worked_shifts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      740 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/471299288da9_add_product_notes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      939 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/d87aeb7da072_allow_null_for_purchase_buyer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      835 2019-02-06 22:42:50.000000 rattail-0.9.99/rattail/db/alembic/versions/40a4855cb22d_add_receiving_truck_dump_children_first.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2260 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/35b451f8cc27_add_product_cost_discount.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      807 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/8b02c6eaf318_grow_datasync_change_source_consumer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      595 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/e1edeba632f8_grow_role_name.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1654 2019-04-24 03:41:44.000000 rattail-0.9.99/rattail/db/alembic/versions/90d5e8185d44_add_category_family_for_product_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1099 2019-03-08 19:47:35.000000 rattail-0.9.99/rattail/db/alembic/versions/5b393c108673_add_product_volatile.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      723 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/c384c65995db_make_cost_case_size_decimal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      572 2015-02-05 17:33:54.000000 rattail-0.9.99/rattail/db/alembic/versions/2e3f33b8ea46_increase_vendor_name_length.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1241 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a48db300576a_add_unit_pack_products.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      622 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/d042f5e34b77_add_person_modified.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      866 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/6c68c814f3c2_grow_change_key_columns.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      705 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/1f21b32fd2a7_add_inventory_prev_on_hand.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1138 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/27bcaa3c7f5f_add_employee_x_store.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1138 2019-04-18 23:11:45.000000 rattail-0.9.99/rattail/db/alembic/versions/5dee2f796f25_add_item_codes_for_pricing_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      699 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/f5c936a4cc62_add_inventory_batch_mode.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      632 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/528c049eb5b7_add_role_session_timeout.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      730 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/139fea9de0a0_add_upgrade_status.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      835 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a03ee3718ff4_add_dept_exempt_from_gross_sales.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3dc08453a5d3_add_batch_pricing_row_vendor.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6774 2019-04-18 00:55:51.000000 rattail-0.9.99/rattail/db/alembic/versions/4e5526fae79e_add_newproduct_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      882 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/16a72305f72c_add_purchase_item_item_id.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1335 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/b50a59f35e3f_add_scheduled_shifts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      976 2015-02-27 07:44:51.000000 rattail-0.9.99/rattail/db/alembic/versions/321f8f7b3887_add_product_special_order.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      996 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/0c91cf7d557b_add_invadjust_reason.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      615 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/c2af678f010c_make_tax_code_a_string.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1595 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/0a3dca1cd299_add_product_batch_row_item_entry.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      597 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/391fac830cb1_grow_category_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      640 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/765ce0ae5bbd_add_inventory_reason_hidden.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      757 2018-11-18 01:25:38.000000 rattail-0.9.99/rattail/db/alembic/versions/5ef33e961026_add_customer_wholesale.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1102 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/af4c4ec011fb_add_purchase_ship_method.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1819 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/40326eb83e18_add_messages.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/eb4e965ce771_grow_inventory_total_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      927 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/6551a4d9ff25_add_receiving_truck_dump_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4748 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3350e0220faf_add_purchases.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      653 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/14d23631733d_grow_datasyncchange_payload_type.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      825 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/aa32b6e51129_grow_product_description.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1812 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/b5aa18867ab3_add_purchase_batch_row_claim.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    35667 2015-02-10 05:51:10.000000 rattail-0.9.99/rattail/db/alembic/versions/47d30c955111_add_versioning.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2581 2019-03-01 16:57:54.000000 rattail-0.9.99/rattail/db/alembic/versions/03be1584f923_add_purchase_batch_truck_dump_status.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      765 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/51756b0edcdf_add_product_default_pack.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/9f1d111fa775_update_brand_version.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     3492 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/3df3144cec58_add_mailingaddress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      706 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/8c17754a6bbf_add_purchase_batch_complete.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1421 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/064f71d774ad_add_batch_ids.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1244 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/ea9718f6e6c6_add_product_store_info.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2872 2015-02-27 00:18:56.000000 rattail-0.9.99/rattail/db/alembic/versions/ee253b66b7b_add_tax.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1012 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/de4ebbf5bbb3_add_brand_confirmed.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      866 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/c1bfb033050d_add_vendor_catalog_row_cost_ref.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      625 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/195ceb6abeb3_add_customer_number.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1048 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/c2085638f487_add_pricing_batch_true_unit_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      652 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/2fe69ea73233_add_inventory_reason_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1996 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/123af5f6a0bc_add_purchase_damaged_expired_counts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1290 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/687646b42fce_add_batch_complete.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1074 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/e63d53698e9f_add_department_flags.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    27560 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/e9fca3d787ea_remove_old_versioning.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      789 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/86632a7bc5b5_add_employee_full_time.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      576 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/37e0e46ec6fe_add_user_last_login.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      778 2019-05-07 22:04:59.000000 rattail-0.9.99/rattail/db/alembic/versions/abd43933c6c6_add_report_output_params.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      923 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a8c96f5491ae_add_purchase_po_line_number.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1237 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/fd935205655d_add_item_id_for_product_batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2627 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/043d4bafc0be_add_batch_status.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1014 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/1242c7a0e24a_add_user_events.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      994 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/234c79420312_add_product_image.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1313 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/ff8662bbdb53_add_email_attempt.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2567 2018-12-18 22:43:20.000000 rattail-0.9.99/rattail/db/alembic/versions/bd7acb7028da_add_product_batch_subdepartment.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      772 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a9b37b388e56_add_product_status.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1120 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/ccd32c44393f_add_columns_for_vendor_catalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      731 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3f1e4a7b5268_add_catalog_suggested_retail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1576 2019-01-09 17:15:09.000000 rattail-0.9.99/rattail/db/alembic/versions/4db5dbf725f5_add_batch_extra_data.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      990 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/4137e9938122_add_foodstamp_and_tax_flags.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      688 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/5b88c82dbd8d_add_case_quantity_for_inventory_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      643 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3b5e0b87c176_add_user_active_sticky.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      659 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/09ed5bdc99f1_make_depositlink_code_a_string.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4013 2018-12-20 04:08:20.000000 rattail-0.9.99/rattail/db/alembic/versions/f3781f071de3_add_members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      956 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/86042c0323c6_add_credit_product_discarded.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      801 2018-12-19 21:09:36.000000 rattail-0.9.99/rattail/db/alembic/versions/45b90e4f8ab4_grow_product_uom_abbreviation.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4353 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/d6ca20fe9452_add_custorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1303 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a47a4d73b662_use_decimal_qty_for_handheld_inventory_.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      618 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/4da3fe4a368f_add_email_invalid_flag.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5675 2019-04-19 17:56:35.000000 rattail-0.9.99/rattail/db/alembic/versions/e1685bf9f1ad_add_product_batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      894 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/0174642e7b60_add_vendor_catalog_future.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      865 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/65098d24972f_add_transaction_meta.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1193 2019-04-18 21:21:23.000000 rattail-0.9.99/rattail/db/alembic/versions/727c63fcde2d_add_allowances_to_vendorcatalog_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3107 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/23600f00cda7_add_person_notes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      646 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/b9658d212053_add_customer_active_in_pos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19199 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3a500dc55e0f_add_more_versions.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      638 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/0b90d5c59fd7_add_person_middle_name.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      698 2015-02-12 02:00:12.000000 rattail-0.9.99/rattail/db/alembic/versions/268ff6454410_add_product_case_pack.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      748 2015-03-10 21:03:19.000000 rattail-0.9.99/rattail/db/alembic/versions/3623367c499f_add_product_last_sold.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      674 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/aa5962fb998e_add_inventory_unit_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      706 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/d67dee1cb849_grow_inventory_row_total_cost.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1242 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/835215361bb_add_change_uuid.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1193 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/57d12767eb53_add_employee_x_department.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1536 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/539c2df56562_add_batch_description.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2208 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a5a7358ed27f_inventory_from_handheld_batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      957 2019-03-07 21:38:03.000000 rattail-0.9.99/rattail/db/alembic/versions/6118198dc4db_add_purchase_batch_row_invoice_total_.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    35081 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a28c3583c8f0_add_product_versioning.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      691 2018-12-01 01:20:14.000000 rattail-0.9.99/rattail/db/alembic/versions/648cb088658c_add_batch_pricing_old_price_margin.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1307 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/0a5a866f2a3d_add_report_output.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      592 2015-02-11 08:49:31.000000 rattail-0.9.99/rattail/db/alembic/versions/f950be5601a_make_employee_person_unique.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2005 2015-02-27 06:10:01.000000 rattail-0.9.99/rattail/db/alembic/versions/3544687ae150_improve_size_fields.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1154 2015-02-24 02:04:59.000000 rattail-0.9.99/rattail/db/alembic/versions/3ef0fbcfb42e_make_invoice_quantities_decimal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3961 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3f266c89a3d4_add_pricing_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      688 2018-11-19 01:55:07.000000 rattail-0.9.99/rattail/db/alembic/versions/e645676eb37a_add_pricing_batch_suggested_price.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      949 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/20ec527fad0a_add_purchase_batch_row_item.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      635 2018-12-19 01:04:54.000000 rattail-0.9.99/rattail/db/alembic/versions/c5f39e2dec78_add_label_batch_label_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/4a4ae7ebdae6_add_purchase_batch_mode.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      925 2015-02-11 04:25:39.000000 rattail-0.9.99/rattail/db/alembic/versions/1513dc6d6ca7_add_product_deleted.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      859 2018-11-19 03:02:50.000000 rattail-0.9.99/rattail/db/alembic/versions/d28d28bc3cd0_add_pricing_batch_margin_diff.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1902 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/d3b6e3c971b4_add_product_future_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2610 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/7f88949a7ab9_add_employee_history.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2752 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3b2859694c53_add_new_versioning.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2121 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/3e79dd89fe12_add_label_handheld_batch_es_tie.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      878 2019-06-07 21:44:29.000000 rattail-0.9.99/rattail/db/alembic/versions/64d163d9de3a_add_purchase_batch_po_total_calculated.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      678 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/be079e974a52_add_purchase_batch_order_quantities_.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1065 2019-10-05 00:11:22.000000 rattail-0.9.99/rattail/db/alembic/versions/4f026ae58751_add_user_local_only.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      833 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/b3432785a839_add_inventory_total_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1727 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a809caf23cf0_grow_vendorcatalog_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      868 2018-12-19 00:20:25.000000 rattail-0.9.99/rattail/db/alembic/versions/95a66a59d420_add_label_batch_label_profile.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      965 2015-02-27 06:30:24.000000 rattail-0.9.99/rattail/db/alembic/versions/3c33f288ad62_add_product_discountable.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-12-19 01:05:51.000000 rattail-0.9.99/rattail/db/alembic/versions/a7b7246e48e2_grow_label_profile_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      823 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/92a49edc45c3_add_purchase_batch_invoice_file.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1052 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/11a9145414a9_add_product_suggested_price.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      835 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/6ef6db00abe8_add_product_discontinued.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      678 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/fb4bd12cbd37_add_label_batch_static_prices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      637 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/c37154504ae1_add_receiving_truck_dump.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1384 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/3a7029aed67_fix_user_x_role_null_bug.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      894 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a295dee8d1e9_add_credit_total.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      785 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/8e965902bf93_add_product_item_id_item_type.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      773 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/05d1ed3a4a28_add_vendor_abbreviation.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1269 2015-02-27 07:09:00.000000 rattail-0.9.99/rattail/db/alembic/versions/3f0d2a97f12a_add_vendor_schedule_fields.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14469 2015-02-07 21:40:45.000000 rattail-0.9.99/rattail/db/alembic/versions/33b76c3cb892_rename_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      798 2018-12-05 00:19:31.000000 rattail-0.9.99/rattail/db/alembic/versions/f7dc4e92752c_add_label_profile_sync_me.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5824 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/09976b73e96a_add_labels_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1233 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/977a76f259bd_add_purchase_shipped_counts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      897 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/90a3338b187b_add_credit_vendor_item_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1053 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/adcb91f473c3_add_purchase_item_out_of_stock.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      672 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/a33583135905_add_inventory_variance.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1500 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/830a20917c49_add_batch_row_modified.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8310 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/193c2dcdd14d_add_purchase_credits.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      573 2015-03-03 01:32:46.000000 rattail-0.9.99/rattail/db/alembic/versions/6cadbeb3f82_grow_report_code_name.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    25068 2015-01-27 18:54:45.000000 rattail-0.9.99/rattail/db/alembic/versions/1515aa76b64a_initial_schema.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3291 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/42edf57f1ae2_prevent_null_for_batch_comlete.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1036 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/cc3de1ca0689_add_customer_active_in_pos_sticky.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      675 2018-11-26 01:47:31.000000 rattail-0.9.99/rattail/db/alembic/versions/7eb0903932ff_add_pricing_batch_min_diff_percent.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1114 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/188810a5f9db_add_datasync_change.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/36ffa8b83782_make_batch_filename_nullable.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1573 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/cd23a59c5d89_add_dept_to_product_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      652 2018-12-18 04:05:26.000000 rattail-0.9.99/rattail/db/alembic/versions/c02430f167c2_add_pricing_batch_filename.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1086 2018-11-27 00:05:41.000000 rattail-0.9.99/rattail/db/alembic/versions/04f17c46b42f_grow_batch_pricing_row_margins.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1317 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/4bd528bca236_add_purchase_department.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5699 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/9a5511fdc9f5_add_purchase_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      916 2015-02-27 01:03:56.000000 rattail-0.9.99/rattail/db/alembic/versions/3f5be78f0f18_add_product_organic.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      818 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/14d83595afa1_add_category_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      741 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/45d7d92f4aa6_add_price_batch_thresholds.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)      645 2016-12-17 08:39:11.000000 rattail-0.9.99/rattail/db/alembic/versions/6e6d6e2ef0e_grow_change_class_name.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3163 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/4d2c5bdfecff_remove_legacy_batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      755 2015-02-14 10:02:44.000000 rattail-0.9.99/rattail/db/alembic/versions/2dd756a44a16_add_batchrow_status_text.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      837 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/0f4cb39da3cc_add_product_scancode_uom_abbrev.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      861 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/6a02ca0279c9_add_manual_flag_to_price_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3148 2015-02-27 00:18:56.000000 rattail-0.9.99/rattail/db/alembic/versions/2d046576154c_add_deposit_link.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      738 2015-02-12 01:14:37.000000 rattail-0.9.99/rattail/db/alembic/versions/571c070b7080_enlarge_product_cost_code.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      700 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/19da5ebe6fb5_add_label_batch_filename.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1433 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/versions/9305c1f493b4_add_batch_notes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      701 2019-01-08 18:34:55.000000 rattail-0.9.99/rattail/db/alembic/versions/fd7cf00b2918_grow_pricing_batch_row_markup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      610 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/script.py.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2013 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/alembic/env.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2679 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/dump.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/sync/
+-rw-r--r--   0 lance     (1000) lance     (1000)    12100 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/sync/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2052 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/sync/linux.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2423 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/sync/win32.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6462 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5797 2019-10-02 23:57:06.000000 rattail-0.9.99/rattail/db/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2041 2019-03-20 21:05:28.000000 rattail-0.9.99/rattail/db/types.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8361 2019-07-29 03:55:13.000000 rattail-0.9.99/rattail/db/cache.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5769 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/org.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5795 2019-01-31 04:58:30.000000 rattail-0.9.99/rattail/db/model/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4357 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4592 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/bouncer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8268 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/custorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3516 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9770 2019-07-31 02:47:08.000000 rattail-0.9.99/rattail/db/model/employees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5551 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/shifts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20450 2019-03-07 17:44:28.000000 rattail-0.9.99/rattail/db/model/purchase.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6832 2018-12-20 19:47:13.000000 rattail-0.9.99/rattail/db/model/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2124 2019-05-07 22:12:17.000000 rattail-0.9.99/rattail/db/model/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9826 2019-10-02 23:10:32.000000 rattail-0.9.99/rattail/db/model/contact.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3650 2019-04-19 18:19:41.000000 rattail-0.9.99/rattail/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4157 2018-12-19 01:01:57.000000 rattail-0.9.99/rattail/db/model/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2876 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    31847 2019-04-17 22:00:52.000000 rattail-0.9.99/rattail/db/model/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9443 2019-10-04 22:30:34.000000 rattail-0.9.99/rattail/db/model/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4472 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/messages.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3268 2019-07-03 01:51:01.000000 rattail-0.9.99/rattail/db/model/exports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11105 2019-08-25 20:00:52.000000 rattail-0.9.99/rattail/db/model/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6674 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8286 2019-10-05 00:06:28.000000 rattail-0.9.99/rattail/db/model/people.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/db/model/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)    15563 2019-09-17 22:17:21.000000 rattail-0.9.99/rattail/db/model/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2351 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/batch/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5276 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/batch/vendorinvoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5859 2019-04-24 03:39:32.000000 rattail-0.9.99/rattail/db/model/batch/product.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14538 2019-06-07 21:43:36.000000 rattail-0.9.99/rattail/db/model/batch/purchase.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1233 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8513 2018-12-19 01:04:14.000000 rattail-0.9.99/rattail/db/model/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6734 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7232 2019-04-18 21:20:56.000000 rattail-0.9.99/rattail/db/model/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6958 2019-04-18 23:10:58.000000 rattail-0.9.99/rattail/db/model/batch/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2324 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/batch/dynamic.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8055 2019-04-18 01:30:02.000000 rattail-0.9.99/rattail/db/model/batch/newproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4884 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/model/tempmon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6252 2019-06-11 03:17:43.000000 rattail-0.9.99/rattail/db/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5191 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/db/load.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1433 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/threads.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/contrib/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.99/rattail/contrib/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/contrib/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.99/rattail/contrib/vendors/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3590 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/dutchvalley.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3128 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/lotuslight.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5053 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/kehe.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4413 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/contrib/vendors/catalogs/unfi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/contrib/vendors/invoices/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2899 2019-01-24 20:04:56.000000 rattail-0.9.99/rattail/contrib/vendors/invoices/alberts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.99/rattail/contrib/vendors/invoices/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3270 2019-01-21 22:06:17.000000 rattail-0.9.99/rattail/contrib/vendors/invoices/kehe.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5079 2019-01-22 19:45:32.000000 rattail-0.9.99/rattail/contrib/vendors/invoices/unfi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1949 2018-12-03 03:25:44.000000 rattail-0.9.99/rattail/core.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/config/
+-rw-r--r--   0 lance     (1000) lance     (1000)      653 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/datasync.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)     2733 2018-12-01 23:55:42.000000 rattail-0.9.99/rattail/data/config/rattail.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      200 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/without-versioning.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)     1740 2018-12-01 22:37:08.000000 rattail-0.9.99/rattail/data/config/web.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      393 2018-07-05 07:17:19.000000 rattail-0.9.99/rattail/data/config/silent.conf~
+-rw-r--r--   0 lance     (1000) lance     (1000)      196 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/with-versioning.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      379 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/silent.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      852 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/filemon.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      393 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/config/quiet.conf
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/images/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7770 2013-07-22 19:33:54.000000 rattail-0.9.99/rattail/data/images/rattail_avatar.png
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/new-batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2519 2019-09-17 21:49:43.000000 rattail-0.9.99/rattail/data/new-batch/webview.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      702 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/new-batch/handler.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2750 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/new-batch/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3143 2019-08-17 07:08:35.000000 rattail-0.9.99/rattail/data/project/setup.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      182 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/MANIFEST.in_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)       28 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+dot+gitignore_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      177 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/README.rst_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/README
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/versions/.keepme
+-rw-r--r--   0 lance     (1000) lance     (1000)      640 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/script.py.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2017 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/alembic/env.py_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1184 2018-12-01 22:06:48.000000 rattail-0.9.99/rattail/data/project/+package+/db/model/core.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      288 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/db/model/__init__.py_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/web/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1133 2019-03-22 19:34:56.000000 rattail-0.9.99/rattail/data/project/+package+/web/app.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)     4353 2018-12-01 22:17:32.000000 rattail-0.9.99/rattail/data/project/+package+/web/menus.py~
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/
+-rw-r--r--   0 lance     (1000) lance     (1000)      711 2018-12-01 22:32:49.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl~
+-rw-r--r--   0 lance     (1000) lance     (1000)      810 2019-04-17 19:47:58.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/mobile/
+-rw-r--r--   0 lance     (1000) lance     (1000)      398 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/mobile/home.mako_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)     1171 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/templates/mobile/base.mako_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)     2386 2018-12-01 22:18:11.000000 rattail-0.9.99/rattail/data/project/+package+/web/menus.py_tmpl~
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/web/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)      371 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/views/common.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)     1349 2019-03-23 00:41:04.000000 rattail-0.9.99/rattail/data/project/+package+/web/views/__init__.py_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/project/+package+/web/static/
+-rw-r--r--   0 lance     (1000) lance     (1000)      211 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/static/__init__.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)     5142 2019-03-22 04:59:12.000000 rattail-0.9.99/rattail/data/project/+package+/web/menus.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      423 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/web/subscribers.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      527 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/emails.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      829 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/commands.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)      157 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/__init__.py_tmpl
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/project/+package+/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      526 2018-12-01 22:25:25.000000 rattail-0.9.99/rattail/data/project/+package+/config.py_tmpl
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/data/sample/
+-rw-r--r--   0 lance     (1000) lance     (1000)       51 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Brand.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      241 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/CustomerPerson.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)       69 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Store.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      418 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Product.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      124 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Vendor.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      141 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/VendorContact.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      281 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Subdepartment.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      228 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/EmployeeStore.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      306 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/User.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      253 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Employee.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      245 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Person.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      308 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/ProductCost.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      149 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Department.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)      201 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/data/sample/Customer.csv
+-rw-r--r--   0 lance     (1000) lance     (1000)     4838 2019-02-06 20:28:07.000000 rattail-0.9.99/rattail/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3979 2019-04-19 22:19:26.000000 rattail-0.9.99/rattail/progress.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/bouncer/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1015 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/bouncer/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5135 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/bouncer/handler.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4732 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/bouncer/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6644 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/bouncer/daemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1774 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/poddoc.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4960 2019-04-18 01:27:15.000000 rattail-0.9.99/rattail/gpc.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1439 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2691 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    17920 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_changes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7273 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5191 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1288 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2878 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/test_init.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2252 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/model/test_people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1483 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/model/test_users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1463 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/model/test_customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      696 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/db/model/test_datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1600 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_logging.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2006 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      341 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1178 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_csvutil.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3249 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      700 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_exceptions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2849 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_time.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      696 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_mail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7680 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_daemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6884 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/sil/
+-rw-r--r--   0 lance     (1000) lance     (1000)      456 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/sil/test_columns.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/sil/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      753 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_files.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/filemon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1804 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/filemon/test_util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/filemon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6594 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/filemon/test_actions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12154 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/filemon/test_config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3731 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/filemon/test_linux.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/tests/commands/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7514 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/commands/test_core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/commands/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5082 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/tests/test_barcodes.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/templates/mail/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5859 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/rattail_import_updates.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1292 2019-02-13 20:23:35.000000 rattail-0.9.99/rattail/templates/mail/datasync_error_consumer_process_changes.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      770 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/user_feedback.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      957 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/upgrade_failure.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1888 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/filemon_action_error.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      906 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/upgrade_success.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      459 2019-09-30 19:34:16.000000 rattail-0.9.99/rattail/templates/mail/run_n_mail.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1698 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/templates/mail/datasync_error_watcher_get_changes.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5187 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/exceptions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    17301 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/enum.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3807 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/logging.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/reporting/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4963 2019-05-09 19:47:38.000000 rattail-0.9.99/rattail/reporting/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3404 2019-05-07 21:58:29.000000 rattail-0.9.99/rattail/reporting/handlers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1150 2019-05-07 22:19:10.000000 rattail-0.9.99/rattail/reporting/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3575 2019-05-07 22:47:45.000000 rattail-0.9.99/rattail/reporting/excel.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6249 2019-07-29 18:09:48.000000 rattail-0.9.99/rattail/importing/sqlalchemy.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13797 2019-10-05 00:48:47.000000 rattail-0.9.99/rattail/importing/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7472 2019-08-16 01:06:00.000000 rattail-0.9.99/rattail/importing/csv.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7771 2019-02-19 01:32:29.000000 rattail-0.9.99/rattail/importing/rattail_bulk.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    26596 2019-09-17 19:11:09.000000 rattail-0.9.99/rattail/importing/handlers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1391 2019-07-29 17:44:14.000000 rattail-0.9.99/rattail/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5580 2019-07-29 17:40:49.000000 rattail-0.9.99/rattail/importing/exporters.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    30229 2019-07-29 16:39:05.000000 rattail-0.9.99/rattail/importing/importers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10519 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/importing/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3243 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/importing/postgresql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    88251 2019-10-05 00:39:36.000000 rattail-0.9.99/rattail/importing/model.py
+-rw-------   0 lance     (1000) lance     (1000)     7719 2019-06-05 19:14:09.000000 rattail-0.9.99/rattail/importing/sample.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1836 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/pod.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1427 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11328 2019-01-21 22:23:06.000000 rattail-0.9.99/rattail/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8426 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/palm.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4265 2019-06-05 19:29:18.000000 rattail-0.9.99/rattail/wince.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2015-01-19 06:19:47.000000 rattail-0.9.99/rattail/vendors/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4467 2019-04-18 22:01:11.000000 rattail-0.9.99/rattail/vendors/catalogs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4131 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/vendors/invoices.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/trainwreck/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/trainwreck/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/trainwreck/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11489 2019-09-10 18:37:33.000000 rattail-0.9.99/rattail/trainwreck/db/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/trainwreck/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2019-07-25 22:29:00.000000 rattail-0.9.99/rattail/trainwreck/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2416 2019-07-26 04:11:10.000000 rattail-0.9.99/rattail/trainwreck/importing/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2342 2019-07-26 04:09:39.000000 rattail-0.9.99/rattail/trainwreck/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4159 2019-07-28 19:48:28.000000 rattail-0.9.99/rattail/trainwreck/importing/trainwreck.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      131 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6569 2019-09-10 21:56:17.000000 rattail-0.9.99/rattail/trainwreck/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1680 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/trainwreck/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1889 2019-03-08 20:02:01.000000 rattail-0.9.99/rattail/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8304 2019-09-20 01:07:44.000000 rattail-0.9.99/rattail/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/sil/
+-rw-r--r--   0 lance     (1000) lance     (1000)    11136 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/sil/writer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1208 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/sil/exceptions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1289 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/sil/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6029 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/sil/columns.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2039 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/sil/batches.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7210 2019-02-13 20:22:58.000000 rattail-0.9.99/rattail/emails.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7563 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/files.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6358 2019-02-11 19:58:11.000000 rattail-0.9.99/rattail/time.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/filemon/
+-rw-r--r--   0 lance     (1000) lance     (1000)      999 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/filemon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2237 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/filemon/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4818 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/filemon/linux.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14326 2019-07-09 00:08:18.000000 rattail-0.9.99/rattail/filemon/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7586 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/filemon/actions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8765 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/filemon/win32.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/commands/
+-rw-r--r--   0 lance     (1000) lance     (1000)    52530 2019-09-30 19:34:23.000000 rattail-0.9.99/rattail/commands/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19257 2019-07-29 17:32:46.000000 rattail-0.9.99/rattail/commands/importing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1198 2019-07-29 17:21:34.000000 rattail-0.9.99/rattail/commands/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2984 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/commands/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    22945 2019-09-26 00:25:36.000000 rattail-0.9.99/rattail/commands/backup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2765 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/commands/dev.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6580 2019-04-29 14:24:13.000000 rattail-0.9.99/rattail/commands/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    30360 2019-09-10 21:48:46.000000 rattail-0.9.99/rattail/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7049 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/csvutil.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20931 2019-09-30 18:56:08.000000 rattail-0.9.99/rattail/mail.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/datasync/
+-rw-r--r--   0 lance     (1000) lance     (1000)    14670 2019-09-14 20:07:36.000000 rattail-0.9.99/rattail/datasync/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1215 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/datasync/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3885 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/datasync/watchers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4082 2018-11-24 21:50:56.000000 rattail-0.9.99/rattail/datasync/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9124 2019-09-20 20:07:17.000000 rattail-0.9.99/rattail/datasync/consumers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4942 2019-02-13 20:26:24.000000 rattail-0.9.99/rattail/datasync/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13968 2019-02-13 20:27:32.000000 rattail-0.9.99/rattail/datasync/daemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       49 2019-10-07 16:54:17.000000 rattail-0.9.99/rattail/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6480 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/barcodes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4471 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/daemon.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-10-07 16:55:27.000000 rattail-0.9.99/rattail/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7884 2019-04-19 17:06:36.000000 rattail-0.9.99/rattail/batch/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6529 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/batch/vendorinvoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5511 2019-04-24 03:50:21.000000 rattail-0.9.99/rattail/batch/product.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    99334 2019-06-08 18:16:30.000000 rattail-0.9.99/rattail/batch/purchase.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29941 2019-09-18 15:55:02.000000 rattail-0.9.99/rattail/batch/handlers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1103 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13152 2019-04-19 18:20:53.000000 rattail-0.9.99/rattail/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4561 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/batch/importer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6478 2019-09-04 16:09:16.000000 rattail-0.9.99/rattail/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3779 2018-12-11 19:53:49.000000 rattail-0.9.99/rattail/batch/filemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7373 2019-05-03 16:49:53.000000 rattail-0.9.99/rattail/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6885 2019-05-30 18:16:49.000000 rattail-0.9.99/rattail/batch/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1601 2018-11-17 22:12:16.000000 rattail-0.9.99/rattail/batch/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4919 2019-04-18 01:31:02.000000 rattail-0.9.99/rattail/batch/newproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7476 2019-09-20 22:24:25.000000 rattail-0.9.99/rattail/excel.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6735 2019-02-20 02:51:21.000000 rattail-0.9.99/rattail/settings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3189 2019-10-04 19:58:15.000000 rattail-0.9.99/rattail/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8934 2019-09-13 01:54:41.000000 rattail-0.9.99/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      505 2018-11-17 22:12:16.000000 rattail-0.9.99/covered.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-11-17 22:12:16.000000 rattail-0.9.99/COPYING.txt
```

### Comparing `rattail-0.9.98/PKG-INFO` & `rattail-0.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail
-Version: 0.9.98
+Version: 0.9.99
 Summary: Retail Software Framework
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Description: 
         Rattail
```

### Comparing `rattail-0.9.98/CHANGES.rst` & `rattail-0.9.99/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 
 CHANGELOG
 =========
 
+0.9.99 (2019-10-07)
+-------------------
+
+* Tweak Luigi summary filter logic for detecting "all good" message.
+
+* Add ``local_only`` flag for Person, User, plus "Global" importers.
+
+
 0.9.98 (2019-10-04)
 -------------------
 
 * Add ``remove_email()`` etc. for ContactMixin.
 
 * Provide default/fallback node title for importers' sake.
```

### Comparing `rattail-0.9.98/rattail.egg-info/PKG-INFO` & `rattail-0.9.99/rattail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail
-Version: 0.9.98
+Version: 0.9.99
 Summary: Retail Software Framework
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Description: 
         Rattail
```

### Comparing `rattail-0.9.98/rattail.egg-info/entry_points.txt` & `rattail-0.9.99/rattail.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail.egg-info/SOURCES.txt` & `rattail-0.9.99/rattail.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,15 @@
 rattail/db/alembic/versions/47d30c955111_add_versioning.py
 rattail/db/alembic/versions/4a4ae7ebdae6_add_purchase_batch_mode.py
 rattail/db/alembic/versions/4bd528bca236_add_purchase_department.py
 rattail/db/alembic/versions/4d2c5bdfecff_remove_legacy_batches.py
 rattail/db/alembic/versions/4da3fe4a368f_add_email_invalid_flag.py
 rattail/db/alembic/versions/4db5dbf725f5_add_batch_extra_data.py
 rattail/db/alembic/versions/4e5526fae79e_add_newproduct_batch.py
+rattail/db/alembic/versions/4f026ae58751_add_user_local_only.py
 rattail/db/alembic/versions/51756b0edcdf_add_product_default_pack.py
 rattail/db/alembic/versions/528c049eb5b7_add_role_session_timeout.py
 rattail/db/alembic/versions/539c2df56562_add_batch_description.py
 rattail/db/alembic/versions/571c070b7080_enlarge_product_cost_code.py
 rattail/db/alembic/versions/57d12767eb53_add_employee_x_department.py
 rattail/db/alembic/versions/5b393c108673_add_product_volatile.py
 rattail/db/alembic/versions/5b88c82dbd8d_add_case_quantity_for_inventory_batch.py
```

### Comparing `rattail-0.9.98/rattail/win32/registry.py` & `rattail-0.9.99/rattail/win32/registry.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/win32/__init__.py` & `rattail-0.9.99/rattail/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/win32/service.py` & `rattail-0.9.99/rattail/win32/service.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/win32/users.py` & `rattail-0.9.99/rattail/win32/users.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/core.py` & `rattail-0.9.99/rattail/db/core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/org.py` & `rattail-0.9.99/rattail/db/api/org.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/stores.py` & `rattail-0.9.99/rattail/db/api/stores.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/__init__.py` & `rattail-0.9.99/rattail/db/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/products.py` & `rattail-0.9.99/rattail/db/api/products.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/users.py` & `rattail-0.9.99/rattail/db/api/users.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/vendors.py` & `rattail-0.9.99/rattail/db/api/vendors.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/people.py` & `rattail-0.9.99/rattail/db/api/people.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/api/settings.py` & `rattail-0.9.99/rattail/db/api/settings.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/changes.py` & `rattail-0.9.99/rattail/db/changes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/diffs.py` & `rattail-0.9.99/rattail/db/diffs.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/__init__.py` & `rattail-0.9.99/rattail/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/continuum.py` & `rattail-0.9.99/rattail/db/continuum.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/9740f0dcf84b_add_tempmon.py` & `rattail-0.9.99/rattail/db/alembic/versions/9740f0dcf84b_add_tempmon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6a1ec8b93637_add_productcost_discontinued.py` & `rattail-0.9.99/rattail/db/alembic/versions/6a1ec8b93637_add_productcost_discontinued.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/1f8e3cf6b2a2_add_handheld_batches.py` & `rattail-0.9.99/rattail/db/alembic/versions/1f8e3cf6b2a2_add_handheld_batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/69d924015613_add_product_inventory.py` & `rattail-0.9.99/rattail/db/alembic/versions/69d924015613_add_product_inventory.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/33c3b9acc341_make_message_recips_unique.py` & `rattail-0.9.99/rattail/db/alembic/versions/33c3b9acc341_make_message_recips_unique.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/35b1da3be8f5_add_bouncer.py` & `rattail-0.9.99/rattail/db/alembic/versions/35b1da3be8f5_add_bouncer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/9de6ffc1d2af_add_product_price_required.py` & `rattail-0.9.99/rattail/db/alembic/versions/9de6ffc1d2af_add_product_price_required.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e5c3eab67b28_add_upgrades.py` & `rattail-0.9.99/rattail/db/alembic/versions/e5c3eab67b28_add_upgrades.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/218562884128_add_vendor_invoice.py` & `rattail-0.9.99/rattail/db/alembic/versions/218562884128_add_vendor_invoice.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/7ba105af22a7_add_some_product_flags.py` & `rattail-0.9.99/rattail/db/alembic/versions/7ba105af22a7_add_some_product_flags.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/b82daacc86b7_add_importer_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/b82daacc86b7_add_importer_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/017daa26c36c_add_employee_worked_shifts.py` & `rattail-0.9.99/rattail/db/alembic/versions/017daa26c36c_add_employee_worked_shifts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/471299288da9_add_product_notes.py` & `rattail-0.9.99/rattail/db/alembic/versions/471299288da9_add_product_notes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d87aeb7da072_allow_null_for_purchase_buyer.py` & `rattail-0.9.99/rattail/db/alembic/versions/d87aeb7da072_allow_null_for_purchase_buyer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/40a4855cb22d_add_receiving_truck_dump_children_first.py` & `rattail-0.9.99/rattail/db/alembic/versions/40a4855cb22d_add_receiving_truck_dump_children_first.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/35b451f8cc27_add_product_cost_discount.py` & `rattail-0.9.99/rattail/db/alembic/versions/35b451f8cc27_add_product_cost_discount.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/8b02c6eaf318_grow_datasync_change_source_consumer.py` & `rattail-0.9.99/rattail/db/alembic/versions/8b02c6eaf318_grow_datasync_change_source_consumer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e1edeba632f8_grow_role_name.py` & `rattail-0.9.99/rattail/db/alembic/versions/e1edeba632f8_grow_role_name.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/90d5e8185d44_add_category_family_for_product_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/90d5e8185d44_add_category_family_for_product_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/5b393c108673_add_product_volatile.py` & `rattail-0.9.99/rattail/db/alembic/versions/5b393c108673_add_product_volatile.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c384c65995db_make_cost_case_size_decimal.py` & `rattail-0.9.99/rattail/db/alembic/versions/c384c65995db_make_cost_case_size_decimal.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/2e3f33b8ea46_increase_vendor_name_length.py` & `rattail-0.9.99/rattail/db/alembic/versions/2e3f33b8ea46_increase_vendor_name_length.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a48db300576a_add_unit_pack_products.py` & `rattail-0.9.99/rattail/db/alembic/versions/a48db300576a_add_unit_pack_products.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d042f5e34b77_add_person_modified.py` & `rattail-0.9.99/rattail/db/alembic/versions/d042f5e34b77_add_person_modified.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6c68c814f3c2_grow_change_key_columns.py` & `rattail-0.9.99/rattail/db/alembic/versions/6c68c814f3c2_grow_change_key_columns.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/1f21b32fd2a7_add_inventory_prev_on_hand.py` & `rattail-0.9.99/rattail/db/alembic/versions/1f21b32fd2a7_add_inventory_prev_on_hand.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/27bcaa3c7f5f_add_employee_x_store.py` & `rattail-0.9.99/rattail/db/alembic/versions/27bcaa3c7f5f_add_employee_x_store.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/5dee2f796f25_add_item_codes_for_pricing_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/5dee2f796f25_add_item_codes_for_pricing_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/f5c936a4cc62_add_inventory_batch_mode.py` & `rattail-0.9.99/rattail/db/alembic/versions/f5c936a4cc62_add_inventory_batch_mode.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/528c049eb5b7_add_role_session_timeout.py` & `rattail-0.9.99/rattail/db/alembic/versions/528c049eb5b7_add_role_session_timeout.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/139fea9de0a0_add_upgrade_status.py` & `rattail-0.9.99/rattail/db/alembic/versions/139fea9de0a0_add_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a03ee3718ff4_add_dept_exempt_from_gross_sales.py` & `rattail-0.9.99/rattail/db/alembic/versions/a03ee3718ff4_add_dept_exempt_from_gross_sales.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3dc08453a5d3_add_batch_pricing_row_vendor.py` & `rattail-0.9.99/rattail/db/alembic/versions/3dc08453a5d3_add_batch_pricing_row_vendor.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4e5526fae79e_add_newproduct_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/4e5526fae79e_add_newproduct_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/16a72305f72c_add_purchase_item_item_id.py` & `rattail-0.9.99/rattail/db/alembic/versions/16a72305f72c_add_purchase_item_item_id.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/b50a59f35e3f_add_scheduled_shifts.py` & `rattail-0.9.99/rattail/db/alembic/versions/b50a59f35e3f_add_scheduled_shifts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/321f8f7b3887_add_product_special_order.py` & `rattail-0.9.99/rattail/db/alembic/versions/321f8f7b3887_add_product_special_order.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0c91cf7d557b_add_invadjust_reason.py` & `rattail-0.9.99/rattail/db/alembic/versions/0c91cf7d557b_add_invadjust_reason.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c2af678f010c_make_tax_code_a_string.py` & `rattail-0.9.99/rattail/db/alembic/versions/c2af678f010c_make_tax_code_a_string.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0a3dca1cd299_add_product_batch_row_item_entry.py` & `rattail-0.9.99/rattail/db/alembic/versions/0a3dca1cd299_add_product_batch_row_item_entry.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/391fac830cb1_grow_category_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/391fac830cb1_grow_category_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/765ce0ae5bbd_add_inventory_reason_hidden.py` & `rattail-0.9.99/rattail/db/alembic/versions/765ce0ae5bbd_add_inventory_reason_hidden.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/5ef33e961026_add_customer_wholesale.py` & `rattail-0.9.99/rattail/db/alembic/versions/5ef33e961026_add_customer_wholesale.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/af4c4ec011fb_add_purchase_ship_method.py` & `rattail-0.9.99/rattail/db/alembic/versions/af4c4ec011fb_add_purchase_ship_method.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/40326eb83e18_add_messages.py` & `rattail-0.9.99/rattail/db/alembic/versions/40326eb83e18_add_messages.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/eb4e965ce771_grow_inventory_total_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/eb4e965ce771_grow_inventory_total_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6551a4d9ff25_add_receiving_truck_dump_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/6551a4d9ff25_add_receiving_truck_dump_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3350e0220faf_add_purchases.py` & `rattail-0.9.99/rattail/db/alembic/versions/3350e0220faf_add_purchases.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/14d23631733d_grow_datasyncchange_payload_type.py` & `rattail-0.9.99/rattail/db/alembic/versions/14d23631733d_grow_datasyncchange_payload_type.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/aa32b6e51129_grow_product_description.py` & `rattail-0.9.99/rattail/db/alembic/versions/aa32b6e51129_grow_product_description.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/b5aa18867ab3_add_purchase_batch_row_claim.py` & `rattail-0.9.99/rattail/db/alembic/versions/b5aa18867ab3_add_purchase_batch_row_claim.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/47d30c955111_add_versioning.py` & `rattail-0.9.99/rattail/db/alembic/versions/47d30c955111_add_versioning.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/03be1584f923_add_purchase_batch_truck_dump_status.py` & `rattail-0.9.99/rattail/db/alembic/versions/03be1584f923_add_purchase_batch_truck_dump_status.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/51756b0edcdf_add_product_default_pack.py` & `rattail-0.9.99/rattail/db/alembic/versions/51756b0edcdf_add_product_default_pack.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/9f1d111fa775_update_brand_version.py` & `rattail-0.9.99/rattail/db/alembic/versions/9f1d111fa775_update_brand_version.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3df3144cec58_add_mailingaddress.py` & `rattail-0.9.99/rattail/db/alembic/versions/3df3144cec58_add_mailingaddress.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/8c17754a6bbf_add_purchase_batch_complete.py` & `rattail-0.9.99/rattail/db/alembic/versions/8c17754a6bbf_add_purchase_batch_complete.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/064f71d774ad_add_batch_ids.py` & `rattail-0.9.99/rattail/db/alembic/versions/064f71d774ad_add_batch_ids.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/ea9718f6e6c6_add_product_store_info.py` & `rattail-0.9.99/rattail/db/alembic/versions/ea9718f6e6c6_add_product_store_info.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/ee253b66b7b_add_tax.py` & `rattail-0.9.99/rattail/db/alembic/versions/ee253b66b7b_add_tax.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/de4ebbf5bbb3_add_brand_confirmed.py` & `rattail-0.9.99/rattail/db/alembic/versions/de4ebbf5bbb3_add_brand_confirmed.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c1bfb033050d_add_vendor_catalog_row_cost_ref.py` & `rattail-0.9.99/rattail/db/alembic/versions/c1bfb033050d_add_vendor_catalog_row_cost_ref.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/195ceb6abeb3_add_customer_number.py` & `rattail-0.9.99/rattail/db/alembic/versions/195ceb6abeb3_add_customer_number.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c2085638f487_add_pricing_batch_true_unit_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/c2085638f487_add_pricing_batch_true_unit_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/2fe69ea73233_add_inventory_reason_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/2fe69ea73233_add_inventory_reason_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/123af5f6a0bc_add_purchase_damaged_expired_counts.py` & `rattail-0.9.99/rattail/db/alembic/versions/123af5f6a0bc_add_purchase_damaged_expired_counts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/687646b42fce_add_batch_complete.py` & `rattail-0.9.99/rattail/db/alembic/versions/687646b42fce_add_batch_complete.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e63d53698e9f_add_department_flags.py` & `rattail-0.9.99/rattail/db/alembic/versions/e63d53698e9f_add_department_flags.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e9fca3d787ea_remove_old_versioning.py` & `rattail-0.9.99/rattail/db/alembic/versions/e9fca3d787ea_remove_old_versioning.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/86632a7bc5b5_add_employee_full_time.py` & `rattail-0.9.99/rattail/db/alembic/versions/86632a7bc5b5_add_employee_full_time.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/37e0e46ec6fe_add_user_last_login.py` & `rattail-0.9.99/rattail/db/alembic/versions/37e0e46ec6fe_add_user_last_login.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/abd43933c6c6_add_report_output_params.py` & `rattail-0.9.99/rattail/db/alembic/versions/abd43933c6c6_add_report_output_params.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a8c96f5491ae_add_purchase_po_line_number.py` & `rattail-0.9.99/rattail/db/alembic/versions/a8c96f5491ae_add_purchase_po_line_number.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/fd935205655d_add_item_id_for_product_batches.py` & `rattail-0.9.99/rattail/db/alembic/versions/fd935205655d_add_item_id_for_product_batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/043d4bafc0be_add_batch_status.py` & `rattail-0.9.99/rattail/db/alembic/versions/043d4bafc0be_add_batch_status.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/1242c7a0e24a_add_user_events.py` & `rattail-0.9.99/rattail/db/alembic/versions/1242c7a0e24a_add_user_events.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/234c79420312_add_product_image.py` & `rattail-0.9.99/rattail/db/alembic/versions/234c79420312_add_product_image.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/ff8662bbdb53_add_email_attempt.py` & `rattail-0.9.99/rattail/db/alembic/versions/ff8662bbdb53_add_email_attempt.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/bd7acb7028da_add_product_batch_subdepartment.py` & `rattail-0.9.99/rattail/db/alembic/versions/bd7acb7028da_add_product_batch_subdepartment.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a9b37b388e56_add_product_status.py` & `rattail-0.9.99/rattail/db/alembic/versions/a9b37b388e56_add_product_status.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/ccd32c44393f_add_columns_for_vendor_catalog.py` & `rattail-0.9.99/rattail/db/alembic/versions/ccd32c44393f_add_columns_for_vendor_catalog.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3f1e4a7b5268_add_catalog_suggested_retail.py` & `rattail-0.9.99/rattail/db/alembic/versions/3f1e4a7b5268_add_catalog_suggested_retail.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4db5dbf725f5_add_batch_extra_data.py` & `rattail-0.9.99/rattail/db/alembic/versions/4db5dbf725f5_add_batch_extra_data.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4137e9938122_add_foodstamp_and_tax_flags.py` & `rattail-0.9.99/rattail/db/alembic/versions/4137e9938122_add_foodstamp_and_tax_flags.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/5b88c82dbd8d_add_case_quantity_for_inventory_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/5b88c82dbd8d_add_case_quantity_for_inventory_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3b5e0b87c176_add_user_active_sticky.py` & `rattail-0.9.99/rattail/db/alembic/versions/3b5e0b87c176_add_user_active_sticky.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/09ed5bdc99f1_make_depositlink_code_a_string.py` & `rattail-0.9.99/rattail/db/alembic/versions/09ed5bdc99f1_make_depositlink_code_a_string.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/f3781f071de3_add_members.py` & `rattail-0.9.99/rattail/db/alembic/versions/f3781f071de3_add_members.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/86042c0323c6_add_credit_product_discarded.py` & `rattail-0.9.99/rattail/db/alembic/versions/86042c0323c6_add_credit_product_discarded.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/45b90e4f8ab4_grow_product_uom_abbreviation.py` & `rattail-0.9.99/rattail/db/alembic/versions/45b90e4f8ab4_grow_product_uom_abbreviation.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d6ca20fe9452_add_custorders.py` & `rattail-0.9.99/rattail/db/alembic/versions/d6ca20fe9452_add_custorders.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a47a4d73b662_use_decimal_qty_for_handheld_inventory_.py` & `rattail-0.9.99/rattail/db/alembic/versions/a47a4d73b662_use_decimal_qty_for_handheld_inventory_.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4da3fe4a368f_add_email_invalid_flag.py` & `rattail-0.9.99/rattail/db/alembic/versions/4da3fe4a368f_add_email_invalid_flag.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e1685bf9f1ad_add_product_batches.py` & `rattail-0.9.99/rattail/db/alembic/versions/e1685bf9f1ad_add_product_batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0174642e7b60_add_vendor_catalog_future.py` & `rattail-0.9.99/rattail/db/alembic/versions/0174642e7b60_add_vendor_catalog_future.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/65098d24972f_add_transaction_meta.py` & `rattail-0.9.99/rattail/db/alembic/versions/65098d24972f_add_transaction_meta.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/727c63fcde2d_add_allowances_to_vendorcatalog_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/727c63fcde2d_add_allowances_to_vendorcatalog_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/23600f00cda7_add_person_notes.py` & `rattail-0.9.99/rattail/db/alembic/versions/23600f00cda7_add_person_notes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/b9658d212053_add_customer_active_in_pos.py` & `rattail-0.9.99/rattail/db/alembic/versions/b9658d212053_add_customer_active_in_pos.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3a500dc55e0f_add_more_versions.py` & `rattail-0.9.99/rattail/db/alembic/versions/3a500dc55e0f_add_more_versions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0b90d5c59fd7_add_person_middle_name.py` & `rattail-0.9.99/rattail/db/alembic/versions/0b90d5c59fd7_add_person_middle_name.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/268ff6454410_add_product_case_pack.py` & `rattail-0.9.99/rattail/db/alembic/versions/268ff6454410_add_product_case_pack.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3623367c499f_add_product_last_sold.py` & `rattail-0.9.99/rattail/db/alembic/versions/3623367c499f_add_product_last_sold.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/aa5962fb998e_add_inventory_unit_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/aa5962fb998e_add_inventory_unit_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d67dee1cb849_grow_inventory_row_total_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/d67dee1cb849_grow_inventory_row_total_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/835215361bb_add_change_uuid.py` & `rattail-0.9.99/rattail/db/alembic/versions/835215361bb_add_change_uuid.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/57d12767eb53_add_employee_x_department.py` & `rattail-0.9.99/rattail/db/alembic/versions/57d12767eb53_add_employee_x_department.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/539c2df56562_add_batch_description.py` & `rattail-0.9.99/rattail/db/alembic/versions/539c2df56562_add_batch_description.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a5a7358ed27f_inventory_from_handheld_batches.py` & `rattail-0.9.99/rattail/db/alembic/versions/a5a7358ed27f_inventory_from_handheld_batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6118198dc4db_add_purchase_batch_row_invoice_total_.py` & `rattail-0.9.99/rattail/db/alembic/versions/6118198dc4db_add_purchase_batch_row_invoice_total_.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a28c3583c8f0_add_product_versioning.py` & `rattail-0.9.99/rattail/db/alembic/versions/a28c3583c8f0_add_product_versioning.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/648cb088658c_add_batch_pricing_old_price_margin.py` & `rattail-0.9.99/rattail/db/alembic/versions/648cb088658c_add_batch_pricing_old_price_margin.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0a5a866f2a3d_add_report_output.py` & `rattail-0.9.99/rattail/db/alembic/versions/0a5a866f2a3d_add_report_output.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/f950be5601a_make_employee_person_unique.py` & `rattail-0.9.99/rattail/db/alembic/versions/f950be5601a_make_employee_person_unique.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3544687ae150_improve_size_fields.py` & `rattail-0.9.99/rattail/db/alembic/versions/3544687ae150_improve_size_fields.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3ef0fbcfb42e_make_invoice_quantities_decimal.py` & `rattail-0.9.99/rattail/db/alembic/versions/3ef0fbcfb42e_make_invoice_quantities_decimal.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3f266c89a3d4_add_pricing_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/3f266c89a3d4_add_pricing_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/e645676eb37a_add_pricing_batch_suggested_price.py` & `rattail-0.9.99/rattail/db/alembic/versions/e645676eb37a_add_pricing_batch_suggested_price.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/20ec527fad0a_add_purchase_batch_row_item.py` & `rattail-0.9.99/rattail/db/alembic/versions/20ec527fad0a_add_purchase_batch_row_item.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c5f39e2dec78_add_label_batch_label_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/c5f39e2dec78_add_label_batch_label_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4a4ae7ebdae6_add_purchase_batch_mode.py` & `rattail-0.9.99/rattail/db/alembic/versions/4a4ae7ebdae6_add_purchase_batch_mode.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/1513dc6d6ca7_add_product_deleted.py` & `rattail-0.9.99/rattail/db/alembic/versions/1513dc6d6ca7_add_product_deleted.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d28d28bc3cd0_add_pricing_batch_margin_diff.py` & `rattail-0.9.99/rattail/db/alembic/versions/d28d28bc3cd0_add_pricing_batch_margin_diff.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/d3b6e3c971b4_add_product_future_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/d3b6e3c971b4_add_product_future_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/7f88949a7ab9_add_employee_history.py` & `rattail-0.9.99/rattail/db/alembic/versions/7f88949a7ab9_add_employee_history.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3b2859694c53_add_new_versioning.py` & `rattail-0.9.99/rattail/db/alembic/versions/3b2859694c53_add_new_versioning.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3e79dd89fe12_add_label_handheld_batch_es_tie.py` & `rattail-0.9.99/rattail/db/alembic/versions/3e79dd89fe12_add_label_handheld_batch_es_tie.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/64d163d9de3a_add_purchase_batch_po_total_calculated.py` & `rattail-0.9.99/rattail/db/alembic/versions/64d163d9de3a_add_purchase_batch_po_total_calculated.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/be079e974a52_add_purchase_batch_order_quantities_.py` & `rattail-0.9.99/rattail/db/alembic/versions/be079e974a52_add_purchase_batch_order_quantities_.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/b3432785a839_add_inventory_total_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/b3432785a839_add_inventory_total_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a809caf23cf0_grow_vendorcatalog_cost.py` & `rattail-0.9.99/rattail/db/alembic/versions/a809caf23cf0_grow_vendorcatalog_cost.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/95a66a59d420_add_label_batch_label_profile.py` & `rattail-0.9.99/rattail/db/alembic/versions/95a66a59d420_add_label_batch_label_profile.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3c33f288ad62_add_product_discountable.py` & `rattail-0.9.99/rattail/db/alembic/versions/3c33f288ad62_add_product_discountable.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a7b7246e48e2_grow_label_profile_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/a7b7246e48e2_grow_label_profile_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/92a49edc45c3_add_purchase_batch_invoice_file.py` & `rattail-0.9.99/rattail/db/alembic/versions/92a49edc45c3_add_purchase_batch_invoice_file.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/11a9145414a9_add_product_suggested_price.py` & `rattail-0.9.99/rattail/db/alembic/versions/11a9145414a9_add_product_suggested_price.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6ef6db00abe8_add_product_discontinued.py` & `rattail-0.9.99/rattail/db/alembic/versions/6ef6db00abe8_add_product_discontinued.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/fb4bd12cbd37_add_label_batch_static_prices.py` & `rattail-0.9.99/rattail/db/alembic/versions/fb4bd12cbd37_add_label_batch_static_prices.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c37154504ae1_add_receiving_truck_dump.py` & `rattail-0.9.99/rattail/db/alembic/versions/c37154504ae1_add_receiving_truck_dump.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3a7029aed67_fix_user_x_role_null_bug.py` & `rattail-0.9.99/rattail/db/alembic/versions/3a7029aed67_fix_user_x_role_null_bug.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a295dee8d1e9_add_credit_total.py` & `rattail-0.9.99/rattail/db/alembic/versions/a295dee8d1e9_add_credit_total.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/8e965902bf93_add_product_item_id_item_type.py` & `rattail-0.9.99/rattail/db/alembic/versions/8e965902bf93_add_product_item_id_item_type.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/05d1ed3a4a28_add_vendor_abbreviation.py` & `rattail-0.9.99/rattail/db/alembic/versions/05d1ed3a4a28_add_vendor_abbreviation.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3f0d2a97f12a_add_vendor_schedule_fields.py` & `rattail-0.9.99/rattail/db/alembic/versions/3f0d2a97f12a_add_vendor_schedule_fields.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/33b76c3cb892_rename_tables.py` & `rattail-0.9.99/rattail/db/alembic/versions/33b76c3cb892_rename_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/f7dc4e92752c_add_label_profile_sync_me.py` & `rattail-0.9.99/rattail/db/alembic/versions/f7dc4e92752c_add_label_profile_sync_me.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/09976b73e96a_add_labels_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/09976b73e96a_add_labels_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/977a76f259bd_add_purchase_shipped_counts.py` & `rattail-0.9.99/rattail/db/alembic/versions/977a76f259bd_add_purchase_shipped_counts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/90a3338b187b_add_credit_vendor_item_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/90a3338b187b_add_credit_vendor_item_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/adcb91f473c3_add_purchase_item_out_of_stock.py` & `rattail-0.9.99/rattail/db/alembic/versions/adcb91f473c3_add_purchase_item_out_of_stock.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/a33583135905_add_inventory_variance.py` & `rattail-0.9.99/rattail/db/alembic/versions/a33583135905_add_inventory_variance.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/830a20917c49_add_batch_row_modified.py` & `rattail-0.9.99/rattail/db/alembic/versions/830a20917c49_add_batch_row_modified.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/193c2dcdd14d_add_purchase_credits.py` & `rattail-0.9.99/rattail/db/alembic/versions/193c2dcdd14d_add_purchase_credits.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6cadbeb3f82_grow_report_code_name.py` & `rattail-0.9.99/rattail/db/alembic/versions/6cadbeb3f82_grow_report_code_name.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/1515aa76b64a_initial_schema.py` & `rattail-0.9.99/rattail/db/alembic/versions/1515aa76b64a_initial_schema.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/42edf57f1ae2_prevent_null_for_batch_comlete.py` & `rattail-0.9.99/rattail/db/alembic/versions/42edf57f1ae2_prevent_null_for_batch_comlete.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/cc3de1ca0689_add_customer_active_in_pos_sticky.py` & `rattail-0.9.99/rattail/db/alembic/versions/cc3de1ca0689_add_customer_active_in_pos_sticky.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/7eb0903932ff_add_pricing_batch_min_diff_percent.py` & `rattail-0.9.99/rattail/db/alembic/versions/7eb0903932ff_add_pricing_batch_min_diff_percent.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/188810a5f9db_add_datasync_change.py` & `rattail-0.9.99/rattail/db/alembic/versions/188810a5f9db_add_datasync_change.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/36ffa8b83782_make_batch_filename_nullable.py` & `rattail-0.9.99/rattail/db/alembic/versions/36ffa8b83782_make_batch_filename_nullable.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/cd23a59c5d89_add_dept_to_product_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/cd23a59c5d89_add_dept_to_product_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/c02430f167c2_add_pricing_batch_filename.py` & `rattail-0.9.99/rattail/db/alembic/versions/c02430f167c2_add_pricing_batch_filename.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/04f17c46b42f_grow_batch_pricing_row_margins.py` & `rattail-0.9.99/rattail/db/alembic/versions/04f17c46b42f_grow_batch_pricing_row_margins.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4bd528bca236_add_purchase_department.py` & `rattail-0.9.99/rattail/db/alembic/versions/4bd528bca236_add_purchase_department.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/9a5511fdc9f5_add_purchase_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/9a5511fdc9f5_add_purchase_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/3f5be78f0f18_add_product_organic.py` & `rattail-0.9.99/rattail/db/alembic/versions/3f5be78f0f18_add_product_organic.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/14d83595afa1_add_category_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/14d83595afa1_add_category_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/45d7d92f4aa6_add_price_batch_thresholds.py` & `rattail-0.9.99/rattail/db/alembic/versions/45d7d92f4aa6_add_price_batch_thresholds.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6e6d6e2ef0e_grow_change_class_name.py` & `rattail-0.9.99/rattail/db/alembic/versions/6e6d6e2ef0e_grow_change_class_name.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/4d2c5bdfecff_remove_legacy_batches.py` & `rattail-0.9.99/rattail/db/alembic/versions/4d2c5bdfecff_remove_legacy_batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/2dd756a44a16_add_batchrow_status_text.py` & `rattail-0.9.99/rattail/db/alembic/versions/2dd756a44a16_add_batchrow_status_text.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/0f4cb39da3cc_add_product_scancode_uom_abbrev.py` & `rattail-0.9.99/rattail/db/alembic/versions/0f4cb39da3cc_add_product_scancode_uom_abbrev.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/6a02ca0279c9_add_manual_flag_to_price_batch.py` & `rattail-0.9.99/rattail/db/alembic/versions/6a02ca0279c9_add_manual_flag_to_price_batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/2d046576154c_add_deposit_link.py` & `rattail-0.9.99/rattail/db/alembic/versions/2d046576154c_add_deposit_link.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/571c070b7080_enlarge_product_cost_code.py` & `rattail-0.9.99/rattail/db/alembic/versions/571c070b7080_enlarge_product_cost_code.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/19da5ebe6fb5_add_label_batch_filename.py` & `rattail-0.9.99/rattail/db/alembic/versions/19da5ebe6fb5_add_label_batch_filename.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/9305c1f493b4_add_batch_notes.py` & `rattail-0.9.99/rattail/db/alembic/versions/9305c1f493b4_add_batch_notes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/versions/fd7cf00b2918_grow_pricing_batch_row_markup.py` & `rattail-0.9.99/rattail/db/alembic/versions/fd7cf00b2918_grow_pricing_batch_row_markup.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/script.py.mako` & `rattail-0.9.99/rattail/db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/alembic/env.py` & `rattail-0.9.99/rattail/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/dump.py` & `rattail-0.9.99/rattail/db/dump.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/sync/__init__.py` & `rattail-0.9.99/rattail/db/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/sync/linux.py` & `rattail-0.9.99/rattail/db/sync/linux.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/sync/win32.py` & `rattail-0.9.99/rattail/db/sync/win32.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/auth.py` & `rattail-0.9.99/rattail/db/auth.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/util.py` & `rattail-0.9.99/rattail/db/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/types.py` & `rattail-0.9.99/rattail/db/types.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/cache.py` & `rattail-0.9.99/rattail/db/cache.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/org.py` & `rattail-0.9.99/rattail/db/model/org.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/core.py` & `rattail-0.9.99/rattail/db/model/core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/upgrades.py` & `rattail-0.9.99/rattail/db/model/upgrades.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/bouncer.py` & `rattail-0.9.99/rattail/db/model/bouncer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/custorders.py` & `rattail-0.9.99/rattail/db/model/custorders.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/stores.py` & `rattail-0.9.99/rattail/db/model/stores.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/employees.py` & `rattail-0.9.99/rattail/db/model/employees.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/shifts.py` & `rattail-0.9.99/rattail/db/model/shifts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/purchase.py` & `rattail-0.9.99/rattail/db/model/purchase.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/members.py` & `rattail-0.9.99/rattail/db/model/members.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/reports.py` & `rattail-0.9.99/rattail/db/model/reports.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/contact.py` & `rattail-0.9.99/rattail/db/model/contact.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/__init__.py` & `rattail-0.9.99/rattail/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/labels.py` & `rattail-0.9.99/rattail/db/model/labels.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/datasync.py` & `rattail-0.9.99/rattail/db/model/datasync.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/products.py` & `rattail-0.9.99/rattail/db/model/products.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/users.py` & `rattail-0.9.99/rattail/db/model/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,14 +128,19 @@
     accounts from another system, esp. on a regular basis, you might be keeping
     the :attr:`active` flag in sync along with that.  But in some cases you
     might want to *not* keep the active flag in sync, for certain accounts.
     Hence this "active sticky" flag, which may be used to mark certain accounts
     as off-limits from the general active flag sync.
     """)
 
+    local_only = sa.Column(sa.Boolean(), nullable=True, doc="""
+    Flag indicating the user account is somehow specific to the "local" app
+    node etc. and should not be synced elsewhere.
+    """)
+
     last_login = sa.Column(sa.DateTime(), nullable=True, doc="""
     Timestamp when user last logged into the system.
     """)
 
     def __str__(self):
         if self.person and str(self.person):
             return str(self.person)
```

### Comparing `rattail-0.9.98/rattail/db/model/messages.py` & `rattail-0.9.99/rattail/db/model/messages.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/exports.py` & `rattail-0.9.99/rattail/db/model/exports.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/customers.py` & `rattail-0.9.99/rattail/db/model/customers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/vendors.py` & `rattail-0.9.99/rattail/db/model/vendors.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/people.py` & `rattail-0.9.99/rattail/db/model/people.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 
     uuid = uuid_column()
     first_name = sa.Column(sa.String(length=50), nullable=True)
     middle_name = sa.Column(sa.String(length=50), nullable=True)
     last_name = sa.Column(sa.String(length=50), nullable=True)
     # TODO: rename this to 'full_name' at some point...?
     display_name = sa.Column(sa.String(length=100), nullable=True)
+
+    local_only = sa.Column(sa.Boolean(), nullable=True, doc="""
+    Flag indicating the person is somehow specific to the "local" app node
+    etc. and should not be synced elsewhere.
+    """)
+
     modified = sa.Column(sa.DateTime(), nullable=True, onupdate=datetime.datetime.utcnow)
 
     users = orm.relationship(
         'User', doc="""
         List of user accounts associated with this person.
         """)
```

### Comparing `rattail-0.9.98/rattail/db/model/batch/core.py` & `rattail-0.9.99/rattail/db/model/batch/core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/handheld.py` & `rattail-0.9.99/rattail/db/model/batch/handheld.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/vendorinvoice.py` & `rattail-0.9.99/rattail/db/model/batch/vendorinvoice.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/product.py` & `rattail-0.9.99/rattail/db/model/batch/product.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/purchase.py` & `rattail-0.9.99/rattail/db/model/batch/purchase.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/__init__.py` & `rattail-0.9.99/rattail/db/model/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/labels.py` & `rattail-0.9.99/rattail/db/model/batch/labels.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/inventory.py` & `rattail-0.9.99/rattail/db/model/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/vendorcatalog.py` & `rattail-0.9.99/rattail/db/model/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/pricing.py` & `rattail-0.9.99/rattail/db/model/batch/pricing.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/dynamic.py` & `rattail-0.9.99/rattail/db/model/batch/dynamic.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/batch/newproduct.py` & `rattail-0.9.99/rattail/db/model/batch/newproduct.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/model/tempmon.py` & `rattail-0.9.99/rattail/db/model/tempmon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/config.py` & `rattail-0.9.99/rattail/db/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/db/load.py` & `rattail-0.9.99/rattail/db/load.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/threads.py` & `rattail-0.9.99/rattail/threads.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/catalogs/dutchvalley.py` & `rattail-0.9.99/rattail/contrib/vendors/catalogs/dutchvalley.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/catalogs/lotuslight.py` & `rattail-0.9.99/rattail/contrib/vendors/catalogs/lotuslight.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/catalogs/kehe.py` & `rattail-0.9.99/rattail/contrib/vendors/catalogs/kehe.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/catalogs/unfi.py` & `rattail-0.9.99/rattail/contrib/vendors/catalogs/unfi.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/invoices/alberts.py` & `rattail-0.9.99/rattail/contrib/vendors/invoices/alberts.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/invoices/kehe.py` & `rattail-0.9.99/rattail/contrib/vendors/invoices/kehe.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/contrib/vendors/invoices/unfi.py` & `rattail-0.9.99/rattail/contrib/vendors/invoices/unfi.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/core.py` & `rattail-0.9.99/rattail/core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/config/datasync.conf` & `rattail-0.9.99/rattail/data/config/datasync.conf`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/config/rattail.conf` & `rattail-0.9.99/rattail/data/config/rattail.conf`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/config/web.conf` & `rattail-0.9.99/rattail/data/config/web.conf`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/config/filemon.conf` & `rattail-0.9.99/rattail/data/config/filemon.conf`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/images/rattail_avatar.png` & `rattail-0.9.99/rattail/data/images/rattail_avatar.png`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/new-batch/webview.py` & `rattail-0.9.99/rattail/data/new-batch/webview.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/new-batch/handler.py` & `rattail-0.9.99/rattail/data/new-batch/handler.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/new-batch/model.py` & `rattail-0.9.99/rattail/data/new-batch/model.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/setup.py_tmpl` & `rattail-0.9.99/rattail/data/project/setup.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/db/alembic/script.py.mako` & `rattail-0.9.99/rattail/data/project/+package+/db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/db/alembic/env.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/db/alembic/env.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/db/model/core.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/db/model/core.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/app.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/web/app.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/menus.py~` & `rattail-0.9.99/rattail/data/project/+package+/web/menus.py~`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl~` & `rattail-0.9.99/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl~`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/web/templates/base_meta.mako_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/templates/mobile/base.mako_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/web/templates/mobile/base.mako_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/menus.py_tmpl~` & `rattail-0.9.99/rattail/data/project/+package+/web/menus.py_tmpl~`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/views/__init__.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/web/views/__init__.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/web/menus.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/web/menus.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/emails.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/emails.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/commands.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/commands.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/data/project/+package+/config.py_tmpl` & `rattail-0.9.99/rattail/data/project/+package+/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/upgrades.py` & `rattail-0.9.99/rattail/upgrades.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/progress.py` & `rattail-0.9.99/rattail/progress.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/bouncer/__init__.py` & `rattail-0.9.99/rattail/bouncer/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/bouncer/handler.py` & `rattail-0.9.99/rattail/bouncer/handler.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/bouncer/config.py` & `rattail-0.9.99/rattail/bouncer/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/bouncer/daemon.py` & `rattail-0.9.99/rattail/bouncer/daemon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/poddoc.py` & `rattail-0.9.99/rattail/poddoc.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/gpc.py` & `rattail-0.9.99/rattail/gpc.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_util.py` & `rattail-0.9.99/rattail/tests/db/test_util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_core.py` & `rattail-0.9.99/rattail/tests/db/test_core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_changes.py` & `rattail-0.9.99/rattail/tests/db/test_changes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_model.py` & `rattail-0.9.99/rattail/tests/db/test_model.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_config.py` & `rattail-0.9.99/rattail/tests/db/test_config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_auth.py` & `rattail-0.9.99/rattail/tests/db/test_auth.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/test_init.py` & `rattail-0.9.99/rattail/tests/db/test_init.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/model/test_people.py` & `rattail-0.9.99/rattail/tests/db/model/test_people.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/model/test_users.py` & `rattail-0.9.99/rattail/tests/db/model/test_users.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/model/test_customers.py` & `rattail-0.9.99/rattail/tests/db/model/test_customers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/db/model/test_datasync.py` & `rattail-0.9.99/rattail/tests/db/model/test_datasync.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_logging.py` & `rattail-0.9.99/rattail/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_util.py` & `rattail-0.9.99/rattail/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_csvutil.py` & `rattail-0.9.99/rattail/tests/test_csvutil.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/__init__.py` & `rattail-0.9.99/rattail/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_exceptions.py` & `rattail-0.9.99/rattail/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_time.py` & `rattail-0.9.99/rattail/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_mail.py` & `rattail-0.9.99/rattail/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_daemon.py` & `rattail-0.9.99/rattail/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_config.py` & `rattail-0.9.99/rattail/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_files.py` & `rattail-0.9.99/rattail/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/filemon/test_util.py` & `rattail-0.9.99/rattail/tests/filemon/test_util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/filemon/test_actions.py` & `rattail-0.9.99/rattail/tests/filemon/test_actions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/filemon/test_config.py` & `rattail-0.9.99/rattail/tests/filemon/test_config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/filemon/test_linux.py` & `rattail-0.9.99/rattail/tests/filemon/test_linux.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/commands/test_core.py` & `rattail-0.9.99/rattail/tests/commands/test_core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/tests/test_barcodes.py` & `rattail-0.9.99/rattail/tests/test_barcodes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/rattail_import_updates.html.mako` & `rattail-0.9.99/rattail/templates/mail/rattail_import_updates.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/datasync_error_consumer_process_changes.html.mako` & `rattail-0.9.99/rattail/templates/mail/datasync_error_consumer_process_changes.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/user_feedback.html.mako` & `rattail-0.9.99/rattail/templates/mail/user_feedback.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/upgrade_failure.html.mako` & `rattail-0.9.99/rattail/templates/mail/upgrade_failure.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/filemon_action_error.html.mako` & `rattail-0.9.99/rattail/templates/mail/filemon_action_error.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/upgrade_success.html.mako` & `rattail-0.9.99/rattail/templates/mail/upgrade_success.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/templates/mail/datasync_error_watcher_get_changes.html.mako` & `rattail-0.9.99/rattail/templates/mail/datasync_error_watcher_get_changes.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/exceptions.py` & `rattail-0.9.99/rattail/exceptions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/enum.py` & `rattail-0.9.99/rattail/enum.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/logging.py` & `rattail-0.9.99/rattail/logging.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/reporting/reports.py` & `rattail-0.9.99/rattail/reporting/reports.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/reporting/handlers.py` & `rattail-0.9.99/rattail/reporting/handlers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/reporting/__init__.py` & `rattail-0.9.99/rattail/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/reporting/excel.py` & `rattail-0.9.99/rattail/reporting/excel.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/sqlalchemy.py` & `rattail-0.9.99/rattail/importing/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/rattail.py` & `rattail-0.9.99/rattail/importing/rattail.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 ################################################################################
 """
 Rattail -> Rattail data import
 """
 
 from __future__ import unicode_literals, absolute_import
 
+import sqlalchemy as sa
+
 from rattail.db import Session
 from rattail.importing import model
 from rattail.importing.handlers import FromSQLAlchemyHandler, ToSQLAlchemyHandler
 from rattail.importing.sqlalchemy import FromSQLAlchemySameToSame
 from rattail.util import OrderedDict
 
 
@@ -65,19 +67,21 @@
     """
     Common base class for Rattail -> Rattail data import/export handlers.
     """
 
     def get_importers(self):
         importers = OrderedDict()
         importers['Person'] = PersonImporter
+        importers['GlobalPerson'] = GlobalPersonImporter
         importers['PersonEmailAddress'] = PersonEmailAddressImporter
         importers['PersonPhoneNumber'] = PersonPhoneNumberImporter
         importers['PersonMailingAddress'] = PersonMailingAddressImporter
         importers['User'] = UserImporter
         importers['AdminUser'] = AdminUserImporter
+        importers['GlobalUser'] = GlobalUserImporter
         importers['Message'] = MessageImporter
         importers['MessageRecipient'] = MessageRecipientImporter
         importers['Store'] = StoreImporter
         importers['StorePhoneNumber'] = StorePhoneNumberImporter
         importers['Employee'] = EmployeeImporter
         importers['EmployeeStore'] = EmployeeStoreImporter
         importers['EmployeeEmailAddress'] = EmployeeEmailAddressImporter
@@ -115,18 +119,26 @@
         importers['ProductVolatile'] = ProductVolatileImporter
         importers['ProductImage'] = ProductImageImporter
         importers['LabelProfile'] = LabelProfileImporter
         return importers
 
     def get_default_keys(self):
         keys = self.get_importer_keys()
-        if 'AdminUser' in keys:
-            keys.remove('AdminUser')
-        if 'ProductImage' in keys:
-            keys.remove('ProductImage')
+
+        avoid_by_default = [
+            'GlobalPerson',
+            'AdminUser',
+            'GlobalUser',
+            'ProductImage',
+        ]
+
+        for key in avoid_by_default:
+            if key in keys:
+                keys.remove(key)
+
         return keys
 
 
 class FromRattailToRattailImport(FromRattailToRattailBase, FromRattailHandler, ToRattailHandler):
     """
     Handler for Rattail (other) -> Rattail (local) data import.
 
@@ -177,26 +189,62 @@
     Base class for Rattail -> Rattail data importers.
     """
 
 
 class PersonImporter(FromRattail, model.PersonImporter):
     pass
 
+
+class GlobalPersonImporter(FromRattail, model.GlobalPersonImporter):
+    """
+    This is a customized version of the :class:`PersonImporter`, which simply
+    avoids "local only" person accounts.
+    """
+
+    def query(self):
+        query = super(GlobalPersonImporter, self).query()
+
+        # never include "local only" people
+        query = query.filter(sa.or_(
+            self.host_model_class.local_only == False,
+            self.host_model_class.local_only == None))
+
+        return query
+
+
 class PersonEmailAddressImporter(FromRattail, model.PersonEmailAddressImporter):
     pass
 
 class PersonPhoneNumberImporter(FromRattail, model.PersonPhoneNumberImporter):
     pass
 
 class PersonMailingAddressImporter(FromRattail, model.PersonMailingAddressImporter):
     pass
 
 class UserImporter(FromRattail, model.UserImporter):
     pass
 
+
+class GlobalUserImporter(FromRattail, model.GlobalUserImporter):
+    """
+    This is a customized version of the :class:`UserImporter`, which simply
+    avoids "local only" user accounts.
+    """
+
+    def query(self):
+        query = super(GlobalUserImporter, self).query()
+
+        # never include "local only" users
+        query = query.filter(sa.or_(
+            self.host_model_class.local_only == False,
+            self.host_model_class.local_only == None))
+
+        return query
+
+
 class AdminUserImporter(FromRattail, model.AdminUserImporter):
 
     @property
     def supported_fields(self):
         return super(AdminUserImporter, self).supported_fields + [
             'admin',
         ]
```

### Comparing `rattail-0.9.98/rattail/importing/csv.py` & `rattail-0.9.99/rattail/importing/csv.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/rattail_bulk.py` & `rattail-0.9.99/rattail/importing/rattail_bulk.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/handlers.py` & `rattail-0.9.99/rattail/importing/handlers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/__init__.py` & `rattail-0.9.99/rattail/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/exporters.py` & `rattail-0.9.99/rattail/importing/exporters.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/importers.py` & `rattail-0.9.99/rattail/importing/importers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/versions.py` & `rattail-0.9.99/rattail/importing/versions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/postgresql.py` & `rattail-0.9.99/rattail/importing/postgresql.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/importing/model.py` & `rattail-0.9.99/rattail/importing/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2018 Lance Edgar
+#  Copyright © 2010-2019 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -26,14 +26,15 @@
 
 from __future__ import unicode_literals, absolute_import
 
 import datetime
 import logging
 
 import six
+import sqlalchemy as sa
 from sqlalchemy import orm
 from sqlalchemy.orm.exc import NoResultFound
 
 from rattail.db import model, auth
 from rattail.importing import ToSQLAlchemy, BatchImporter
 from rattail.db.util import maxlen, normalize_full_name, format_phone_number, normalize_phone_number
 from rattail.time import localtime, make_utc
@@ -82,14 +83,31 @@
 class PersonImporter(ToRattail):
     """
     Person data importer.
     """
     model_class = model.Person
 
 
+class GlobalPersonImporter(PersonImporter):
+    """
+    This is a customized version of the :class:`PersonImporter`, which simply
+    avoids "local only" person accounts.
+    """
+
+    def cache_query(self):
+        query = super(GlobalPersonImporter, self).cache_query()
+
+        # never include "local only" people
+        query = query.filter(sa.or_(
+            self.model_class.local_only == False,
+            self.model_class.local_only == None))
+
+        return query
+
+
 class PersonEmailAddressImporter(ToRattail):
     """
     Person email address data importer.
     """
     model_class = model.PersonEmailAddress
 
     @property
@@ -279,14 +297,31 @@
                         user.roles.append(admin)
                 else:
                     if admin in user.roles:
                         user.roles.remove(admin)
             return user
 
 
+class GlobalUserImporter(UserImporter):
+    """
+    This is a customized version of the :class:`UserImporter`, which simply
+    avoids "local only" user accounts.
+    """
+
+    def cache_query(self):
+        query = super(GlobalUserImporter, self).cache_query()
+
+        # never include "local only" users
+        query = query.filter(sa.or_(
+            self.model_class.local_only == False,
+            self.model_class.local_only == None))
+
+        return query
+
+
 class MessageImporter(ToRattail):
     """
     User message data importer.
     """
     model_class = model.Message
```

### Comparing `rattail-0.9.98/rattail/importing/sample.py` & `rattail-0.9.99/rattail/importing/sample.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/pod.py` & `rattail-0.9.99/rattail/pod.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/__init__.py` & `rattail-0.9.99/rattail/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/labels.py` & `rattail-0.9.99/rattail/labels.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/palm.py` & `rattail-0.9.99/rattail/palm.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/wince.py` & `rattail-0.9.99/rattail/wince.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/vendors/catalogs.py` & `rattail-0.9.99/rattail/vendors/catalogs.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/vendors/invoices.py` & `rattail-0.9.99/rattail/vendors/invoices.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/db/model.py` & `rattail-0.9.99/rattail/trainwreck/db/model.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/importing/__init__.py` & `rattail-0.9.99/rattail/trainwreck/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/importing/util.py` & `rattail-0.9.99/rattail/trainwreck/importing/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/importing/model.py` & `rattail-0.9.99/rattail/trainwreck/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/importing/trainwreck.py` & `rattail-0.9.99/rattail/trainwreck/importing/trainwreck.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/commands.py` & `rattail-0.9.99/rattail/trainwreck/commands.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/trainwreck/config.py` & `rattail-0.9.99/rattail/trainwreck/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/pricing.py` & `rattail-0.9.99/rattail/pricing.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/util.py` & `rattail-0.9.99/rattail/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/sil/writer.py` & `rattail-0.9.99/rattail/sil/writer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/sil/exceptions.py` & `rattail-0.9.99/rattail/sil/exceptions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/sil/__init__.py` & `rattail-0.9.99/rattail/sil/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/sil/columns.py` & `rattail-0.9.99/rattail/sil/columns.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/sil/batches.py` & `rattail-0.9.99/rattail/sil/batches.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/emails.py` & `rattail-0.9.99/rattail/emails.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/files.py` & `rattail-0.9.99/rattail/files.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/time.py` & `rattail-0.9.99/rattail/time.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/__init__.py` & `rattail-0.9.99/rattail/filemon/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/util.py` & `rattail-0.9.99/rattail/filemon/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/linux.py` & `rattail-0.9.99/rattail/filemon/linux.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/config.py` & `rattail-0.9.99/rattail/filemon/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/actions.py` & `rattail-0.9.99/rattail/filemon/actions.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/filemon/win32.py` & `rattail-0.9.99/rattail/filemon/win32.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/core.py` & `rattail-0.9.99/rattail/commands/core.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/importing.py` & `rattail-0.9.99/rattail/commands/importing.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/__init__.py` & `rattail-0.9.99/rattail/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/products.py` & `rattail-0.9.99/rattail/commands/products.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/backup.py` & `rattail-0.9.99/rattail/commands/backup.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/dev.py` & `rattail-0.9.99/rattail/commands/dev.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/commands/batch.py` & `rattail-0.9.99/rattail/commands/batch.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/config.py` & `rattail-0.9.99/rattail/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/csvutil.py` & `rattail-0.9.99/rattail/csvutil.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/mail.py` & `rattail-0.9.99/rattail/mail.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/rattail.py` & `rattail-0.9.99/rattail/datasync/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/__init__.py` & `rattail-0.9.99/rattail/datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/watchers.py` & `rattail-0.9.99/rattail/datasync/watchers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/util.py` & `rattail-0.9.99/rattail/datasync/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/consumers.py` & `rattail-0.9.99/rattail/datasync/consumers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/config.py` & `rattail-0.9.99/rattail/datasync/config.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/datasync/daemon.py` & `rattail-0.9.99/rattail/datasync/daemon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/barcodes.py` & `rattail-0.9.99/rattail/barcodes.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/daemon.py` & `rattail-0.9.99/rattail/daemon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/handheld.py` & `rattail-0.9.99/rattail/batch/handheld.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/vendorinvoice.py` & `rattail-0.9.99/rattail/batch/vendorinvoice.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/product.py` & `rattail-0.9.99/rattail/batch/product.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/purchase.py` & `rattail-0.9.99/rattail/batch/purchase.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/handlers.py` & `rattail-0.9.99/rattail/batch/handlers.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/__init__.py` & `rattail-0.9.99/rattail/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/labels.py` & `rattail-0.9.99/rattail/batch/labels.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/importer.py` & `rattail-0.9.99/rattail/batch/importer.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/inventory.py` & `rattail-0.9.99/rattail/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/filemon.py` & `rattail-0.9.99/rattail/batch/filemon.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/vendorcatalog.py` & `rattail-0.9.99/rattail/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/pricing.py` & `rattail-0.9.99/rattail/batch/pricing.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/util.py` & `rattail-0.9.99/rattail/batch/util.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/batch/newproduct.py` & `rattail-0.9.99/rattail/batch/newproduct.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/excel.py` & `rattail-0.9.99/rattail/excel.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/settings.py` & `rattail-0.9.99/rattail/settings.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/rattail/luigi.py` & `rattail-0.9.99/rattail/luigi.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,14 +82,20 @@
 class WarnSummaryIfProblems(logging.Filter):
     """
     Custom logging filter, to elevate the Luigi "execution summary" message to
     WARNING level, if any problems are detected for the run.  Note that this
     simply checks for the ``:)`` message to know if there were problem.
     """
 
+    good_messages = [
+        "This progress looks :) because there were no failed tasks or missing external dependencies",
+        "This progress looks :) because there were no failed tasks or missing dependencies",
+    ]
+
+
     def filter(self, record):
         if record.name == 'luigi-interface' and record.levelno == logging.INFO:
             if "===== Luigi Execution Summary =====" in record.msg:
-                if "This progress looks :) because there were no failed tasks or missing dependencies" not in record.msg:
+                if not any([msg in record.msg for msg in self.good_messages]):
                     record.levelno = logging.WARNING
                     record.levelname = 'WARNING'
         return True
```

### Comparing `rattail-0.9.98/setup.py` & `rattail-0.9.99/setup.py`

 * *Files identical despite different names*

### Comparing `rattail-0.9.98/COPYING.txt` & `rattail-0.9.99/COPYING.txt`

 * *Files identical despite different names*

