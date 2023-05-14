# Comparing `tmp/investor8-sdk-1.1.80.tar.gz` & `tmp/investor8-sdk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investor8-sdk-1.1.80.tar", last modified: Sun May 14 14:13:58 2023, max compression
+gzip compressed data, was "investor8-sdk-1.1.9.tar", last modified: Tue Apr 12 14:29:22 2022, max compression
```

## Comparing `investor8-sdk-1.1.80.tar` & `investor8-sdk-1.1.9.tar`

### file list

```diff
@@ -1,289 +1,460 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:58.106369 investor8-sdk-1.1.80/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    26839 2023-05-14 14:13:58.106369 investor8-sdk-1.1.80/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    26206 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/README.md
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:57.786351 investor8-sdk-1.1.80/investor8_sdk/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8002 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:57.794352 investor8-sdk-1.1.80/investor8_sdk/api/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21896 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/api/earnings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.80/investor8_sdk/api/email_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37163 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/api/financials_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    95062 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55709 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/news_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21615 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/price_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25818 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/screener_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4737 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/search_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10888 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/settings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60662 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/stock_info_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11021 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    62859 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api/user_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25090 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/api_client.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8523 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/configuration.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:57.870356 investor8-sdk-1.1.80/investor8_sdk/models/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7276 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/models/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3705 2023-05-14 14:13:51.000000 investor8-sdk-1.1.80/investor8_sdk/models/active_company_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2023-05-14 14:13:51.000000 investor8-sdk-1.1.80/investor8_sdk/models/add_to_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6948 2023-05-14 14:13:51.000000 investor8-sdk-1.1.80/investor8_sdk/models/authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2564 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/authorize_account_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/change_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8307 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3776 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_auth_req_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9701 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4679 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_screen_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_update_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_user_res_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4682 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3967 2022-05-17 22:57:20.000000 investor8-sdk-1.1.80/investor8_sdk/models/current_metadat_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15390 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17728 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/current_momentum_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6663 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11983 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/detailed_latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2622 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/discovery_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22123 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/earning_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.80/investor8_sdk/models/email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14737 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/financial_metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6287 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/financial_report_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13652 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/financial_tag.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4336 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/financials_growth.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13096 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/get_list_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16129 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/get_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3856 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/get_screens_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3961 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8020 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5353 2023-05-14 14:13:52.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3996 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_indicator_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4102 2022-05-17 22:57:21.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_metadata_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4699 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_metric_value_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10253 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5663 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6659 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/historical_value_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2551 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5161 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4174 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4210 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4991 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/latest_financial_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4996 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/latest_financials_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4691 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/latest_financials_with_growth_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9535 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3881 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7221 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/log_terminal_usage.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3888 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3963 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/login_with_code_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.80/investor8_sdk/models/market_highlight.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10246 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/market_highlight_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2594 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6192 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.80/investor8_sdk/models/metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5539 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7972 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/metrics_by_period_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14094 2023-03-19 11:02:32.000000 investor8-sdk-1.1.80/investor8_sdk/models/metrics_metadata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6618 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/metrics_metadata_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6294 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/momentum_metric_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4536 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/monthly_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3826 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/monthly_returns.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4191 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/news_categories_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2537 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/news_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3743 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/period_metric_value.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/period_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.80/investor8_sdk/models/plot_detail_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.80/investor8_sdk/models/plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3633 2023-05-14 14:13:53.000000 investor8-sdk-1.1.80/investor8_sdk/models/plot_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3977 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/previous_close_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2541 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/profile_name.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16061 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/recent_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3903 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/remove_from_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/rename_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2525 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/req_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/reset_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4476 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/result_field.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7256 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/return_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20474 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/sa_attributes_prices.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5293 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/sa_sector_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6333 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/screen.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5793 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/screen_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4529 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/screening_condition.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3770 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/sector_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11239 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/standardized_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19718 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12763 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5181 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7661 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15908 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_info_master_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16468 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_ipo.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17068 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19810 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_news_details.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2583 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_news_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10969 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_popularity_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4356 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_popularity_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7177 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_price.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11136 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11193 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_rating_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19887 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/stock_summary_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/string_message_result.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3988 2023-05-14 14:13:54.000000 investor8-sdk-1.1.80/investor8_sdk/models/symbols_current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4111 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/symbols_historical_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8621 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/tag_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5876 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/tag_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7157 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/terminal_log_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4015 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/terminal_log_os_versions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6951 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/trading_calendar_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17515 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/upcoming_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/update_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/user.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19274 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/validate_watchlist_name_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.80/investor8_sdk/models/validate_watchlist_name_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5043 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/value_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.80/investor8_sdk/models/view_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5532 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/watchlist.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4968 2023-05-14 14:13:55.000000 investor8-sdk-1.1.80/investor8_sdk/models/watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13045 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/investor8_sdk/rest.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:57.790351 investor8-sdk-1.1.80/investor8_sdk.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    26839 2023-05-14 14:13:57.000000 investor8-sdk-1.1.80/investor8_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10429 2023-05-14 14:13:57.000000 investor8-sdk-1.1.80/investor8_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2023-05-14 14:13:57.000000 investor8-sdk-1.1.80/investor8_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       64 2023-05-14 14:13:57.000000 investor8-sdk-1.1.80/investor8_sdk.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       19 2023-05-14 14:13:57.000000 investor8-sdk-1.1.80/investor8_sdk.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2023-05-14 14:13:58.106369 investor8-sdk-1.1.80/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1585 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/setup.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:58.102368 investor8-sdk-1.1.80/test/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-05-14 14:13:56.000000 investor8-sdk-1.1.80/test/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.80/test/test_active_company_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.80/test/test_add_to_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.80/test/test_authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.80/test/test_authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.80/test/test_authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.80/test/test_authorize_account_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.80/test/test_change_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.80/test/test_create_auth_req_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.80/test/test_create_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      962 2023-01-09 08:00:15.000000 investor8-sdk-1.1.80/test/test_create_screen_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_create_update_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.80/test/test_create_user_res_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.80/test/test_create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:15.000000 investor8-sdk-1.1.80/test/test_current_metadat_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.80/test/test_current_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_current_momentum_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_detailed_latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-07-24 00:19:52.000000 investor8-sdk-1.1.80/test/test_discovery_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_earning_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_earnings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_email_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.80/test/test_financial_metric_metadata_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_financial_report_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_financial_tag.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_financials_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_financials_growth.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1046 2023-04-06 07:43:55.000000 investor8-sdk-1.1.80/test/test_get_list_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1012 2023-04-06 07:43:55.000000 investor8-sdk-1.1.80/test/test_get_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      998 2023-01-09 08:00:16.000000 investor8-sdk-1.1.80/test/test_get_screens_by_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.80/test/test_get_user_plots_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.80/test/test_get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.80/test/test_historical_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.80/test/test_historical_indicator_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1047 2022-05-11 07:51:16.000000 investor8-sdk-1.1.80/test/test_historical_metadata_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:16.000000 investor8-sdk-1.1.80/test/test_historical_metric_value_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_historical_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_historical_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_historical_value_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.80/test/test_i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.80/test/test_i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.80/test/test_i8_terminal_version_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_latest_financial_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.80/test/test_latest_financials_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_latest_financials_with_growth_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.80/test/test_log_terminal_usage.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.80/test/test_login_with_code_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_market_highlight.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_market_highlight_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.80/test/test_metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.80/test/test_metric_metadata_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      988 2023-05-07 19:23:44.000000 investor8-sdk-1.1.80/test/test_metrics_by_period_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.80/test/test_metrics_metadata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-05-11 07:51:16.000000 investor8-sdk-1.1.80/test/test_metrics_metadata_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_momentum_metric_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_monthly_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_monthly_returns.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_news_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_news_categories_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_news_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_period_metric_value.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_period_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.80/test/test_plot.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.80/test/test_plot_detail_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.80/test/test_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.80/test/test_plot_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_previous_close_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_price_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_profile_name.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_recent_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.80/test/test_remove_from_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.80/test/test_rename_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_req_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_reset_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_result_field.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_return_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_sa_attributes_prices.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_sa_sector_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      886 2023-01-09 08:00:17.000000 investor8-sdk-1.1.80/test/test_screen.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      912 2023-01-09 08:00:17.000000 investor8-sdk-1.1.80/test/test_screen_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.80/test/test_screener_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1002 2022-10-17 20:31:24.000000 investor8-sdk-1.1.80/test/test_screening_condition.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.80/test/test_search_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_sector_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.80/test/test_settings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_standardized_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.80/test/test_stock_info_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_info_master_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.80/test/test_stock_ipo.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_news_details.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_news_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_popularity_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_popularity_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_price.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.80/test/test_stock_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_rating_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_stock_summary_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_string_message_result.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-28 11:55:23.000000 investor8-sdk-1.1.80/test/test_symbols_current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2022-05-28 11:55:23.000000 investor8-sdk-1.1.80/test/test_symbols_historical_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_tag_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_tag_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.80/test/test_tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      933 2022-04-23 22:58:49.000000 investor8-sdk-1.1.80/test/test_terminal_log_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1017 2022-04-26 22:55:39.000000 investor8-sdk-1.1.80/test/test_terminal_log_os_versions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.80/test/test_trading_calendar_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_upcoming_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.80/test/test_update_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.80/test/test_update_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_user.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.80/test/test_user_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.80/test/test_validate_watchlist_name_request_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.80/test/test_validate_watchlist_name_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.80/test/test_value_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.80/test/test_view_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.80/test/test_watchlist.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.80/test/test_watchlist_dto.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    24117 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/README.md
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:21.976057 investor8-sdk-1.1.9/investor8-sdk/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6683 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.008058 investor8-sdk-1.1.9/investor8-sdk/api/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      657 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22037 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    36089 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53494 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/metrics_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76825 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17866 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22457 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4743 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54811 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11081 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/tags_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100956 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api_client.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8232 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.160067 investor8-sdk-1.1.9/investor8-sdk/models/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5963 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-17 08:35:43.000000 investor8-sdk-1.1.9/investor8-sdk/models/authentication_request.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/company_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/email_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8957 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-13 23:15:07.000000 investor8-sdk-1.1.9/investor8-sdk/models/get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/get_watchlists_by_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/history_length.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/list_exchange_sector_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/login_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10369 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_detail_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9401 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/send_email_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11161 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.164068 investor8-sdk-1.1.9/investor8_sdk/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6915 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.172068 investor8-sdk-1.1.9/investor8_sdk/api/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21875 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/earnings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.9/investor8_sdk/api/email_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37142 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/financials_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    84567 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55688 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/news_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21594 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/price_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22295 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/screener_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4716 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/search_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10867 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/settings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60641 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/stock_info_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11000 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    41760 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/user_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api_client.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8501 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.236072 investor8-sdk-1.1.9/investor8_sdk/models/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6189 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/models/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3684 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/active_company_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3861 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/add_to_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6927 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2543 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/change_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3755 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_auth_req_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9680 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_update_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_user_res_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4661 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4359 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/current_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17707 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/current_momentum_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/detailed_latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/earning_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12479 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_report_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12079 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_tag.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financials_growth.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7999 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3975 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_indicator_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_value_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5140 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4153 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4189 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financial_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_with_growth_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7200 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/log_terminal_usage.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3867 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3942 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/login_with_code_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10225 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6171 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8808 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/metrics_metadata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/momentum_metric_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/monthly_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/monthly_returns.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/news_categories_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/news_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/period_metric_value.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/period_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_detail_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/previous_close_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/profile_name.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/recent_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/remove_from_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/rename_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2504 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/req_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/reset_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/result_field.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/return_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sa_attributes_prices.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sa_sector_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sector_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/standardized_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_info_master_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_ipo.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news_details.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_price.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_rating_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_summary_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/string_message_result.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/tag_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/tag_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6930 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/trading_calendar_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/upcoming_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/update_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/user.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17586 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/value_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.9/investor8_sdk/models/view_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/watchlist.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.164068 investor8-sdk-1.1.9/investor8_sdk.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17185 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/setup.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.240072 investor8-sdk-1.1.9/swagger_client/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6783 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.268074 investor8-sdk-1.1.9/swagger_client/api/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      668 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    21759 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7123 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    35928 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53243 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/metrics_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76448 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17777 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22350 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4726 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54542 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11028 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/tags_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100424 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25072 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api_client.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8233 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.412082 investor8-sdk-1.1.9/swagger_client/models/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6050 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/models/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/authentication_request.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/company_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/email_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7482 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/get_watchlists_by_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/history_length.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/list_exchange_sector_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/login_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10057 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/send_email_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10584 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.576092 investor8-sdk-1.1.9/test/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/test/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.9/test/test_active_company_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.9/test/test_add_to_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.9/test/test_authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.9/test/test_authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.9/test/test_authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.9/test/test_authorize_account_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.9/test/test_change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.9/test/test_create_auth_req_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.9/test/test_create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.9/test/test_create_user_res_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.9/test/test_create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.9/test/test_current_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.9/test/test_financial_metric_metadata_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.9/test/test_get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.9/test/test_get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.9/test/test_historical_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.9/test/test_historical_indicator_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.9/test/test_i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.9/test/test_i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.9/test/test_i8_terminal_version_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.9/test/test_log_terminal_usage.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.9/test/test_login_with_code_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.9/test/test_metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.9/test/test_metric_metadata_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.9/test/test_metrics_metadata.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.9/test/test_plot.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.9/test/test_plot_detail_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.9/test/test_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.9/test/test_plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.9/test/test_remove_from_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.9/test/test_rename_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.9/test/test_settings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.9/test/test_stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.9/test/test_trading_calendar_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.9/test/test_update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.9/test/test_validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.9/test/test_validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.9/test/test_view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_watchlist_dto.py
```

### Comparing `investor8-sdk-1.1.80/PKG-INFO` & `investor8-sdk-1.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-Metadata-Version: 2.1
-Name: investor8-sdk
-Version: 1.1.80
-Summary: Investoreight Core API
-Home-page: UNKNOWN
-Author-email: info@investoreight.com
-License: UNKNOWN
-Project-URL: Homepage, https://www.investoreight.com/
-Project-URL: Documentation, https://github.com/investoreight/investor8-sdk#readme
-Project-URL: Download, https://github.com/investoreight/investor8-sdk/releases
-Project-URL: Source Code, https://github.com/investoreight/investor8-sdk
-Project-URL: Bug Tracker, https://github.com/investoreight/investor8-sdk/issues
-Keywords: Swagger,Investoreight Core API
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # investor8-sdk
-Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html
+No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
-- Package version: 1.1.80
+- Package version: 1.1.9
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
-For more information, please visit [https://www.investoreight.com](https://www.investoreight.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install git+https://github.com/investoreight/investor8-sdk.git
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/investoreight/investor8-sdk.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
 import investor8_sdk 
 ```
 
 ### Setuptools
@@ -225,27 +208,24 @@
 *MetricsApi* | [**get_aggregated_earning_returns_by_ticker**](docs/MetricsApi.md#get_aggregated_earning_returns_by_ticker) | **GET** /Metrics/earning/ticker/{ticker} | 
 *MetricsApi* | [**get_all_latest_daily_metrics**](docs/MetricsApi.md#get_all_latest_daily_metrics) | **GET** /Metrics/daily/all/latest | 
 *MetricsApi* | [**get_all_latest_financial_metrics**](docs/MetricsApi.md#get_all_latest_financial_metrics) | **GET** /Metrics/financial/all/latest | 
 *MetricsApi* | [**get_all_latest_value_metrics**](docs/MetricsApi.md#get_all_latest_value_metrics) | **GET** /Metrics/value/all/latest | 
 *MetricsApi* | [**get_current_metrics**](docs/MetricsApi.md#get_current_metrics) | **GET** /Metrics/current | 
 *MetricsApi* | [**get_current_momentum**](docs/MetricsApi.md#get_current_momentum) | **GET** /Metrics/momentum/current/{ticker} | 
 *MetricsApi* | [**get_distinct_metric_metadata_properties**](docs/MetricsApi.md#get_distinct_metric_metadata_properties) | **GET** /Metrics/metadata/properties/distinct | 
-*MetricsApi* | [**get_distinct_metric_metadata_screening_conditions**](docs/MetricsApi.md#get_distinct_metric_metadata_screening_conditions) | **GET** /Metrics/metadata/screeningconditions/distinct | 
 *MetricsApi* | [**get_historical_daily_metrics**](docs/MetricsApi.md#get_historical_daily_metrics) | **GET** /Metrics/historical/daily/{ticker} | 
 *MetricsApi* | [**get_historical_growth_metrics**](docs/MetricsApi.md#get_historical_growth_metrics) | **GET** /Metrics/growth/historical/{ticker} | 
 *MetricsApi* | [**get_historical_indicators**](docs/MetricsApi.md#get_historical_indicators) | **GET** /Metrics/historical/indicators/{ticker} | 
 *MetricsApi* | [**get_historical_metrics**](docs/MetricsApi.md#get_historical_metrics) | **GET** /Metrics/historical | 
 *MetricsApi* | [**get_historical_momentum**](docs/MetricsApi.md#get_historical_momentum) | **GET** /Metrics/momentum/historical/{ticker} | 
 *MetricsApi* | [**get_historical_value**](docs/MetricsApi.md#get_historical_value) | **GET** /Metrics/historical/value/{ticker} | 
-*MetricsApi* | [**get_latest_financials_period**](docs/MetricsApi.md#get_latest_financials_period) | **GET** /Metrics/financials/latest/period | 
 *MetricsApi* | [**get_latest_growth_metrics**](docs/MetricsApi.md#get_latest_growth_metrics) | **GET** /Metrics/growth/latest/{ticker} | 
 *MetricsApi* | [**get_list_financial_metrics_metadata**](docs/MetricsApi.md#get_list_financial_metrics_metadata) | **GET** /Metrics/metadata/list/financials | 
 *MetricsApi* | [**get_list_metrics_metadata**](docs/MetricsApi.md#get_list_metrics_metadata) | **GET** /Metrics/metadata/list | 
 *MetricsApi* | [**get_market_index_returns**](docs/MetricsApi.md#get_market_index_returns) | **GET** /Metrics/merket/returns/{ticker} | 
-*MetricsApi* | [**get_metrics_by_period**](docs/MetricsApi.md#get_metrics_by_period) | **GET** /Metrics/byperiod | 
 *MetricsApi* | [**get_metrics_metadata**](docs/MetricsApi.md#get_metrics_metadata) | **GET** /Metrics/metadata/{name} | 
 *MetricsApi* | [**get_monthly_returns**](docs/MetricsApi.md#get_monthly_returns) | **GET** /Metrics/returns/monthly/{ticker}/{sinceYear} | 
 *MetricsApi* | [**get_raw_historical_returns**](docs/MetricsApi.md#get_raw_historical_returns) | **GET** /Metrics/earning/raw/historical/{ticker} | 
 *MetricsApi* | [**get_sector_returns**](docs/MetricsApi.md#get_sector_returns) | **GET** /Metrics/sector/returns | 
 *NewsApi* | [**get**](docs/NewsApi.md#get) | **GET** /News/{id} | 
 *NewsApi* | [**get_aggregated_ticker_news**](docs/NewsApi.md#get_aggregated_ticker_news) | **GET** /News/aggregated/{ticker} | 
 *NewsApi* | [**get_all_sectors_news**](docs/NewsApi.md#get_all_sectors_news) | **GET** /News/sector/all/{size} | 
@@ -269,15 +249,14 @@
 *PriceApi* | [**get_today_intraday_prices**](docs/PriceApi.md#get_today_intraday_prices) | **GET** /Price/intraday/today | 
 *ScreenerApi* | [**get_all_sectors_returns**](docs/ScreenerApi.md#get_all_sectors_returns) | **GET** /Screener/sectors/all_returns | 
 *ScreenerApi* | [**get_all_sectors_returns_today_sa**](docs/ScreenerApi.md#get_all_sectors_returns_today_sa) | **GET** /Screener/sa/sector/returns/today | 
 *ScreenerApi* | [**get_dow_tickers**](docs/ScreenerApi.md#get_dow_tickers) | **GET** /Screener/dow/tickers | 
 *ScreenerApi* | [**get_list_ip_os**](docs/ScreenerApi.md#get_list_ip_os) | **GET** /Screener/ipo/list | 
 *ScreenerApi* | [**get_top_stocks**](docs/ScreenerApi.md#get_top_stocks) | **GET** /Screener/top/{category} | 
 *ScreenerApi* | [**get_upcoming_ipos**](docs/ScreenerApi.md#get_upcoming_ipos) | **GET** /Screener/ipo/upcoming | 
-*ScreenerApi* | [**search**](docs/ScreenerApi.md#search) | **GET** /Screener/search | 
 *SearchApi* | [**search_stocks**](docs/SearchApi.md#search_stocks) | **GET** /Search/{query}/{size} | 
 *SettingsApi* | [**check_i8t_version**](docs/SettingsApi.md#check_i8t_version) | **GET** /Settings/i8terminal/version/check/{version} | 
 *SettingsApi* | [**get_i8t_version**](docs/SettingsApi.md#get_i8t_version) | **GET** /Settings/i8terminal/version | 
 *SettingsApi* | [**set_i8t_version**](docs/SettingsApi.md#set_i8t_version) | **PUT** /Settings/i8terminal/version | 
 *StockInfoApi* | [**get_all_active_companies**](docs/StockInfoApi.md#get_all_active_companies) | **GET** /StockInfo/companies/active | 
 *StockInfoApi* | [**get_all_stock_info**](docs/StockInfoApi.md#get_all_stock_info) | **GET** /StockInfo/all/{marketIndex} | 
 *StockInfoApi* | [**get_all_stocks_popularity**](docs/StockInfoApi.md#get_all_stocks_popularity) | **GET** /StockInfo/popularity/all | 
@@ -297,22 +276,16 @@
 *StockInfoApi* | [**healthy_check**](docs/StockInfoApi.md#healthy_check) | **GET** /health | 
 *TagsApi* | [**get_all_tags_info**](docs/TagsApi.md#get_all_tags_info) | **GET** /Tags/all/info | 
 *TagsApi* | [**get_all_ticker_tags**](docs/TagsApi.md#get_all_ticker_tags) | **GET** /Tags/all/ticker | 
 *TagsApi* | [**get_tag_details**](docs/TagsApi.md#get_tag_details) | **GET** /Tags/{tagId} | 
 *UserApi* | [**add_to_watchlist**](docs/UserApi.md#add_to_watchlist) | **POST** /User/watchlist/add | 
 *UserApi* | [**create_login_authentication_request**](docs/UserApi.md#create_login_authentication_request) | **POST** /User/authentication/request/login | 
 *UserApi* | [**create_plot**](docs/UserApi.md#create_plot) | **POST** /User/plot | 
-*UserApi* | [**create_screen**](docs/UserApi.md#create_screen) | **POST** /User/screen | 
 *UserApi* | [**create_watchlist**](docs/UserApi.md#create_watchlist) | **POST** /User/watchlist | 
-*UserApi* | [**get_aggregated_terminal_os_and_versions**](docs/UserApi.md#get_aggregated_terminal_os_and_versions) | **GET** /User/terminal/os/versions | 
 *UserApi* | [**get_roles**](docs/UserApi.md#get_roles) | **GET** /User/roles | 
-*UserApi* | [**get_screen**](docs/UserApi.md#get_screen) | **GET** /User/screen/{id} | 
-*UserApi* | [**get_screens_by_user**](docs/UserApi.md#get_screens_by_user) | **GET** /User/screen/byuser/{userId} | 
-*UserApi* | [**get_terminal_log**](docs/UserApi.md#get_terminal_log) | **GET** /User/terminal/log/{id} | 
-*UserApi* | [**get_terminal_logs**](docs/UserApi.md#get_terminal_logs) | **GET** /User/terminal/list/log | 
 *UserApi* | [**get_watchlist**](docs/UserApi.md#get_watchlist) | **GET** /User/watchlist/{id} | 
 *UserApi* | [**get_watchlist_by_name_user_id**](docs/UserApi.md#get_watchlist_by_name_user_id) | **GET** /User/watchlist/byname | 
 *UserApi* | [**get_watchlists_by_user**](docs/UserApi.md#get_watchlists_by_user) | **GET** /User/watchlist/byuser/{userId} | 
 *UserApi* | [**log_terminal_usage**](docs/UserApi.md#log_terminal_usage) | **POST** /User/terminal/log | 
 *UserApi* | [**login_user**](docs/UserApi.md#login_user) | **POST** /User/login | 
 *UserApi* | [**login_with_code**](docs/UserApi.md#login_with_code) | **POST** /User/login/code | 
 *UserApi* | [**remove_from_watchlist**](docs/UserApi.md#remove_from_watchlist) | **POST** /User/watchlist/remove | 
@@ -322,34 +295,28 @@
  - [ActiveCompanyDto](docs/ActiveCompanyDto.md)
  - [AddToWatchlistDto](docs/AddToWatchlistDto.md)
  - [AuthenticationRequest](docs/AuthenticationRequest.md)
  - [AuthenticationSource](docs/AuthenticationSource.md)
  - [CompanyInfoDto](docs/CompanyInfoDto.md)
  - [CreateAuthReqDto](docs/CreateAuthReqDto.md)
  - [CreatePlotDto](docs/CreatePlotDto.md)
- - [CreateScreenDto](docs/CreateScreenDto.md)
  - [CreateWatchlistDto](docs/CreateWatchlistDto.md)
  - [CurrentMetricsDto](docs/CurrentMetricsDto.md)
  - [CurrentMomentumMetricsDto](docs/CurrentMomentumMetricsDto.md)
  - [DailyMetricsDto](docs/DailyMetricsDto.md)
  - [DetailedLatestPriceDto](docs/DetailedLatestPriceDto.md)
- - [DiscoverySource](docs/DiscoverySource.md)
  - [EarningMetricsDto](docs/EarningMetricsDto.md)
  - [FinancialMetricMetadataDto](docs/FinancialMetricMetadataDto.md)
  - [FinancialReportDto](docs/FinancialReportDto.md)
  - [FinancialTag](docs/FinancialTag.md)
  - [FinancialsGrowth](docs/FinancialsGrowth.md)
- - [GetListMetricsMetadataDto](docs/GetListMetricsMetadataDto.md)
- - [GetMetricsMetadataDto](docs/GetMetricsMetadataDto.md)
- - [GetScreensByUserDto](docs/GetScreensByUserDto.md)
  - [GetWatchlistsByUserDto](docs/GetWatchlistsByUserDto.md)
  - [HistoricalDailyMetricsDto](docs/HistoricalDailyMetricsDto.md)
  - [HistoricalFinancialMetrics](docs/HistoricalFinancialMetrics.md)
  - [HistoricalIndicatorDto](docs/HistoricalIndicatorDto.md)
- - [HistoricalMetricValueDto](docs/HistoricalMetricValueDto.md)
  - [HistoricalReturn](docs/HistoricalReturn.md)
  - [HistoricalReturnsDto](docs/HistoricalReturnsDto.md)
  - [HistoricalValueMetrics](docs/HistoricalValueMetrics.md)
  - [HistoryLength](docs/HistoryLength.md)
  - [I8TerminalCheckVersionDto](docs/I8TerminalCheckVersionDto.md)
  - [I8TerminalVersion](docs/I8TerminalVersion.md)
  - [I8TerminalVersionDto](docs/I8TerminalVersionDto.md)
@@ -361,16 +328,15 @@
  - [LogTerminalUsage](docs/LogTerminalUsage.md)
  - [LoginUserDto](docs/LoginUserDto.md)
  - [LoginWithCodeDto](docs/LoginWithCodeDto.md)
  - [MarketHighlightDto](docs/MarketHighlightDto.md)
  - [MarketHighlightStatus](docs/MarketHighlightStatus.md)
  - [MetadataPropertiesDto](docs/MetadataPropertiesDto.md)
  - [Metrics](docs/Metrics.md)
- - [MetricsByPeriodDto](docs/MetricsByPeriodDto.md)
- - [MetricsMetadataResponseDto](docs/MetricsMetadataResponseDto.md)
+ - [MetricsMetadata](docs/MetricsMetadata.md)
  - [MomentumMetricDto](docs/MomentumMetricDto.md)
  - [MonthlyMetrics](docs/MonthlyMetrics.md)
  - [MonthlyReturns](docs/MonthlyReturns.md)
  - [NewsCategoriesDto](docs/NewsCategoriesDto.md)
  - [NewsSource](docs/NewsSource.md)
  - [PeriodMetricValue](docs/PeriodMetricValue.md)
  - [PeriodReturn](docs/PeriodReturn.md)
@@ -380,17 +346,14 @@
  - [RecentEarningDto](docs/RecentEarningDto.md)
  - [RemoveFromWatchlistDto](docs/RemoveFromWatchlistDto.md)
  - [ReqType](docs/ReqType.md)
  - [ResultField](docs/ResultField.md)
  - [ReturnMetrics](docs/ReturnMetrics.md)
  - [SAAttributesPrices](docs/SAAttributesPrices.md)
  - [SASectorPriceDto](docs/SASectorPriceDto.md)
- - [Screen](docs/Screen.md)
- - [ScreenDto](docs/ScreenDto.md)
- - [ScreeningCondition](docs/ScreeningCondition.md)
  - [SectorReturnsDto](docs/SectorReturnsDto.md)
  - [StandardizedFinancial](docs/StandardizedFinancial.md)
  - [StockEarningDto](docs/StockEarningDto.md)
  - [StockFinancial](docs/StockFinancial.md)
  - [StockFinancialMetrics](docs/StockFinancialMetrics.md)
  - [StockInfoDto](docs/StockInfoDto.md)
  - [StockInfoMasterDto](docs/StockInfoMasterDto.md)
@@ -400,20 +363,16 @@
  - [StockNewsStatus](docs/StockNewsStatus.md)
  - [StockPopularityDetailsDto](docs/StockPopularityDetailsDto.md)
  - [StockPopularityDto](docs/StockPopularityDto.md)
  - [StockPrice](docs/StockPrice.md)
  - [StockPriceDto](docs/StockPriceDto.md)
  - [StockRatingDto](docs/StockRatingDto.md)
  - [StockSummaryDto](docs/StockSummaryDto.md)
- - [SymbolsCurrentMetricsDto](docs/SymbolsCurrentMetricsDto.md)
- - [SymbolsHistoricalMetricsDto](docs/SymbolsHistoricalMetricsDto.md)
  - [TagDetailsDto](docs/TagDetailsDto.md)
  - [TagInfoDto](docs/TagInfoDto.md)
- - [TerminalLogDto](docs/TerminalLogDto.md)
- - [TerminalLogOSVersionsDto](docs/TerminalLogOSVersionsDto.md)
  - [TradingCalendarDetailsDto](docs/TradingCalendarDetailsDto.md)
  - [UpcomingEarningDto](docs/UpcomingEarningDto.md)
  - [UserDto](docs/UserDto.md)
  - [ValueMetricsDto](docs/ValueMetricsDto.md)
  - [Watchlist](docs/Watchlist.md)
  - [WatchlistDto](docs/WatchlistDto.md)
 
@@ -431,10 +390,8 @@
 - **Type**: API key
 - **API key parameter name**: Authorization
 - **Location**: HTTP header
 
 
 ## Author
 
-info@investoreight.com
-
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from investor8_sdk.api.earnings_api import EarningsApi
@@ -33,34 +33,28 @@
 from investor8_sdk.models.active_company_dto import ActiveCompanyDto
 from investor8_sdk.models.add_to_watchlist_dto import AddToWatchlistDto
 from investor8_sdk.models.authentication_request import AuthenticationRequest
 from investor8_sdk.models.authentication_source import AuthenticationSource
 from investor8_sdk.models.company_info_dto import CompanyInfoDto
 from investor8_sdk.models.create_auth_req_dto import CreateAuthReqDto
 from investor8_sdk.models.create_plot_dto import CreatePlotDto
-from investor8_sdk.models.create_screen_dto import CreateScreenDto
 from investor8_sdk.models.create_watchlist_dto import CreateWatchlistDto
 from investor8_sdk.models.current_metrics_dto import CurrentMetricsDto
 from investor8_sdk.models.current_momentum_metrics_dto import CurrentMomentumMetricsDto
 from investor8_sdk.models.daily_metrics_dto import DailyMetricsDto
 from investor8_sdk.models.detailed_latest_price_dto import DetailedLatestPriceDto
-from investor8_sdk.models.discovery_source import DiscoverySource
 from investor8_sdk.models.earning_metrics_dto import EarningMetricsDto
 from investor8_sdk.models.financial_metric_metadata_dto import FinancialMetricMetadataDto
 from investor8_sdk.models.financial_report_dto import FinancialReportDto
 from investor8_sdk.models.financial_tag import FinancialTag
 from investor8_sdk.models.financials_growth import FinancialsGrowth
-from investor8_sdk.models.get_list_metrics_metadata_dto import GetListMetricsMetadataDto
-from investor8_sdk.models.get_metrics_metadata_dto import GetMetricsMetadataDto
-from investor8_sdk.models.get_screens_by_user_dto import GetScreensByUserDto
 from investor8_sdk.models.get_watchlists_by_user_dto import GetWatchlistsByUserDto
 from investor8_sdk.models.historical_daily_metrics_dto import HistoricalDailyMetricsDto
 from investor8_sdk.models.historical_financial_metrics import HistoricalFinancialMetrics
 from investor8_sdk.models.historical_indicator_dto import HistoricalIndicatorDto
-from investor8_sdk.models.historical_metric_value_dto import HistoricalMetricValueDto
 from investor8_sdk.models.historical_return import HistoricalReturn
 from investor8_sdk.models.historical_returns_dto import HistoricalReturnsDto
 from investor8_sdk.models.historical_value_metrics import HistoricalValueMetrics
 from investor8_sdk.models.history_length import HistoryLength
 from investor8_sdk.models.i8_terminal_check_version_dto import I8TerminalCheckVersionDto
 from investor8_sdk.models.i8_terminal_version import I8TerminalVersion
 from investor8_sdk.models.i8_terminal_version_dto import I8TerminalVersionDto
@@ -72,16 +66,15 @@
 from investor8_sdk.models.log_terminal_usage import LogTerminalUsage
 from investor8_sdk.models.login_user_dto import LoginUserDto
 from investor8_sdk.models.login_with_code_dto import LoginWithCodeDto
 from investor8_sdk.models.market_highlight_dto import MarketHighlightDto
 from investor8_sdk.models.market_highlight_status import MarketHighlightStatus
 from investor8_sdk.models.metadata_properties_dto import MetadataPropertiesDto
 from investor8_sdk.models.metrics import Metrics
-from investor8_sdk.models.metrics_by_period_dto import MetricsByPeriodDto
-from investor8_sdk.models.metrics_metadata_response_dto import MetricsMetadataResponseDto
+from investor8_sdk.models.metrics_metadata import MetricsMetadata
 from investor8_sdk.models.momentum_metric_dto import MomentumMetricDto
 from investor8_sdk.models.monthly_metrics import MonthlyMetrics
 from investor8_sdk.models.monthly_returns import MonthlyReturns
 from investor8_sdk.models.news_categories_dto import NewsCategoriesDto
 from investor8_sdk.models.news_source import NewsSource
 from investor8_sdk.models.period_metric_value import PeriodMetricValue
 from investor8_sdk.models.period_return import PeriodReturn
@@ -91,17 +84,14 @@
 from investor8_sdk.models.recent_earning_dto import RecentEarningDto
 from investor8_sdk.models.remove_from_watchlist_dto import RemoveFromWatchlistDto
 from investor8_sdk.models.req_type import ReqType
 from investor8_sdk.models.result_field import ResultField
 from investor8_sdk.models.return_metrics import ReturnMetrics
 from investor8_sdk.models.sa_attributes_prices import SAAttributesPrices
 from investor8_sdk.models.sa_sector_price_dto import SASectorPriceDto
-from investor8_sdk.models.screen import Screen
-from investor8_sdk.models.screen_dto import ScreenDto
-from investor8_sdk.models.screening_condition import ScreeningCondition
 from investor8_sdk.models.sector_returns_dto import SectorReturnsDto
 from investor8_sdk.models.standardized_financial import StandardizedFinancial
 from investor8_sdk.models.stock_earning_dto import StockEarningDto
 from investor8_sdk.models.stock_financial import StockFinancial
 from investor8_sdk.models.stock_financial_metrics import StockFinancialMetrics
 from investor8_sdk.models.stock_info_dto import StockInfoDto
 from investor8_sdk.models.stock_info_master_dto import StockInfoMasterDto
@@ -111,19 +101,15 @@
 from investor8_sdk.models.stock_news_status import StockNewsStatus
 from investor8_sdk.models.stock_popularity_details_dto import StockPopularityDetailsDto
 from investor8_sdk.models.stock_popularity_dto import StockPopularityDto
 from investor8_sdk.models.stock_price import StockPrice
 from investor8_sdk.models.stock_price_dto import StockPriceDto
 from investor8_sdk.models.stock_rating_dto import StockRatingDto
 from investor8_sdk.models.stock_summary_dto import StockSummaryDto
-from investor8_sdk.models.symbols_current_metrics_dto import SymbolsCurrentMetricsDto
-from investor8_sdk.models.symbols_historical_metrics_dto import SymbolsHistoricalMetricsDto
 from investor8_sdk.models.tag_details_dto import TagDetailsDto
 from investor8_sdk.models.tag_info_dto import TagInfoDto
-from investor8_sdk.models.terminal_log_dto import TerminalLogDto
-from investor8_sdk.models.terminal_log_os_versions_dto import TerminalLogOSVersionsDto
 from investor8_sdk.models.trading_calendar_details_dto import TradingCalendarDetailsDto
 from investor8_sdk.models.upcoming_earning_dto import UpcomingEarningDto
 from investor8_sdk.models.user_dto import UserDto
 from investor8_sdk.models.value_metrics_dto import ValueMetricsDto
 from investor8_sdk.models.watchlist import Watchlist
 from investor8_sdk.models.watchlist_dto import WatchlistDto
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/earnings_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/earnings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/email_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/financials_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/financials_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/metrics_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/metrics_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
@@ -498,17 +498,19 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_current_metrics(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str symbols:
+        :param str tickers:
         :param str metrics:
-        :return: SymbolsCurrentMetricsDto
+        :param str period_type:
+        :param bool refresh_cache:
+        :return: list[CurrentMetricsDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_current_metrics_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -520,22 +522,24 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_current_metrics_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str symbols:
+        :param str tickers:
         :param str metrics:
-        :return: SymbolsCurrentMetricsDto
+        :param str period_type:
+        :param bool refresh_cache:
+        :return: list[CurrentMetricsDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['symbols', 'metrics']  # noqa: E501
+        all_params = ['tickers', 'metrics', 'period_type', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -548,18 +552,22 @@
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'symbols' in params:
-            query_params.append(('symbols', params['symbols']))  # noqa: E501
+        if 'tickers' in params:
+            query_params.append(('tickers', params['tickers']))  # noqa: E501
         if 'metrics' in params:
             query_params.append(('metrics', params['metrics']))  # noqa: E501
+        if 'period_type' in params:
+            query_params.append(('periodType', params['period_type']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -574,15 +582,15 @@
             '/Metrics/current', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='SymbolsCurrentMetricsDto',  # noqa: E501
+            response_type='list[CurrentMetricsDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -764,99 +772,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_distinct_metric_metadata_screening_conditions(self, **kwargs):  # noqa: E501
-        """get_distinct_metric_metadata_screening_conditions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_distinct_metric_metadata_screening_conditions(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :return: list[ScreeningCondition]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_distinct_metric_metadata_screening_conditions_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_distinct_metric_metadata_screening_conditions_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def get_distinct_metric_metadata_screening_conditions_with_http_info(self, **kwargs):  # noqa: E501
-        """get_distinct_metric_metadata_screening_conditions  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_distinct_metric_metadata_screening_conditions_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :return: list[ScreeningCondition]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = []  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_distinct_metric_metadata_screening_conditions" % key
-                )
-            params[key] = val
-        del params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/Metrics/metadata/screeningconditions/distinct', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[ScreeningCondition]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def get_historical_daily_metrics(self, ticker, **kwargs):  # noqa: E501
         """get_historical_daily_metrics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_historical_daily_metrics(ticker, async_req=True)
         >>> result = thread.get()
@@ -1169,21 +1092,21 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_historical_metrics(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str symbols:
+        :param str tickers:
         :param str metrics:
-        :param int from_period_offset:
-        :param int to_period_offset:
         :param datetime from_date:
         :param datetime to_date:
-        :return: SymbolsHistoricalMetricsDto
+        :param str period_type:
+        :param bool refresh_cache:
+        :return: dict(str, dict(str, dict(str, float)))
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_historical_metrics_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -1195,26 +1118,26 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_historical_metrics_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str symbols:
+        :param str tickers:
         :param str metrics:
-        :param int from_period_offset:
-        :param int to_period_offset:
         :param datetime from_date:
         :param datetime to_date:
-        :return: SymbolsHistoricalMetricsDto
+        :param str period_type:
+        :param bool refresh_cache:
+        :return: dict(str, dict(str, dict(str, float)))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['symbols', 'metrics', 'from_period_offset', 'to_period_offset', 'from_date', 'to_date']  # noqa: E501
+        all_params = ['tickers', 'metrics', 'from_date', 'to_date', 'period_type', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1227,26 +1150,26 @@
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'symbols' in params:
-            query_params.append(('symbols', params['symbols']))  # noqa: E501
+        if 'tickers' in params:
+            query_params.append(('tickers', params['tickers']))  # noqa: E501
         if 'metrics' in params:
             query_params.append(('metrics', params['metrics']))  # noqa: E501
-        if 'from_period_offset' in params:
-            query_params.append(('fromPeriodOffset', params['from_period_offset']))  # noqa: E501
-        if 'to_period_offset' in params:
-            query_params.append(('toPeriodOffset', params['to_period_offset']))  # noqa: E501
         if 'from_date' in params:
             query_params.append(('fromDate', params['from_date']))  # noqa: E501
         if 'to_date' in params:
             query_params.append(('toDate', params['to_date']))  # noqa: E501
+        if 'period_type' in params:
+            query_params.append(('periodType', params['period_type']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1261,15 +1184,15 @@
             '/Metrics/historical', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='SymbolsHistoricalMetricsDto',  # noqa: E501
+            response_type='dict(str, dict(str, dict(str, float)))',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -1467,107 +1390,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_latest_financials_period(self, **kwargs):  # noqa: E501
-        """get_latest_financials_period  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_latest_financials_period(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str period_type:
-        :param bool refresh_cache:
-        :return: dict(str, str)
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_latest_financials_period_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_latest_financials_period_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def get_latest_financials_period_with_http_info(self, **kwargs):  # noqa: E501
-        """get_latest_financials_period  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_latest_financials_period_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str period_type:
-        :param bool refresh_cache:
-        :return: dict(str, str)
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['period_type', 'refresh_cache']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_latest_financials_period" % key
-                )
-            params[key] = val
-        del params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'period_type' in params:
-            query_params.append(('periodType', params['period_type']))  # noqa: E501
-        if 'refresh_cache' in params:
-            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/Metrics/financials/latest/period', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='dict(str, str)',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def get_latest_growth_metrics(self, ticker, **kwargs):  # noqa: E501
         """get_latest_growth_metrics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_latest_growth_metrics(ticker, async_req=True)
         >>> result = thread.get()
@@ -1756,20 +1586,17 @@
 
         :param async_req bool
         :param str category:
         :param str type:
         :param str display_format:
         :param str data_format:
         :param str name:
-        :param str soft_delete:
         :param int page_index:
         :param int page_size:
-        :param str sort_by:
-        :param str sort_direction:
-        :return: list[GetListMetricsMetadataDto]
+        :return: list[MetricsMetadata]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_list_metrics_metadata_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -1786,25 +1613,22 @@
 
         :param async_req bool
         :param str category:
         :param str type:
         :param str display_format:
         :param str data_format:
         :param str name:
-        :param str soft_delete:
         :param int page_index:
         :param int page_size:
-        :param str sort_by:
-        :param str sort_direction:
-        :return: list[GetListMetricsMetadataDto]
+        :return: list[MetricsMetadata]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['category', 'type', 'display_format', 'data_format', 'name', 'soft_delete', 'page_index', 'page_size', 'sort_by', 'sort_direction']  # noqa: E501
+        all_params = ['category', 'type', 'display_format', 'data_format', 'name', 'page_index', 'page_size']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1827,24 +1651,18 @@
             query_params.append(('type', params['type']))  # noqa: E501
         if 'display_format' in params:
             query_params.append(('displayFormat', params['display_format']))  # noqa: E501
         if 'data_format' in params:
             query_params.append(('dataFormat', params['data_format']))  # noqa: E501
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
-        if 'soft_delete' in params:
-            query_params.append(('softDelete', params['soft_delete']))  # noqa: E501
         if 'page_index' in params:
             query_params.append(('pageIndex', params['page_index']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
-        if 'sort_by' in params:
-            query_params.append(('sortBy', params['sort_by']))  # noqa: E501
-        if 'sort_direction' in params:
-            query_params.append(('sortDirection', params['sort_direction']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1859,15 +1677,15 @@
             '/Metrics/metadata/list', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[GetListMetricsMetadataDto]',  # noqa: E501
+            response_type='list[MetricsMetadata]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -1964,114 +1782,25 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_metrics_by_period(self, **kwargs):  # noqa: E501
-        """get_metrics_by_period  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_metrics_by_period(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str identifiers:
-        :return: list[MetricsByPeriodDto]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_metrics_by_period_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_metrics_by_period_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def get_metrics_by_period_with_http_info(self, **kwargs):  # noqa: E501
-        """get_metrics_by_period  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_metrics_by_period_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str identifiers:
-        :return: list[MetricsByPeriodDto]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['identifiers']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_metrics_by_period" % key
-                )
-            params[key] = val
-        del params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'identifiers' in params:
-            query_params.append(('identifiers', params['identifiers']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/Metrics/byperiod', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[MetricsByPeriodDto]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def get_metrics_metadata(self, name, **kwargs):  # noqa: E501
         """get_metrics_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_metrics_metadata(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: (required)
-        :return: GetMetricsMetadataDto
+        :return: MetricsMetadata
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_metrics_metadata_with_http_info(name, **kwargs)  # noqa: E501
         else:
@@ -2084,15 +1813,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_metrics_metadata_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: (required)
-        :return: GetMetricsMetadataDto
+        :return: MetricsMetadata
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -2138,15 +1867,15 @@
             '/Metrics/metadata/{name}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='GetMetricsMetadataDto',  # noqa: E501
+            response_type='MetricsMetadata',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/news_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/news_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/price_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/price_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/screener_api.py` & `investor8-sdk-1.1.9/swagger_client/api/screener_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from investor8_sdk.api_client import ApiClient
+from swagger_client.api_client import ApiClient
 
 
 class ScreenerApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
@@ -100,18 +100,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/sectors/all_returns', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -185,18 +185,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/sa/sector/returns/today', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -274,18 +274,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/dow/tickers', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -371,18 +371,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/ipo/list', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -488,18 +488,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/top/{category}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -581,18 +581,18 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
             '/Screener/ipo/upcoming', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -601,104 +601,7 @@
             response_type='list[StockIpo]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
-
-    def search(self, **kwargs):  # noqa: E501
-        """search  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str conditions:
-        :param str order_by:
-        :param str order_direction:
-        :return: list[str]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.search_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def search_with_http_info(self, **kwargs):  # noqa: E501
-        """search  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str conditions:
-        :param str order_by:
-        :param str order_direction:
-        :return: list[str]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['conditions', 'order_by', 'order_direction']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method search" % key
-                )
-            params[key] = val
-        del params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'conditions' in params:
-            query_params.append(('conditions', params['conditions']))  # noqa: E501
-        if 'order_by' in params:
-            query_params.append(('orderBy', params['order_by']))  # noqa: E501
-        if 'order_direction' in params:
-            query_params.append(('orderDirection', params['order_direction']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/Screener/search', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[str]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/search_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/search_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from investor8_sdk.api_client import ApiClient
+from investor8-sdk.api_client import ApiClient
 
 
 class SearchApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
@@ -108,15 +108,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/Search/{query}/{size}', 'GET',
             path_params,
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/settings_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/settings_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/stock_info_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/stock_info_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/tags_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/tags_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api/user_api.py` & `investor8-sdk-1.1.9/swagger_client/api/stock_info_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1666 +1,1417 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from investor8_sdk.api_client import ApiClient
+from swagger_client.api_client import ApiClient
 
 
-class UserApi(object):
+class StockInfoApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def add_to_watchlist(self, **kwargs):  # noqa: E501
-        """add_to_watchlist  # noqa: E501
+    def get_all_stock_info(self, market_index, **kwargs):  # noqa: E501
+        """get_all_stock_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.add_to_watchlist(async_req=True)
+        >>> thread = api.get_all_stock_info(market_index, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param AddToWatchlistDto body:
-        :return: Watchlist
+        :param str market_index: (required)
+        :param bool refresh_cache:
+        :return: dict(str, StockInfoDto)
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.add_to_watchlist_with_http_info(**kwargs)  # noqa: E501
+            return self.get_all_stock_info_with_http_info(market_index, **kwargs)  # noqa: E501
         else:
-            (data) = self.add_to_watchlist_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_all_stock_info_with_http_info(market_index, **kwargs)  # noqa: E501
             return data
 
-    def add_to_watchlist_with_http_info(self, **kwargs):  # noqa: E501
-        """add_to_watchlist  # noqa: E501
+    def get_all_stock_info_with_http_info(self, market_index, **kwargs):  # noqa: E501
+        """get_all_stock_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.add_to_watchlist_with_http_info(async_req=True)
+        >>> thread = api.get_all_stock_info_with_http_info(market_index, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param AddToWatchlistDto body:
-        :return: Watchlist
+        :param str market_index: (required)
+        :param bool refresh_cache:
+        :return: dict(str, StockInfoDto)
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['market_index', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method add_to_watchlist" % key
+                    " to method get_all_stock_info" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'market_index' is set
+        if ('market_index' not in params or
+                params['market_index'] is None):
+            raise ValueError("Missing the required parameter `market_index` when calling `get_all_stock_info`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'market_index' in params:
+            path_params['marketIndex'] = params['market_index']  # noqa: E501
 
         query_params = []
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist/add', 'POST',
+            '/StockInfo/all/{marketIndex}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Watchlist',  # noqa: E501
+            response_type='dict(str, StockInfoDto)',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_login_authentication_request(self, **kwargs):  # noqa: E501
-        """create_login_authentication_request  # noqa: E501
+    def get_all_stocks_popularity(self, **kwargs):  # noqa: E501
+        """get_all_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_login_authentication_request(async_req=True)
+        >>> thread = api.get_all_stocks_popularity(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateAuthReqDto body:
-        :return: AuthenticationRequest
+        :param bool refresh_cache:
+        :return: list[StockPopularityDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.create_login_authentication_request_with_http_info(**kwargs)  # noqa: E501
+            return self.get_all_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.create_login_authentication_request_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_all_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def create_login_authentication_request_with_http_info(self, **kwargs):  # noqa: E501
-        """create_login_authentication_request  # noqa: E501
+    def get_all_stocks_popularity_with_http_info(self, **kwargs):  # noqa: E501
+        """get_all_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_login_authentication_request_with_http_info(async_req=True)
+        >>> thread = api.get_all_stocks_popularity_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateAuthReqDto body:
-        :return: AuthenticationRequest
+        :param bool refresh_cache:
+        :return: list[StockPopularityDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_login_authentication_request" % key
+                    " to method get_all_stocks_popularity" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/User/authentication/request/login', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='AuthenticationRequest',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def create_plot(self, **kwargs):  # noqa: E501
-        """create_plot  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_plot(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param CreatePlotDto body:
-        :return: PlotResponseDto
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.create_plot_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.create_plot_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def create_plot_with_http_info(self, **kwargs):  # noqa: E501
-        """create_plot  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_plot_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param CreatePlotDto body:
-        :return: PlotResponseDto
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['body']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method create_plot" % key
-                )
-            params[key] = val
-        del params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/plot', 'POST',
+            '/StockInfo/popularity/all', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PlotResponseDto',  # noqa: E501
+            response_type='list[StockPopularityDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_screen(self, **kwargs):  # noqa: E501
-        """create_screen  # noqa: E501
+    def get_company_info(self, ticker, **kwargs):  # noqa: E501
+        """get_company_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_screen(async_req=True)
+        >>> thread = api.get_company_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateScreenDto body:
-        :return: Screen
+        :param str ticker: (required)
+        :return: CompanyInfoDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.create_screen_with_http_info(**kwargs)  # noqa: E501
+            return self.get_company_info_with_http_info(ticker, **kwargs)  # noqa: E501
         else:
-            (data) = self.create_screen_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_company_info_with_http_info(ticker, **kwargs)  # noqa: E501
             return data
 
-    def create_screen_with_http_info(self, **kwargs):  # noqa: E501
-        """create_screen  # noqa: E501
+    def get_company_info_with_http_info(self, ticker, **kwargs):  # noqa: E501
+        """get_company_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_screen_with_http_info(async_req=True)
+        >>> thread = api.get_company_info_with_http_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateScreenDto body:
-        :return: Screen
+        :param str ticker: (required)
+        :return: CompanyInfoDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['ticker']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_screen" % key
+                    " to method get_company_info" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'ticker' is set
+        if ('ticker' not in params or
+                params['ticker'] is None):
+            raise ValueError("Missing the required parameter `ticker` when calling `get_company_info`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'ticker' in params:
+            path_params['ticker'] = params['ticker']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/screen', 'POST',
+            '/StockInfo/companyinfo/{ticker}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Screen',  # noqa: E501
+            response_type='CompanyInfoDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_watchlist(self, **kwargs):  # noqa: E501
-        """create_watchlist  # noqa: E501
+    def get_latest_rating(self, ticker, **kwargs):  # noqa: E501
+        """get_latest_rating  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_watchlist(async_req=True)
+        >>> thread = api.get_latest_rating(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateWatchlistDto body:
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockRatingDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.create_watchlist_with_http_info(**kwargs)  # noqa: E501
+            return self.get_latest_rating_with_http_info(ticker, **kwargs)  # noqa: E501
         else:
-            (data) = self.create_watchlist_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_latest_rating_with_http_info(ticker, **kwargs)  # noqa: E501
             return data
 
-    def create_watchlist_with_http_info(self, **kwargs):  # noqa: E501
-        """create_watchlist  # noqa: E501
+    def get_latest_rating_with_http_info(self, ticker, **kwargs):  # noqa: E501
+        """get_latest_rating  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_watchlist_with_http_info(async_req=True)
+        >>> thread = api.get_latest_rating_with_http_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateWatchlistDto body:
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockRatingDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['ticker', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_watchlist" % key
+                    " to method get_latest_rating" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'ticker' is set
+        if ('ticker' not in params or
+                params['ticker'] is None):
+            raise ValueError("Missing the required parameter `ticker` when calling `get_latest_rating`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'ticker' in params:
+            path_params['ticker'] = params['ticker']  # noqa: E501
 
         query_params = []
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist', 'POST',
+            '/StockInfo/rating/latest/{ticker}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Watchlist',  # noqa: E501
+            response_type='StockRatingDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_aggregated_terminal_os_and_versions(self, **kwargs):  # noqa: E501
-        """get_aggregated_terminal_os_and_versions  # noqa: E501
+    def get_list_exchange_sector(self, **kwargs):  # noqa: E501
+        """get_list_exchange_sector  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_aggregated_terminal_os_and_versions(async_req=True)
+        >>> thread = api.get_list_exchange_sector(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: TerminalLogOSVersionsDto
+        :param bool refresh_cache:
+        :return: ListExchangeSectorDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_aggregated_terminal_os_and_versions_with_http_info(**kwargs)  # noqa: E501
+            return self.get_list_exchange_sector_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.get_aggregated_terminal_os_and_versions_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_list_exchange_sector_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def get_aggregated_terminal_os_and_versions_with_http_info(self, **kwargs):  # noqa: E501
-        """get_aggregated_terminal_os_and_versions  # noqa: E501
+    def get_list_exchange_sector_with_http_info(self, **kwargs):  # noqa: E501
+        """get_list_exchange_sector  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_aggregated_terminal_os_and_versions_with_http_info(async_req=True)
+        >>> thread = api.get_list_exchange_sector_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: TerminalLogOSVersionsDto
+        :param bool refresh_cache:
+        :return: ListExchangeSectorDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = []  # noqa: E501
+        all_params = ['refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_aggregated_terminal_os_and_versions" % key
+                    " to method get_list_exchange_sector" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/terminal/os/versions', 'GET',
+            '/StockInfo/list/exchangesector', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='TerminalLogOSVersionsDto',  # noqa: E501
+            response_type='ListExchangeSectorDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_roles(self, **kwargs):  # noqa: E501
-        """get_roles  # noqa: E501
+    def get_stock_info(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_roles(async_req=True)
+        >>> thread = api.get_stock_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[str]
+        :param str ticker: (required)
+        :return: StockInfoDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_roles_with_http_info(**kwargs)  # noqa: E501
+            return self.get_stock_info_with_http_info(ticker, **kwargs)  # noqa: E501
         else:
-            (data) = self.get_roles_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_stock_info_with_http_info(ticker, **kwargs)  # noqa: E501
             return data
 
-    def get_roles_with_http_info(self, **kwargs):  # noqa: E501
-        """get_roles  # noqa: E501
+    def get_stock_info_with_http_info(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_info  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_roles_with_http_info(async_req=True)
+        >>> thread = api.get_stock_info_with_http_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[str]
+        :param str ticker: (required)
+        :return: StockInfoDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = []  # noqa: E501
+        all_params = ['ticker']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_roles" % key
+                    " to method get_stock_info" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'ticker' is set
+        if ('ticker' not in params or
+                params['ticker'] is None):
+            raise ValueError("Missing the required parameter `ticker` when calling `get_stock_info`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/User/roles', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[str]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def get_screen(self, id, **kwargs):  # noqa: E501
-        """get_screen  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_screen(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: (required)
-        :return: Screen
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_screen_with_http_info(id, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_screen_with_http_info(id, **kwargs)  # noqa: E501
-            return data
-
-    def get_screen_with_http_info(self, id, **kwargs):  # noqa: E501
-        """get_screen  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_screen_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: (required)
-        :return: Screen
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['id']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_screen" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `get_screen`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
+        if 'ticker' in params:
+            path_params['ticker'] = params['ticker']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/screen/{id}', 'GET',
+            '/StockInfo/{ticker}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Screen',  # noqa: E501
+            response_type='StockInfoDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_screens_by_user(self, user_id, **kwargs):  # noqa: E501
-        """get_screens_by_user  # noqa: E501
+    def get_stock_info_0(self, **kwargs):  # noqa: E501
+        """get_stock_info_0  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_screens_by_user(user_id, async_req=True)
+        >>> thread = api.get_stock_info_0(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str user_id: (required)
-        :return: GetScreensByUserDto
+        :param list[str] body:
+        :return: list[StockInfoDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_screens_by_user_with_http_info(user_id, **kwargs)  # noqa: E501
+            return self.get_stock_info_0_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.get_screens_by_user_with_http_info(user_id, **kwargs)  # noqa: E501
+            (data) = self.get_stock_info_0_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def get_screens_by_user_with_http_info(self, user_id, **kwargs):  # noqa: E501
-        """get_screens_by_user  # noqa: E501
+    def get_stock_info_0_with_http_info(self, **kwargs):  # noqa: E501
+        """get_stock_info_0  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_screens_by_user_with_http_info(user_id, async_req=True)
+        >>> thread = api.get_stock_info_0_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str user_id: (required)
-        :return: GetScreensByUserDto
+        :param list[str] body:
+        :return: list[StockInfoDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['user_id']  # noqa: E501
+        all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_screens_by_user" % key
+                    " to method get_stock_info_0" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'user_id' is set
-        if ('user_id' not in params or
-                params['user_id'] is None):
-            raise ValueError("Missing the required parameter `user_id` when calling `get_screens_by_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'user_id' in params:
-            path_params['userId'] = params['user_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'body' in params:
+            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/User/screen/byuser/{userId}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='GetScreensByUserDto',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def get_terminal_log(self, id, **kwargs):  # noqa: E501
-        """get_terminal_log  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_terminal_log(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: (required)
-        :return: TerminalLogDto
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_terminal_log_with_http_info(id, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_terminal_log_with_http_info(id, **kwargs)  # noqa: E501
-            return data
-
-    def get_terminal_log_with_http_info(self, id, **kwargs):  # noqa: E501
-        """get_terminal_log  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_terminal_log_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: (required)
-        :return: TerminalLogDto
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['id']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_terminal_log" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `get_terminal_log`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/terminal/log/{id}', 'GET',
+            '/StockInfo', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='TerminalLogDto',  # noqa: E501
+            response_type='list[StockInfoDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_terminal_logs(self, **kwargs):  # noqa: E501
-        """get_terminal_logs  # noqa: E501
+    def get_stock_info_list(self, **kwargs):  # noqa: E501
+        """get_stock_info_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_terminal_logs(async_req=True)
+        >>> thread = api.get_stock_info_list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str version:
-        :param str os:
-        :param bool has_exception:
         :param int page_index:
         :param int page_size:
-        :return: list[TerminalLogDto]
+        :param str exchange:
+        :param str sector:
+        :param str market_index:
+        :param bool is_active:
+        :param bool refresh_cache:
+        :return: list[StockPriceDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_terminal_logs_with_http_info(**kwargs)  # noqa: E501
+            return self.get_stock_info_list_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.get_terminal_logs_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_stock_info_list_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def get_terminal_logs_with_http_info(self, **kwargs):  # noqa: E501
-        """get_terminal_logs  # noqa: E501
+    def get_stock_info_list_with_http_info(self, **kwargs):  # noqa: E501
+        """get_stock_info_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_terminal_logs_with_http_info(async_req=True)
+        >>> thread = api.get_stock_info_list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str version:
-        :param str os:
-        :param bool has_exception:
         :param int page_index:
         :param int page_size:
-        :return: list[TerminalLogDto]
+        :param str exchange:
+        :param str sector:
+        :param str market_index:
+        :param bool is_active:
+        :param bool refresh_cache:
+        :return: list[StockPriceDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['version', 'os', 'has_exception', 'page_index', 'page_size']  # noqa: E501
+        all_params = ['page_index', 'page_size', 'exchange', 'sector', 'market_index', 'is_active', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_terminal_logs" % key
+                    " to method get_stock_info_list" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'version' in params:
-            query_params.append(('version', params['version']))  # noqa: E501
-        if 'os' in params:
-            query_params.append(('os', params['os']))  # noqa: E501
-        if 'has_exception' in params:
-            query_params.append(('hasException', params['has_exception']))  # noqa: E501
         if 'page_index' in params:
             query_params.append(('pageIndex', params['page_index']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
+        if 'exchange' in params:
+            query_params.append(('exchange', params['exchange']))  # noqa: E501
+        if 'sector' in params:
+            query_params.append(('sector', params['sector']))  # noqa: E501
+        if 'market_index' in params:
+            query_params.append(('marketIndex', params['market_index']))  # noqa: E501
+        if 'is_active' in params:
+            query_params.append(('isActive', params['is_active']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/terminal/list/log', 'GET',
+            '/StockInfo/list', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[TerminalLogDto]',  # noqa: E501
+            response_type='list[StockPriceDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_watchlist(self, id, **kwargs):  # noqa: E501
-        """get_watchlist  # noqa: E501
+    def get_stock_info_master(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_info_master  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlist(id, async_req=True)
+        >>> thread = api.get_stock_info_master(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: (required)
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockInfoMasterDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_watchlist_with_http_info(id, **kwargs)  # noqa: E501
+            return self.get_stock_info_master_with_http_info(ticker, **kwargs)  # noqa: E501
         else:
-            (data) = self.get_watchlist_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.get_stock_info_master_with_http_info(ticker, **kwargs)  # noqa: E501
             return data
 
-    def get_watchlist_with_http_info(self, id, **kwargs):  # noqa: E501
-        """get_watchlist  # noqa: E501
+    def get_stock_info_master_with_http_info(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_info_master  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlist_with_http_info(id, async_req=True)
+        >>> thread = api.get_stock_info_master_with_http_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: (required)
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockInfoMasterDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['id']  # noqa: E501
+        all_params = ['ticker', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_watchlist" % key
+                    " to method get_stock_info_master" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `get_watchlist`")  # noqa: E501
+        # verify the required parameter 'ticker' is set
+        if ('ticker' not in params or
+                params['ticker'] is None):
+            raise ValueError("Missing the required parameter `ticker` when calling `get_stock_info_master`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
+        if 'ticker' in params:
+            path_params['ticker'] = params['ticker']  # noqa: E501
 
         query_params = []
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist/{id}', 'GET',
+            '/StockInfo/{ticker}/master', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Watchlist',  # noqa: E501
+            response_type='StockInfoMasterDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_watchlist_by_name_user_id(self, **kwargs):  # noqa: E501
-        """get_watchlist_by_name_user_id  # noqa: E501
+    def get_stock_summary(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_summary  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlist_by_name_user_id(async_req=True)
+        >>> thread = api.get_stock_summary(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name:
-        :param str user_id:
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockSummaryDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_watchlist_by_name_user_id_with_http_info(**kwargs)  # noqa: E501
+            return self.get_stock_summary_with_http_info(ticker, **kwargs)  # noqa: E501
         else:
-            (data) = self.get_watchlist_by_name_user_id_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_stock_summary_with_http_info(ticker, **kwargs)  # noqa: E501
             return data
 
-    def get_watchlist_by_name_user_id_with_http_info(self, **kwargs):  # noqa: E501
-        """get_watchlist_by_name_user_id  # noqa: E501
+    def get_stock_summary_with_http_info(self, ticker, **kwargs):  # noqa: E501
+        """get_stock_summary  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlist_by_name_user_id_with_http_info(async_req=True)
+        >>> thread = api.get_stock_summary_with_http_info(ticker, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name:
-        :param str user_id:
-        :return: Watchlist
+        :param str ticker: (required)
+        :param bool refresh_cache:
+        :return: StockSummaryDto
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'user_id']  # noqa: E501
+        all_params = ['ticker', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_watchlist_by_name_user_id" % key
+                    " to method get_stock_summary" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'ticker' is set
+        if ('ticker' not in params or
+                params['ticker'] is None):
+            raise ValueError("Missing the required parameter `ticker` when calling `get_stock_summary`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'ticker' in params:
+            path_params['ticker'] = params['ticker']  # noqa: E501
 
         query_params = []
-        if 'name' in params:
-            query_params.append(('name', params['name']))  # noqa: E501
-        if 'user_id' in params:
-            query_params.append(('userId', params['user_id']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist/byname', 'GET',
+            '/StockInfo/{ticker}/summary', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Watchlist',  # noqa: E501
+            response_type='StockSummaryDto',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_watchlists_by_user(self, user_id, **kwargs):  # noqa: E501
-        """get_watchlists_by_user  # noqa: E501
+    def get_stock_summary_multi(self, **kwargs):  # noqa: E501
+        """get_stock_summary_multi  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlists_by_user(user_id, async_req=True)
+        >>> thread = api.get_stock_summary_multi(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str user_id: (required)
-        :return: GetWatchlistsByUserDto
+        :param str tickers:
+        :param bool refresh_cache:
+        :return: list[StockSummaryDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_watchlists_by_user_with_http_info(user_id, **kwargs)  # noqa: E501
+            return self.get_stock_summary_multi_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.get_watchlists_by_user_with_http_info(user_id, **kwargs)  # noqa: E501
+            (data) = self.get_stock_summary_multi_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def get_watchlists_by_user_with_http_info(self, user_id, **kwargs):  # noqa: E501
-        """get_watchlists_by_user  # noqa: E501
+    def get_stock_summary_multi_with_http_info(self, **kwargs):  # noqa: E501
+        """get_stock_summary_multi  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_watchlists_by_user_with_http_info(user_id, async_req=True)
+        >>> thread = api.get_stock_summary_multi_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str user_id: (required)
-        :return: GetWatchlistsByUserDto
+        :param str tickers:
+        :param bool refresh_cache:
+        :return: list[StockSummaryDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['user_id']  # noqa: E501
+        all_params = ['tickers', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_watchlists_by_user" % key
+                    " to method get_stock_summary_multi" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'user_id' is set
-        if ('user_id' not in params or
-                params['user_id'] is None):
-            raise ValueError("Missing the required parameter `user_id` when calling `get_watchlists_by_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'user_id' in params:
-            path_params['userId'] = params['user_id']  # noqa: E501
 
         query_params = []
+        if 'tickers' in params:
+            query_params.append(('tickers', params['tickers']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist/byuser/{userId}', 'GET',
+            '/StockInfo/summary', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='GetWatchlistsByUserDto',  # noqa: E501
+            response_type='list[StockSummaryDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def log_terminal_usage(self, **kwargs):  # noqa: E501
-        """log_terminal_usage  # noqa: E501
+    def get_stocks_popularity(self, **kwargs):  # noqa: E501
+        """get_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.log_terminal_usage(async_req=True)
+        >>> thread = api.get_stocks_popularity(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LogTerminalUsage body:
-        :return: LogTerminalUsage
+        :param str tickers:
+        :param bool refresh_cache:
+        :return: list[StockPopularityDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.log_terminal_usage_with_http_info(**kwargs)  # noqa: E501
+            return self.get_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.log_terminal_usage_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def log_terminal_usage_with_http_info(self, **kwargs):  # noqa: E501
-        """log_terminal_usage  # noqa: E501
+    def get_stocks_popularity_with_http_info(self, **kwargs):  # noqa: E501
+        """get_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.log_terminal_usage_with_http_info(async_req=True)
+        >>> thread = api.get_stocks_popularity_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LogTerminalUsage body:
-        :return: LogTerminalUsage
+        :param str tickers:
+        :param bool refresh_cache:
+        :return: list[StockPopularityDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['tickers', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method log_terminal_usage" % key
+                    " to method get_stocks_popularity" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'tickers' in params:
+            query_params.append(('tickers', params['tickers']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/terminal/log', 'POST',
+            '/StockInfo/popularity', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='LogTerminalUsage',  # noqa: E501
+            response_type='list[StockPopularityDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def login_user(self, **kwargs):  # noqa: E501
-        """login_user  # noqa: E501
+    def get_stocks_popularity_by_sector(self, **kwargs):  # noqa: E501
+        """get_stocks_popularity_by_sector  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.login_user(async_req=True)
+        >>> thread = api.get_stocks_popularity_by_sector(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LoginUserDto body:
-        :return: UserDto
+        :param int cutoff:
+        :param bool refresh_cache:
+        :return: dict(str, list[StockPopularityDetailsDto])
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.login_user_with_http_info(**kwargs)  # noqa: E501
+            return self.get_stocks_popularity_by_sector_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.login_user_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_stocks_popularity_by_sector_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def login_user_with_http_info(self, **kwargs):  # noqa: E501
-        """login_user  # noqa: E501
+    def get_stocks_popularity_by_sector_with_http_info(self, **kwargs):  # noqa: E501
+        """get_stocks_popularity_by_sector  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.login_user_with_http_info(async_req=True)
+        >>> thread = api.get_stocks_popularity_by_sector_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LoginUserDto body:
-        :return: UserDto
+        :param int cutoff:
+        :param bool refresh_cache:
+        :return: dict(str, list[StockPopularityDetailsDto])
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['cutoff', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method login_user" % key
+                    " to method get_stocks_popularity_by_sector" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'cutoff' in params:
+            query_params.append(('cutoff', params['cutoff']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/login', 'POST',
+            '/StockInfo/popularity/bysector', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UserDto',  # noqa: E501
+            response_type='dict(str, list[StockPopularityDetailsDto])',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def login_with_code(self, **kwargs):  # noqa: E501
-        """login_with_code  # noqa: E501
+    def get_top_stocks_popularity(self, **kwargs):  # noqa: E501
+        """get_top_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.login_with_code(async_req=True)
+        >>> thread = api.get_top_stocks_popularity(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LoginWithCodeDto body:
-        :return: UserDto
+        :param int cutoff:
+        :param bool refresh_cache:
+        :return: list[StockPopularityDetailsDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.login_with_code_with_http_info(**kwargs)  # noqa: E501
+            return self.get_top_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.login_with_code_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.get_top_stocks_popularity_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def login_with_code_with_http_info(self, **kwargs):  # noqa: E501
-        """login_with_code  # noqa: E501
+    def get_top_stocks_popularity_with_http_info(self, **kwargs):  # noqa: E501
+        """get_top_stocks_popularity  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.login_with_code_with_http_info(async_req=True)
+        >>> thread = api.get_top_stocks_popularity_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param LoginWithCodeDto body:
-        :return: UserDto
+        :param int cutoff:
+        :param bool refresh_cache:
+        :return: list[StockPopularityDetailsDto]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['cutoff', 'refresh_cache']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method login_with_code" % key
+                    " to method get_top_stocks_popularity" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'cutoff' in params:
+            query_params.append(('cutoff', params['cutoff']))  # noqa: E501
+        if 'refresh_cache' in params:
+            query_params.append(('refreshCache', params['refresh_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/login/code', 'POST',
+            '/StockInfo/popularity/top', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UserDto',  # noqa: E501
+            response_type='list[StockPopularityDetailsDto]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def remove_from_watchlist(self, **kwargs):  # noqa: E501
-        """remove_from_watchlist  # noqa: E501
+    def healthy_check(self, **kwargs):  # noqa: E501
+        """healthy_check  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.remove_from_watchlist(async_req=True)
+        >>> thread = api.healthy_check(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RemoveFromWatchlistDto body:
-        :return: Watchlist
+        :return: bool
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.remove_from_watchlist_with_http_info(**kwargs)  # noqa: E501
+            return self.healthy_check_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.remove_from_watchlist_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.healthy_check_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def remove_from_watchlist_with_http_info(self, **kwargs):  # noqa: E501
-        """remove_from_watchlist  # noqa: E501
+    def healthy_check_with_http_info(self, **kwargs):  # noqa: E501
+        """healthy_check  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.remove_from_watchlist_with_http_info(async_req=True)
+        >>> thread = api.healthy_check_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RemoveFromWatchlistDto body:
-        :return: Watchlist
+        :return: bool
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method remove_from_watchlist" % key
+                    " to method healthy_check" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -1669,35 +1420,29 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['apiKey', 'bearerCoreAuth']  # noqa: E501
+        auth_settings = ['apiKey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/User/watchlist/remove', 'POST',
+            '/health', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Watchlist',  # noqa: E501
+            response_type='bool',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/api_client.py` & `investor8-sdk-1.1.9/investor8-sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
 import mimetypes
@@ -18,17 +18,17 @@
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
-from investor8_sdk.configuration import Configuration
-import investor8_sdk.models
-from investor8_sdk import rest
+from investor8-sdk.configuration import Configuration
+import investor8-sdk.models
+from investor8-sdk import rest
 
 
 class ApiClient(object):
     """Generic API client for Swagger client library builds.
 
     Swagger generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.1.80/python'
+        self.user_agent = 'Swagger-Codegen/1.0.4/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
@@ -253,15 +253,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(investor8_sdk.models, klass)
+                klass = getattr(investor8-sdk.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/configuration.py` & `investor8-sdk-1.1.9/investor8_sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
 import logging
@@ -250,9 +250,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.1\n"\
-               "SDK Package Version: 1.1.80".\
+               "SDK Package Version: 1.1.9".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from investor8_sdk.models.active_company_dto import ActiveCompanyDto
 from investor8_sdk.models.add_to_watchlist_dto import AddToWatchlistDto
 from investor8_sdk.models.authentication_request import AuthenticationRequest
 from investor8_sdk.models.authentication_source import AuthenticationSource
 from investor8_sdk.models.company_info_dto import CompanyInfoDto
 from investor8_sdk.models.create_auth_req_dto import CreateAuthReqDto
 from investor8_sdk.models.create_plot_dto import CreatePlotDto
-from investor8_sdk.models.create_screen_dto import CreateScreenDto
 from investor8_sdk.models.create_watchlist_dto import CreateWatchlistDto
 from investor8_sdk.models.current_metrics_dto import CurrentMetricsDto
 from investor8_sdk.models.current_momentum_metrics_dto import CurrentMomentumMetricsDto
 from investor8_sdk.models.daily_metrics_dto import DailyMetricsDto
 from investor8_sdk.models.detailed_latest_price_dto import DetailedLatestPriceDto
-from investor8_sdk.models.discovery_source import DiscoverySource
 from investor8_sdk.models.earning_metrics_dto import EarningMetricsDto
 from investor8_sdk.models.financial_metric_metadata_dto import FinancialMetricMetadataDto
 from investor8_sdk.models.financial_report_dto import FinancialReportDto
 from investor8_sdk.models.financial_tag import FinancialTag
 from investor8_sdk.models.financials_growth import FinancialsGrowth
-from investor8_sdk.models.get_list_metrics_metadata_dto import GetListMetricsMetadataDto
-from investor8_sdk.models.get_metrics_metadata_dto import GetMetricsMetadataDto
-from investor8_sdk.models.get_screens_by_user_dto import GetScreensByUserDto
 from investor8_sdk.models.get_watchlists_by_user_dto import GetWatchlistsByUserDto
 from investor8_sdk.models.historical_daily_metrics_dto import HistoricalDailyMetricsDto
 from investor8_sdk.models.historical_financial_metrics import HistoricalFinancialMetrics
 from investor8_sdk.models.historical_indicator_dto import HistoricalIndicatorDto
-from investor8_sdk.models.historical_metric_value_dto import HistoricalMetricValueDto
 from investor8_sdk.models.historical_return import HistoricalReturn
 from investor8_sdk.models.historical_returns_dto import HistoricalReturnsDto
 from investor8_sdk.models.historical_value_metrics import HistoricalValueMetrics
 from investor8_sdk.models.history_length import HistoryLength
 from investor8_sdk.models.i8_terminal_check_version_dto import I8TerminalCheckVersionDto
 from investor8_sdk.models.i8_terminal_version import I8TerminalVersion
 from investor8_sdk.models.i8_terminal_version_dto import I8TerminalVersionDto
@@ -56,16 +50,15 @@
 from investor8_sdk.models.log_terminal_usage import LogTerminalUsage
 from investor8_sdk.models.login_user_dto import LoginUserDto
 from investor8_sdk.models.login_with_code_dto import LoginWithCodeDto
 from investor8_sdk.models.market_highlight_dto import MarketHighlightDto
 from investor8_sdk.models.market_highlight_status import MarketHighlightStatus
 from investor8_sdk.models.metadata_properties_dto import MetadataPropertiesDto
 from investor8_sdk.models.metrics import Metrics
-from investor8_sdk.models.metrics_by_period_dto import MetricsByPeriodDto
-from investor8_sdk.models.metrics_metadata_response_dto import MetricsMetadataResponseDto
+from investor8_sdk.models.metrics_metadata import MetricsMetadata
 from investor8_sdk.models.momentum_metric_dto import MomentumMetricDto
 from investor8_sdk.models.monthly_metrics import MonthlyMetrics
 from investor8_sdk.models.monthly_returns import MonthlyReturns
 from investor8_sdk.models.news_categories_dto import NewsCategoriesDto
 from investor8_sdk.models.news_source import NewsSource
 from investor8_sdk.models.period_metric_value import PeriodMetricValue
 from investor8_sdk.models.period_return import PeriodReturn
@@ -75,17 +68,14 @@
 from investor8_sdk.models.recent_earning_dto import RecentEarningDto
 from investor8_sdk.models.remove_from_watchlist_dto import RemoveFromWatchlistDto
 from investor8_sdk.models.req_type import ReqType
 from investor8_sdk.models.result_field import ResultField
 from investor8_sdk.models.return_metrics import ReturnMetrics
 from investor8_sdk.models.sa_attributes_prices import SAAttributesPrices
 from investor8_sdk.models.sa_sector_price_dto import SASectorPriceDto
-from investor8_sdk.models.screen import Screen
-from investor8_sdk.models.screen_dto import ScreenDto
-from investor8_sdk.models.screening_condition import ScreeningCondition
 from investor8_sdk.models.sector_returns_dto import SectorReturnsDto
 from investor8_sdk.models.standardized_financial import StandardizedFinancial
 from investor8_sdk.models.stock_earning_dto import StockEarningDto
 from investor8_sdk.models.stock_financial import StockFinancial
 from investor8_sdk.models.stock_financial_metrics import StockFinancialMetrics
 from investor8_sdk.models.stock_info_dto import StockInfoDto
 from investor8_sdk.models.stock_info_master_dto import StockInfoMasterDto
@@ -95,19 +85,15 @@
 from investor8_sdk.models.stock_news_status import StockNewsStatus
 from investor8_sdk.models.stock_popularity_details_dto import StockPopularityDetailsDto
 from investor8_sdk.models.stock_popularity_dto import StockPopularityDto
 from investor8_sdk.models.stock_price import StockPrice
 from investor8_sdk.models.stock_price_dto import StockPriceDto
 from investor8_sdk.models.stock_rating_dto import StockRatingDto
 from investor8_sdk.models.stock_summary_dto import StockSummaryDto
-from investor8_sdk.models.symbols_current_metrics_dto import SymbolsCurrentMetricsDto
-from investor8_sdk.models.symbols_historical_metrics_dto import SymbolsHistoricalMetricsDto
 from investor8_sdk.models.tag_details_dto import TagDetailsDto
 from investor8_sdk.models.tag_info_dto import TagInfoDto
-from investor8_sdk.models.terminal_log_dto import TerminalLogDto
-from investor8_sdk.models.terminal_log_os_versions_dto import TerminalLogOSVersionsDto
 from investor8_sdk.models.trading_calendar_details_dto import TradingCalendarDetailsDto
 from investor8_sdk.models.upcoming_earning_dto import UpcomingEarningDto
 from investor8_sdk.models.user_dto import UserDto
 from investor8_sdk.models.value_metrics_dto import ValueMetricsDto
 from investor8_sdk.models.watchlist import Watchlist
 from investor8_sdk.models.watchlist_dto import WatchlistDto
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/active_company_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/active_company_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/add_to_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/add_to_watchlist_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/authentication_request.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authentication_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/authentication_source.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authentication_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/authorize_account_request_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/authorize_account_response_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/change_password_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/company_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/company_info_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_auth_req_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_auth_req_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_plot_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_screen_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_watchlist_dto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CreateScreenDto(object):
+class CreateWatchlistDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'user_id': 'str',
         'name': 'str',
-        'conditions': 'str'
+        'tickers': 'list[str]'
     }
 
     attribute_map = {
         'user_id': 'UserId',
         'name': 'Name',
-        'conditions': 'Conditions'
+        'tickers': 'Tickers'
     }
 
-    def __init__(self, user_id=None, name=None, conditions=None):  # noqa: E501
-        """CreateScreenDto - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, user_id=None, name=None, tickers=None):  # noqa: E501
+        """CreateWatchlistDto - a model defined in Swagger"""  # noqa: E501
         self._user_id = None
         self._name = None
-        self._conditions = None
+        self._tickers = None
         self.discriminator = None
         self.user_id = user_id
         self.name = name
-        self.conditions = conditions
+        self.tickers = tickers
 
     @property
     def user_id(self):
-        """Gets the user_id of this CreateScreenDto.  # noqa: E501
+        """Gets the user_id of this CreateWatchlistDto.  # noqa: E501
 
 
-        :return: The user_id of this CreateScreenDto.  # noqa: E501
+        :return: The user_id of this CreateWatchlistDto.  # noqa: E501
         :rtype: str
         """
         return self._user_id
 
     @user_id.setter
     def user_id(self, user_id):
-        """Sets the user_id of this CreateScreenDto.
+        """Sets the user_id of this CreateWatchlistDto.
 
 
-        :param user_id: The user_id of this CreateScreenDto.  # noqa: E501
+        :param user_id: The user_id of this CreateWatchlistDto.  # noqa: E501
         :type: str
         """
         if user_id is None:
             raise ValueError("Invalid value for `user_id`, must not be `None`")  # noqa: E501
 
         self._user_id = user_id
 
     @property
     def name(self):
-        """Gets the name of this CreateScreenDto.  # noqa: E501
+        """Gets the name of this CreateWatchlistDto.  # noqa: E501
 
 
-        :return: The name of this CreateScreenDto.  # noqa: E501
+        :return: The name of this CreateWatchlistDto.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateScreenDto.
+        """Sets the name of this CreateWatchlistDto.
 
 
-        :param name: The name of this CreateScreenDto.  # noqa: E501
+        :param name: The name of this CreateWatchlistDto.  # noqa: E501
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def conditions(self):
-        """Gets the conditions of this CreateScreenDto.  # noqa: E501
+    def tickers(self):
+        """Gets the tickers of this CreateWatchlistDto.  # noqa: E501
 
 
-        :return: The conditions of this CreateScreenDto.  # noqa: E501
-        :rtype: str
+        :return: The tickers of this CreateWatchlistDto.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._conditions
+        return self._tickers
 
-    @conditions.setter
-    def conditions(self, conditions):
-        """Sets the conditions of this CreateScreenDto.
+    @tickers.setter
+    def tickers(self, tickers):
+        """Sets the tickers of this CreateWatchlistDto.
 
 
-        :param conditions: The conditions of this CreateScreenDto.  # noqa: E501
-        :type: str
+        :param tickers: The tickers of this CreateWatchlistDto.  # noqa: E501
+        :type: list[str]
         """
-        if conditions is None:
-            raise ValueError("Invalid value for `conditions`, must not be `None`")  # noqa: E501
+        if tickers is None:
+            raise ValueError("Invalid value for `tickers`, must not be `None`")  # noqa: E501
 
-        self._conditions = conditions
+        self._tickers = tickers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -135,15 +135,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CreateScreenDto, dict):
+        if issubclass(CreateWatchlistDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -151,15 +151,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateScreenDto):
+        if not isinstance(other, CreateWatchlistDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_update_news.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_user_res_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/create_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_watchlist_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
@@ -41,17 +41,20 @@
 
     def __init__(self, user_id=None, name=None, tickers=None):  # noqa: E501
         """CreateWatchlistDto - a model defined in Swagger"""  # noqa: E501
         self._user_id = None
         self._name = None
         self._tickers = None
         self.discriminator = None
-        self.user_id = user_id
-        self.name = name
-        self.tickers = tickers
+        if user_id is not None:
+            self.user_id = user_id
+        if name is not None:
+            self.name = name
+        if tickers is not None:
+            self.tickers = tickers
 
     @property
     def user_id(self):
         """Gets the user_id of this CreateWatchlistDto.  # noqa: E501
 
 
         :return: The user_id of this CreateWatchlistDto.  # noqa: E501
@@ -63,16 +66,14 @@
     def user_id(self, user_id):
         """Sets the user_id of this CreateWatchlistDto.
 
 
         :param user_id: The user_id of this CreateWatchlistDto.  # noqa: E501
         :type: str
         """
-        if user_id is None:
-            raise ValueError("Invalid value for `user_id`, must not be `None`")  # noqa: E501
 
         self._user_id = user_id
 
     @property
     def name(self):
         """Gets the name of this CreateWatchlistDto.  # noqa: E501
 
@@ -86,16 +87,14 @@
     def name(self, name):
         """Sets the name of this CreateWatchlistDto.
 
 
         :param name: The name of this CreateWatchlistDto.  # noqa: E501
         :type: str
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def tickers(self):
         """Gets the tickers of this CreateWatchlistDto.  # noqa: E501
 
@@ -109,16 +108,14 @@
     def tickers(self, tickers):
         """Sets the tickers of this CreateWatchlistDto.
 
 
         :param tickers: The tickers of this CreateWatchlistDto.  # noqa: E501
         :type: list[str]
         """
-        if tickers is None:
-            raise ValueError("Invalid value for `tickers`, must not be `None`")  # noqa: E501
 
         self._tickers = tickers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/current_metadat_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/current_metrics_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,87 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CurrentMetadatMetricsDto(object):
+class CurrentMetricsDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'list[CurrentMetricsDto]',
-        'metadata': 'list[MetricsMetadataResponseDto]'
+        'ticker': 'str',
+        'metric': 'str',
+        'value': 'float'
     }
 
     attribute_map = {
-        'data': 'Data',
-        'metadata': 'Metadata'
+        'ticker': 'Ticker',
+        'metric': 'Metric',
+        'value': 'Value'
     }
 
-    def __init__(self, data=None, metadata=None):  # noqa: E501
-        """CurrentMetadatMetricsDto - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._metadata = None
+    def __init__(self, ticker=None, metric=None, value=None):  # noqa: E501
+        """CurrentMetricsDto - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._metric = None
+        self._value = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        if metadata is not None:
-            self.metadata = metadata
+        if ticker is not None:
+            self.ticker = ticker
+        if metric is not None:
+            self.metric = metric
+        if value is not None:
+            self.value = value
 
     @property
-    def data(self):
-        """Gets the data of this CurrentMetadatMetricsDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this CurrentMetricsDto.  # noqa: E501
 
 
-        :return: The data of this CurrentMetadatMetricsDto.  # noqa: E501
-        :rtype: list[CurrentMetricsDto]
+        :return: The ticker of this CurrentMetricsDto.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self._ticker
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this CurrentMetadatMetricsDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this CurrentMetricsDto.
 
 
-        :param data: The data of this CurrentMetadatMetricsDto.  # noqa: E501
-        :type: list[CurrentMetricsDto]
+        :param ticker: The ticker of this CurrentMetricsDto.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self._ticker = ticker
 
     @property
-    def metadata(self):
-        """Gets the metadata of this CurrentMetadatMetricsDto.  # noqa: E501
+    def metric(self):
+        """Gets the metric of this CurrentMetricsDto.  # noqa: E501
 
 
-        :return: The metadata of this CurrentMetadatMetricsDto.  # noqa: E501
-        :rtype: list[MetricsMetadataResponseDto]
+        :return: The metric of this CurrentMetricsDto.  # noqa: E501
+        :rtype: str
         """
-        return self._metadata
+        return self._metric
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this CurrentMetadatMetricsDto.
+    @metric.setter
+    def metric(self, metric):
+        """Sets the metric of this CurrentMetricsDto.
 
 
-        :param metadata: The metadata of this CurrentMetadatMetricsDto.  # noqa: E501
-        :type: list[MetricsMetadataResponseDto]
+        :param metric: The metric of this CurrentMetricsDto.  # noqa: E501
+        :type: str
         """
 
-        self._metadata = metadata
+        self._metric = metric
+
+    @property
+    def value(self):
+        """Gets the value of this CurrentMetricsDto.  # noqa: E501
+
+
+        :return: The value of this CurrentMetricsDto.  # noqa: E501
+        :rtype: float
+        """
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        """Sets the value of this CurrentMetricsDto.
+
+
+        :param value: The value of this CurrentMetricsDto.  # noqa: E501
+        :type: float
+        """
+
+        self._value = value
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CurrentMetadatMetricsDto, dict):
+        if issubclass(CurrentMetricsDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CurrentMetadatMetricsDto):
+        if not isinstance(other, CurrentMetricsDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/current_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_ipo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,513 +1,565 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CurrentMetricsDto(object):
+class StockIpo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'symbol': 'str',
-        'metric': 'str',
-        'input_metric': 'str',
-        'value': 'str',
-        'period': 'str',
-        'last_modified': 'datetime',
-        'overall_rank': 'int',
-        'overall_count': 'int',
-        'spx_rank': 'int',
-        'spx_count': 'int',
-        'nasdaq_rank': 'int',
-        'nasdaq_count': 'int',
-        'dow_rank': 'int',
-        'dow_count': 'int',
-        'sector_rank': 'int',
-        'sector_count': 'int',
-        'industry_rank': 'int',
-        'industry_count': 'int'
+        'id': 'str',
+        'ticker': 'str',
+        'status': 'str',
+        'timestamp': 'int',
+        'exchange': 'str',
+        'open': 'float',
+        'close': 'float',
+        'volume': 'float',
+        'day_change': 'float',
+        'week_change': 'float',
+        'month_change': 'float',
+        'offer_amount': 'float',
+        'share_count': 'float',
+        'share_count_highest': 'float',
+        'share_count_lowest': 'float',
+        'share_price': 'float',
+        'share_price_highest': 'float',
+        'share_price_lowest': 'float',
+        'announcement_url': 'str',
+        'sec_report_url': 'str'
     }
 
     attribute_map = {
-        'symbol': 'Symbol',
-        'metric': 'Metric',
-        'input_metric': 'InputMetric',
-        'value': 'Value',
-        'period': 'Period',
-        'last_modified': 'LastModified',
-        'overall_rank': 'OverallRank',
-        'overall_count': 'OverallCount',
-        'spx_rank': 'SpxRank',
-        'spx_count': 'SpxCount',
-        'nasdaq_rank': 'NasdaqRank',
-        'nasdaq_count': 'NasdaqCount',
-        'dow_rank': 'DowRank',
-        'dow_count': 'DowCount',
-        'sector_rank': 'SectorRank',
-        'sector_count': 'SectorCount',
-        'industry_rank': 'IndustryRank',
-        'industry_count': 'IndustryCount'
+        'id': 'Id',
+        'ticker': 'Ticker',
+        'status': 'Status',
+        'timestamp': 'Timestamp',
+        'exchange': 'Exchange',
+        'open': 'Open',
+        'close': 'Close',
+        'volume': 'Volume',
+        'day_change': 'DayChange',
+        'week_change': 'WeekChange',
+        'month_change': 'MonthChange',
+        'offer_amount': 'OfferAmount',
+        'share_count': 'ShareCount',
+        'share_count_highest': 'ShareCountHighest',
+        'share_count_lowest': 'ShareCountLowest',
+        'share_price': 'SharePrice',
+        'share_price_highest': 'SharePriceHighest',
+        'share_price_lowest': 'SharePriceLowest',
+        'announcement_url': 'AnnouncementUrl',
+        'sec_report_url': 'SecReportUrl'
     }
 
-    def __init__(self, symbol=None, metric=None, input_metric=None, value=None, period=None, last_modified=None, overall_rank=None, overall_count=None, spx_rank=None, spx_count=None, nasdaq_rank=None, nasdaq_count=None, dow_rank=None, dow_count=None, sector_rank=None, sector_count=None, industry_rank=None, industry_count=None):  # noqa: E501
-        """CurrentMetricsDto - a model defined in Swagger"""  # noqa: E501
-        self._symbol = None
-        self._metric = None
-        self._input_metric = None
-        self._value = None
-        self._period = None
-        self._last_modified = None
-        self._overall_rank = None
-        self._overall_count = None
-        self._spx_rank = None
-        self._spx_count = None
-        self._nasdaq_rank = None
-        self._nasdaq_count = None
-        self._dow_rank = None
-        self._dow_count = None
-        self._sector_rank = None
-        self._sector_count = None
-        self._industry_rank = None
-        self._industry_count = None
+    def __init__(self, id=None, ticker=None, status=None, timestamp=None, exchange=None, open=None, close=None, volume=None, day_change=None, week_change=None, month_change=None, offer_amount=None, share_count=None, share_count_highest=None, share_count_lowest=None, share_price=None, share_price_highest=None, share_price_lowest=None, announcement_url=None, sec_report_url=None):  # noqa: E501
+        """StockIpo - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._ticker = None
+        self._status = None
+        self._timestamp = None
+        self._exchange = None
+        self._open = None
+        self._close = None
+        self._volume = None
+        self._day_change = None
+        self._week_change = None
+        self._month_change = None
+        self._offer_amount = None
+        self._share_count = None
+        self._share_count_highest = None
+        self._share_count_lowest = None
+        self._share_price = None
+        self._share_price_highest = None
+        self._share_price_lowest = None
+        self._announcement_url = None
+        self._sec_report_url = None
         self.discriminator = None
-        if symbol is not None:
-            self.symbol = symbol
-        if metric is not None:
-            self.metric = metric
-        if input_metric is not None:
-            self.input_metric = input_metric
-        if value is not None:
-            self.value = value
-        if period is not None:
-            self.period = period
-        if last_modified is not None:
-            self.last_modified = last_modified
-        if overall_rank is not None:
-            self.overall_rank = overall_rank
-        if overall_count is not None:
-            self.overall_count = overall_count
-        if spx_rank is not None:
-            self.spx_rank = spx_rank
-        if spx_count is not None:
-            self.spx_count = spx_count
-        if nasdaq_rank is not None:
-            self.nasdaq_rank = nasdaq_rank
-        if nasdaq_count is not None:
-            self.nasdaq_count = nasdaq_count
-        if dow_rank is not None:
-            self.dow_rank = dow_rank
-        if dow_count is not None:
-            self.dow_count = dow_count
-        if sector_rank is not None:
-            self.sector_rank = sector_rank
-        if sector_count is not None:
-            self.sector_count = sector_count
-        if industry_rank is not None:
-            self.industry_rank = industry_rank
-        if industry_count is not None:
-            self.industry_count = industry_count
+        if id is not None:
+            self.id = id
+        if ticker is not None:
+            self.ticker = ticker
+        if status is not None:
+            self.status = status
+        if timestamp is not None:
+            self.timestamp = timestamp
+        if exchange is not None:
+            self.exchange = exchange
+        if open is not None:
+            self.open = open
+        if close is not None:
+            self.close = close
+        if volume is not None:
+            self.volume = volume
+        if day_change is not None:
+            self.day_change = day_change
+        if week_change is not None:
+            self.week_change = week_change
+        if month_change is not None:
+            self.month_change = month_change
+        if offer_amount is not None:
+            self.offer_amount = offer_amount
+        if share_count is not None:
+            self.share_count = share_count
+        if share_count_highest is not None:
+            self.share_count_highest = share_count_highest
+        if share_count_lowest is not None:
+            self.share_count_lowest = share_count_lowest
+        if share_price is not None:
+            self.share_price = share_price
+        if share_price_highest is not None:
+            self.share_price_highest = share_price_highest
+        if share_price_lowest is not None:
+            self.share_price_lowest = share_price_lowest
+        if announcement_url is not None:
+            self.announcement_url = announcement_url
+        if sec_report_url is not None:
+            self.sec_report_url = sec_report_url
 
     @property
-    def symbol(self):
-        """Gets the symbol of this CurrentMetricsDto.  # noqa: E501
+    def id(self):
+        """Gets the id of this StockIpo.  # noqa: E501
 
 
-        :return: The symbol of this CurrentMetricsDto.  # noqa: E501
+        :return: The id of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._symbol
+        return self._id
 
-    @symbol.setter
-    def symbol(self, symbol):
-        """Sets the symbol of this CurrentMetricsDto.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StockIpo.
 
 
-        :param symbol: The symbol of this CurrentMetricsDto.  # noqa: E501
+        :param id: The id of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._symbol = symbol
+        self._id = id
 
     @property
-    def metric(self):
-        """Gets the metric of this CurrentMetricsDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this StockIpo.  # noqa: E501
 
 
-        :return: The metric of this CurrentMetricsDto.  # noqa: E501
+        :return: The ticker of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._metric
+        return self._ticker
 
-    @metric.setter
-    def metric(self, metric):
-        """Sets the metric of this CurrentMetricsDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this StockIpo.
 
 
-        :param metric: The metric of this CurrentMetricsDto.  # noqa: E501
+        :param ticker: The ticker of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._metric = metric
+        self._ticker = ticker
 
     @property
-    def input_metric(self):
-        """Gets the input_metric of this CurrentMetricsDto.  # noqa: E501
+    def status(self):
+        """Gets the status of this StockIpo.  # noqa: E501
 
 
-        :return: The input_metric of this CurrentMetricsDto.  # noqa: E501
+        :return: The status of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._input_metric
+        return self._status
 
-    @input_metric.setter
-    def input_metric(self, input_metric):
-        """Sets the input_metric of this CurrentMetricsDto.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this StockIpo.
 
 
-        :param input_metric: The input_metric of this CurrentMetricsDto.  # noqa: E501
+        :param status: The status of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._input_metric = input_metric
+        self._status = status
 
     @property
-    def value(self):
-        """Gets the value of this CurrentMetricsDto.  # noqa: E501
+    def timestamp(self):
+        """Gets the timestamp of this StockIpo.  # noqa: E501
 
 
-        :return: The value of this CurrentMetricsDto.  # noqa: E501
-        :rtype: str
+        :return: The timestamp of this StockIpo.  # noqa: E501
+        :rtype: int
         """
-        return self._value
+        return self._timestamp
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this CurrentMetricsDto.
+    @timestamp.setter
+    def timestamp(self, timestamp):
+        """Sets the timestamp of this StockIpo.
 
 
-        :param value: The value of this CurrentMetricsDto.  # noqa: E501
-        :type: str
+        :param timestamp: The timestamp of this StockIpo.  # noqa: E501
+        :type: int
         """
 
-        self._value = value
+        self._timestamp = timestamp
 
     @property
-    def period(self):
-        """Gets the period of this CurrentMetricsDto.  # noqa: E501
+    def exchange(self):
+        """Gets the exchange of this StockIpo.  # noqa: E501
 
 
-        :return: The period of this CurrentMetricsDto.  # noqa: E501
+        :return: The exchange of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._period
+        return self._exchange
 
-    @period.setter
-    def period(self, period):
-        """Sets the period of this CurrentMetricsDto.
+    @exchange.setter
+    def exchange(self, exchange):
+        """Sets the exchange of this StockIpo.
 
 
-        :param period: The period of this CurrentMetricsDto.  # noqa: E501
+        :param exchange: The exchange of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._period = period
+        self._exchange = exchange
 
     @property
-    def last_modified(self):
-        """Gets the last_modified of this CurrentMetricsDto.  # noqa: E501
+    def open(self):
+        """Gets the open of this StockIpo.  # noqa: E501
 
 
-        :return: The last_modified of this CurrentMetricsDto.  # noqa: E501
-        :rtype: datetime
+        :return: The open of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._last_modified
+        return self._open
 
-    @last_modified.setter
-    def last_modified(self, last_modified):
-        """Sets the last_modified of this CurrentMetricsDto.
+    @open.setter
+    def open(self, open):
+        """Sets the open of this StockIpo.
 
 
-        :param last_modified: The last_modified of this CurrentMetricsDto.  # noqa: E501
-        :type: datetime
+        :param open: The open of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._last_modified = last_modified
+        self._open = open
 
     @property
-    def overall_rank(self):
-        """Gets the overall_rank of this CurrentMetricsDto.  # noqa: E501
+    def close(self):
+        """Gets the close of this StockIpo.  # noqa: E501
 
 
-        :return: The overall_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The close of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._overall_rank
+        return self._close
 
-    @overall_rank.setter
-    def overall_rank(self, overall_rank):
-        """Sets the overall_rank of this CurrentMetricsDto.
+    @close.setter
+    def close(self, close):
+        """Sets the close of this StockIpo.
 
 
-        :param overall_rank: The overall_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param close: The close of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._overall_rank = overall_rank
+        self._close = close
 
     @property
-    def overall_count(self):
-        """Gets the overall_count of this CurrentMetricsDto.  # noqa: E501
+    def volume(self):
+        """Gets the volume of this StockIpo.  # noqa: E501
 
 
-        :return: The overall_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The volume of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._overall_count
+        return self._volume
 
-    @overall_count.setter
-    def overall_count(self, overall_count):
-        """Sets the overall_count of this CurrentMetricsDto.
+    @volume.setter
+    def volume(self, volume):
+        """Sets the volume of this StockIpo.
 
 
-        :param overall_count: The overall_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param volume: The volume of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._overall_count = overall_count
+        self._volume = volume
 
     @property
-    def spx_rank(self):
-        """Gets the spx_rank of this CurrentMetricsDto.  # noqa: E501
+    def day_change(self):
+        """Gets the day_change of this StockIpo.  # noqa: E501
 
 
-        :return: The spx_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The day_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._spx_rank
+        return self._day_change
 
-    @spx_rank.setter
-    def spx_rank(self, spx_rank):
-        """Sets the spx_rank of this CurrentMetricsDto.
+    @day_change.setter
+    def day_change(self, day_change):
+        """Sets the day_change of this StockIpo.
 
 
-        :param spx_rank: The spx_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param day_change: The day_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._spx_rank = spx_rank
+        self._day_change = day_change
 
     @property
-    def spx_count(self):
-        """Gets the spx_count of this CurrentMetricsDto.  # noqa: E501
+    def week_change(self):
+        """Gets the week_change of this StockIpo.  # noqa: E501
 
 
-        :return: The spx_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The week_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._spx_count
+        return self._week_change
 
-    @spx_count.setter
-    def spx_count(self, spx_count):
-        """Sets the spx_count of this CurrentMetricsDto.
+    @week_change.setter
+    def week_change(self, week_change):
+        """Sets the week_change of this StockIpo.
 
 
-        :param spx_count: The spx_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param week_change: The week_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._spx_count = spx_count
+        self._week_change = week_change
 
     @property
-    def nasdaq_rank(self):
-        """Gets the nasdaq_rank of this CurrentMetricsDto.  # noqa: E501
+    def month_change(self):
+        """Gets the month_change of this StockIpo.  # noqa: E501
 
 
-        :return: The nasdaq_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The month_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._nasdaq_rank
+        return self._month_change
 
-    @nasdaq_rank.setter
-    def nasdaq_rank(self, nasdaq_rank):
-        """Sets the nasdaq_rank of this CurrentMetricsDto.
+    @month_change.setter
+    def month_change(self, month_change):
+        """Sets the month_change of this StockIpo.
 
 
-        :param nasdaq_rank: The nasdaq_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param month_change: The month_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._nasdaq_rank = nasdaq_rank
+        self._month_change = month_change
 
     @property
-    def nasdaq_count(self):
-        """Gets the nasdaq_count of this CurrentMetricsDto.  # noqa: E501
+    def offer_amount(self):
+        """Gets the offer_amount of this StockIpo.  # noqa: E501
 
 
-        :return: The nasdaq_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The offer_amount of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._nasdaq_count
+        return self._offer_amount
 
-    @nasdaq_count.setter
-    def nasdaq_count(self, nasdaq_count):
-        """Sets the nasdaq_count of this CurrentMetricsDto.
+    @offer_amount.setter
+    def offer_amount(self, offer_amount):
+        """Sets the offer_amount of this StockIpo.
 
 
-        :param nasdaq_count: The nasdaq_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param offer_amount: The offer_amount of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._nasdaq_count = nasdaq_count
+        self._offer_amount = offer_amount
 
     @property
-    def dow_rank(self):
-        """Gets the dow_rank of this CurrentMetricsDto.  # noqa: E501
+    def share_count(self):
+        """Gets the share_count of this StockIpo.  # noqa: E501
 
 
-        :return: The dow_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_count of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._dow_rank
+        return self._share_count
 
-    @dow_rank.setter
-    def dow_rank(self, dow_rank):
-        """Sets the dow_rank of this CurrentMetricsDto.
+    @share_count.setter
+    def share_count(self, share_count):
+        """Sets the share_count of this StockIpo.
 
 
-        :param dow_rank: The dow_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_count: The share_count of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._dow_rank = dow_rank
+        self._share_count = share_count
 
     @property
-    def dow_count(self):
-        """Gets the dow_count of this CurrentMetricsDto.  # noqa: E501
+    def share_count_highest(self):
+        """Gets the share_count_highest of this StockIpo.  # noqa: E501
 
 
-        :return: The dow_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_count_highest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._dow_count
+        return self._share_count_highest
 
-    @dow_count.setter
-    def dow_count(self, dow_count):
-        """Sets the dow_count of this CurrentMetricsDto.
+    @share_count_highest.setter
+    def share_count_highest(self, share_count_highest):
+        """Sets the share_count_highest of this StockIpo.
 
 
-        :param dow_count: The dow_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_count_highest: The share_count_highest of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._dow_count = dow_count
+        self._share_count_highest = share_count_highest
 
     @property
-    def sector_rank(self):
-        """Gets the sector_rank of this CurrentMetricsDto.  # noqa: E501
+    def share_count_lowest(self):
+        """Gets the share_count_lowest of this StockIpo.  # noqa: E501
 
 
-        :return: The sector_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_count_lowest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._sector_rank
+        return self._share_count_lowest
 
-    @sector_rank.setter
-    def sector_rank(self, sector_rank):
-        """Sets the sector_rank of this CurrentMetricsDto.
+    @share_count_lowest.setter
+    def share_count_lowest(self, share_count_lowest):
+        """Sets the share_count_lowest of this StockIpo.
 
 
-        :param sector_rank: The sector_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_count_lowest: The share_count_lowest of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._sector_rank = sector_rank
+        self._share_count_lowest = share_count_lowest
 
     @property
-    def sector_count(self):
-        """Gets the sector_count of this CurrentMetricsDto.  # noqa: E501
+    def share_price(self):
+        """Gets the share_price of this StockIpo.  # noqa: E501
 
 
-        :return: The sector_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_price of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._sector_count
+        return self._share_price
 
-    @sector_count.setter
-    def sector_count(self, sector_count):
-        """Sets the sector_count of this CurrentMetricsDto.
+    @share_price.setter
+    def share_price(self, share_price):
+        """Sets the share_price of this StockIpo.
 
 
-        :param sector_count: The sector_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_price: The share_price of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._sector_count = sector_count
+        self._share_price = share_price
 
     @property
-    def industry_rank(self):
-        """Gets the industry_rank of this CurrentMetricsDto.  # noqa: E501
+    def share_price_highest(self):
+        """Gets the share_price_highest of this StockIpo.  # noqa: E501
 
 
-        :return: The industry_rank of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_price_highest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._industry_rank
+        return self._share_price_highest
 
-    @industry_rank.setter
-    def industry_rank(self, industry_rank):
-        """Sets the industry_rank of this CurrentMetricsDto.
+    @share_price_highest.setter
+    def share_price_highest(self, share_price_highest):
+        """Sets the share_price_highest of this StockIpo.
 
 
-        :param industry_rank: The industry_rank of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_price_highest: The share_price_highest of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._industry_rank = industry_rank
+        self._share_price_highest = share_price_highest
 
     @property
-    def industry_count(self):
-        """Gets the industry_count of this CurrentMetricsDto.  # noqa: E501
+    def share_price_lowest(self):
+        """Gets the share_price_lowest of this StockIpo.  # noqa: E501
 
 
-        :return: The industry_count of this CurrentMetricsDto.  # noqa: E501
-        :rtype: int
+        :return: The share_price_lowest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._industry_count
+        return self._share_price_lowest
 
-    @industry_count.setter
-    def industry_count(self, industry_count):
-        """Sets the industry_count of this CurrentMetricsDto.
+    @share_price_lowest.setter
+    def share_price_lowest(self, share_price_lowest):
+        """Sets the share_price_lowest of this StockIpo.
 
 
-        :param industry_count: The industry_count of this CurrentMetricsDto.  # noqa: E501
-        :type: int
+        :param share_price_lowest: The share_price_lowest of this StockIpo.  # noqa: E501
+        :type: float
+        """
+
+        self._share_price_lowest = share_price_lowest
+
+    @property
+    def announcement_url(self):
+        """Gets the announcement_url of this StockIpo.  # noqa: E501
+
+
+        :return: The announcement_url of this StockIpo.  # noqa: E501
+        :rtype: str
+        """
+        return self._announcement_url
+
+    @announcement_url.setter
+    def announcement_url(self, announcement_url):
+        """Sets the announcement_url of this StockIpo.
+
+
+        :param announcement_url: The announcement_url of this StockIpo.  # noqa: E501
+        :type: str
+        """
+
+        self._announcement_url = announcement_url
+
+    @property
+    def sec_report_url(self):
+        """Gets the sec_report_url of this StockIpo.  # noqa: E501
+
+
+        :return: The sec_report_url of this StockIpo.  # noqa: E501
+        :rtype: str
+        """
+        return self._sec_report_url
+
+    @sec_report_url.setter
+    def sec_report_url(self, sec_report_url):
+        """Sets the sec_report_url of this StockIpo.
+
+
+        :param sec_report_url: The sec_report_url of this StockIpo.  # noqa: E501
+        :type: str
         """
 
-        self._industry_count = industry_count
+        self._sec_report_url = sec_report_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -522,15 +574,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CurrentMetricsDto, dict):
+        if issubclass(StockIpo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -538,15 +590,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CurrentMetricsDto):
+        if not isinstance(other, StockIpo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/current_momentum_metrics_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/daily_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/daily_metrics_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/detailed_latest_price_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/discovery_source.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class DiscoverySource(object):
+class StockNewsStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
+    _0 = "0"
     _1 = "1"
     _2 = "2"
     _3 = "3"
     _4 = "4"
-    _5 = "5"
-    _6 = "6"
-    _7 = "7"
-    _8 = "8"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """DiscoverySource - a model defined in Swagger"""  # noqa: E501
+        """StockNewsStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -66,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DiscoverySource, dict):
+        if issubclass(StockNewsStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -82,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DiscoverySource):
+        if not isinstance(other, StockNewsStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/earning_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/earning_metrics_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/email_type.py` & `investor8-sdk-1.1.9/investor8-sdk/models/email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/financial_metric_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financial_metric_metadata_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
@@ -36,18 +36,15 @@
         'statement_code': 'str',
         'section_name': 'str',
         'sub_section_name': 'str',
         'tag_order': 'int',
         'section_order': 'int',
         'sub_section_order': 'int',
         'is_significant': 'bool',
-        'short_description': 'str',
-        'type': 'str',
-        'data_format': 'str',
-        'display_format': 'str'
+        'short_description': 'str'
     }
 
     attribute_map = {
         'name': 'Name',
         'tag': 'Tag',
         'metric_name': 'MetricName',
         'parent': 'Parent',
@@ -55,38 +52,32 @@
         'statement_code': 'StatementCode',
         'section_name': 'SectionName',
         'sub_section_name': 'SubSectionName',
         'tag_order': 'TagOrder',
         'section_order': 'SectionOrder',
         'sub_section_order': 'SubSectionOrder',
         'is_significant': 'IsSignificant',
-        'short_description': 'ShortDescription',
-        'type': 'Type',
-        'data_format': 'DataFormat',
-        'display_format': 'DisplayFormat'
+        'short_description': 'ShortDescription'
     }
 
-    def __init__(self, name=None, tag=None, metric_name=None, parent=None, unit=None, statement_code=None, section_name=None, sub_section_name=None, tag_order=None, section_order=None, sub_section_order=None, is_significant=None, short_description=None, type=None, data_format=None, display_format=None):  # noqa: E501
+    def __init__(self, name=None, tag=None, metric_name=None, parent=None, unit=None, statement_code=None, section_name=None, sub_section_name=None, tag_order=None, section_order=None, sub_section_order=None, is_significant=None, short_description=None):  # noqa: E501
         """FinancialMetricMetadataDto - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._tag = None
         self._metric_name = None
         self._parent = None
         self._unit = None
         self._statement_code = None
         self._section_name = None
         self._sub_section_name = None
         self._tag_order = None
         self._section_order = None
         self._sub_section_order = None
         self._is_significant = None
         self._short_description = None
-        self._type = None
-        self._data_format = None
-        self._display_format = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if tag is not None:
             self.tag = tag
         if metric_name is not None:
             self.metric_name = metric_name
@@ -106,20 +97,14 @@
             self.section_order = section_order
         if sub_section_order is not None:
             self.sub_section_order = sub_section_order
         if is_significant is not None:
             self.is_significant = is_significant
         if short_description is not None:
             self.short_description = short_description
-        if type is not None:
-            self.type = type
-        if data_format is not None:
-            self.data_format = data_format
-        if display_format is not None:
-            self.display_format = display_format
 
     @property
     def name(self):
         """Gets the name of this FinancialMetricMetadataDto.  # noqa: E501
 
 
         :return: The name of this FinancialMetricMetadataDto.  # noqa: E501
@@ -386,77 +371,14 @@
 
         :param short_description: The short_description of this FinancialMetricMetadataDto.  # noqa: E501
         :type: str
         """
 
         self._short_description = short_description
 
-    @property
-    def type(self):
-        """Gets the type of this FinancialMetricMetadataDto.  # noqa: E501
-
-
-        :return: The type of this FinancialMetricMetadataDto.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this FinancialMetricMetadataDto.
-
-
-        :param type: The type of this FinancialMetricMetadataDto.  # noqa: E501
-        :type: str
-        """
-
-        self._type = type
-
-    @property
-    def data_format(self):
-        """Gets the data_format of this FinancialMetricMetadataDto.  # noqa: E501
-
-
-        :return: The data_format of this FinancialMetricMetadataDto.  # noqa: E501
-        :rtype: str
-        """
-        return self._data_format
-
-    @data_format.setter
-    def data_format(self, data_format):
-        """Sets the data_format of this FinancialMetricMetadataDto.
-
-
-        :param data_format: The data_format of this FinancialMetricMetadataDto.  # noqa: E501
-        :type: str
-        """
-
-        self._data_format = data_format
-
-    @property
-    def display_format(self):
-        """Gets the display_format of this FinancialMetricMetadataDto.  # noqa: E501
-
-
-        :return: The display_format of this FinancialMetricMetadataDto.  # noqa: E501
-        :rtype: str
-        """
-        return self._display_format
-
-    @display_format.setter
-    def display_format(self, display_format):
-        """Sets the display_format of this FinancialMetricMetadataDto.
-
-
-        :param display_format: The display_format of this FinancialMetricMetadataDto.  # noqa: E501
-        :type: str
-        """
-
-        self._display_format = display_format
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/financial_report_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/financial_report_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/financials_growth.py` & `investor8-sdk-1.1.9/investor8-sdk/models/financials_growth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/get_list_metrics_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,409 +1,409 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GetListMetricsMetadataDto(object):
+class User(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'str',
-        'metric_name': 'str',
-        'display_name': 'str',
-        'unit': 'str',
-        'categories': 'list[str]',
-        'data_format': 'str',
-        'display_format': 'str',
-        'type': 'str',
+        'first_name': 'str',
+        'last_name': 'str',
+        'email': 'str',
+        'roles': 'list[str]',
+        'opt_for_newsletter': 'bool',
+        'country': 'str',
+        'email_confirmed': 'bool',
+        'created_time': 'int',
         'last_modified': 'int',
-        'period_type_default': 'str',
-        'aliases': 'str',
-        'colorable': 'bool',
-        'short_description': 'str',
-        'soft_delete': 'bool'
+        'profile_name': 'str',
+        'api_key': 'str',
+        'auth_source': 'str',
+        'external_id': 'str'
     }
 
     attribute_map = {
         'id': 'Id',
-        'metric_name': 'MetricName',
-        'display_name': 'DisplayName',
-        'unit': 'Unit',
-        'categories': 'Categories',
-        'data_format': 'DataFormat',
-        'display_format': 'DisplayFormat',
-        'type': 'Type',
+        'first_name': 'FirstName',
+        'last_name': 'LastName',
+        'email': 'Email',
+        'roles': 'Roles',
+        'opt_for_newsletter': 'OptForNewsletter',
+        'country': 'Country',
+        'email_confirmed': 'EmailConfirmed',
+        'created_time': 'CreatedTime',
         'last_modified': 'LastModified',
-        'period_type_default': 'PeriodTypeDefault',
-        'aliases': 'Aliases',
-        'colorable': 'Colorable',
-        'short_description': 'ShortDescription',
-        'soft_delete': 'SoftDelete'
+        'profile_name': 'ProfileName',
+        'api_key': 'ApiKey',
+        'auth_source': 'AuthSource',
+        'external_id': 'ExternalId'
     }
 
-    def __init__(self, id=None, metric_name=None, display_name=None, unit=None, categories=None, data_format=None, display_format=None, type=None, last_modified=None, period_type_default=None, aliases=None, colorable=None, short_description=None, soft_delete=None):  # noqa: E501
-        """GetListMetricsMetadataDto - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, auth_source=None, external_id=None):  # noqa: E501
+        """User - a model defined in Swagger"""  # noqa: E501
         self._id = None
-        self._metric_name = None
-        self._display_name = None
-        self._unit = None
-        self._categories = None
-        self._data_format = None
-        self._display_format = None
-        self._type = None
+        self._first_name = None
+        self._last_name = None
+        self._email = None
+        self._roles = None
+        self._opt_for_newsletter = None
+        self._country = None
+        self._email_confirmed = None
+        self._created_time = None
         self._last_modified = None
-        self._period_type_default = None
-        self._aliases = None
-        self._colorable = None
-        self._short_description = None
-        self._soft_delete = None
+        self._profile_name = None
+        self._api_key = None
+        self._auth_source = None
+        self._external_id = None
         self.discriminator = None
         if id is not None:
             self.id = id
-        if metric_name is not None:
-            self.metric_name = metric_name
-        if display_name is not None:
-            self.display_name = display_name
-        if unit is not None:
-            self.unit = unit
-        if categories is not None:
-            self.categories = categories
-        if data_format is not None:
-            self.data_format = data_format
-        if display_format is not None:
-            self.display_format = display_format
-        if type is not None:
-            self.type = type
+        if first_name is not None:
+            self.first_name = first_name
+        if last_name is not None:
+            self.last_name = last_name
+        if email is not None:
+            self.email = email
+        if roles is not None:
+            self.roles = roles
+        if opt_for_newsletter is not None:
+            self.opt_for_newsletter = opt_for_newsletter
+        if country is not None:
+            self.country = country
+        if email_confirmed is not None:
+            self.email_confirmed = email_confirmed
+        if created_time is not None:
+            self.created_time = created_time
         if last_modified is not None:
             self.last_modified = last_modified
-        if period_type_default is not None:
-            self.period_type_default = period_type_default
-        if aliases is not None:
-            self.aliases = aliases
-        if colorable is not None:
-            self.colorable = colorable
-        if short_description is not None:
-            self.short_description = short_description
-        if soft_delete is not None:
-            self.soft_delete = soft_delete
+        if profile_name is not None:
+            self.profile_name = profile_name
+        if api_key is not None:
+            self.api_key = api_key
+        if auth_source is not None:
+            self.auth_source = auth_source
+        if external_id is not None:
+            self.external_id = external_id
 
     @property
     def id(self):
-        """Gets the id of this GetListMetricsMetadataDto.  # noqa: E501
+        """Gets the id of this User.  # noqa: E501
 
 
-        :return: The id of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The id of this User.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this GetListMetricsMetadataDto.
+        """Sets the id of this User.
 
 
-        :param id: The id of this GetListMetricsMetadataDto.  # noqa: E501
+        :param id: The id of this User.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
-    def metric_name(self):
-        """Gets the metric_name of this GetListMetricsMetadataDto.  # noqa: E501
+    def first_name(self):
+        """Gets the first_name of this User.  # noqa: E501
 
 
-        :return: The metric_name of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The first_name of this User.  # noqa: E501
         :rtype: str
         """
-        return self._metric_name
+        return self._first_name
 
-    @metric_name.setter
-    def metric_name(self, metric_name):
-        """Sets the metric_name of this GetListMetricsMetadataDto.
+    @first_name.setter
+    def first_name(self, first_name):
+        """Sets the first_name of this User.
 
 
-        :param metric_name: The metric_name of this GetListMetricsMetadataDto.  # noqa: E501
+        :param first_name: The first_name of this User.  # noqa: E501
         :type: str
         """
 
-        self._metric_name = metric_name
+        self._first_name = first_name
 
     @property
-    def display_name(self):
-        """Gets the display_name of this GetListMetricsMetadataDto.  # noqa: E501
+    def last_name(self):
+        """Gets the last_name of this User.  # noqa: E501
 
 
-        :return: The display_name of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The last_name of this User.  # noqa: E501
         :rtype: str
         """
-        return self._display_name
+        return self._last_name
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this GetListMetricsMetadataDto.
+    @last_name.setter
+    def last_name(self, last_name):
+        """Sets the last_name of this User.
 
 
-        :param display_name: The display_name of this GetListMetricsMetadataDto.  # noqa: E501
+        :param last_name: The last_name of this User.  # noqa: E501
         :type: str
         """
 
-        self._display_name = display_name
+        self._last_name = last_name
 
     @property
-    def unit(self):
-        """Gets the unit of this GetListMetricsMetadataDto.  # noqa: E501
+    def email(self):
+        """Gets the email of this User.  # noqa: E501
 
 
-        :return: The unit of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The email of this User.  # noqa: E501
         :rtype: str
         """
-        return self._unit
+        return self._email
 
-    @unit.setter
-    def unit(self, unit):
-        """Sets the unit of this GetListMetricsMetadataDto.
+    @email.setter
+    def email(self, email):
+        """Sets the email of this User.
 
 
-        :param unit: The unit of this GetListMetricsMetadataDto.  # noqa: E501
+        :param email: The email of this User.  # noqa: E501
         :type: str
         """
 
-        self._unit = unit
+        self._email = email
 
     @property
-    def categories(self):
-        """Gets the categories of this GetListMetricsMetadataDto.  # noqa: E501
+    def roles(self):
+        """Gets the roles of this User.  # noqa: E501
 
 
-        :return: The categories of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The roles of this User.  # noqa: E501
         :rtype: list[str]
         """
-        return self._categories
+        return self._roles
 
-    @categories.setter
-    def categories(self, categories):
-        """Sets the categories of this GetListMetricsMetadataDto.
+    @roles.setter
+    def roles(self, roles):
+        """Sets the roles of this User.
 
 
-        :param categories: The categories of this GetListMetricsMetadataDto.  # noqa: E501
+        :param roles: The roles of this User.  # noqa: E501
         :type: list[str]
         """
 
-        self._categories = categories
+        self._roles = roles
 
     @property
-    def data_format(self):
-        """Gets the data_format of this GetListMetricsMetadataDto.  # noqa: E501
+    def opt_for_newsletter(self):
+        """Gets the opt_for_newsletter of this User.  # noqa: E501
 
 
-        :return: The data_format of this GetListMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The opt_for_newsletter of this User.  # noqa: E501
+        :rtype: bool
         """
-        return self._data_format
+        return self._opt_for_newsletter
 
-    @data_format.setter
-    def data_format(self, data_format):
-        """Sets the data_format of this GetListMetricsMetadataDto.
+    @opt_for_newsletter.setter
+    def opt_for_newsletter(self, opt_for_newsletter):
+        """Sets the opt_for_newsletter of this User.
 
 
-        :param data_format: The data_format of this GetListMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param opt_for_newsletter: The opt_for_newsletter of this User.  # noqa: E501
+        :type: bool
         """
 
-        self._data_format = data_format
+        self._opt_for_newsletter = opt_for_newsletter
 
     @property
-    def display_format(self):
-        """Gets the display_format of this GetListMetricsMetadataDto.  # noqa: E501
+    def country(self):
+        """Gets the country of this User.  # noqa: E501
 
 
-        :return: The display_format of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The country of this User.  # noqa: E501
         :rtype: str
         """
-        return self._display_format
+        return self._country
 
-    @display_format.setter
-    def display_format(self, display_format):
-        """Sets the display_format of this GetListMetricsMetadataDto.
+    @country.setter
+    def country(self, country):
+        """Sets the country of this User.
 
 
-        :param display_format: The display_format of this GetListMetricsMetadataDto.  # noqa: E501
+        :param country: The country of this User.  # noqa: E501
         :type: str
         """
 
-        self._display_format = display_format
+        self._country = country
 
     @property
-    def type(self):
-        """Gets the type of this GetListMetricsMetadataDto.  # noqa: E501
+    def email_confirmed(self):
+        """Gets the email_confirmed of this User.  # noqa: E501
 
 
-        :return: The type of this GetListMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The email_confirmed of this User.  # noqa: E501
+        :rtype: bool
         """
-        return self._type
+        return self._email_confirmed
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this GetListMetricsMetadataDto.
+    @email_confirmed.setter
+    def email_confirmed(self, email_confirmed):
+        """Sets the email_confirmed of this User.
 
 
-        :param type: The type of this GetListMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param email_confirmed: The email_confirmed of this User.  # noqa: E501
+        :type: bool
         """
 
-        self._type = type
+        self._email_confirmed = email_confirmed
 
     @property
-    def last_modified(self):
-        """Gets the last_modified of this GetListMetricsMetadataDto.  # noqa: E501
+    def created_time(self):
+        """Gets the created_time of this User.  # noqa: E501
 
 
-        :return: The last_modified of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The created_time of this User.  # noqa: E501
         :rtype: int
         """
-        return self._last_modified
+        return self._created_time
 
-    @last_modified.setter
-    def last_modified(self, last_modified):
-        """Sets the last_modified of this GetListMetricsMetadataDto.
+    @created_time.setter
+    def created_time(self, created_time):
+        """Sets the created_time of this User.
 
 
-        :param last_modified: The last_modified of this GetListMetricsMetadataDto.  # noqa: E501
+        :param created_time: The created_time of this User.  # noqa: E501
         :type: int
         """
 
-        self._last_modified = last_modified
+        self._created_time = created_time
 
     @property
-    def period_type_default(self):
-        """Gets the period_type_default of this GetListMetricsMetadataDto.  # noqa: E501
+    def last_modified(self):
+        """Gets the last_modified of this User.  # noqa: E501
 
 
-        :return: The period_type_default of this GetListMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The last_modified of this User.  # noqa: E501
+        :rtype: int
         """
-        return self._period_type_default
+        return self._last_modified
 
-    @period_type_default.setter
-    def period_type_default(self, period_type_default):
-        """Sets the period_type_default of this GetListMetricsMetadataDto.
+    @last_modified.setter
+    def last_modified(self, last_modified):
+        """Sets the last_modified of this User.
 
 
-        :param period_type_default: The period_type_default of this GetListMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param last_modified: The last_modified of this User.  # noqa: E501
+        :type: int
         """
 
-        self._period_type_default = period_type_default
+        self._last_modified = last_modified
 
     @property
-    def aliases(self):
-        """Gets the aliases of this GetListMetricsMetadataDto.  # noqa: E501
+    def profile_name(self):
+        """Gets the profile_name of this User.  # noqa: E501
 
 
-        :return: The aliases of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The profile_name of this User.  # noqa: E501
         :rtype: str
         """
-        return self._aliases
+        return self._profile_name
 
-    @aliases.setter
-    def aliases(self, aliases):
-        """Sets the aliases of this GetListMetricsMetadataDto.
+    @profile_name.setter
+    def profile_name(self, profile_name):
+        """Sets the profile_name of this User.
 
 
-        :param aliases: The aliases of this GetListMetricsMetadataDto.  # noqa: E501
+        :param profile_name: The profile_name of this User.  # noqa: E501
         :type: str
         """
 
-        self._aliases = aliases
+        self._profile_name = profile_name
 
     @property
-    def colorable(self):
-        """Gets the colorable of this GetListMetricsMetadataDto.  # noqa: E501
+    def api_key(self):
+        """Gets the api_key of this User.  # noqa: E501
 
 
-        :return: The colorable of this GetListMetricsMetadataDto.  # noqa: E501
-        :rtype: bool
+        :return: The api_key of this User.  # noqa: E501
+        :rtype: str
         """
-        return self._colorable
+        return self._api_key
 
-    @colorable.setter
-    def colorable(self, colorable):
-        """Sets the colorable of this GetListMetricsMetadataDto.
+    @api_key.setter
+    def api_key(self, api_key):
+        """Sets the api_key of this User.
 
 
-        :param colorable: The colorable of this GetListMetricsMetadataDto.  # noqa: E501
-        :type: bool
+        :param api_key: The api_key of this User.  # noqa: E501
+        :type: str
         """
 
-        self._colorable = colorable
+        self._api_key = api_key
 
     @property
-    def short_description(self):
-        """Gets the short_description of this GetListMetricsMetadataDto.  # noqa: E501
+    def auth_source(self):
+        """Gets the auth_source of this User.  # noqa: E501
 
 
-        :return: The short_description of this GetListMetricsMetadataDto.  # noqa: E501
+        :return: The auth_source of this User.  # noqa: E501
         :rtype: str
         """
-        return self._short_description
+        return self._auth_source
 
-    @short_description.setter
-    def short_description(self, short_description):
-        """Sets the short_description of this GetListMetricsMetadataDto.
+    @auth_source.setter
+    def auth_source(self, auth_source):
+        """Sets the auth_source of this User.
 
 
-        :param short_description: The short_description of this GetListMetricsMetadataDto.  # noqa: E501
+        :param auth_source: The auth_source of this User.  # noqa: E501
         :type: str
         """
 
-        self._short_description = short_description
+        self._auth_source = auth_source
 
     @property
-    def soft_delete(self):
-        """Gets the soft_delete of this GetListMetricsMetadataDto.  # noqa: E501
+    def external_id(self):
+        """Gets the external_id of this User.  # noqa: E501
 
 
-        :return: The soft_delete of this GetListMetricsMetadataDto.  # noqa: E501
-        :rtype: bool
+        :return: The external_id of this User.  # noqa: E501
+        :rtype: str
         """
-        return self._soft_delete
+        return self._external_id
 
-    @soft_delete.setter
-    def soft_delete(self, soft_delete):
-        """Sets the soft_delete of this GetListMetricsMetadataDto.
+    @external_id.setter
+    def external_id(self, external_id):
+        """Sets the external_id of this User.
 
 
-        :param soft_delete: The soft_delete of this GetListMetricsMetadataDto.  # noqa: E501
-        :type: bool
+        :param external_id: The external_id of this User.  # noqa: E501
+        :type: str
         """
 
-        self._soft_delete = soft_delete
+        self._external_id = external_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -418,15 +418,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GetListMetricsMetadataDto, dict):
+        if issubclass(User, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -434,15 +434,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GetListMetricsMetadataDto):
+        if not isinstance(other, User):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/get_metrics_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_ipo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,513 +1,565 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GetMetricsMetadataDto(object):
+class StockIpo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'str',
-        'metric_name': 'str',
-        'display_name': 'str',
-        'description': 'str',
-        'unit': 'str',
-        'categories': 'list[str]',
-        'data_format': 'str',
-        'display_format': 'str',
-        'type': 'str',
-        'last_modified': 'int',
-        'period_type_default': 'str',
-        'remarks': 'str',
-        'aliases': 'str',
-        'colorable': 'bool',
-        'short_description': 'str',
-        'soft_delete': 'bool',
-        'screening_conditions': 'list[ScreeningCondition]',
-        'internal_comment': 'str'
+        'ticker': 'str',
+        'status': 'str',
+        'timestamp': 'int',
+        'exchange': 'str',
+        'open': 'float',
+        'close': 'float',
+        'volume': 'float',
+        'day_change': 'float',
+        'week_change': 'float',
+        'month_change': 'float',
+        'offer_amount': 'float',
+        'share_count': 'float',
+        'share_count_highest': 'float',
+        'share_count_lowest': 'float',
+        'share_price': 'float',
+        'share_price_highest': 'float',
+        'share_price_lowest': 'float',
+        'announcement_url': 'str',
+        'sec_report_url': 'str'
     }
 
     attribute_map = {
         'id': 'Id',
-        'metric_name': 'MetricName',
-        'display_name': 'DisplayName',
-        'description': 'Description',
-        'unit': 'Unit',
-        'categories': 'Categories',
-        'data_format': 'DataFormat',
-        'display_format': 'DisplayFormat',
-        'type': 'Type',
-        'last_modified': 'LastModified',
-        'period_type_default': 'PeriodTypeDefault',
-        'remarks': 'Remarks',
-        'aliases': 'Aliases',
-        'colorable': 'Colorable',
-        'short_description': 'ShortDescription',
-        'soft_delete': 'SoftDelete',
-        'screening_conditions': 'ScreeningConditions',
-        'internal_comment': 'InternalComment'
+        'ticker': 'Ticker',
+        'status': 'Status',
+        'timestamp': 'Timestamp',
+        'exchange': 'Exchange',
+        'open': 'Open',
+        'close': 'Close',
+        'volume': 'Volume',
+        'day_change': 'DayChange',
+        'week_change': 'WeekChange',
+        'month_change': 'MonthChange',
+        'offer_amount': 'OfferAmount',
+        'share_count': 'ShareCount',
+        'share_count_highest': 'ShareCountHighest',
+        'share_count_lowest': 'ShareCountLowest',
+        'share_price': 'SharePrice',
+        'share_price_highest': 'SharePriceHighest',
+        'share_price_lowest': 'SharePriceLowest',
+        'announcement_url': 'AnnouncementUrl',
+        'sec_report_url': 'SecReportUrl'
     }
 
-    def __init__(self, id=None, metric_name=None, display_name=None, description=None, unit=None, categories=None, data_format=None, display_format=None, type=None, last_modified=None, period_type_default=None, remarks=None, aliases=None, colorable=None, short_description=None, soft_delete=None, screening_conditions=None, internal_comment=None):  # noqa: E501
-        """GetMetricsMetadataDto - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, id=None, ticker=None, status=None, timestamp=None, exchange=None, open=None, close=None, volume=None, day_change=None, week_change=None, month_change=None, offer_amount=None, share_count=None, share_count_highest=None, share_count_lowest=None, share_price=None, share_price_highest=None, share_price_lowest=None, announcement_url=None, sec_report_url=None):  # noqa: E501
+        """StockIpo - a model defined in Swagger"""  # noqa: E501
         self._id = None
-        self._metric_name = None
-        self._display_name = None
-        self._description = None
-        self._unit = None
-        self._categories = None
-        self._data_format = None
-        self._display_format = None
-        self._type = None
-        self._last_modified = None
-        self._period_type_default = None
-        self._remarks = None
-        self._aliases = None
-        self._colorable = None
-        self._short_description = None
-        self._soft_delete = None
-        self._screening_conditions = None
-        self._internal_comment = None
+        self._ticker = None
+        self._status = None
+        self._timestamp = None
+        self._exchange = None
+        self._open = None
+        self._close = None
+        self._volume = None
+        self._day_change = None
+        self._week_change = None
+        self._month_change = None
+        self._offer_amount = None
+        self._share_count = None
+        self._share_count_highest = None
+        self._share_count_lowest = None
+        self._share_price = None
+        self._share_price_highest = None
+        self._share_price_lowest = None
+        self._announcement_url = None
+        self._sec_report_url = None
         self.discriminator = None
         if id is not None:
             self.id = id
-        if metric_name is not None:
-            self.metric_name = metric_name
-        if display_name is not None:
-            self.display_name = display_name
-        if description is not None:
-            self.description = description
-        if unit is not None:
-            self.unit = unit
-        if categories is not None:
-            self.categories = categories
-        if data_format is not None:
-            self.data_format = data_format
-        if display_format is not None:
-            self.display_format = display_format
-        if type is not None:
-            self.type = type
-        if last_modified is not None:
-            self.last_modified = last_modified
-        if period_type_default is not None:
-            self.period_type_default = period_type_default
-        if remarks is not None:
-            self.remarks = remarks
-        if aliases is not None:
-            self.aliases = aliases
-        if colorable is not None:
-            self.colorable = colorable
-        if short_description is not None:
-            self.short_description = short_description
-        if soft_delete is not None:
-            self.soft_delete = soft_delete
-        if screening_conditions is not None:
-            self.screening_conditions = screening_conditions
-        if internal_comment is not None:
-            self.internal_comment = internal_comment
+        if ticker is not None:
+            self.ticker = ticker
+        if status is not None:
+            self.status = status
+        if timestamp is not None:
+            self.timestamp = timestamp
+        if exchange is not None:
+            self.exchange = exchange
+        if open is not None:
+            self.open = open
+        if close is not None:
+            self.close = close
+        if volume is not None:
+            self.volume = volume
+        if day_change is not None:
+            self.day_change = day_change
+        if week_change is not None:
+            self.week_change = week_change
+        if month_change is not None:
+            self.month_change = month_change
+        if offer_amount is not None:
+            self.offer_amount = offer_amount
+        if share_count is not None:
+            self.share_count = share_count
+        if share_count_highest is not None:
+            self.share_count_highest = share_count_highest
+        if share_count_lowest is not None:
+            self.share_count_lowest = share_count_lowest
+        if share_price is not None:
+            self.share_price = share_price
+        if share_price_highest is not None:
+            self.share_price_highest = share_price_highest
+        if share_price_lowest is not None:
+            self.share_price_lowest = share_price_lowest
+        if announcement_url is not None:
+            self.announcement_url = announcement_url
+        if sec_report_url is not None:
+            self.sec_report_url = sec_report_url
 
     @property
     def id(self):
-        """Gets the id of this GetMetricsMetadataDto.  # noqa: E501
+        """Gets the id of this StockIpo.  # noqa: E501
 
 
-        :return: The id of this GetMetricsMetadataDto.  # noqa: E501
+        :return: The id of this StockIpo.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this GetMetricsMetadataDto.
+        """Sets the id of this StockIpo.
 
 
-        :param id: The id of this GetMetricsMetadataDto.  # noqa: E501
+        :param id: The id of this StockIpo.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
-    def metric_name(self):
-        """Gets the metric_name of this GetMetricsMetadataDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this StockIpo.  # noqa: E501
 
 
-        :return: The metric_name of this GetMetricsMetadataDto.  # noqa: E501
+        :return: The ticker of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._metric_name
+        return self._ticker
 
-    @metric_name.setter
-    def metric_name(self, metric_name):
-        """Sets the metric_name of this GetMetricsMetadataDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this StockIpo.
 
 
-        :param metric_name: The metric_name of this GetMetricsMetadataDto.  # noqa: E501
+        :param ticker: The ticker of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._metric_name = metric_name
+        self._ticker = ticker
 
     @property
-    def display_name(self):
-        """Gets the display_name of this GetMetricsMetadataDto.  # noqa: E501
+    def status(self):
+        """Gets the status of this StockIpo.  # noqa: E501
 
 
-        :return: The display_name of this GetMetricsMetadataDto.  # noqa: E501
+        :return: The status of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._display_name
+        return self._status
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this GetMetricsMetadataDto.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this StockIpo.
 
 
-        :param display_name: The display_name of this GetMetricsMetadataDto.  # noqa: E501
+        :param status: The status of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._display_name = display_name
+        self._status = status
 
     @property
-    def description(self):
-        """Gets the description of this GetMetricsMetadataDto.  # noqa: E501
+    def timestamp(self):
+        """Gets the timestamp of this StockIpo.  # noqa: E501
 
 
-        :return: The description of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The timestamp of this StockIpo.  # noqa: E501
+        :rtype: int
         """
-        return self._description
+        return self._timestamp
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this GetMetricsMetadataDto.
+    @timestamp.setter
+    def timestamp(self, timestamp):
+        """Sets the timestamp of this StockIpo.
 
 
-        :param description: The description of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param timestamp: The timestamp of this StockIpo.  # noqa: E501
+        :type: int
         """
 
-        self._description = description
+        self._timestamp = timestamp
 
     @property
-    def unit(self):
-        """Gets the unit of this GetMetricsMetadataDto.  # noqa: E501
+    def exchange(self):
+        """Gets the exchange of this StockIpo.  # noqa: E501
 
 
-        :return: The unit of this GetMetricsMetadataDto.  # noqa: E501
+        :return: The exchange of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._unit
+        return self._exchange
 
-    @unit.setter
-    def unit(self, unit):
-        """Sets the unit of this GetMetricsMetadataDto.
+    @exchange.setter
+    def exchange(self, exchange):
+        """Sets the exchange of this StockIpo.
 
 
-        :param unit: The unit of this GetMetricsMetadataDto.  # noqa: E501
+        :param exchange: The exchange of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._unit = unit
+        self._exchange = exchange
 
     @property
-    def categories(self):
-        """Gets the categories of this GetMetricsMetadataDto.  # noqa: E501
+    def open(self):
+        """Gets the open of this StockIpo.  # noqa: E501
 
 
-        :return: The categories of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: list[str]
+        :return: The open of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._categories
+        return self._open
 
-    @categories.setter
-    def categories(self, categories):
-        """Sets the categories of this GetMetricsMetadataDto.
+    @open.setter
+    def open(self, open):
+        """Sets the open of this StockIpo.
 
 
-        :param categories: The categories of this GetMetricsMetadataDto.  # noqa: E501
-        :type: list[str]
+        :param open: The open of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._categories = categories
+        self._open = open
 
     @property
-    def data_format(self):
-        """Gets the data_format of this GetMetricsMetadataDto.  # noqa: E501
+    def close(self):
+        """Gets the close of this StockIpo.  # noqa: E501
 
 
-        :return: The data_format of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The close of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._data_format
+        return self._close
 
-    @data_format.setter
-    def data_format(self, data_format):
-        """Sets the data_format of this GetMetricsMetadataDto.
+    @close.setter
+    def close(self, close):
+        """Sets the close of this StockIpo.
 
 
-        :param data_format: The data_format of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param close: The close of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._data_format = data_format
+        self._close = close
 
     @property
-    def display_format(self):
-        """Gets the display_format of this GetMetricsMetadataDto.  # noqa: E501
+    def volume(self):
+        """Gets the volume of this StockIpo.  # noqa: E501
 
 
-        :return: The display_format of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The volume of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._display_format
+        return self._volume
 
-    @display_format.setter
-    def display_format(self, display_format):
-        """Sets the display_format of this GetMetricsMetadataDto.
+    @volume.setter
+    def volume(self, volume):
+        """Sets the volume of this StockIpo.
 
 
-        :param display_format: The display_format of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param volume: The volume of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._display_format = display_format
+        self._volume = volume
 
     @property
-    def type(self):
-        """Gets the type of this GetMetricsMetadataDto.  # noqa: E501
+    def day_change(self):
+        """Gets the day_change of this StockIpo.  # noqa: E501
 
 
-        :return: The type of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The day_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._type
+        return self._day_change
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this GetMetricsMetadataDto.
+    @day_change.setter
+    def day_change(self, day_change):
+        """Sets the day_change of this StockIpo.
 
 
-        :param type: The type of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param day_change: The day_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._type = type
+        self._day_change = day_change
 
     @property
-    def last_modified(self):
-        """Gets the last_modified of this GetMetricsMetadataDto.  # noqa: E501
+    def week_change(self):
+        """Gets the week_change of this StockIpo.  # noqa: E501
 
 
-        :return: The last_modified of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: int
+        :return: The week_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._last_modified
+        return self._week_change
 
-    @last_modified.setter
-    def last_modified(self, last_modified):
-        """Sets the last_modified of this GetMetricsMetadataDto.
+    @week_change.setter
+    def week_change(self, week_change):
+        """Sets the week_change of this StockIpo.
 
 
-        :param last_modified: The last_modified of this GetMetricsMetadataDto.  # noqa: E501
-        :type: int
+        :param week_change: The week_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._last_modified = last_modified
+        self._week_change = week_change
 
     @property
-    def period_type_default(self):
-        """Gets the period_type_default of this GetMetricsMetadataDto.  # noqa: E501
+    def month_change(self):
+        """Gets the month_change of this StockIpo.  # noqa: E501
 
 
-        :return: The period_type_default of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The month_change of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._period_type_default
+        return self._month_change
 
-    @period_type_default.setter
-    def period_type_default(self, period_type_default):
-        """Sets the period_type_default of this GetMetricsMetadataDto.
+    @month_change.setter
+    def month_change(self, month_change):
+        """Sets the month_change of this StockIpo.
 
 
-        :param period_type_default: The period_type_default of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param month_change: The month_change of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._period_type_default = period_type_default
+        self._month_change = month_change
 
     @property
-    def remarks(self):
-        """Gets the remarks of this GetMetricsMetadataDto.  # noqa: E501
+    def offer_amount(self):
+        """Gets the offer_amount of this StockIpo.  # noqa: E501
 
 
-        :return: The remarks of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The offer_amount of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._remarks
+        return self._offer_amount
 
-    @remarks.setter
-    def remarks(self, remarks):
-        """Sets the remarks of this GetMetricsMetadataDto.
+    @offer_amount.setter
+    def offer_amount(self, offer_amount):
+        """Sets the offer_amount of this StockIpo.
 
 
-        :param remarks: The remarks of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param offer_amount: The offer_amount of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._remarks = remarks
+        self._offer_amount = offer_amount
 
     @property
-    def aliases(self):
-        """Gets the aliases of this GetMetricsMetadataDto.  # noqa: E501
+    def share_count(self):
+        """Gets the share_count of this StockIpo.  # noqa: E501
 
 
-        :return: The aliases of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The share_count of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._aliases
+        return self._share_count
 
-    @aliases.setter
-    def aliases(self, aliases):
-        """Sets the aliases of this GetMetricsMetadataDto.
+    @share_count.setter
+    def share_count(self, share_count):
+        """Sets the share_count of this StockIpo.
 
 
-        :param aliases: The aliases of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param share_count: The share_count of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._aliases = aliases
+        self._share_count = share_count
 
     @property
-    def colorable(self):
-        """Gets the colorable of this GetMetricsMetadataDto.  # noqa: E501
+    def share_count_highest(self):
+        """Gets the share_count_highest of this StockIpo.  # noqa: E501
 
 
-        :return: The colorable of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: bool
+        :return: The share_count_highest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._colorable
+        return self._share_count_highest
 
-    @colorable.setter
-    def colorable(self, colorable):
-        """Sets the colorable of this GetMetricsMetadataDto.
+    @share_count_highest.setter
+    def share_count_highest(self, share_count_highest):
+        """Sets the share_count_highest of this StockIpo.
 
 
-        :param colorable: The colorable of this GetMetricsMetadataDto.  # noqa: E501
-        :type: bool
+        :param share_count_highest: The share_count_highest of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._colorable = colorable
+        self._share_count_highest = share_count_highest
 
     @property
-    def short_description(self):
-        """Gets the short_description of this GetMetricsMetadataDto.  # noqa: E501
+    def share_count_lowest(self):
+        """Gets the share_count_lowest of this StockIpo.  # noqa: E501
 
 
-        :return: The short_description of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: str
+        :return: The share_count_lowest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._short_description
+        return self._share_count_lowest
 
-    @short_description.setter
-    def short_description(self, short_description):
-        """Sets the short_description of this GetMetricsMetadataDto.
+    @share_count_lowest.setter
+    def share_count_lowest(self, share_count_lowest):
+        """Sets the share_count_lowest of this StockIpo.
 
 
-        :param short_description: The short_description of this GetMetricsMetadataDto.  # noqa: E501
-        :type: str
+        :param share_count_lowest: The share_count_lowest of this StockIpo.  # noqa: E501
+        :type: float
+        """
+
+        self._share_count_lowest = share_count_lowest
+
+    @property
+    def share_price(self):
+        """Gets the share_price of this StockIpo.  # noqa: E501
+
+
+        :return: The share_price of this StockIpo.  # noqa: E501
+        :rtype: float
         """
+        return self._share_price
+
+    @share_price.setter
+    def share_price(self, share_price):
+        """Sets the share_price of this StockIpo.
 
-        self._short_description = short_description
+
+        :param share_price: The share_price of this StockIpo.  # noqa: E501
+        :type: float
+        """
+
+        self._share_price = share_price
 
     @property
-    def soft_delete(self):
-        """Gets the soft_delete of this GetMetricsMetadataDto.  # noqa: E501
+    def share_price_highest(self):
+        """Gets the share_price_highest of this StockIpo.  # noqa: E501
 
 
-        :return: The soft_delete of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: bool
+        :return: The share_price_highest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._soft_delete
+        return self._share_price_highest
 
-    @soft_delete.setter
-    def soft_delete(self, soft_delete):
-        """Sets the soft_delete of this GetMetricsMetadataDto.
+    @share_price_highest.setter
+    def share_price_highest(self, share_price_highest):
+        """Sets the share_price_highest of this StockIpo.
 
 
-        :param soft_delete: The soft_delete of this GetMetricsMetadataDto.  # noqa: E501
-        :type: bool
+        :param share_price_highest: The share_price_highest of this StockIpo.  # noqa: E501
+        :type: float
         """
 
-        self._soft_delete = soft_delete
+        self._share_price_highest = share_price_highest
 
     @property
-    def screening_conditions(self):
-        """Gets the screening_conditions of this GetMetricsMetadataDto.  # noqa: E501
+    def share_price_lowest(self):
+        """Gets the share_price_lowest of this StockIpo.  # noqa: E501
 
 
-        :return: The screening_conditions of this GetMetricsMetadataDto.  # noqa: E501
-        :rtype: list[ScreeningCondition]
+        :return: The share_price_lowest of this StockIpo.  # noqa: E501
+        :rtype: float
         """
-        return self._screening_conditions
+        return self._share_price_lowest
 
-    @screening_conditions.setter
-    def screening_conditions(self, screening_conditions):
-        """Sets the screening_conditions of this GetMetricsMetadataDto.
+    @share_price_lowest.setter
+    def share_price_lowest(self, share_price_lowest):
+        """Sets the share_price_lowest of this StockIpo.
 
 
-        :param screening_conditions: The screening_conditions of this GetMetricsMetadataDto.  # noqa: E501
-        :type: list[ScreeningCondition]
+        :param share_price_lowest: The share_price_lowest of this StockIpo.  # noqa: E501
+        :type: float
+        """
+
+        self._share_price_lowest = share_price_lowest
+
+    @property
+    def announcement_url(self):
+        """Gets the announcement_url of this StockIpo.  # noqa: E501
+
+
+        :return: The announcement_url of this StockIpo.  # noqa: E501
+        :rtype: str
+        """
+        return self._announcement_url
+
+    @announcement_url.setter
+    def announcement_url(self, announcement_url):
+        """Sets the announcement_url of this StockIpo.
+
+
+        :param announcement_url: The announcement_url of this StockIpo.  # noqa: E501
+        :type: str
         """
 
-        self._screening_conditions = screening_conditions
+        self._announcement_url = announcement_url
 
     @property
-    def internal_comment(self):
-        """Gets the internal_comment of this GetMetricsMetadataDto.  # noqa: E501
+    def sec_report_url(self):
+        """Gets the sec_report_url of this StockIpo.  # noqa: E501
 
 
-        :return: The internal_comment of this GetMetricsMetadataDto.  # noqa: E501
+        :return: The sec_report_url of this StockIpo.  # noqa: E501
         :rtype: str
         """
-        return self._internal_comment
+        return self._sec_report_url
 
-    @internal_comment.setter
-    def internal_comment(self, internal_comment):
-        """Sets the internal_comment of this GetMetricsMetadataDto.
+    @sec_report_url.setter
+    def sec_report_url(self, sec_report_url):
+        """Sets the sec_report_url of this StockIpo.
 
 
-        :param internal_comment: The internal_comment of this GetMetricsMetadataDto.  # noqa: E501
+        :param sec_report_url: The sec_report_url of this StockIpo.  # noqa: E501
         :type: str
         """
 
-        self._internal_comment = internal_comment
+        self._sec_report_url = sec_report_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -522,15 +574,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GetMetricsMetadataDto, dict):
+        if issubclass(StockIpo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -538,15 +590,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GetMetricsMetadataDto):
+        if not isinstance(other, StockIpo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/get_screens_by_user_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/get_watchlists_by_user_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GetScreensByUserDto(object):
+class GetWatchlistsByUserDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'user_id': 'str',
-        'screens': 'list[ScreenDto]'
+        'watchlists': 'list[WatchlistDto]'
     }
 
     attribute_map = {
         'user_id': 'UserId',
-        'screens': 'Screens'
+        'watchlists': 'Watchlists'
     }
 
-    def __init__(self, user_id=None, screens=None):  # noqa: E501
-        """GetScreensByUserDto - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, user_id=None, watchlists=None):  # noqa: E501
+        """GetWatchlistsByUserDto - a model defined in Swagger"""  # noqa: E501
         self._user_id = None
-        self._screens = None
+        self._watchlists = None
         self.discriminator = None
         if user_id is not None:
             self.user_id = user_id
-        if screens is not None:
-            self.screens = screens
+        if watchlists is not None:
+            self.watchlists = watchlists
 
     @property
     def user_id(self):
-        """Gets the user_id of this GetScreensByUserDto.  # noqa: E501
+        """Gets the user_id of this GetWatchlistsByUserDto.  # noqa: E501
 
 
-        :return: The user_id of this GetScreensByUserDto.  # noqa: E501
+        :return: The user_id of this GetWatchlistsByUserDto.  # noqa: E501
         :rtype: str
         """
         return self._user_id
 
     @user_id.setter
     def user_id(self, user_id):
-        """Sets the user_id of this GetScreensByUserDto.
+        """Sets the user_id of this GetWatchlistsByUserDto.
 
 
-        :param user_id: The user_id of this GetScreensByUserDto.  # noqa: E501
+        :param user_id: The user_id of this GetWatchlistsByUserDto.  # noqa: E501
         :type: str
         """
 
         self._user_id = user_id
 
     @property
-    def screens(self):
-        """Gets the screens of this GetScreensByUserDto.  # noqa: E501
+    def watchlists(self):
+        """Gets the watchlists of this GetWatchlistsByUserDto.  # noqa: E501
 
 
-        :return: The screens of this GetScreensByUserDto.  # noqa: E501
-        :rtype: list[ScreenDto]
+        :return: The watchlists of this GetWatchlistsByUserDto.  # noqa: E501
+        :rtype: list[WatchlistDto]
         """
-        return self._screens
+        return self._watchlists
 
-    @screens.setter
-    def screens(self, screens):
-        """Sets the screens of this GetScreensByUserDto.
+    @watchlists.setter
+    def watchlists(self, watchlists):
+        """Sets the watchlists of this GetWatchlistsByUserDto.
 
 
-        :param screens: The screens of this GetScreensByUserDto.  # noqa: E501
-        :type: list[ScreenDto]
+        :param watchlists: The watchlists of this GetWatchlistsByUserDto.  # noqa: E501
+        :type: list[WatchlistDto]
         """
 
-        self._screens = screens
+        self._watchlists = watchlists
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GetScreensByUserDto, dict):
+        if issubclass(GetWatchlistsByUserDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GetScreensByUserDto):
+        if not isinstance(other, GetWatchlistsByUserDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/get_watchlists_by_user_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_daily_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_daily_metrics_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_financial_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_financial_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_indicator_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_indicator_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_metadata_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,87 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class HistoricalMetadataMetricsDto(object):
+class StockPopularityDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'dict(str, dict(str, list[HistoricalMetricValueDto]))',
-        'metadata': 'list[MetricsMetadataResponseDto]'
+        'ticker': 'str',
+        'score': 'float',
+        'rank': 'int'
     }
 
     attribute_map = {
-        'data': 'Data',
-        'metadata': 'Metadata'
+        'ticker': 'Ticker',
+        'score': 'Score',
+        'rank': 'Rank'
     }
 
-    def __init__(self, data=None, metadata=None):  # noqa: E501
-        """HistoricalMetadataMetricsDto - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._metadata = None
+    def __init__(self, ticker=None, score=None, rank=None):  # noqa: E501
+        """StockPopularityDto - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._score = None
+        self._rank = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        if metadata is not None:
-            self.metadata = metadata
+        if ticker is not None:
+            self.ticker = ticker
+        if score is not None:
+            self.score = score
+        if rank is not None:
+            self.rank = rank
 
     @property
-    def data(self):
-        """Gets the data of this HistoricalMetadataMetricsDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this StockPopularityDto.  # noqa: E501
 
 
-        :return: The data of this HistoricalMetadataMetricsDto.  # noqa: E501
-        :rtype: dict(str, dict(str, list[HistoricalMetricValueDto]))
+        :return: The ticker of this StockPopularityDto.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self._ticker
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this HistoricalMetadataMetricsDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this StockPopularityDto.
 
 
-        :param data: The data of this HistoricalMetadataMetricsDto.  # noqa: E501
-        :type: dict(str, dict(str, list[HistoricalMetricValueDto]))
+        :param ticker: The ticker of this StockPopularityDto.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self._ticker = ticker
 
     @property
-    def metadata(self):
-        """Gets the metadata of this HistoricalMetadataMetricsDto.  # noqa: E501
+    def score(self):
+        """Gets the score of this StockPopularityDto.  # noqa: E501
 
 
-        :return: The metadata of this HistoricalMetadataMetricsDto.  # noqa: E501
-        :rtype: list[MetricsMetadataResponseDto]
+        :return: The score of this StockPopularityDto.  # noqa: E501
+        :rtype: float
         """
-        return self._metadata
+        return self._score
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this HistoricalMetadataMetricsDto.
+    @score.setter
+    def score(self, score):
+        """Sets the score of this StockPopularityDto.
 
 
-        :param metadata: The metadata of this HistoricalMetadataMetricsDto.  # noqa: E501
-        :type: list[MetricsMetadataResponseDto]
+        :param score: The score of this StockPopularityDto.  # noqa: E501
+        :type: float
         """
 
-        self._metadata = metadata
+        self._score = score
+
+    @property
+    def rank(self):
+        """Gets the rank of this StockPopularityDto.  # noqa: E501
+
+
+        :return: The rank of this StockPopularityDto.  # noqa: E501
+        :rtype: int
+        """
+        return self._rank
+
+    @rank.setter
+    def rank(self, rank):
+        """Sets the rank of this StockPopularityDto.
+
+
+        :param rank: The rank of this StockPopularityDto.  # noqa: E501
+        :type: int
+        """
+
+        self._rank = rank
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(HistoricalMetadataMetricsDto, dict):
+        if issubclass(StockPopularityDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HistoricalMetadataMetricsDto):
+        if not isinstance(other, StockPopularityDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_metric_value_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/value_metrics_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,149 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class HistoricalMetricValueDto(object):
+class ValueMetricsDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'period': 'str',
-        'value': 'str',
-        'period_date_time': 'datetime'
+        'ticker': 'str',
+        'timestamp': 'int',
+        'high52': 'float',
+        'low52': 'float'
     }
 
     attribute_map = {
-        'period': 'Period',
-        'value': 'Value',
-        'period_date_time': 'PeriodDateTime'
+        'ticker': 'Ticker',
+        'timestamp': 'Timestamp',
+        'high52': 'High52',
+        'low52': 'Low52'
     }
 
-    def __init__(self, period=None, value=None, period_date_time=None):  # noqa: E501
-        """HistoricalMetricValueDto - a model defined in Swagger"""  # noqa: E501
-        self._period = None
-        self._value = None
-        self._period_date_time = None
+    def __init__(self, ticker=None, timestamp=None, high52=None, low52=None):  # noqa: E501
+        """ValueMetricsDto - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._timestamp = None
+        self._high52 = None
+        self._low52 = None
         self.discriminator = None
-        if period is not None:
-            self.period = period
-        if value is not None:
-            self.value = value
-        if period_date_time is not None:
-            self.period_date_time = period_date_time
+        if ticker is not None:
+            self.ticker = ticker
+        if timestamp is not None:
+            self.timestamp = timestamp
+        if high52 is not None:
+            self.high52 = high52
+        if low52 is not None:
+            self.low52 = low52
 
     @property
-    def period(self):
-        """Gets the period of this HistoricalMetricValueDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this ValueMetricsDto.  # noqa: E501
 
 
-        :return: The period of this HistoricalMetricValueDto.  # noqa: E501
+        :return: The ticker of this ValueMetricsDto.  # noqa: E501
         :rtype: str
         """
-        return self._period
+        return self._ticker
 
-    @period.setter
-    def period(self, period):
-        """Sets the period of this HistoricalMetricValueDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this ValueMetricsDto.
 
 
-        :param period: The period of this HistoricalMetricValueDto.  # noqa: E501
+        :param ticker: The ticker of this ValueMetricsDto.  # noqa: E501
         :type: str
         """
 
-        self._period = period
+        self._ticker = ticker
 
     @property
-    def value(self):
-        """Gets the value of this HistoricalMetricValueDto.  # noqa: E501
+    def timestamp(self):
+        """Gets the timestamp of this ValueMetricsDto.  # noqa: E501
 
 
-        :return: The value of this HistoricalMetricValueDto.  # noqa: E501
-        :rtype: str
+        :return: The timestamp of this ValueMetricsDto.  # noqa: E501
+        :rtype: int
         """
-        return self._value
+        return self._timestamp
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this HistoricalMetricValueDto.
+    @timestamp.setter
+    def timestamp(self, timestamp):
+        """Sets the timestamp of this ValueMetricsDto.
 
 
-        :param value: The value of this HistoricalMetricValueDto.  # noqa: E501
-        :type: str
+        :param timestamp: The timestamp of this ValueMetricsDto.  # noqa: E501
+        :type: int
+        """
+
+        self._timestamp = timestamp
+
+    @property
+    def high52(self):
+        """Gets the high52 of this ValueMetricsDto.  # noqa: E501
+
+
+        :return: The high52 of this ValueMetricsDto.  # noqa: E501
+        :rtype: float
+        """
+        return self._high52
+
+    @high52.setter
+    def high52(self, high52):
+        """Sets the high52 of this ValueMetricsDto.
+
+
+        :param high52: The high52 of this ValueMetricsDto.  # noqa: E501
+        :type: float
         """
 
-        self._value = value
+        self._high52 = high52
 
     @property
-    def period_date_time(self):
-        """Gets the period_date_time of this HistoricalMetricValueDto.  # noqa: E501
+    def low52(self):
+        """Gets the low52 of this ValueMetricsDto.  # noqa: E501
 
 
-        :return: The period_date_time of this HistoricalMetricValueDto.  # noqa: E501
-        :rtype: datetime
+        :return: The low52 of this ValueMetricsDto.  # noqa: E501
+        :rtype: float
         """
-        return self._period_date_time
+        return self._low52
 
-    @period_date_time.setter
-    def period_date_time(self, period_date_time):
-        """Sets the period_date_time of this HistoricalMetricValueDto.
+    @low52.setter
+    def low52(self, low52):
+        """Sets the low52 of this ValueMetricsDto.
 
 
-        :param period_date_time: The period_date_time of this HistoricalMetricValueDto.  # noqa: E501
-        :type: datetime
+        :param low52: The low52 of this ValueMetricsDto.  # noqa: E501
+        :type: float
         """
 
-        self._period_date_time = period_date_time
+        self._low52 = low52
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(HistoricalMetricValueDto, dict):
+        if issubclass(ValueMetricsDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HistoricalMetricValueDto):
+        if not isinstance(other, ValueMetricsDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_return.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_return.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_returns_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_returns_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/historical_value_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_value_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/history_length.py` & `investor8-sdk-1.1.9/investor8_sdk/models/req_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class HistoryLength(object):
+class ReqType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    _4 = "4"
-    _8 = "8"
-    _16 = "16"
+    _1 = "1"
+    _2 = "2"
+    _3 = "3"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """HistoryLength - a model defined in Swagger"""  # noqa: E501
+        """ReqType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(HistoryLength, dict):
+        if issubclass(ReqType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HistoryLength):
+        if not isinstance(other, ReqType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_check_version_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_version.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class I8TerminalVersion(object):
+class I8TerminalVersionDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'min_version_support': 'MinVersionSupport',
         'latest_version': 'LatestVersion'
     }
 
     def __init__(self, min_version_support=None, latest_version=None):  # noqa: E501
-        """I8TerminalVersion - a model defined in Swagger"""  # noqa: E501
+        """I8TerminalVersionDto - a model defined in Swagger"""  # noqa: E501
         self._min_version_support = None
         self._latest_version = None
         self.discriminator = None
         if min_version_support is not None:
             self.min_version_support = min_version_support
         if latest_version is not None:
             self.latest_version = latest_version
 
     @property
     def min_version_support(self):
-        """Gets the min_version_support of this I8TerminalVersion.  # noqa: E501
+        """Gets the min_version_support of this I8TerminalVersionDto.  # noqa: E501
 
 
-        :return: The min_version_support of this I8TerminalVersion.  # noqa: E501
+        :return: The min_version_support of this I8TerminalVersionDto.  # noqa: E501
         :rtype: str
         """
         return self._min_version_support
 
     @min_version_support.setter
     def min_version_support(self, min_version_support):
-        """Sets the min_version_support of this I8TerminalVersion.
+        """Sets the min_version_support of this I8TerminalVersionDto.
 
 
-        :param min_version_support: The min_version_support of this I8TerminalVersion.  # noqa: E501
+        :param min_version_support: The min_version_support of this I8TerminalVersionDto.  # noqa: E501
         :type: str
         """
 
         self._min_version_support = min_version_support
 
     @property
     def latest_version(self):
-        """Gets the latest_version of this I8TerminalVersion.  # noqa: E501
+        """Gets the latest_version of this I8TerminalVersionDto.  # noqa: E501
 
 
-        :return: The latest_version of this I8TerminalVersion.  # noqa: E501
+        :return: The latest_version of this I8TerminalVersionDto.  # noqa: E501
         :rtype: str
         """
         return self._latest_version
 
     @latest_version.setter
     def latest_version(self, latest_version):
-        """Sets the latest_version of this I8TerminalVersion.
+        """Sets the latest_version of this I8TerminalVersionDto.
 
 
-        :param latest_version: The latest_version of this I8TerminalVersion.  # noqa: E501
+        :param latest_version: The latest_version of this I8TerminalVersionDto.  # noqa: E501
         :type: str
         """
 
         self._latest_version = latest_version
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(I8TerminalVersion, dict):
+        if issubclass(I8TerminalVersionDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, I8TerminalVersion):
+        if not isinstance(other, I8TerminalVersionDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/i8_terminal_version_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class I8TerminalVersionDto(object):
+class I8TerminalVersion(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'min_version_support': 'MinVersionSupport',
         'latest_version': 'LatestVersion'
     }
 
     def __init__(self, min_version_support=None, latest_version=None):  # noqa: E501
-        """I8TerminalVersionDto - a model defined in Swagger"""  # noqa: E501
+        """I8TerminalVersion - a model defined in Swagger"""  # noqa: E501
         self._min_version_support = None
         self._latest_version = None
         self.discriminator = None
         if min_version_support is not None:
             self.min_version_support = min_version_support
         if latest_version is not None:
             self.latest_version = latest_version
 
     @property
     def min_version_support(self):
-        """Gets the min_version_support of this I8TerminalVersionDto.  # noqa: E501
+        """Gets the min_version_support of this I8TerminalVersion.  # noqa: E501
 
 
-        :return: The min_version_support of this I8TerminalVersionDto.  # noqa: E501
+        :return: The min_version_support of this I8TerminalVersion.  # noqa: E501
         :rtype: str
         """
         return self._min_version_support
 
     @min_version_support.setter
     def min_version_support(self, min_version_support):
-        """Sets the min_version_support of this I8TerminalVersionDto.
+        """Sets the min_version_support of this I8TerminalVersion.
 
 
-        :param min_version_support: The min_version_support of this I8TerminalVersionDto.  # noqa: E501
+        :param min_version_support: The min_version_support of this I8TerminalVersion.  # noqa: E501
         :type: str
         """
 
         self._min_version_support = min_version_support
 
     @property
     def latest_version(self):
-        """Gets the latest_version of this I8TerminalVersionDto.  # noqa: E501
+        """Gets the latest_version of this I8TerminalVersion.  # noqa: E501
 
 
-        :return: The latest_version of this I8TerminalVersionDto.  # noqa: E501
+        :return: The latest_version of this I8TerminalVersion.  # noqa: E501
         :rtype: str
         """
         return self._latest_version
 
     @latest_version.setter
     def latest_version(self, latest_version):
-        """Sets the latest_version of this I8TerminalVersionDto.
+        """Sets the latest_version of this I8TerminalVersion.
 
 
-        :param latest_version: The latest_version of this I8TerminalVersionDto.  # noqa: E501
+        :param latest_version: The latest_version of this I8TerminalVersion.  # noqa: E501
         :type: str
         """
 
         self._latest_version = latest_version
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(I8TerminalVersionDto, dict):
+        if issubclass(I8TerminalVersion, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, I8TerminalVersionDto):
+        if not isinstance(other, I8TerminalVersion):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financial_metrics_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/latest_financials_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_with_growth_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/latest_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_price_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/list_exchange_sector_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/log_terminal_usage.py` & `investor8-sdk-1.1.9/investor8_sdk/models/log_terminal_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/login_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/login_user_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/login_with_code_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/login_with_code_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/market_highlight.py` & `investor8-sdk-1.1.9/investor8-sdk/models/market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/market_highlight_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/market_highlight_status.py` & `investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/metadata_properties_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metadata_properties_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/metric_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/metrics_by_period_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/return_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,227 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class MetricsByPeriodDto(object):
+class ReturnMetrics(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'symbol': 'str',
-        'metric': 'str',
-        'value': 'str',
-        'value_numeric': 'float',
-        'period': 'str',
-        'period_type': 'str',
-        'period_date_time': 'datetime'
+        'history_length': 'HistoryLength',
+        'min': 'float',
+        'max': 'float',
+        'avg': 'float',
+        'std': 'float',
+        'positive_return_prob': 'float',
+        'expected_return': 'float'
     }
 
     attribute_map = {
-        'id': 'Id',
-        'symbol': 'Symbol',
-        'metric': 'Metric',
-        'value': 'Value',
-        'value_numeric': 'ValueNumeric',
-        'period': 'Period',
-        'period_type': 'PeriodType',
-        'period_date_time': 'PeriodDateTime'
+        'history_length': 'HistoryLength',
+        'min': 'Min',
+        'max': 'Max',
+        'avg': 'Avg',
+        'std': 'Std',
+        'positive_return_prob': 'PositiveReturnProb',
+        'expected_return': 'ExpectedReturn'
     }
 
-    def __init__(self, id=None, symbol=None, metric=None, value=None, value_numeric=None, period=None, period_type=None, period_date_time=None):  # noqa: E501
-        """MetricsByPeriodDto - a model defined in Swagger"""  # noqa: E501
-        self._id = None
-        self._symbol = None
-        self._metric = None
-        self._value = None
-        self._value_numeric = None
-        self._period = None
-        self._period_type = None
-        self._period_date_time = None
+    def __init__(self, history_length=None, min=None, max=None, avg=None, std=None, positive_return_prob=None, expected_return=None):  # noqa: E501
+        """ReturnMetrics - a model defined in Swagger"""  # noqa: E501
+        self._history_length = None
+        self._min = None
+        self._max = None
+        self._avg = None
+        self._std = None
+        self._positive_return_prob = None
+        self._expected_return = None
         self.discriminator = None
-        if id is not None:
-            self.id = id
-        if symbol is not None:
-            self.symbol = symbol
-        if metric is not None:
-            self.metric = metric
-        if value is not None:
-            self.value = value
-        if value_numeric is not None:
-            self.value_numeric = value_numeric
-        if period is not None:
-            self.period = period
-        if period_type is not None:
-            self.period_type = period_type
-        if period_date_time is not None:
-            self.period_date_time = period_date_time
+        if history_length is not None:
+            self.history_length = history_length
+        if min is not None:
+            self.min = min
+        if max is not None:
+            self.max = max
+        if avg is not None:
+            self.avg = avg
+        if std is not None:
+            self.std = std
+        if positive_return_prob is not None:
+            self.positive_return_prob = positive_return_prob
+        if expected_return is not None:
+            self.expected_return = expected_return
 
     @property
-    def id(self):
-        """Gets the id of this MetricsByPeriodDto.  # noqa: E501
+    def history_length(self):
+        """Gets the history_length of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The id of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
+        :return: The history_length of this ReturnMetrics.  # noqa: E501
+        :rtype: HistoryLength
         """
-        return self._id
+        return self._history_length
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this MetricsByPeriodDto.
+    @history_length.setter
+    def history_length(self, history_length):
+        """Sets the history_length of this ReturnMetrics.
 
 
-        :param id: The id of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
+        :param history_length: The history_length of this ReturnMetrics.  # noqa: E501
+        :type: HistoryLength
         """
 
-        self._id = id
+        self._history_length = history_length
 
     @property
-    def symbol(self):
-        """Gets the symbol of this MetricsByPeriodDto.  # noqa: E501
+    def min(self):
+        """Gets the min of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The symbol of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
-        """
-        return self._symbol
-
-    @symbol.setter
-    def symbol(self, symbol):
-        """Sets the symbol of this MetricsByPeriodDto.
-
-
-        :param symbol: The symbol of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
-        """
-
-        self._symbol = symbol
-
-    @property
-    def metric(self):
-        """Gets the metric of this MetricsByPeriodDto.  # noqa: E501
-
-
-        :return: The metric of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
+        :return: The min of this ReturnMetrics.  # noqa: E501
+        :rtype: float
         """
-        return self._metric
+        return self._min
 
-    @metric.setter
-    def metric(self, metric):
-        """Sets the metric of this MetricsByPeriodDto.
+    @min.setter
+    def min(self, min):
+        """Sets the min of this ReturnMetrics.
 
 
-        :param metric: The metric of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
+        :param min: The min of this ReturnMetrics.  # noqa: E501
+        :type: float
         """
 
-        self._metric = metric
+        self._min = min
 
     @property
-    def value(self):
-        """Gets the value of this MetricsByPeriodDto.  # noqa: E501
+    def max(self):
+        """Gets the max of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The value of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
+        :return: The max of this ReturnMetrics.  # noqa: E501
+        :rtype: float
         """
-        return self._value
+        return self._max
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this MetricsByPeriodDto.
+    @max.setter
+    def max(self, max):
+        """Sets the max of this ReturnMetrics.
 
 
-        :param value: The value of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
+        :param max: The max of this ReturnMetrics.  # noqa: E501
+        :type: float
         """
 
-        self._value = value
+        self._max = max
 
     @property
-    def value_numeric(self):
-        """Gets the value_numeric of this MetricsByPeriodDto.  # noqa: E501
+    def avg(self):
+        """Gets the avg of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The value_numeric of this MetricsByPeriodDto.  # noqa: E501
+        :return: The avg of this ReturnMetrics.  # noqa: E501
         :rtype: float
         """
-        return self._value_numeric
+        return self._avg
 
-    @value_numeric.setter
-    def value_numeric(self, value_numeric):
-        """Sets the value_numeric of this MetricsByPeriodDto.
+    @avg.setter
+    def avg(self, avg):
+        """Sets the avg of this ReturnMetrics.
 
 
-        :param value_numeric: The value_numeric of this MetricsByPeriodDto.  # noqa: E501
+        :param avg: The avg of this ReturnMetrics.  # noqa: E501
         :type: float
         """
 
-        self._value_numeric = value_numeric
+        self._avg = avg
 
     @property
-    def period(self):
-        """Gets the period of this MetricsByPeriodDto.  # noqa: E501
+    def std(self):
+        """Gets the std of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The period of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
+        :return: The std of this ReturnMetrics.  # noqa: E501
+        :rtype: float
         """
-        return self._period
+        return self._std
 
-    @period.setter
-    def period(self, period):
-        """Sets the period of this MetricsByPeriodDto.
+    @std.setter
+    def std(self, std):
+        """Sets the std of this ReturnMetrics.
 
 
-        :param period: The period of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
+        :param std: The std of this ReturnMetrics.  # noqa: E501
+        :type: float
         """
 
-        self._period = period
+        self._std = std
 
     @property
-    def period_type(self):
-        """Gets the period_type of this MetricsByPeriodDto.  # noqa: E501
+    def positive_return_prob(self):
+        """Gets the positive_return_prob of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The period_type of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: str
+        :return: The positive_return_prob of this ReturnMetrics.  # noqa: E501
+        :rtype: float
         """
-        return self._period_type
+        return self._positive_return_prob
 
-    @period_type.setter
-    def period_type(self, period_type):
-        """Sets the period_type of this MetricsByPeriodDto.
+    @positive_return_prob.setter
+    def positive_return_prob(self, positive_return_prob):
+        """Sets the positive_return_prob of this ReturnMetrics.
 
 
-        :param period_type: The period_type of this MetricsByPeriodDto.  # noqa: E501
-        :type: str
+        :param positive_return_prob: The positive_return_prob of this ReturnMetrics.  # noqa: E501
+        :type: float
         """
 
-        self._period_type = period_type
+        self._positive_return_prob = positive_return_prob
 
     @property
-    def period_date_time(self):
-        """Gets the period_date_time of this MetricsByPeriodDto.  # noqa: E501
+    def expected_return(self):
+        """Gets the expected_return of this ReturnMetrics.  # noqa: E501
 
 
-        :return: The period_date_time of this MetricsByPeriodDto.  # noqa: E501
-        :rtype: datetime
+        :return: The expected_return of this ReturnMetrics.  # noqa: E501
+        :rtype: float
         """
-        return self._period_date_time
+        return self._expected_return
 
-    @period_date_time.setter
-    def period_date_time(self, period_date_time):
-        """Sets the period_date_time of this MetricsByPeriodDto.
+    @expected_return.setter
+    def expected_return(self, expected_return):
+        """Sets the expected_return of this ReturnMetrics.
 
 
-        :param period_date_time: The period_date_time of this MetricsByPeriodDto.  # noqa: E501
-        :type: datetime
+        :param expected_return: The expected_return of this ReturnMetrics.  # noqa: E501
+        :type: float
         """
 
-        self._period_date_time = period_date_time
+        self._expected_return = expected_return
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -262,15 +236,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(MetricsByPeriodDto, dict):
+        if issubclass(ReturnMetrics, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -278,15 +252,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MetricsByPeriodDto):
+        if not isinstance(other, ReturnMetrics):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/metrics_metadata.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_financial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,461 +1,409 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class MetricsMetadata(object):
+class StockFinancial(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'metric_name': 'str',
-        'display_name': 'str',
-        'description': 'str',
-        'unit': 'str',
-        'categories': 'list[str]',
-        'data_format': 'str',
-        'display_format': 'str',
-        'type': 'str',
-        'last_modified': 'int',
-        'period_type_default': 'str',
-        'remarks': 'str',
-        'screening_conditions': 'list[ScreeningCondition]',
-        'internal_comment': 'str',
-        'aliases': 'str',
-        'colorable': 'bool',
-        'id': 'str'
+        'id': 'str',
+        'fyq': 'str',
+        'operating_revenue': 'float',
+        'total_revenue': 'float',
+        'total_grossprofit': 'float',
+        'other_income': 'float',
+        'net_income': 'float',
+        'basic_eps': 'float',
+        'diluted_eps': 'float',
+        'dividend_per_share': 'float',
+        'filing_date': 'int',
+        'adjusted_basic_eps': 'float',
+        'year': 'int',
+        'fiscal_quarter': 'int'
     }
 
     attribute_map = {
-        'metric_name': 'MetricName',
-        'display_name': 'DisplayName',
-        'description': 'Description',
-        'unit': 'Unit',
-        'categories': 'Categories',
-        'data_format': 'DataFormat',
-        'display_format': 'DisplayFormat',
-        'type': 'Type',
-        'last_modified': 'LastModified',
-        'period_type_default': 'PeriodTypeDefault',
-        'remarks': 'Remarks',
-        'screening_conditions': 'ScreeningConditions',
-        'internal_comment': 'InternalComment',
-        'aliases': 'Aliases',
-        'colorable': 'Colorable',
-        'id': 'Id'
+        'id': 'Id',
+        'fyq': 'FYQ',
+        'operating_revenue': 'OperatingRevenue',
+        'total_revenue': 'TotalRevenue',
+        'total_grossprofit': 'TotalGrossprofit',
+        'other_income': 'OtherIncome',
+        'net_income': 'NetIncome',
+        'basic_eps': 'BasicEps',
+        'diluted_eps': 'DilutedEps',
+        'dividend_per_share': 'DividendPerShare',
+        'filing_date': 'Filing_Date',
+        'adjusted_basic_eps': 'AdjustedBasicEps',
+        'year': 'Year',
+        'fiscal_quarter': 'FiscalQuarter'
     }
 
-    def __init__(self, metric_name=None, display_name=None, description=None, unit=None, categories=None, data_format=None, display_format=None, type=None, last_modified=None, period_type_default=None, remarks=None, screening_conditions=None, internal_comment=None, aliases=None, colorable=None, id=None):  # noqa: E501
-        """MetricsMetadata - a model defined in Swagger"""  # noqa: E501
-        self._metric_name = None
-        self._display_name = None
-        self._description = None
-        self._unit = None
-        self._categories = None
-        self._data_format = None
-        self._display_format = None
-        self._type = None
-        self._last_modified = None
-        self._period_type_default = None
-        self._remarks = None
-        self._screening_conditions = None
-        self._internal_comment = None
-        self._aliases = None
-        self._colorable = None
+    def __init__(self, id=None, fyq=None, operating_revenue=None, total_revenue=None, total_grossprofit=None, other_income=None, net_income=None, basic_eps=None, diluted_eps=None, dividend_per_share=None, filing_date=None, adjusted_basic_eps=None, year=None, fiscal_quarter=None):  # noqa: E501
+        """StockFinancial - a model defined in Swagger"""  # noqa: E501
         self._id = None
+        self._fyq = None
+        self._operating_revenue = None
+        self._total_revenue = None
+        self._total_grossprofit = None
+        self._other_income = None
+        self._net_income = None
+        self._basic_eps = None
+        self._diluted_eps = None
+        self._dividend_per_share = None
+        self._filing_date = None
+        self._adjusted_basic_eps = None
+        self._year = None
+        self._fiscal_quarter = None
         self.discriminator = None
-        if metric_name is not None:
-            self.metric_name = metric_name
-        if display_name is not None:
-            self.display_name = display_name
-        if description is not None:
-            self.description = description
-        if unit is not None:
-            self.unit = unit
-        if categories is not None:
-            self.categories = categories
-        if data_format is not None:
-            self.data_format = data_format
-        if display_format is not None:
-            self.display_format = display_format
-        if type is not None:
-            self.type = type
-        if last_modified is not None:
-            self.last_modified = last_modified
-        if period_type_default is not None:
-            self.period_type_default = period_type_default
-        if remarks is not None:
-            self.remarks = remarks
-        if screening_conditions is not None:
-            self.screening_conditions = screening_conditions
-        if internal_comment is not None:
-            self.internal_comment = internal_comment
-        if aliases is not None:
-            self.aliases = aliases
-        if colorable is not None:
-            self.colorable = colorable
         if id is not None:
             self.id = id
+        if fyq is not None:
+            self.fyq = fyq
+        if operating_revenue is not None:
+            self.operating_revenue = operating_revenue
+        if total_revenue is not None:
+            self.total_revenue = total_revenue
+        if total_grossprofit is not None:
+            self.total_grossprofit = total_grossprofit
+        if other_income is not None:
+            self.other_income = other_income
+        if net_income is not None:
+            self.net_income = net_income
+        if basic_eps is not None:
+            self.basic_eps = basic_eps
+        if diluted_eps is not None:
+            self.diluted_eps = diluted_eps
+        if dividend_per_share is not None:
+            self.dividend_per_share = dividend_per_share
+        if filing_date is not None:
+            self.filing_date = filing_date
+        if adjusted_basic_eps is not None:
+            self.adjusted_basic_eps = adjusted_basic_eps
+        if year is not None:
+            self.year = year
+        if fiscal_quarter is not None:
+            self.fiscal_quarter = fiscal_quarter
 
     @property
-    def metric_name(self):
-        """Gets the metric_name of this MetricsMetadata.  # noqa: E501
-
-
-        :return: The metric_name of this MetricsMetadata.  # noqa: E501
-        :rtype: str
-        """
-        return self._metric_name
-
-    @metric_name.setter
-    def metric_name(self, metric_name):
-        """Sets the metric_name of this MetricsMetadata.
-
-
-        :param metric_name: The metric_name of this MetricsMetadata.  # noqa: E501
-        :type: str
-        """
-
-        self._metric_name = metric_name
-
-    @property
-    def display_name(self):
-        """Gets the display_name of this MetricsMetadata.  # noqa: E501
-
-
-        :return: The display_name of this MetricsMetadata.  # noqa: E501
-        :rtype: str
-        """
-        return self._display_name
-
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this MetricsMetadata.
-
-
-        :param display_name: The display_name of this MetricsMetadata.  # noqa: E501
-        :type: str
-        """
-
-        self._display_name = display_name
-
-    @property
-    def description(self):
-        """Gets the description of this MetricsMetadata.  # noqa: E501
+    def id(self):
+        """Gets the id of this StockFinancial.  # noqa: E501
 
 
-        :return: The description of this MetricsMetadata.  # noqa: E501
+        :return: The id of this StockFinancial.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._id
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this MetricsMetadata.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StockFinancial.
 
 
-        :param description: The description of this MetricsMetadata.  # noqa: E501
+        :param id: The id of this StockFinancial.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._id = id
 
     @property
-    def unit(self):
-        """Gets the unit of this MetricsMetadata.  # noqa: E501
+    def fyq(self):
+        """Gets the fyq of this StockFinancial.  # noqa: E501
 
 
-        :return: The unit of this MetricsMetadata.  # noqa: E501
+        :return: The fyq of this StockFinancial.  # noqa: E501
         :rtype: str
         """
-        return self._unit
+        return self._fyq
 
-    @unit.setter
-    def unit(self, unit):
-        """Sets the unit of this MetricsMetadata.
+    @fyq.setter
+    def fyq(self, fyq):
+        """Sets the fyq of this StockFinancial.
 
 
-        :param unit: The unit of this MetricsMetadata.  # noqa: E501
+        :param fyq: The fyq of this StockFinancial.  # noqa: E501
         :type: str
         """
 
-        self._unit = unit
+        self._fyq = fyq
 
     @property
-    def categories(self):
-        """Gets the categories of this MetricsMetadata.  # noqa: E501
+    def operating_revenue(self):
+        """Gets the operating_revenue of this StockFinancial.  # noqa: E501
 
 
-        :return: The categories of this MetricsMetadata.  # noqa: E501
-        :rtype: list[str]
+        :return: The operating_revenue of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._categories
+        return self._operating_revenue
 
-    @categories.setter
-    def categories(self, categories):
-        """Sets the categories of this MetricsMetadata.
+    @operating_revenue.setter
+    def operating_revenue(self, operating_revenue):
+        """Sets the operating_revenue of this StockFinancial.
 
 
-        :param categories: The categories of this MetricsMetadata.  # noqa: E501
-        :type: list[str]
+        :param operating_revenue: The operating_revenue of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._categories = categories
+        self._operating_revenue = operating_revenue
 
     @property
-    def data_format(self):
-        """Gets the data_format of this MetricsMetadata.  # noqa: E501
+    def total_revenue(self):
+        """Gets the total_revenue of this StockFinancial.  # noqa: E501
 
 
-        :return: The data_format of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The total_revenue of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._data_format
+        return self._total_revenue
 
-    @data_format.setter
-    def data_format(self, data_format):
-        """Sets the data_format of this MetricsMetadata.
+    @total_revenue.setter
+    def total_revenue(self, total_revenue):
+        """Sets the total_revenue of this StockFinancial.
 
 
-        :param data_format: The data_format of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param total_revenue: The total_revenue of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._data_format = data_format
+        self._total_revenue = total_revenue
 
     @property
-    def display_format(self):
-        """Gets the display_format of this MetricsMetadata.  # noqa: E501
+    def total_grossprofit(self):
+        """Gets the total_grossprofit of this StockFinancial.  # noqa: E501
 
 
-        :return: The display_format of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The total_grossprofit of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._display_format
+        return self._total_grossprofit
 
-    @display_format.setter
-    def display_format(self, display_format):
-        """Sets the display_format of this MetricsMetadata.
+    @total_grossprofit.setter
+    def total_grossprofit(self, total_grossprofit):
+        """Sets the total_grossprofit of this StockFinancial.
 
 
-        :param display_format: The display_format of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param total_grossprofit: The total_grossprofit of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._display_format = display_format
+        self._total_grossprofit = total_grossprofit
 
     @property
-    def type(self):
-        """Gets the type of this MetricsMetadata.  # noqa: E501
+    def other_income(self):
+        """Gets the other_income of this StockFinancial.  # noqa: E501
 
 
-        :return: The type of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The other_income of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._type
+        return self._other_income
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this MetricsMetadata.
+    @other_income.setter
+    def other_income(self, other_income):
+        """Sets the other_income of this StockFinancial.
 
 
-        :param type: The type of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param other_income: The other_income of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._type = type
+        self._other_income = other_income
 
     @property
-    def last_modified(self):
-        """Gets the last_modified of this MetricsMetadata.  # noqa: E501
+    def net_income(self):
+        """Gets the net_income of this StockFinancial.  # noqa: E501
 
 
-        :return: The last_modified of this MetricsMetadata.  # noqa: E501
-        :rtype: int
+        :return: The net_income of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._last_modified
+        return self._net_income
 
-    @last_modified.setter
-    def last_modified(self, last_modified):
-        """Sets the last_modified of this MetricsMetadata.
+    @net_income.setter
+    def net_income(self, net_income):
+        """Sets the net_income of this StockFinancial.
 
 
-        :param last_modified: The last_modified of this MetricsMetadata.  # noqa: E501
-        :type: int
+        :param net_income: The net_income of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._last_modified = last_modified
+        self._net_income = net_income
 
     @property
-    def period_type_default(self):
-        """Gets the period_type_default of this MetricsMetadata.  # noqa: E501
+    def basic_eps(self):
+        """Gets the basic_eps of this StockFinancial.  # noqa: E501
 
 
-        :return: The period_type_default of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The basic_eps of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._period_type_default
+        return self._basic_eps
 
-    @period_type_default.setter
-    def period_type_default(self, period_type_default):
-        """Sets the period_type_default of this MetricsMetadata.
+    @basic_eps.setter
+    def basic_eps(self, basic_eps):
+        """Sets the basic_eps of this StockFinancial.
 
 
-        :param period_type_default: The period_type_default of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param basic_eps: The basic_eps of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._period_type_default = period_type_default
+        self._basic_eps = basic_eps
 
     @property
-    def remarks(self):
-        """Gets the remarks of this MetricsMetadata.  # noqa: E501
+    def diluted_eps(self):
+        """Gets the diluted_eps of this StockFinancial.  # noqa: E501
 
 
-        :return: The remarks of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The diluted_eps of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._remarks
+        return self._diluted_eps
 
-    @remarks.setter
-    def remarks(self, remarks):
-        """Sets the remarks of this MetricsMetadata.
+    @diluted_eps.setter
+    def diluted_eps(self, diluted_eps):
+        """Sets the diluted_eps of this StockFinancial.
 
 
-        :param remarks: The remarks of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param diluted_eps: The diluted_eps of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._remarks = remarks
+        self._diluted_eps = diluted_eps
 
     @property
-    def screening_conditions(self):
-        """Gets the screening_conditions of this MetricsMetadata.  # noqa: E501
+    def dividend_per_share(self):
+        """Gets the dividend_per_share of this StockFinancial.  # noqa: E501
 
 
-        :return: The screening_conditions of this MetricsMetadata.  # noqa: E501
-        :rtype: list[ScreeningCondition]
+        :return: The dividend_per_share of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._screening_conditions
+        return self._dividend_per_share
 
-    @screening_conditions.setter
-    def screening_conditions(self, screening_conditions):
-        """Sets the screening_conditions of this MetricsMetadata.
+    @dividend_per_share.setter
+    def dividend_per_share(self, dividend_per_share):
+        """Sets the dividend_per_share of this StockFinancial.
 
 
-        :param screening_conditions: The screening_conditions of this MetricsMetadata.  # noqa: E501
-        :type: list[ScreeningCondition]
+        :param dividend_per_share: The dividend_per_share of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._screening_conditions = screening_conditions
+        self._dividend_per_share = dividend_per_share
 
     @property
-    def internal_comment(self):
-        """Gets the internal_comment of this MetricsMetadata.  # noqa: E501
+    def filing_date(self):
+        """Gets the filing_date of this StockFinancial.  # noqa: E501
 
 
-        :return: The internal_comment of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The filing_date of this StockFinancial.  # noqa: E501
+        :rtype: int
         """
-        return self._internal_comment
+        return self._filing_date
 
-    @internal_comment.setter
-    def internal_comment(self, internal_comment):
-        """Sets the internal_comment of this MetricsMetadata.
+    @filing_date.setter
+    def filing_date(self, filing_date):
+        """Sets the filing_date of this StockFinancial.
 
 
-        :param internal_comment: The internal_comment of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param filing_date: The filing_date of this StockFinancial.  # noqa: E501
+        :type: int
         """
 
-        self._internal_comment = internal_comment
+        self._filing_date = filing_date
 
     @property
-    def aliases(self):
-        """Gets the aliases of this MetricsMetadata.  # noqa: E501
+    def adjusted_basic_eps(self):
+        """Gets the adjusted_basic_eps of this StockFinancial.  # noqa: E501
 
 
-        :return: The aliases of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The adjusted_basic_eps of this StockFinancial.  # noqa: E501
+        :rtype: float
         """
-        return self._aliases
+        return self._adjusted_basic_eps
 
-    @aliases.setter
-    def aliases(self, aliases):
-        """Sets the aliases of this MetricsMetadata.
+    @adjusted_basic_eps.setter
+    def adjusted_basic_eps(self, adjusted_basic_eps):
+        """Sets the adjusted_basic_eps of this StockFinancial.
 
 
-        :param aliases: The aliases of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param adjusted_basic_eps: The adjusted_basic_eps of this StockFinancial.  # noqa: E501
+        :type: float
         """
 
-        self._aliases = aliases
+        self._adjusted_basic_eps = adjusted_basic_eps
 
     @property
-    def colorable(self):
-        """Gets the colorable of this MetricsMetadata.  # noqa: E501
+    def year(self):
+        """Gets the year of this StockFinancial.  # noqa: E501
 
 
-        :return: The colorable of this MetricsMetadata.  # noqa: E501
-        :rtype: bool
+        :return: The year of this StockFinancial.  # noqa: E501
+        :rtype: int
         """
-        return self._colorable
+        return self._year
 
-    @colorable.setter
-    def colorable(self, colorable):
-        """Sets the colorable of this MetricsMetadata.
+    @year.setter
+    def year(self, year):
+        """Sets the year of this StockFinancial.
 
 
-        :param colorable: The colorable of this MetricsMetadata.  # noqa: E501
-        :type: bool
+        :param year: The year of this StockFinancial.  # noqa: E501
+        :type: int
         """
 
-        self._colorable = colorable
+        self._year = year
 
     @property
-    def id(self):
-        """Gets the id of this MetricsMetadata.  # noqa: E501
+    def fiscal_quarter(self):
+        """Gets the fiscal_quarter of this StockFinancial.  # noqa: E501
 
 
-        :return: The id of this MetricsMetadata.  # noqa: E501
-        :rtype: str
+        :return: The fiscal_quarter of this StockFinancial.  # noqa: E501
+        :rtype: int
         """
-        return self._id
+        return self._fiscal_quarter
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this MetricsMetadata.
+    @fiscal_quarter.setter
+    def fiscal_quarter(self, fiscal_quarter):
+        """Sets the fiscal_quarter of this StockFinancial.
 
 
-        :param id: The id of this MetricsMetadata.  # noqa: E501
-        :type: str
+        :param fiscal_quarter: The fiscal_quarter of this StockFinancial.  # noqa: E501
+        :type: int
         """
 
-        self._id = id
+        self._fiscal_quarter = fiscal_quarter
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -470,15 +418,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(MetricsMetadata, dict):
+        if issubclass(StockFinancial, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -486,15 +434,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MetricsMetadata):
+        if not isinstance(other, StockFinancial):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/momentum_metric_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/momentum_metric_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/monthly_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/monthly_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/monthly_returns.py` & `investor8-sdk-1.1.9/investor8-sdk/models/monthly_returns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/news_categories_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/news_categories_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/news_source.py` & `investor8-sdk-1.1.9/investor8-sdk/models/req_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NewsSource(object):
+class ReqType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    _0 = "0"
     _1 = "1"
     _2 = "2"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
@@ -37,15 +36,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NewsSource - a model defined in Swagger"""  # noqa: E501
+        """ReqType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NewsSource, dict):
+        if issubclass(ReqType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NewsSource):
+        if not isinstance(other, ReqType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/period_metric_value.py` & `investor8-sdk-1.1.9/investor8-sdk/models/period_metric_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/period_return.py` & `investor8-sdk-1.1.9/investor8-sdk/models/period_return.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/plot_detail_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/plot_response_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/plot_response_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/previous_close_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/previous_close_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/profile_name.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_news_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProfileName(object):
+class StockNewsStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
     _0 = "0"
     _1 = "1"
     _2 = "2"
+    _3 = "3"
+    _4 = "4"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """ProfileName - a model defined in Swagger"""  # noqa: E501
+        """StockNewsStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProfileName, dict):
+        if issubclass(StockNewsStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProfileName):
+        if not isinstance(other, StockNewsStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/recent_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/recent_earning_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/remove_from_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/remove_from_watchlist_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/rename_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/req_type.py` & `investor8-sdk-1.1.9/swagger_client/models/req_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
@@ -22,15 +22,14 @@
     """
 
     """
     allowed enum values
     """
     _1 = "1"
     _2 = "2"
-    _3 = "3"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/reset_password_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/result_field.py` & `investor8-sdk-1.1.9/investor8-sdk/models/result_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/return_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/return_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/sa_attributes_prices.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sa_attributes_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/sa_sector_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sa_sector_price_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/screen_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_financial_metrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,175 +1,149 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ScreenDto(object):
+class HistoricalFinancialMetrics(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'name': 'str',
-        'conditions': 'str',
-        'created_time': 'int',
-        'last_modified_time': 'int'
+        'prev': 'list[StockFinancial]',
+        'yo_y': 'list[StockFinancial]',
+        'ttm_growth': 'list[StockFinancial]',
+        'ttm': 'list[StockFinancial]'
     }
 
     attribute_map = {
-        'id': 'Id',
-        'name': 'Name',
-        'conditions': 'Conditions',
-        'created_time': 'CreatedTime',
-        'last_modified_time': 'LastModifiedTime'
+        'prev': 'Prev',
+        'yo_y': 'YoY',
+        'ttm_growth': 'TtmGrowth',
+        'ttm': 'TTM'
     }
 
-    def __init__(self, id=None, name=None, conditions=None, created_time=None, last_modified_time=None):  # noqa: E501
-        """ScreenDto - a model defined in Swagger"""  # noqa: E501
-        self._id = None
-        self._name = None
-        self._conditions = None
-        self._created_time = None
-        self._last_modified_time = None
+    def __init__(self, prev=None, yo_y=None, ttm_growth=None, ttm=None):  # noqa: E501
+        """HistoricalFinancialMetrics - a model defined in Swagger"""  # noqa: E501
+        self._prev = None
+        self._yo_y = None
+        self._ttm_growth = None
+        self._ttm = None
         self.discriminator = None
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
-        if conditions is not None:
-            self.conditions = conditions
-        if created_time is not None:
-            self.created_time = created_time
-        if last_modified_time is not None:
-            self.last_modified_time = last_modified_time
+        if prev is not None:
+            self.prev = prev
+        if yo_y is not None:
+            self.yo_y = yo_y
+        if ttm_growth is not None:
+            self.ttm_growth = ttm_growth
+        if ttm is not None:
+            self.ttm = ttm
 
     @property
-    def id(self):
-        """Gets the id of this ScreenDto.  # noqa: E501
+    def prev(self):
+        """Gets the prev of this HistoricalFinancialMetrics.  # noqa: E501
 
 
-        :return: The id of this ScreenDto.  # noqa: E501
-        :rtype: str
+        :return: The prev of this HistoricalFinancialMetrics.  # noqa: E501
+        :rtype: list[StockFinancial]
         """
-        return self._id
+        return self._prev
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ScreenDto.
+    @prev.setter
+    def prev(self, prev):
+        """Sets the prev of this HistoricalFinancialMetrics.
 
 
-        :param id: The id of this ScreenDto.  # noqa: E501
-        :type: str
+        :param prev: The prev of this HistoricalFinancialMetrics.  # noqa: E501
+        :type: list[StockFinancial]
         """
 
-        self._id = id
+        self._prev = prev
 
     @property
-    def name(self):
-        """Gets the name of this ScreenDto.  # noqa: E501
+    def yo_y(self):
+        """Gets the yo_y of this HistoricalFinancialMetrics.  # noqa: E501
 
 
-        :return: The name of this ScreenDto.  # noqa: E501
-        :rtype: str
+        :return: The yo_y of this HistoricalFinancialMetrics.  # noqa: E501
+        :rtype: list[StockFinancial]
         """
-        return self._name
+        return self._yo_y
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ScreenDto.
+    @yo_y.setter
+    def yo_y(self, yo_y):
+        """Sets the yo_y of this HistoricalFinancialMetrics.
 
 
-        :param name: The name of this ScreenDto.  # noqa: E501
-        :type: str
+        :param yo_y: The yo_y of this HistoricalFinancialMetrics.  # noqa: E501
+        :type: list[StockFinancial]
         """
 
-        self._name = name
+        self._yo_y = yo_y
 
     @property
-    def conditions(self):
-        """Gets the conditions of this ScreenDto.  # noqa: E501
+    def ttm_growth(self):
+        """Gets the ttm_growth of this HistoricalFinancialMetrics.  # noqa: E501
 
 
-        :return: The conditions of this ScreenDto.  # noqa: E501
-        :rtype: str
+        :return: The ttm_growth of this HistoricalFinancialMetrics.  # noqa: E501
+        :rtype: list[StockFinancial]
         """
-        return self._conditions
+        return self._ttm_growth
 
-    @conditions.setter
-    def conditions(self, conditions):
-        """Sets the conditions of this ScreenDto.
+    @ttm_growth.setter
+    def ttm_growth(self, ttm_growth):
+        """Sets the ttm_growth of this HistoricalFinancialMetrics.
 
 
-        :param conditions: The conditions of this ScreenDto.  # noqa: E501
-        :type: str
+        :param ttm_growth: The ttm_growth of this HistoricalFinancialMetrics.  # noqa: E501
+        :type: list[StockFinancial]
         """
 
-        self._conditions = conditions
+        self._ttm_growth = ttm_growth
 
     @property
-    def created_time(self):
-        """Gets the created_time of this ScreenDto.  # noqa: E501
+    def ttm(self):
+        """Gets the ttm of this HistoricalFinancialMetrics.  # noqa: E501
 
 
-        :return: The created_time of this ScreenDto.  # noqa: E501
-        :rtype: int
+        :return: The ttm of this HistoricalFinancialMetrics.  # noqa: E501
+        :rtype: list[StockFinancial]
         """
-        return self._created_time
+        return self._ttm
 
-    @created_time.setter
-    def created_time(self, created_time):
-        """Sets the created_time of this ScreenDto.
+    @ttm.setter
+    def ttm(self, ttm):
+        """Sets the ttm of this HistoricalFinancialMetrics.
 
 
-        :param created_time: The created_time of this ScreenDto.  # noqa: E501
-        :type: int
+        :param ttm: The ttm of this HistoricalFinancialMetrics.  # noqa: E501
+        :type: list[StockFinancial]
         """
 
-        self._created_time = created_time
-
-    @property
-    def last_modified_time(self):
-        """Gets the last_modified_time of this ScreenDto.  # noqa: E501
-
-
-        :return: The last_modified_time of this ScreenDto.  # noqa: E501
-        :rtype: int
-        """
-        return self._last_modified_time
-
-    @last_modified_time.setter
-    def last_modified_time(self, last_modified_time):
-        """Sets the last_modified_time of this ScreenDto.
-
-
-        :param last_modified_time: The last_modified_time of this ScreenDto.  # noqa: E501
-        :type: int
-        """
-
-        self._last_modified_time = last_modified_time
+        self._ttm = ttm
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -184,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ScreenDto, dict):
+        if issubclass(HistoricalFinancialMetrics, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ScreenDto):
+        if not isinstance(other, HistoricalFinancialMetrics):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/screening_condition.py` & `investor8-sdk-1.1.9/investor8-sdk/models/reset_password_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,97 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ScreeningCondition(object):
+class ResetPasswordDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'condition': 'str',
-        'display': 'str',
-        'es_query': 'str'
+        'request_id': 'str',
+        'password': 'str'
     }
 
     attribute_map = {
-        'condition': 'Condition',
-        'display': 'Display',
-        'es_query': 'ESQuery'
+        'request_id': 'RequestId',
+        'password': 'Password'
     }
 
-    def __init__(self, condition=None, display=None, es_query=None):  # noqa: E501
-        """ScreeningCondition - a model defined in Swagger"""  # noqa: E501
-        self._condition = None
-        self._display = None
-        self._es_query = None
+    def __init__(self, request_id=None, password=None):  # noqa: E501
+        """ResetPasswordDto - a model defined in Swagger"""  # noqa: E501
+        self._request_id = None
+        self._password = None
         self.discriminator = None
-        if condition is not None:
-            self.condition = condition
-        if display is not None:
-            self.display = display
-        if es_query is not None:
-            self.es_query = es_query
+        if request_id is not None:
+            self.request_id = request_id
+        if password is not None:
+            self.password = password
 
     @property
-    def condition(self):
-        """Gets the condition of this ScreeningCondition.  # noqa: E501
+    def request_id(self):
+        """Gets the request_id of this ResetPasswordDto.  # noqa: E501
 
 
-        :return: The condition of this ScreeningCondition.  # noqa: E501
+        :return: The request_id of this ResetPasswordDto.  # noqa: E501
         :rtype: str
         """
-        return self._condition
+        return self._request_id
 
-    @condition.setter
-    def condition(self, condition):
-        """Sets the condition of this ScreeningCondition.
+    @request_id.setter
+    def request_id(self, request_id):
+        """Sets the request_id of this ResetPasswordDto.
 
 
-        :param condition: The condition of this ScreeningCondition.  # noqa: E501
+        :param request_id: The request_id of this ResetPasswordDto.  # noqa: E501
         :type: str
         """
 
-        self._condition = condition
+        self._request_id = request_id
 
     @property
-    def display(self):
-        """Gets the display of this ScreeningCondition.  # noqa: E501
+    def password(self):
+        """Gets the password of this ResetPasswordDto.  # noqa: E501
 
 
-        :return: The display of this ScreeningCondition.  # noqa: E501
+        :return: The password of this ResetPasswordDto.  # noqa: E501
         :rtype: str
         """
-        return self._display
+        return self._password
 
-    @display.setter
-    def display(self, display):
-        """Sets the display of this ScreeningCondition.
+    @password.setter
+    def password(self, password):
+        """Sets the password of this ResetPasswordDto.
 
 
-        :param display: The display of this ScreeningCondition.  # noqa: E501
+        :param password: The password of this ResetPasswordDto.  # noqa: E501
         :type: str
         """
 
-        self._display = display
-
-    @property
-    def es_query(self):
-        """Gets the es_query of this ScreeningCondition.  # noqa: E501
-
-
-        :return: The es_query of this ScreeningCondition.  # noqa: E501
-        :rtype: str
-        """
-        return self._es_query
-
-    @es_query.setter
-    def es_query(self, es_query):
-        """Sets the es_query of this ScreeningCondition.
-
-
-        :param es_query: The es_query of this ScreeningCondition.  # noqa: E501
-        :type: str
-        """
-
-        self._es_query = es_query
+        self._password = password
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ScreeningCondition, dict):
+        if issubclass(ResetPasswordDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ScreeningCondition):
+        if not isinstance(other, ResetPasswordDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/sector_returns_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sector_returns_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/send_email_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/standardized_financial.py` & `investor8-sdk-1.1.9/investor8-sdk/models/standardized_financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_earning_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_financial.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_financial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_financial_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_financial_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_info_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_info_master_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_info_master_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_ipo.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_ipo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_news.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_news_details.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_news_status.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_news_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_details_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_popularity_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_price.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_price_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_rating_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_rating_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/stock_summary_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/string_message_result.py` & `investor8-sdk-1.1.9/investor8-sdk/models/string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/symbols_current_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_popularity_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SymbolsCurrentMetricsDto(object):
+class StockPopularityDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'list[CurrentMetricsDto]',
-        'metadata': 'list[MetricsMetadataResponseDto]'
+        'ticker': 'str',
+        'score': 'float',
+        'rank': 'int'
     }
 
     attribute_map = {
-        'data': 'Data',
-        'metadata': 'Metadata'
+        'ticker': 'Ticker',
+        'score': 'Score',
+        'rank': 'Rank'
     }
 
-    def __init__(self, data=None, metadata=None):  # noqa: E501
-        """SymbolsCurrentMetricsDto - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._metadata = None
+    def __init__(self, ticker=None, score=None, rank=None):  # noqa: E501
+        """StockPopularityDto - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._score = None
+        self._rank = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        if metadata is not None:
-            self.metadata = metadata
+        if ticker is not None:
+            self.ticker = ticker
+        if score is not None:
+            self.score = score
+        if rank is not None:
+            self.rank = rank
 
     @property
-    def data(self):
-        """Gets the data of this SymbolsCurrentMetricsDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this StockPopularityDto.  # noqa: E501
 
 
-        :return: The data of this SymbolsCurrentMetricsDto.  # noqa: E501
-        :rtype: list[CurrentMetricsDto]
+        :return: The ticker of this StockPopularityDto.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self._ticker
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this SymbolsCurrentMetricsDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this StockPopularityDto.
 
 
-        :param data: The data of this SymbolsCurrentMetricsDto.  # noqa: E501
-        :type: list[CurrentMetricsDto]
+        :param ticker: The ticker of this StockPopularityDto.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self._ticker = ticker
 
     @property
-    def metadata(self):
-        """Gets the metadata of this SymbolsCurrentMetricsDto.  # noqa: E501
+    def score(self):
+        """Gets the score of this StockPopularityDto.  # noqa: E501
 
 
-        :return: The metadata of this SymbolsCurrentMetricsDto.  # noqa: E501
-        :rtype: list[MetricsMetadataResponseDto]
+        :return: The score of this StockPopularityDto.  # noqa: E501
+        :rtype: float
         """
-        return self._metadata
+        return self._score
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this SymbolsCurrentMetricsDto.
+    @score.setter
+    def score(self, score):
+        """Sets the score of this StockPopularityDto.
 
 
-        :param metadata: The metadata of this SymbolsCurrentMetricsDto.  # noqa: E501
-        :type: list[MetricsMetadataResponseDto]
+        :param score: The score of this StockPopularityDto.  # noqa: E501
+        :type: float
         """
 
-        self._metadata = metadata
+        self._score = score
+
+    @property
+    def rank(self):
+        """Gets the rank of this StockPopularityDto.  # noqa: E501
+
+
+        :return: The rank of this StockPopularityDto.  # noqa: E501
+        :rtype: int
+        """
+        return self._rank
+
+    @rank.setter
+    def rank(self, rank):
+        """Sets the rank of this StockPopularityDto.
+
+
+        :param rank: The rank of this StockPopularityDto.  # noqa: E501
+        :type: int
+        """
+
+        self._rank = rank
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SymbolsCurrentMetricsDto, dict):
+        if issubclass(StockPopularityDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SymbolsCurrentMetricsDto):
+        if not isinstance(other, StockPopularityDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/symbols_historical_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/reset_password_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SymbolsHistoricalMetricsDto(object):
+class ResetPasswordDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'dict(str, dict(str, list[HistoricalMetricValueDto]))',
-        'metadata': 'list[MetricsMetadataResponseDto]'
+        'request_id': 'str',
+        'password': 'str'
     }
 
     attribute_map = {
-        'data': 'Data',
-        'metadata': 'Metadata'
+        'request_id': 'RequestId',
+        'password': 'Password'
     }
 
-    def __init__(self, data=None, metadata=None):  # noqa: E501
-        """SymbolsHistoricalMetricsDto - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._metadata = None
+    def __init__(self, request_id=None, password=None):  # noqa: E501
+        """ResetPasswordDto - a model defined in Swagger"""  # noqa: E501
+        self._request_id = None
+        self._password = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        if metadata is not None:
-            self.metadata = metadata
+        if request_id is not None:
+            self.request_id = request_id
+        if password is not None:
+            self.password = password
 
     @property
-    def data(self):
-        """Gets the data of this SymbolsHistoricalMetricsDto.  # noqa: E501
+    def request_id(self):
+        """Gets the request_id of this ResetPasswordDto.  # noqa: E501
 
 
-        :return: The data of this SymbolsHistoricalMetricsDto.  # noqa: E501
-        :rtype: dict(str, dict(str, list[HistoricalMetricValueDto]))
+        :return: The request_id of this ResetPasswordDto.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self._request_id
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this SymbolsHistoricalMetricsDto.
+    @request_id.setter
+    def request_id(self, request_id):
+        """Sets the request_id of this ResetPasswordDto.
 
 
-        :param data: The data of this SymbolsHistoricalMetricsDto.  # noqa: E501
-        :type: dict(str, dict(str, list[HistoricalMetricValueDto]))
+        :param request_id: The request_id of this ResetPasswordDto.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self._request_id = request_id
 
     @property
-    def metadata(self):
-        """Gets the metadata of this SymbolsHistoricalMetricsDto.  # noqa: E501
+    def password(self):
+        """Gets the password of this ResetPasswordDto.  # noqa: E501
 
 
-        :return: The metadata of this SymbolsHistoricalMetricsDto.  # noqa: E501
-        :rtype: list[MetricsMetadataResponseDto]
+        :return: The password of this ResetPasswordDto.  # noqa: E501
+        :rtype: str
         """
-        return self._metadata
+        return self._password
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this SymbolsHistoricalMetricsDto.
+    @password.setter
+    def password(self, password):
+        """Sets the password of this ResetPasswordDto.
 
 
-        :param metadata: The metadata of this SymbolsHistoricalMetricsDto.  # noqa: E501
-        :type: list[MetricsMetadataResponseDto]
+        :param password: The password of this ResetPasswordDto.  # noqa: E501
+        :type: str
         """
 
-        self._metadata = metadata
+        self._password = password
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SymbolsHistoricalMetricsDto, dict):
+        if issubclass(ResetPasswordDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SymbolsHistoricalMetricsDto):
+        if not isinstance(other, ResetPasswordDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/tag_details_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/tag_details_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/tag_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/tag_info_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/terminal_log_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_price.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,253 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TerminalLogDto(object):
+class StockPrice(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'command': 'str',
-        'usage_date_time': 'datetime',
-        'version': 'str',
-        'os': 'str',
-        'app_instance_id': 'str',
-        'exception': 'str'
+        'ticker': 'str',
+        'timestamp': 'int',
+        'open': 'float',
+        'close': 'float',
+        'low': 'float',
+        'high': 'float',
+        'volume': 'float',
+        'id': 'str'
     }
 
     attribute_map = {
-        'id': 'Id',
-        'command': 'Command',
-        'usage_date_time': 'UsageDateTime',
-        'version': 'Version',
-        'os': 'OS',
-        'app_instance_id': 'AppInstanceId',
-        'exception': 'Exception'
+        'ticker': 'Ticker',
+        'timestamp': 'Timestamp',
+        'open': 'Open',
+        'close': 'Close',
+        'low': 'Low',
+        'high': 'High',
+        'volume': 'Volume',
+        'id': 'Id'
     }
 
-    def __init__(self, id=None, command=None, usage_date_time=None, version=None, os=None, app_instance_id=None, exception=None):  # noqa: E501
-        """TerminalLogDto - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, ticker=None, timestamp=None, open=None, close=None, low=None, high=None, volume=None, id=None):  # noqa: E501
+        """StockPrice - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._timestamp = None
+        self._open = None
+        self._close = None
+        self._low = None
+        self._high = None
+        self._volume = None
         self._id = None
-        self._command = None
-        self._usage_date_time = None
-        self._version = None
-        self._os = None
-        self._app_instance_id = None
-        self._exception = None
         self.discriminator = None
+        if ticker is not None:
+            self.ticker = ticker
+        if timestamp is not None:
+            self.timestamp = timestamp
+        if open is not None:
+            self.open = open
+        if close is not None:
+            self.close = close
+        if low is not None:
+            self.low = low
+        if high is not None:
+            self.high = high
+        if volume is not None:
+            self.volume = volume
         if id is not None:
             self.id = id
-        if command is not None:
-            self.command = command
-        if usage_date_time is not None:
-            self.usage_date_time = usage_date_time
-        if version is not None:
-            self.version = version
-        if os is not None:
-            self.os = os
-        if app_instance_id is not None:
-            self.app_instance_id = app_instance_id
-        if exception is not None:
-            self.exception = exception
 
     @property
-    def id(self):
-        """Gets the id of this TerminalLogDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this StockPrice.  # noqa: E501
 
 
-        :return: The id of this TerminalLogDto.  # noqa: E501
+        :return: The ticker of this StockPrice.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._ticker
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this TerminalLogDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this StockPrice.
 
 
-        :param id: The id of this TerminalLogDto.  # noqa: E501
+        :param ticker: The ticker of this StockPrice.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._ticker = ticker
 
     @property
-    def command(self):
-        """Gets the command of this TerminalLogDto.  # noqa: E501
+    def timestamp(self):
+        """Gets the timestamp of this StockPrice.  # noqa: E501
 
 
-        :return: The command of this TerminalLogDto.  # noqa: E501
-        :rtype: str
+        :return: The timestamp of this StockPrice.  # noqa: E501
+        :rtype: int
         """
-        return self._command
+        return self._timestamp
 
-    @command.setter
-    def command(self, command):
-        """Sets the command of this TerminalLogDto.
+    @timestamp.setter
+    def timestamp(self, timestamp):
+        """Sets the timestamp of this StockPrice.
 
 
-        :param command: The command of this TerminalLogDto.  # noqa: E501
-        :type: str
+        :param timestamp: The timestamp of this StockPrice.  # noqa: E501
+        :type: int
         """
 
-        self._command = command
+        self._timestamp = timestamp
 
     @property
-    def usage_date_time(self):
-        """Gets the usage_date_time of this TerminalLogDto.  # noqa: E501
+    def open(self):
+        """Gets the open of this StockPrice.  # noqa: E501
 
 
-        :return: The usage_date_time of this TerminalLogDto.  # noqa: E501
-        :rtype: datetime
+        :return: The open of this StockPrice.  # noqa: E501
+        :rtype: float
         """
-        return self._usage_date_time
+        return self._open
 
-    @usage_date_time.setter
-    def usage_date_time(self, usage_date_time):
-        """Sets the usage_date_time of this TerminalLogDto.
+    @open.setter
+    def open(self, open):
+        """Sets the open of this StockPrice.
 
 
-        :param usage_date_time: The usage_date_time of this TerminalLogDto.  # noqa: E501
-        :type: datetime
+        :param open: The open of this StockPrice.  # noqa: E501
+        :type: float
         """
 
-        self._usage_date_time = usage_date_time
+        self._open = open
 
     @property
-    def version(self):
-        """Gets the version of this TerminalLogDto.  # noqa: E501
+    def close(self):
+        """Gets the close of this StockPrice.  # noqa: E501
 
 
-        :return: The version of this TerminalLogDto.  # noqa: E501
-        :rtype: str
+        :return: The close of this StockPrice.  # noqa: E501
+        :rtype: float
         """
-        return self._version
+        return self._close
 
-    @version.setter
-    def version(self, version):
-        """Sets the version of this TerminalLogDto.
+    @close.setter
+    def close(self, close):
+        """Sets the close of this StockPrice.
 
 
-        :param version: The version of this TerminalLogDto.  # noqa: E501
-        :type: str
+        :param close: The close of this StockPrice.  # noqa: E501
+        :type: float
         """
 
-        self._version = version
+        self._close = close
 
     @property
-    def os(self):
-        """Gets the os of this TerminalLogDto.  # noqa: E501
+    def low(self):
+        """Gets the low of this StockPrice.  # noqa: E501
 
 
-        :return: The os of this TerminalLogDto.  # noqa: E501
-        :rtype: str
+        :return: The low of this StockPrice.  # noqa: E501
+        :rtype: float
         """
-        return self._os
+        return self._low
 
-    @os.setter
-    def os(self, os):
-        """Sets the os of this TerminalLogDto.
+    @low.setter
+    def low(self, low):
+        """Sets the low of this StockPrice.
 
 
-        :param os: The os of this TerminalLogDto.  # noqa: E501
-        :type: str
+        :param low: The low of this StockPrice.  # noqa: E501
+        :type: float
         """
 
-        self._os = os
+        self._low = low
 
     @property
-    def app_instance_id(self):
-        """Gets the app_instance_id of this TerminalLogDto.  # noqa: E501
+    def high(self):
+        """Gets the high of this StockPrice.  # noqa: E501
 
 
-        :return: The app_instance_id of this TerminalLogDto.  # noqa: E501
-        :rtype: str
+        :return: The high of this StockPrice.  # noqa: E501
+        :rtype: float
         """
-        return self._app_instance_id
+        return self._high
 
-    @app_instance_id.setter
-    def app_instance_id(self, app_instance_id):
-        """Sets the app_instance_id of this TerminalLogDto.
+    @high.setter
+    def high(self, high):
+        """Sets the high of this StockPrice.
 
 
-        :param app_instance_id: The app_instance_id of this TerminalLogDto.  # noqa: E501
-        :type: str
+        :param high: The high of this StockPrice.  # noqa: E501
+        :type: float
+        """
+
+        self._high = high
+
+    @property
+    def volume(self):
+        """Gets the volume of this StockPrice.  # noqa: E501
+
+
+        :return: The volume of this StockPrice.  # noqa: E501
+        :rtype: float
+        """
+        return self._volume
+
+    @volume.setter
+    def volume(self, volume):
+        """Sets the volume of this StockPrice.
+
+
+        :param volume: The volume of this StockPrice.  # noqa: E501
+        :type: float
         """
 
-        self._app_instance_id = app_instance_id
+        self._volume = volume
 
     @property
-    def exception(self):
-        """Gets the exception of this TerminalLogDto.  # noqa: E501
+    def id(self):
+        """Gets the id of this StockPrice.  # noqa: E501
 
 
-        :return: The exception of this TerminalLogDto.  # noqa: E501
+        :return: The id of this StockPrice.  # noqa: E501
         :rtype: str
         """
-        return self._exception
+        return self._id
 
-    @exception.setter
-    def exception(self, exception):
-        """Sets the exception of this TerminalLogDto.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StockPrice.
 
 
-        :param exception: The exception of this TerminalLogDto.  # noqa: E501
+        :param id: The id of this StockPrice.  # noqa: E501
         :type: str
         """
 
-        self._exception = exception
+        self._id = id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -236,15 +262,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TerminalLogDto, dict):
+        if issubclass(StockPrice, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -252,15 +278,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TerminalLogDto):
+        if not isinstance(other, StockPrice):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/terminal_log_os_versions_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financials_growth.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TerminalLogOSVersionsDto(object):
+class FinancialsGrowth(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'version_list': 'list[str]',
-        'os_list': 'list[str]'
+        'prev': 'StockFinancial',
+        'yo_y': 'StockFinancial',
+        'ttm': 'StockFinancial'
     }
 
     attribute_map = {
-        'version_list': 'VersionList',
-        'os_list': 'OSList'
+        'prev': 'Prev',
+        'yo_y': 'YoY',
+        'ttm': 'TTM'
     }
 
-    def __init__(self, version_list=None, os_list=None):  # noqa: E501
-        """TerminalLogOSVersionsDto - a model defined in Swagger"""  # noqa: E501
-        self._version_list = None
-        self._os_list = None
+    def __init__(self, prev=None, yo_y=None, ttm=None):  # noqa: E501
+        """FinancialsGrowth - a model defined in Swagger"""  # noqa: E501
+        self._prev = None
+        self._yo_y = None
+        self._ttm = None
         self.discriminator = None
-        if version_list is not None:
-            self.version_list = version_list
-        if os_list is not None:
-            self.os_list = os_list
+        if prev is not None:
+            self.prev = prev
+        if yo_y is not None:
+            self.yo_y = yo_y
+        if ttm is not None:
+            self.ttm = ttm
 
     @property
-    def version_list(self):
-        """Gets the version_list of this TerminalLogOSVersionsDto.  # noqa: E501
+    def prev(self):
+        """Gets the prev of this FinancialsGrowth.  # noqa: E501
 
 
-        :return: The version_list of this TerminalLogOSVersionsDto.  # noqa: E501
-        :rtype: list[str]
+        :return: The prev of this FinancialsGrowth.  # noqa: E501
+        :rtype: StockFinancial
         """
-        return self._version_list
+        return self._prev
 
-    @version_list.setter
-    def version_list(self, version_list):
-        """Sets the version_list of this TerminalLogOSVersionsDto.
+    @prev.setter
+    def prev(self, prev):
+        """Sets the prev of this FinancialsGrowth.
 
 
-        :param version_list: The version_list of this TerminalLogOSVersionsDto.  # noqa: E501
-        :type: list[str]
+        :param prev: The prev of this FinancialsGrowth.  # noqa: E501
+        :type: StockFinancial
         """
 
-        self._version_list = version_list
+        self._prev = prev
 
     @property
-    def os_list(self):
-        """Gets the os_list of this TerminalLogOSVersionsDto.  # noqa: E501
+    def yo_y(self):
+        """Gets the yo_y of this FinancialsGrowth.  # noqa: E501
 
 
-        :return: The os_list of this TerminalLogOSVersionsDto.  # noqa: E501
-        :rtype: list[str]
+        :return: The yo_y of this FinancialsGrowth.  # noqa: E501
+        :rtype: StockFinancial
         """
-        return self._os_list
+        return self._yo_y
 
-    @os_list.setter
-    def os_list(self, os_list):
-        """Sets the os_list of this TerminalLogOSVersionsDto.
+    @yo_y.setter
+    def yo_y(self, yo_y):
+        """Sets the yo_y of this FinancialsGrowth.
 
 
-        :param os_list: The os_list of this TerminalLogOSVersionsDto.  # noqa: E501
-        :type: list[str]
+        :param yo_y: The yo_y of this FinancialsGrowth.  # noqa: E501
+        :type: StockFinancial
         """
 
-        self._os_list = os_list
+        self._yo_y = yo_y
+
+    @property
+    def ttm(self):
+        """Gets the ttm of this FinancialsGrowth.  # noqa: E501
+
+
+        :return: The ttm of this FinancialsGrowth.  # noqa: E501
+        :rtype: StockFinancial
+        """
+        return self._ttm
+
+    @ttm.setter
+    def ttm(self, ttm):
+        """Sets the ttm of this FinancialsGrowth.
+
+
+        :param ttm: The ttm of this FinancialsGrowth.  # noqa: E501
+        :type: StockFinancial
+        """
+
+        self._ttm = ttm
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TerminalLogOSVersionsDto, dict):
+        if issubclass(FinancialsGrowth, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TerminalLogOSVersionsDto):
+        if not isinstance(other, FinancialsGrowth):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/trading_calendar_details_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/trading_calendar_details_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/upcoming_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/upcoming_earning_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/update_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/user.py` & `investor8-sdk-1.1.9/investor8-sdk/models/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,52 +35,46 @@
         'roles': 'list[str]',
         'opt_for_newsletter': 'bool',
         'country': 'str',
         'email_confirmed': 'bool',
         'created_time': 'int',
         'last_modified': 'int',
         'profile_name': 'str',
-        'api_key': 'str',
-        'auth_source': 'str',
-        'external_id': 'str'
+        'api_key': 'str'
     }
 
     attribute_map = {
         'id': 'Id',
         'first_name': 'FirstName',
         'last_name': 'LastName',
         'email': 'Email',
         'roles': 'Roles',
         'opt_for_newsletter': 'OptForNewsletter',
         'country': 'Country',
         'email_confirmed': 'EmailConfirmed',
         'created_time': 'CreatedTime',
         'last_modified': 'LastModified',
         'profile_name': 'ProfileName',
-        'api_key': 'ApiKey',
-        'auth_source': 'AuthSource',
-        'external_id': 'ExternalId'
+        'api_key': 'ApiKey'
     }
 
-    def __init__(self, id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, auth_source=None, external_id=None):  # noqa: E501
+    def __init__(self, id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None):  # noqa: E501
         """User - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._first_name = None
         self._last_name = None
         self._email = None
         self._roles = None
         self._opt_for_newsletter = None
         self._country = None
         self._email_confirmed = None
         self._created_time = None
         self._last_modified = None
         self._profile_name = None
         self._api_key = None
-        self._auth_source = None
-        self._external_id = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if first_name is not None:
             self.first_name = first_name
         if last_name is not None:
             self.last_name = last_name
@@ -98,18 +92,14 @@
             self.created_time = created_time
         if last_modified is not None:
             self.last_modified = last_modified
         if profile_name is not None:
             self.profile_name = profile_name
         if api_key is not None:
             self.api_key = api_key
-        if auth_source is not None:
-            self.auth_source = auth_source
-        if external_id is not None:
-            self.external_id = external_id
 
     @property
     def id(self):
         """Gets the id of this User.  # noqa: E501
 
 
         :return: The id of this User.  # noqa: E501
@@ -355,56 +345,14 @@
 
         :param api_key: The api_key of this User.  # noqa: E501
         :type: str
         """
 
         self._api_key = api_key
 
-    @property
-    def auth_source(self):
-        """Gets the auth_source of this User.  # noqa: E501
-
-
-        :return: The auth_source of this User.  # noqa: E501
-        :rtype: str
-        """
-        return self._auth_source
-
-    @auth_source.setter
-    def auth_source(self, auth_source):
-        """Sets the auth_source of this User.
-
-
-        :param auth_source: The auth_source of this User.  # noqa: E501
-        :type: str
-        """
-
-        self._auth_source = auth_source
-
-    @property
-    def external_id(self):
-        """Gets the external_id of this User.  # noqa: E501
-
-
-        :return: The external_id of this User.  # noqa: E501
-        :rtype: str
-        """
-        return self._external_id
-
-    @external_id.setter
-    def external_id(self, external_id):
-        """Sets the external_id of this User.
-
-
-        :param external_id: The external_id of this User.  # noqa: E501
-        :type: str
-        """
-
-        self._external_id = external_id
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/user_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
@@ -44,17 +44,15 @@
         'premium_start_date': 'datetime',
         'charging_start_date': 'datetime',
         'charging_next_date': 'datetime',
         'cancel_date': 'datetime',
         'auth_source': 'AuthenticationSource',
         'subscription_id': 'str',
         'referer': 'str',
-        'allow_terminal_logging': 'bool',
-        'stripe_customer_id': 'str',
-        'discovery_source': 'DiscoverySource'
+        'allow_terminal_logging': 'bool'
     }
 
     attribute_map = {
         'user_id': 'UserId',
         'first_name': 'FirstName',
         'last_name': 'LastName',
         'email': 'Email',
@@ -70,20 +68,18 @@
         'premium_start_date': 'PremiumStartDate',
         'charging_start_date': 'ChargingStartDate',
         'charging_next_date': 'ChargingNextDate',
         'cancel_date': 'CancelDate',
         'auth_source': 'AuthSource',
         'subscription_id': 'SubscriptionId',
         'referer': 'Referer',
-        'allow_terminal_logging': 'AllowTerminalLogging',
-        'stripe_customer_id': 'StripeCustomerId',
-        'discovery_source': 'DiscoverySource'
+        'allow_terminal_logging': 'AllowTerminalLogging'
     }
 
-    def __init__(self, user_id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, token=None, premium_start_date=None, charging_start_date=None, charging_next_date=None, cancel_date=None, auth_source=None, subscription_id=None, referer=None, allow_terminal_logging=None, stripe_customer_id=None, discovery_source=None):  # noqa: E501
+    def __init__(self, user_id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, token=None, premium_start_date=None, charging_start_date=None, charging_next_date=None, cancel_date=None, auth_source=None, subscription_id=None, referer=None, allow_terminal_logging=None):  # noqa: E501
         """UserDto - a model defined in Swagger"""  # noqa: E501
         self._user_id = None
         self._first_name = None
         self._last_name = None
         self._email = None
         self._roles = None
         self._opt_for_newsletter = None
@@ -98,16 +94,14 @@
         self._charging_start_date = None
         self._charging_next_date = None
         self._cancel_date = None
         self._auth_source = None
         self._subscription_id = None
         self._referer = None
         self._allow_terminal_logging = None
-        self._stripe_customer_id = None
-        self._discovery_source = None
         self.discriminator = None
         self.user_id = user_id
         if first_name is not None:
             self.first_name = first_name
         if last_name is not None:
             self.last_name = last_name
         if email is not None:
@@ -142,18 +136,14 @@
             self.auth_source = auth_source
         if subscription_id is not None:
             self.subscription_id = subscription_id
         if referer is not None:
             self.referer = referer
         if allow_terminal_logging is not None:
             self.allow_terminal_logging = allow_terminal_logging
-        if stripe_customer_id is not None:
-            self.stripe_customer_id = stripe_customer_id
-        if discovery_source is not None:
-            self.discovery_source = discovery_source
 
     @property
     def user_id(self):
         """Gets the user_id of this UserDto.  # noqa: E501
 
 
         :return: The user_id of this UserDto.  # noqa: E501
@@ -590,56 +580,14 @@
 
         :param allow_terminal_logging: The allow_terminal_logging of this UserDto.  # noqa: E501
         :type: bool
         """
 
         self._allow_terminal_logging = allow_terminal_logging
 
-    @property
-    def stripe_customer_id(self):
-        """Gets the stripe_customer_id of this UserDto.  # noqa: E501
-
-
-        :return: The stripe_customer_id of this UserDto.  # noqa: E501
-        :rtype: str
-        """
-        return self._stripe_customer_id
-
-    @stripe_customer_id.setter
-    def stripe_customer_id(self, stripe_customer_id):
-        """Sets the stripe_customer_id of this UserDto.
-
-
-        :param stripe_customer_id: The stripe_customer_id of this UserDto.  # noqa: E501
-        :type: str
-        """
-
-        self._stripe_customer_id = stripe_customer_id
-
-    @property
-    def discovery_source(self):
-        """Gets the discovery_source of this UserDto.  # noqa: E501
-
-
-        :return: The discovery_source of this UserDto.  # noqa: E501
-        :rtype: DiscoverySource
-        """
-        return self._discovery_source
-
-    @discovery_source.setter
-    def discovery_source(self, discovery_source):
-        """Sets the discovery_source of this UserDto.
-
-
-        :param discovery_source: The discovery_source of this UserDto.  # noqa: E501
-        :type: DiscoverySource
-        """
-
-        self._discovery_source = discovery_source
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/value_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/value_metrics_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/view_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/watchlist.py` & `investor8-sdk-1.1.9/investor8-sdk/models/watchlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/models/watchlist_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/watchlist_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
```

### Comparing `investor8-sdk-1.1.80/investor8_sdk/rest.py` & `investor8-sdk-1.1.9/investor8-sdk/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
 import json
```

### Comparing `investor8-sdk-1.1.80/test/test_active_company_dto.py` & `investor8-sdk-1.1.9/test/test_active_company_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_add_to_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_add_to_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_authentication_request.py` & `investor8-sdk-1.1.9/test/test_authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_authentication_source.py` & `investor8-sdk-1.1.9/test/test_authentication_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_authorize_account_request_dto.py` & `investor8-sdk-1.1.9/test/test_authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_authorize_account_response_dto.py` & `investor8-sdk-1.1.9/test/test_authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_change_password_dto.py` & `investor8-sdk-1.1.9/test/test_change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_company_info_dto.py` & `investor8-sdk-1.1.9/test/test_company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_auth_req_dto.py` & `investor8-sdk-1.1.9/test/test_create_auth_req_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_plot_dto.py` & `investor8-sdk-1.1.9/test/test_create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_screen_dto.py` & `investor8-sdk-1.1.9/test/test_user_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.create_screen_dto import CreateScreenDto  # noqa: E501
+from investor8_sdk.models.user_dto import UserDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestCreateScreenDto(unittest.TestCase):
-    """CreateScreenDto unit test stubs"""
+class TestUserDto(unittest.TestCase):
+    """UserDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateScreenDto(self):
-        """Test CreateScreenDto"""
+    def testUserDto(self):
+        """Test UserDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.create_screen_dto.CreateScreenDto()  # noqa: E501
+        # model = investor8_sdk.models.user_dto.UserDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_create_update_news.py` & `investor8-sdk-1.1.9/test/test_create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_user_dto.py` & `investor8-sdk-1.1.9/test/test_create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_user_res_dto.py` & `investor8-sdk-1.1.9/test/test_create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_create_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_current_metadat_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_financials_growth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.current_metadat_metrics_dto import CurrentMetadatMetricsDto  # noqa: E501
+from investor8_sdk.models.financials_growth import FinancialsGrowth  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestCurrentMetadatMetricsDto(unittest.TestCase):
-    """CurrentMetadatMetricsDto unit test stubs"""
+class TestFinancialsGrowth(unittest.TestCase):
+    """FinancialsGrowth unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrentMetadatMetricsDto(self):
-        """Test CurrentMetadatMetricsDto"""
+    def testFinancialsGrowth(self):
+        """Test FinancialsGrowth"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.current_metadat_metrics_dto.CurrentMetadatMetricsDto()  # noqa: E501
+        # model = investor8_sdk.models.financials_growth.FinancialsGrowth()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_current_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_daily_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/test/test_detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_discovery_source.py` & `investor8-sdk-1.1.9/test/test_login_user_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.discovery_source import DiscoverySource  # noqa: E501
+from investor8_sdk.models.login_user_dto import LoginUserDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestDiscoverySource(unittest.TestCase):
-    """DiscoverySource unit test stubs"""
+class TestLoginUserDto(unittest.TestCase):
+    """LoginUserDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDiscoverySource(self):
-        """Test DiscoverySource"""
+    def testLoginUserDto(self):
+        """Test LoginUserDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.discovery_source.DiscoverySource()  # noqa: E501
+        # model = investor8_sdk.models.login_user_dto.LoginUserDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_earning_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_earnings_api.py` & `investor8-sdk-1.1.9/test/test_earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_email_api.py` & `investor8-sdk-1.1.9/test/test_email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_email_type.py` & `investor8-sdk-1.1.9/test/test_email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_financial_metric_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_financial_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_financial_report_dto.py` & `investor8-sdk-1.1.9/test/test_financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_financial_tag.py` & `investor8-sdk-1.1.9/test/test_financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_financials_api.py` & `investor8-sdk-1.1.9/test/test_financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_financials_growth.py` & `investor8-sdk-1.1.9/test/test_latest_financial_metrics_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.financials_growth import FinancialsGrowth  # noqa: E501
+from investor8_sdk.models.latest_financial_metrics_dto import LatestFinancialMetricsDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestFinancialsGrowth(unittest.TestCase):
-    """FinancialsGrowth unit test stubs"""
+class TestLatestFinancialMetricsDto(unittest.TestCase):
+    """LatestFinancialMetricsDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFinancialsGrowth(self):
-        """Test FinancialsGrowth"""
+    def testLatestFinancialMetricsDto(self):
+        """Test LatestFinancialMetricsDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.financials_growth.FinancialsGrowth()  # noqa: E501
+        # model = investor8_sdk.models.latest_financial_metrics_dto.LatestFinancialMetricsDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_get_list_metrics_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_send_email_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.get_list_metrics_metadata_dto import GetListMetricsMetadataDto  # noqa: E501
+from investor8_sdk.models.send_email_dto import SendEmailDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestGetListMetricsMetadataDto(unittest.TestCase):
-    """GetListMetricsMetadataDto unit test stubs"""
+class TestSendEmailDto(unittest.TestCase):
+    """SendEmailDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetListMetricsMetadataDto(self):
-        """Test GetListMetricsMetadataDto"""
+    def testSendEmailDto(self):
+        """Test SendEmailDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.get_list_metrics_metadata_dto.GetListMetricsMetadataDto()  # noqa: E501
+        # model = investor8_sdk.models.send_email_dto.SendEmailDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_get_metrics_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.get_metrics_metadata_dto import GetMetricsMetadataDto  # noqa: E501
+from investor8_sdk.models.metrics import Metrics  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestGetMetricsMetadataDto(unittest.TestCase):
-    """GetMetricsMetadataDto unit test stubs"""
+class TestMetrics(unittest.TestCase):
+    """Metrics unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetMetricsMetadataDto(self):
-        """Test GetMetricsMetadataDto"""
+    def testMetrics(self):
+        """Test Metrics"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.get_metrics_metadata_dto.GetMetricsMetadataDto()  # noqa: E501
+        # model = investor8_sdk.models.metrics.Metrics()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_get_screens_by_user_dto.py` & `investor8-sdk-1.1.9/test/test_stock_ipo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.get_screens_by_user_dto import GetScreensByUserDto  # noqa: E501
+from investor8_sdk.models.stock_ipo import StockIpo  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestGetScreensByUserDto(unittest.TestCase):
-    """GetScreensByUserDto unit test stubs"""
+class TestStockIpo(unittest.TestCase):
+    """StockIpo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetScreensByUserDto(self):
-        """Test GetScreensByUserDto"""
+    def testStockIpo(self):
+        """Test StockIpo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.get_screens_by_user_dto.GetScreensByUserDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_ipo.StockIpo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_get_user_plots_dto.py` & `investor8-sdk-1.1.9/test/test_get_user_plots_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/test/test_get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_daily_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_historical_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_financial_metrics.py` & `investor8-sdk-1.1.9/test/test_historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_indicator_dto.py` & `investor8-sdk-1.1.9/test/test_historical_indicator_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_metadata_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_metadata_properties_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.historical_metadata_metrics_dto import HistoricalMetadataMetricsDto  # noqa: E501
+from investor8_sdk.models.metadata_properties_dto import MetadataPropertiesDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestHistoricalMetadataMetricsDto(unittest.TestCase):
-    """HistoricalMetadataMetricsDto unit test stubs"""
+class TestMetadataPropertiesDto(unittest.TestCase):
+    """MetadataPropertiesDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHistoricalMetadataMetricsDto(self):
-        """Test HistoricalMetadataMetricsDto"""
+    def testMetadataPropertiesDto(self):
+        """Test MetadataPropertiesDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.historical_metadata_metrics_dto.HistoricalMetadataMetricsDto()  # noqa: E501
+        # model = investor8_sdk.models.metadata_properties_dto.MetadataPropertiesDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_historical_metric_value_dto.py` & `investor8-sdk-1.1.9/test/test_metric_metadata_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.historical_metric_value_dto import HistoricalMetricValueDto  # noqa: E501
+from investor8_sdk.models.metric_metadata_dto import MetricMetadataDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestHistoricalMetricValueDto(unittest.TestCase):
-    """HistoricalMetricValueDto unit test stubs"""
+class TestMetricMetadataDto(unittest.TestCase):
+    """MetricMetadataDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHistoricalMetricValueDto(self):
-        """Test HistoricalMetricValueDto"""
+    def testMetricMetadataDto(self):
+        """Test MetricMetadataDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.historical_metric_value_dto.HistoricalMetricValueDto()  # noqa: E501
+        # model = investor8_sdk.models.metric_metadata_dto.MetricMetadataDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_historical_return.py` & `investor8-sdk-1.1.9/test/test_historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_returns_dto.py` & `investor8-sdk-1.1.9/test/test_historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_historical_value_metrics.py` & `investor8-sdk-1.1.9/test/test_historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_history_length.py` & `investor8-sdk-1.1.9/test/test_history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_check_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_i8_terminal_version.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_version.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_i8_terminal_version_dto.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_stock_financial_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.latest_financial_metrics_dto import LatestFinancialMetricsDto  # noqa: E501
+from investor8_sdk.models.stock_financial_metrics import StockFinancialMetrics  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestLatestFinancialMetricsDto(unittest.TestCase):
-    """LatestFinancialMetricsDto unit test stubs"""
+class TestStockFinancialMetrics(unittest.TestCase):
+    """StockFinancialMetrics unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLatestFinancialMetricsDto(self):
-        """Test LatestFinancialMetricsDto"""
+    def testStockFinancialMetrics(self):
+        """Test StockFinancialMetrics"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.latest_financial_metrics_dto.LatestFinancialMetricsDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_financial_metrics.StockFinancialMetrics()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_latest_financials_dto.py` & `investor8-sdk-1.1.9/test/test_latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/test/test_latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_latest_price_dto.py` & `investor8-sdk-1.1.9/test/test_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/test/test_list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_log_terminal_usage.py` & `investor8-sdk-1.1.9/test/test_log_terminal_usage.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_login_user_dto.py` & `investor8-sdk-1.1.9/test/test_view_plot_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.login_user_dto import LoginUserDto  # noqa: E501
+from investor8_sdk.models.view_plot_dto import ViewPlotDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestLoginUserDto(unittest.TestCase):
-    """LoginUserDto unit test stubs"""
+class TestViewPlotDto(unittest.TestCase):
+    """ViewPlotDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLoginUserDto(self):
-        """Test LoginUserDto"""
+    def testViewPlotDto(self):
+        """Test ViewPlotDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.login_user_dto.LoginUserDto()  # noqa: E501
+        # model = investor8_sdk.models.view_plot_dto.ViewPlotDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_login_with_code_dto.py` & `investor8-sdk-1.1.9/test/test_login_with_code_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_market_highlight.py` & `investor8-sdk-1.1.9/test/test_market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_market_highlight_dto.py` & `investor8-sdk-1.1.9/test/test_market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_market_highlight_status.py` & `investor8-sdk-1.1.9/test/test_market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_metadata_properties_dto.py` & `investor8-sdk-1.1.9/test/test_trading_calendar_details_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.metadata_properties_dto import MetadataPropertiesDto  # noqa: E501
+from investor8_sdk.models.trading_calendar_details_dto import TradingCalendarDetailsDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestMetadataPropertiesDto(unittest.TestCase):
-    """MetadataPropertiesDto unit test stubs"""
+class TestTradingCalendarDetailsDto(unittest.TestCase):
+    """TradingCalendarDetailsDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetadataPropertiesDto(self):
-        """Test MetadataPropertiesDto"""
+    def testTradingCalendarDetailsDto(self):
+        """Test TradingCalendarDetailsDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.metadata_properties_dto.MetadataPropertiesDto()  # noqa: E501
+        # model = investor8_sdk.models.trading_calendar_details_dto.TradingCalendarDetailsDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_metric_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_stock_news.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.metric_metadata_dto import MetricMetadataDto  # noqa: E501
+from investor8_sdk.models.stock_news import StockNews  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestMetricMetadataDto(unittest.TestCase):
-    """MetricMetadataDto unit test stubs"""
+class TestStockNews(unittest.TestCase):
+    """StockNews unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricMetadataDto(self):
-        """Test MetricMetadataDto"""
+    def testStockNews(self):
+        """Test StockNews"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.metric_metadata_dto.MetricMetadataDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_news.StockNews()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_metrics.py` & `investor8-sdk-1.1.9/test/test_stock_price.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.metrics import Metrics  # noqa: E501
+from investor8_sdk.models.stock_price import StockPrice  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestMetrics(unittest.TestCase):
-    """Metrics unit test stubs"""
+class TestStockPrice(unittest.TestCase):
+    """StockPrice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetrics(self):
-        """Test Metrics"""
+    def testStockPrice(self):
+        """Test StockPrice"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.metrics.Metrics()  # noqa: E501
+        # model = investor8_sdk.models.stock_price.StockPrice()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_metrics_api.py` & `investor8-sdk-1.1.9/test/test_metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_metrics_by_period_dto.py` & `investor8-sdk-1.1.9/test/test_recent_earning_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.metrics_by_period_dto import MetricsByPeriodDto  # noqa: E501
+from investor8_sdk.models.recent_earning_dto import RecentEarningDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestMetricsByPeriodDto(unittest.TestCase):
-    """MetricsByPeriodDto unit test stubs"""
+class TestRecentEarningDto(unittest.TestCase):
+    """RecentEarningDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricsByPeriodDto(self):
-        """Test MetricsByPeriodDto"""
+    def testRecentEarningDto(self):
+        """Test RecentEarningDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.metrics_by_period_dto.MetricsByPeriodDto()  # noqa: E501
+        # model = investor8_sdk.models.recent_earning_dto.RecentEarningDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_metrics_metadata.py` & `investor8-sdk-1.1.9/test/test_metrics_metadata.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_metrics_metadata_response_dto.py` & `investor8-sdk-1.1.9/test/test_stock_popularity_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.metrics_metadata_response_dto import MetricsMetadataResponseDto  # noqa: E501
+from investor8_sdk.models.stock_popularity_dto import StockPopularityDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestMetricsMetadataResponseDto(unittest.TestCase):
-    """MetricsMetadataResponseDto unit test stubs"""
+class TestStockPopularityDto(unittest.TestCase):
+    """StockPopularityDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricsMetadataResponseDto(self):
-        """Test MetricsMetadataResponseDto"""
+    def testStockPopularityDto(self):
+        """Test StockPopularityDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.metrics_metadata_response_dto.MetricsMetadataResponseDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_popularity_dto.StockPopularityDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_momentum_metric_dto.py` & `investor8-sdk-1.1.9/test/test_momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_monthly_metrics.py` & `investor8-sdk-1.1.9/test/test_monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_monthly_returns.py` & `investor8-sdk-1.1.9/test/test_monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_news_api.py` & `investor8-sdk-1.1.9/test/test_news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_news_categories_dto.py` & `investor8-sdk-1.1.9/test/test_news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_news_source.py` & `investor8-sdk-1.1.9/test/test_news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_period_metric_value.py` & `investor8-sdk-1.1.9/test/test_period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_period_return.py` & `investor8-sdk-1.1.9/test/test_period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_plot.py` & `investor8-sdk-1.1.9/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_plot_detail_dto.py` & `investor8-sdk-1.1.9/test/test_plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_plot_dto.py` & `investor8-sdk-1.1.9/test/test_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_plot_response_dto.py` & `investor8-sdk-1.1.9/test/test_plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_previous_close_dto.py` & `investor8-sdk-1.1.9/test/test_previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_price_api.py` & `investor8-sdk-1.1.9/test/test_price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_profile_name.py` & `investor8-sdk-1.1.9/test/test_profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_recent_earning_dto.py` & `investor8-sdk-1.1.9/test/test_validate_watchlist_name_response_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.recent_earning_dto import RecentEarningDto  # noqa: E501
+from investor8_sdk.models.validate_watchlist_name_response_dto import ValidateWatchlistNameResponseDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestRecentEarningDto(unittest.TestCase):
-    """RecentEarningDto unit test stubs"""
+class TestValidateWatchlistNameResponseDto(unittest.TestCase):
+    """ValidateWatchlistNameResponseDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRecentEarningDto(self):
-        """Test RecentEarningDto"""
+    def testValidateWatchlistNameResponseDto(self):
+        """Test ValidateWatchlistNameResponseDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.recent_earning_dto.RecentEarningDto()  # noqa: E501
+        # model = investor8_sdk.models.validate_watchlist_name_response_dto.ValidateWatchlistNameResponseDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_remove_from_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_remove_from_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_rename_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_req_type.py` & `investor8-sdk-1.1.9/test/test_req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_reset_password_dto.py` & `investor8-sdk-1.1.9/test/test_reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_result_field.py` & `investor8-sdk-1.1.9/test/test_result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_return_metrics.py` & `investor8-sdk-1.1.9/test/test_return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_sa_attributes_prices.py` & `investor8-sdk-1.1.9/test/test_sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_sa_sector_price_dto.py` & `investor8-sdk-1.1.9/test/test_sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_screen.py` & `investor8-sdk-1.1.9/test/test_tag_info_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.screen import Screen  # noqa: E501
+from investor8_sdk.models.tag_info_dto import TagInfoDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestScreen(unittest.TestCase):
-    """Screen unit test stubs"""
+class TestTagInfoDto(unittest.TestCase):
+    """TagInfoDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScreen(self):
-        """Test Screen"""
+    def testTagInfoDto(self):
+        """Test TagInfoDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.screen.Screen()  # noqa: E501
+        # model = investor8_sdk.models.tag_info_dto.TagInfoDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_screen_dto.py` & `investor8-sdk-1.1.9/test/test_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
-    Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html  # noqa: E501
+    No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.screen_dto import ScreenDto  # noqa: E501
+from investor8_sdk.models.user import User  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestScreenDto(unittest.TestCase):
-    """ScreenDto unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScreenDto(self):
-        """Test ScreenDto"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.screen_dto.ScreenDto()  # noqa: E501
+        # model = investor8_sdk.models.user.User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_screener_api.py` & `investor8-sdk-1.1.9/test/test_screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_screening_condition.py` & `investor8-sdk-1.1.9/test/test_stock_news_details.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Investoreight Core API
+    Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
-    Contact: info@investoreight.com
+    OpenAPI spec version: 1.0
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.screening_condition import ScreeningCondition  # noqa: E501
+from investor8_sdk.models.stock_news_details import StockNewsDetails  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestScreeningCondition(unittest.TestCase):
-    """ScreeningCondition unit test stubs"""
+class TestStockNewsDetails(unittest.TestCase):
+    """StockNewsDetails unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScreeningCondition(self):
-        """Test ScreeningCondition"""
+    def testStockNewsDetails(self):
+        """Test StockNewsDetails"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.screening_condition.ScreeningCondition()  # noqa: E501
+        # model = investor8_sdk.models.stock_news_details.StockNewsDetails()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_search_api.py` & `investor8-sdk-1.1.9/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_sector_returns_dto.py` & `investor8-sdk-1.1.9/test/test_sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_send_email_dto.py` & `investor8-sdk-1.1.9/test/test_stock_price_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.send_email_dto import SendEmailDto  # noqa: E501
+from investor8_sdk.models.stock_price_dto import StockPriceDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestSendEmailDto(unittest.TestCase):
-    """SendEmailDto unit test stubs"""
+class TestStockPriceDto(unittest.TestCase):
+    """StockPriceDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSendEmailDto(self):
-        """Test SendEmailDto"""
+    def testStockPriceDto(self):
+        """Test StockPriceDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.send_email_dto.SendEmailDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_price_dto.StockPriceDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_settings_api.py` & `investor8-sdk-1.1.9/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_standardized_financial.py` & `investor8-sdk-1.1.9/test/test_standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_earning_dto.py` & `investor8-sdk-1.1.9/test/test_stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_financial.py` & `investor8-sdk-1.1.9/test/test_stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_info_api.py` & `investor8-sdk-1.1.9/test/test_stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_info_dto.py` & `investor8-sdk-1.1.9/test/test_stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_info_master_dto.py` & `investor8-sdk-1.1.9/test/test_stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_ipo.py` & `investor8-sdk-1.1.9/test/test_stock_news_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_ipo import StockIpo  # noqa: E501
+from investor8_sdk.models.stock_news_status import StockNewsStatus  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockIpo(unittest.TestCase):
-    """StockIpo unit test stubs"""
+class TestStockNewsStatus(unittest.TestCase):
+    """StockNewsStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockIpo(self):
-        """Test StockIpo"""
+    def testStockNewsStatus(self):
+        """Test StockNewsStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_ipo.StockIpo()  # noqa: E501
+        # model = investor8_sdk.models.stock_news_status.StockNewsStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_news_details.py` & `investor8-sdk-1.1.9/test/test_value_metrics_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_news_details import StockNewsDetails  # noqa: E501
+from investor8_sdk.models.value_metrics_dto import ValueMetricsDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockNewsDetails(unittest.TestCase):
-    """StockNewsDetails unit test stubs"""
+class TestValueMetricsDto(unittest.TestCase):
+    """ValueMetricsDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockNewsDetails(self):
-        """Test StockNewsDetails"""
+    def testValueMetricsDto(self):
+        """Test ValueMetricsDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_news_details.StockNewsDetails()  # noqa: E501
+        # model = investor8_sdk.models.value_metrics_dto.ValueMetricsDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_news_status.py` & `investor8-sdk-1.1.9/test/test_tag_details_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_news_status import StockNewsStatus  # noqa: E501
+from investor8_sdk.models.tag_details_dto import TagDetailsDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockNewsStatus(unittest.TestCase):
-    """StockNewsStatus unit test stubs"""
+class TestTagDetailsDto(unittest.TestCase):
+    """TagDetailsDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockNewsStatus(self):
-        """Test StockNewsStatus"""
+    def testTagDetailsDto(self):
+        """Test TagDetailsDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_news_status.StockNewsStatus()  # noqa: E501
+        # model = investor8_sdk.models.tag_details_dto.TagDetailsDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/test/test_stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_popularity_dto.py` & `investor8-sdk-1.1.9/test/test_stock_summary_dto.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_popularity_dto import StockPopularityDto  # noqa: E501
+from investor8_sdk.models.stock_summary_dto import StockSummaryDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockPopularityDto(unittest.TestCase):
-    """StockPopularityDto unit test stubs"""
+class TestStockSummaryDto(unittest.TestCase):
+    """StockSummaryDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockPopularityDto(self):
-        """Test StockPopularityDto"""
+    def testStockSummaryDto(self):
+        """Test StockSummaryDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_popularity_dto.StockPopularityDto()  # noqa: E501
+        # model = investor8_sdk.models.stock_summary_dto.StockSummaryDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_price.py` & `investor8-sdk-1.1.9/test/test_watchlist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_price import StockPrice  # noqa: E501
+from investor8_sdk.models.watchlist import Watchlist  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockPrice(unittest.TestCase):
-    """StockPrice unit test stubs"""
+class TestWatchlist(unittest.TestCase):
+    """Watchlist unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockPrice(self):
-        """Test StockPrice"""
+    def testWatchlist(self):
+        """Test Watchlist"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_price.StockPrice()  # noqa: E501
+        # model = investor8_sdk.models.watchlist.Watchlist()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_price_dto.py` & `investor8-sdk-1.1.9/test/test_update_plot_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_price_dto import StockPriceDto  # noqa: E501
+from investor8_sdk.models.update_plot_dto import UpdatePlotDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockPriceDto(unittest.TestCase):
-    """StockPriceDto unit test stubs"""
+class TestUpdatePlotDto(unittest.TestCase):
+    """UpdatePlotDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockPriceDto(self):
-        """Test StockPriceDto"""
+    def testUpdatePlotDto(self):
+        """Test UpdatePlotDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_price_dto.StockPriceDto()  # noqa: E501
+        # model = investor8_sdk.models.update_plot_dto.UpdatePlotDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_stock_rating_dto.py` & `investor8-sdk-1.1.9/test/test_stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_stock_summary_dto.py` & `investor8-sdk-1.1.9/test/test_update_watchlist_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.stock_summary_dto import StockSummaryDto  # noqa: E501
+from investor8_sdk.models.update_watchlist_dto import UpdateWatchlistDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestStockSummaryDto(unittest.TestCase):
-    """StockSummaryDto unit test stubs"""
+class TestUpdateWatchlistDto(unittest.TestCase):
+    """UpdateWatchlistDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStockSummaryDto(self):
-        """Test StockSummaryDto"""
+    def testUpdateWatchlistDto(self):
+        """Test UpdateWatchlistDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.stock_summary_dto.StockSummaryDto()  # noqa: E501
+        # model = investor8_sdk.models.update_watchlist_dto.UpdateWatchlistDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_string_message_result.py` & `investor8-sdk-1.1.9/test/test_string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.80/test/test_symbols_current_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_validate_watchlist_name_request_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.symbols_current_metrics_dto import SymbolsCurrentMetricsDto  # noqa: E501
+from investor8_sdk.models.validate_watchlist_name_request_dto import ValidateWatchlistNameRequestDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestSymbolsCurrentMetricsDto(unittest.TestCase):
-    """SymbolsCurrentMetricsDto unit test stubs"""
+class TestValidateWatchlistNameRequestDto(unittest.TestCase):
+    """ValidateWatchlistNameRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSymbolsCurrentMetricsDto(self):
-        """Test SymbolsCurrentMetricsDto"""
+    def testValidateWatchlistNameRequestDto(self):
+        """Test ValidateWatchlistNameRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.symbols_current_metrics_dto.SymbolsCurrentMetricsDto()  # noqa: E501
+        # model = investor8_sdk.models.validate_watchlist_name_request_dto.ValidateWatchlistNameRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_symbols_historical_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_upcoming_earning_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.symbols_historical_metrics_dto import SymbolsHistoricalMetricsDto  # noqa: E501
+from investor8_sdk.models.upcoming_earning_dto import UpcomingEarningDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestSymbolsHistoricalMetricsDto(unittest.TestCase):
-    """SymbolsHistoricalMetricsDto unit test stubs"""
+class TestUpcomingEarningDto(unittest.TestCase):
+    """UpcomingEarningDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSymbolsHistoricalMetricsDto(self):
-        """Test SymbolsHistoricalMetricsDto"""
+    def testUpcomingEarningDto(self):
+        """Test UpcomingEarningDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.symbols_historical_metrics_dto.SymbolsHistoricalMetricsDto()  # noqa: E501
+        # model = investor8_sdk.models.upcoming_earning_dto.UpcomingEarningDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_tag_details_dto.py` & `investor8-sdk-1.1.9/test/test_watchlist_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Investor8.Core
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.0.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.tag_details_dto import TagDetailsDto  # noqa: E501
+from investor8_sdk.models.watchlist_dto import WatchlistDto  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestTagDetailsDto(unittest.TestCase):
-    """TagDetailsDto unit test stubs"""
+class TestWatchlistDto(unittest.TestCase):
+    """WatchlistDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTagDetailsDto(self):
-        """Test TagDetailsDto"""
+    def testWatchlistDto(self):
+        """Test WatchlistDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.tag_details_dto.TagDetailsDto()  # noqa: E501
+        # model = investor8_sdk.models.watchlist_dto.WatchlistDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_tag_info_dto.py` & `investor8-sdk-1.1.9/test/test_tags_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,29 +11,41 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import investor8_sdk
-from investor8_sdk.models.tag_info_dto import TagInfoDto  # noqa: E501
+from investor8_sdk.api.tags_api import TagsApi  # noqa: E501
 from investor8_sdk.rest import ApiException
 
 
-class TestTagInfoDto(unittest.TestCase):
-    """TagInfoDto unit test stubs"""
+class TestTagsApi(unittest.TestCase):
+    """TagsApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = TagsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testTagInfoDto(self):
-        """Test TagInfoDto"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = investor8_sdk.models.tag_info_dto.TagInfoDto()  # noqa: E501
+    def test_get_all_tags_info(self):
+        """Test case for get_all_tags_info
+
+        """
+        pass
+
+    def test_get_all_ticker_tags(self):
+        """Test case for get_all_ticker_tags
+
+        """
+        pass
+
+    def test_get_tag_details(self):
+        """Test case for get_tag_details
+
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `investor8-sdk-1.1.80/test/test_user_api.py` & `investor8-sdk-1.1.9/test/test_user_api.py`

 * *Files identical despite different names*

