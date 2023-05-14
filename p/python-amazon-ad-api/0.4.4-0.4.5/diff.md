# Comparing `tmp/python-amazon-ad-api-0.4.4.tar.gz` & `tmp/python-amazon-ad-api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-ad-api-0.4.4.tar", last modified: Sat Apr 22 12:35:56 2023, max compression
+gzip compressed data, was "python-amazon-ad-api-0.4.5.tar", last modified: Sat May 13 08:35:40 2023, max compression
```

## Comparing `python-amazon-ad-api-0.4.4.tar` & `python-amazon-ad-api-0.4.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.351555 python-amazon-ad-api-0.4.4/ad_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.355555 python-amazon-ad-api-0.4.4/ad_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/advertising_test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/brand_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/creative_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.355555 python-amazon-ad-api-0.4.4/ad_api/api/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/eligibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/manager_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.359555 python-amazon-ad-api-0.4.4/ad_api/api/sb/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ads_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/brands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/landing_page_asins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.359555 python-amazon-ad-api-0.4.4/ad_api/api/sd/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/brand_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns_budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/creatives.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.363555 python-amazon-ad-api-0.4.4/ad_api/api/sp/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_initial_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_consolidated_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaings_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ranked_keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/suggested_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/validation_configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/ad_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/ad_api/base/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.802837 python-amazon-ad-api-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-05-13 08:35:40.802837 python-amazon-ad-api-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.778837 python-amazon-ad-api-0.4.5/ad_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.786837 python-amazon-ad-api-0.4.5/ad_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/advertising_test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/brand_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/creative_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.786837 python-amazon-ad-api-0.4.5/ad_api/api/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/dsp/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/dsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/dsp/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/dsp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/manager_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.794837 python-amazon-ad-api-0.4.5/ad_api/api/sb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/ad_groups_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/ads_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/campaigns_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/landing_page_asins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sb/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.794837 python-amazon-ad-api-0.4.5/ad_api/api/sd/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/brand_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/creatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sd/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.798838 python-amazon-ad-api-0.4.5/ad_api/api/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/ad_groups_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/bid_recommendations_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_initial_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_rules_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_consolidated_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/campaings_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/product_ads_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/product_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/ranked_keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/sp/suggested_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/api/validation_configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.798838 python-amazon-ad-api-0.4.5/ad_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.802837 python-amazon-ad-api-0.4.5/ad_api/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/ad_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:35:40.802837 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-05-13 08:35:40.000000 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-13 08:35:40.000000 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 08:35:40.000000 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-13 08:35:40.000000 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 08:35:40.000000 python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-13 08:35:40.802837 python-amazon-ad-api-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-13 08:35:21.000000 python-amazon-ad-api-0.4.5/setup.py
```

### Comparing `python-amazon-ad-api-0.4.4/LICENSE` & `python-amazon-ad-api-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/PKG-INFO` & `python-amazon-ad-api-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-amazon-ad-api-0.4.4/README.md` & `python-amazon-ad-api-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/__init__.py` & `python-amazon-ad-api-0.4.5/ad_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/advertising_test_account.py` & `python-amazon-ad-api-0.4.5/ad_api/api/advertising_test_account.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/attribution.py` & `python-amazon-ad-api-0.4.5/ad_api/api/attribution.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/audiences.py` & `python-amazon-ad-api-0.4.5/ad_api/api/audiences.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/billing.py` & `python-amazon-ad-api-0.4.5/ad_api/api/billing.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/brand_metrics.py` & `python-amazon-ad-api-0.4.5/ad_api/api/brand_metrics.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/creative_assets.py` & `python-amazon-ad-api-0.4.5/ad_api/api/creative_assets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/dsp/credential_provider.py` & `python-amazon-ad-api-0.4.5/ad_api/api/dsp/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/dsp/reports.py` & `python-amazon-ad-api-0.4.5/ad_api/api/dsp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/eligibility.py` & `python-amazon-ad-api-0.4.5/ad_api/api/eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/history.py` & `python-amazon-ad-api-0.4.5/ad_api/api/history.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/insights.py` & `python-amazon-ad-api-0.4.5/ad_api/api/insights.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/invoices.py` & `python-amazon-ad-api-0.4.5/ad_api/api/invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/localization.py` & `python-amazon-ad-api-0.4.5/ad_api/api/localization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/manager_accounts.py` & `python-amazon-ad-api-0.4.5/ad_api/api/manager_accounts.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/metadata.py` & `python-amazon-ad-api-0.4.5/ad_api/api/metadata.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/portfolios.py` & `python-amazon-ad-api-0.4.5/ad_api/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/profiles.py` & `python-amazon-ad-api-0.4.5/ad_api/api/profiles.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/reports.py` & `python-amazon-ad-api-0.4.5/ad_api/api/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/__init__.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups_v4.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/ad_groups_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/ads_v4.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/ads_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/bid_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/brands.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/brands.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns_v4.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/campaigns_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/landing_page_asins.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/landing_page_asins.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/media.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/media.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/moderation.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/moderation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/reports.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/snapshots.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/stores.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/stores.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sb/targeting_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sb/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/__init__.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/ad_groups.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/bid_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/brand_safety.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/brand_safety.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/budget_rules.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/budget_rules.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns_budget_usage.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/campaigns_budget_usage.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/creatives.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/creatives.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/forecast.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/forecast.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/negative_product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/product_ads.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/reports.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/snapshots.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sd/targeting_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sd/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/__init__.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/ad_groups_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/bid_recommendations_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_initial_recommendation.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_initial_recommendation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_rules.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/budget_rules_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_consolidated_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_consolidated_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_targets.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaign_negative_targets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_budget_usage.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns_budget_usage.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaigns_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaings_optimization.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/campaings_optimization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/negative_product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/product_ads_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting_v3.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/ranked_keywords_recommendations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/ranked_keywords_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/reports.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/snapshots.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/sp/suggested_keywords.py` & `python-amazon-ad-api-0.4.5/ad_api/api/sp/suggested_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/api/validation_configurations.py` & `python-amazon-ad-api-0.4.5/ad_api/api/validation_configurations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/auth/access_token_client.py` & `python-amazon-ad-api-0.4.5/ad_api/auth/access_token_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/__init__.py` & `python-amazon-ad-api-0.4.5/ad_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/api_response.py` & `python-amazon-ad-api-0.4.5/ad_api/base/api_response.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/client.py` & `python-amazon-ad-api-0.4.5/ad_api/base/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/config.py` & `python-amazon-ad-api-0.4.5/ad_api/base/config.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/credential_provider.py` & `python-amazon-ad-api-0.4.5/ad_api/base/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/exceptions.py` & `python-amazon-ad-api-0.4.5/ad_api/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/helpers.py` & `python-amazon-ad-api-0.4.5/ad_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/marketplaces.py` & `python-amazon-ad-api-0.4.5/ad_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/ad_api/base/utils.py` & `python-amazon-ad-api-0.4.5/ad_api/base/utils.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/PKG-INFO` & `python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/SOURCES.txt` & `python-amazon-ad-api-0.4.5/python_amazon_ad_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.4/setup.cfg` & `python-amazon-ad-api-0.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-amazon-ad-api
-version = 0.4.4
+version = 0.4.5
 author = Daniel Alvaro
 author_email = denisneuf@hotmail.com
 description = Python wrapper for the Amazon Advertising API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/denisneuf/python-amazon-ad-api
 project_urls =
```

### Comparing `python-amazon-ad-api-0.4.4/setup.py` & `python-amazon-ad-api-0.4.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='python-amazon-ad-api',
-    version='0.4.4',
+    version='0.4.5',
     install_requires=[
-        "requests>=2.27.1,<2.29.0",
+        "requests>=2.27.1,<2.31.0",
         "six~=1.16.0",
         "cachetools>=5.0,<5.4",
         "pycryptodome>=3.13,<3.18",
         "python-dotenv>=0.19.2,<1.1.0",
         "pytz>=2021.3,<2024.0",
         "confuse>=1.7,<2.1",
     ],
```

