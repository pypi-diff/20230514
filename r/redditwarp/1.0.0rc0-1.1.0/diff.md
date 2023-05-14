# Comparing `tmp/redditwarp-1.0.0rc0.tar.gz` & `tmp/redditwarp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redditwarp-1.0.0rc0.tar", max compression
+gzip compressed data, was "redditwarp-1.1.0.tar", max compression
```

## Comparing `redditwarp-1.0.0rc0.tar` & `redditwarp-1.1.0.tar`

### file list

```diff
@@ -1,544 +1,565 @@
--rw-r--r--   0        0        0     1065 2023-04-04 13:06:30.364674 redditwarp-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     5927 2023-04-04 13:06:30.365266 redditwarp-1.0.0rc0/README.md
--rw-r--r--   0        0        0     1220 2023-04-04 13:06:30.390443 redditwarp-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      194 2023-04-04 13:06:07.292958 redditwarp-1.0.0rc0/redditwarp/ASYNC.py
--rw-r--r--   0        0        0      192 2023-04-04 13:06:07.293146 redditwarp-1.0.0rc0/redditwarp/SYNC.py
--rw-r--r--   0        0        0     3310 2023-04-04 13:06:07.293545 redditwarp-1.0.0rc0/redditwarp/__about__.py
--rw-r--r--   0        0        0      883 2023-04-04 13:06:07.293854 redditwarp-1.0.0rc0/redditwarp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.294111 redditwarp-1.0.0rc0/redditwarp/_cli/__init__.pyi
--rw-r--r--   0        0        0      227 2023-04-04 13:06:07.294634 redditwarp-1.0.0rc0/redditwarp/_cli/access_token.py
--rw-r--r--   0        0        0     8012 2023-04-04 13:06:07.295008 redditwarp-1.0.0rc0/redditwarp/_cli/comment_tree.py
--rw-r--r--   0        0        0     3201 2023-04-04 13:06:07.295249 redditwarp-1.0.0rc0/redditwarp/_cli/exchange_authorization_code.py
--rw-r--r--   0        0        0     3901 2023-04-04 13:06:07.295462 redditwarp-1.0.0rc0/redditwarp/_cli/implicit_flow.py
--rw-r--r--   0        0        0     5909 2023-04-04 13:06:07.295678 redditwarp-1.0.0rc0/redditwarp/_cli/refresh_token.py
--rw-r--r--   0        0        0     3045 2023-04-04 13:06:07.295923 redditwarp-1.0.0rc0/redditwarp/_cli/revoke_token.py
--rw-r--r--   0        0        0      325 2023-04-04 13:06:07.296711 redditwarp-1.0.0rc0/redditwarp/auth/ASYNC.py
--rw-r--r--   0        0        0      321 2023-04-04 13:06:07.296968 redditwarp-1.0.0rc0/redditwarp/auth/SYNC.py
--rw-r--r--   0        0        0      313 2023-04-04 13:06:07.297313 redditwarp-1.0.0rc0/redditwarp/auth/__init__.py
--rw-r--r--   0        0        0     5356 2023-04-04 13:06:07.297679 redditwarp-1.0.0rc0/redditwarp/auth/exceptions.py
--rw-r--r--   0        0        0     2067 2023-04-04 13:06:07.298023 redditwarp-1.0.0rc0/redditwarp/auth/grants.py
--rw-r--r--   0        0        0     1142 2023-04-04 13:06:07.298334 redditwarp-1.0.0rc0/redditwarp/auth/token.py
--rw-r--r--   0        0        0     3120 2023-04-04 13:06:07.299179 redditwarp-1.0.0rc0/redditwarp/auth/token_obtainment_client_ASYNC.py
--rw-r--r--   0        0        0     3094 2023-04-04 13:06:07.299826 redditwarp-1.0.0rc0/redditwarp/auth/token_obtainment_client_SYNC.py
--rw-r--r--   0        0        0     2617 2023-04-04 13:06:07.300475 redditwarp-1.0.0rc0/redditwarp/auth/token_revocation_client_ASYNC.py
--rw-r--r--   0        0        0     2579 2023-04-04 13:06:07.301108 redditwarp-1.0.0rc0/redditwarp/auth/token_revocation_client_SYNC.py
--rw-r--r--   0        0        0      111 2023-04-04 13:06:07.301476 redditwarp-1.0.0rc0/redditwarp/auth/types.py
--rw-r--r--   0        0        0     1413 2023-04-04 13:06:07.301783 redditwarp-1.0.0rc0/redditwarp/auth/utils.py
--rw-r--r--   0        0        0     5519 2023-04-04 13:06:07.302451 redditwarp-1.0.0rc0/redditwarp/client_ASYNC.py
--rw-r--r--   0        0        0     9566 2023-04-04 13:06:07.303213 redditwarp-1.0.0rc0/redditwarp/client_SYNC.py
--rw-r--r--   0        0        0      565 2023-04-04 13:06:07.303868 redditwarp-1.0.0rc0/redditwarp/core/ASYNC.py
--rw-r--r--   0        0        0      557 2023-04-04 13:06:07.304232 redditwarp-1.0.0rc0/redditwarp/core/SYNC.py
--rw-r--r--   0        0        0      247 2023-04-04 13:06:07.304494 redditwarp-1.0.0rc0/redditwarp/core/__init__.py
--rw-r--r--   0        0        0     6813 2023-04-04 13:06:07.305105 redditwarp-1.0.0rc0/redditwarp/core/authorizer_ASYNC.py
--rw-r--r--   0        0        0     6395 2023-04-04 13:06:07.305709 redditwarp-1.0.0rc0/redditwarp/core/authorizer_SYNC.py
--rw-r--r--   0        0        0      957 2023-04-04 13:06:07.306305 redditwarp-1.0.0rc0/redditwarp/core/const.py
--rw-r--r--   0        0        0      885 2023-04-04 13:06:07.306919 redditwarp-1.0.0rc0/redditwarp/core/direct_by_origin_ASYNC.py
--rw-r--r--   0        0        0      865 2023-04-04 13:06:07.307497 redditwarp-1.0.0rc0/redditwarp/core/direct_by_origin_SYNC.py
--rw-r--r--   0        0        0     4146 2023-04-04 13:06:07.307882 redditwarp-1.0.0rc0/redditwarp/core/exceptions.py
--rw-r--r--   0        0        0      362 2023-04-04 13:06:07.308266 redditwarp-1.0.0rc0/redditwarp/core/grants.py
--rw-r--r--   0        0        0     4667 2023-04-04 13:06:07.308977 redditwarp-1.0.0rc0/redditwarp/core/http_client_ASYNC.py
--rw-r--r--   0        0        0     4642 2023-04-04 13:06:07.309586 redditwarp-1.0.0rc0/redditwarp/core/http_client_SYNC.py
--rw-r--r--   0        0        0     2746 2023-04-04 13:06:07.310295 redditwarp-1.0.0rc0/redditwarp/core/rate_limited_ASYNC.py
--rw-r--r--   0        0        0     2030 2023-04-04 13:06:07.310870 redditwarp-1.0.0rc0/redditwarp/core/rate_limited_SYNC.py
--rw-r--r--   0        0        0     4078 2023-04-04 13:06:07.311526 redditwarp-1.0.0rc0/redditwarp/core/recorded_ASYNC.py
--rw-r--r--   0        0        0     4064 2023-04-04 13:06:07.312153 redditwarp-1.0.0rc0/redditwarp/core/recorded_SYNC.py
--rw-r--r--   0        0        0      859 2023-04-04 13:06:07.312958 redditwarp-1.0.0rc0/redditwarp/core/reddit_please_send_json_ASYNC.py
--rw-r--r--   0        0        0      845 2023-04-04 13:06:07.313666 redditwarp-1.0.0rc0/redditwarp/core/reddit_please_send_json_SYNC.py
--rw-r--r--   0        0        0     1186 2023-04-04 13:06:07.314287 redditwarp-1.0.0rc0/redditwarp/core/reddit_token_obtainment_client_ASYNC.py
--rw-r--r--   0        0        0     1173 2023-04-04 13:06:07.314938 redditwarp-1.0.0rc0/redditwarp/core/reddit_token_obtainment_client_SYNC.py
--rw-r--r--   0        0        0      524 2023-04-04 13:06:07.315224 redditwarp-1.0.0rc0/redditwarp/core/user_agent_ASYNC.py
--rw-r--r--   0        0        0      523 2023-04-04 13:06:07.315568 redditwarp-1.0.0rc0/redditwarp/core/user_agent_SYNC.py
--rw-r--r--   0        0        0       58 2023-04-04 13:06:07.315867 redditwarp-1.0.0rc0/redditwarp/dark/ASYNC.py
--rw-r--r--   0        0        0       57 2023-04-04 13:06:07.316145 redditwarp-1.0.0rc0/redditwarp/dark/SYNC.py
--rw-r--r--   0        0        0       67 2023-04-04 13:06:07.316361 redditwarp-1.0.0rc0/redditwarp/dark/__init__.py
--rw-r--r--   0        0        0      163 2023-04-04 13:06:07.316623 redditwarp-1.0.0rc0/redditwarp/dark/auth/ASYNC.py
--rw-r--r--   0        0        0      161 2023-04-04 13:06:07.316801 redditwarp-1.0.0rc0/redditwarp/dark/auth/SYNC.py
--rw-r--r--   0        0        0      122 2023-04-04 13:06:07.317677 redditwarp-1.0.0rc0/redditwarp/dark/auth/__init__.py
--rw-r--r--   0        0        0     1166 2023-04-04 13:06:07.318343 redditwarp-1.0.0rc0/redditwarp/dark/auth/exceptions.py
--rw-r--r--   0        0        0      821 2023-04-04 13:06:07.318610 redditwarp-1.0.0rc0/redditwarp/dark/auth/token.py
--rw-r--r--   0        0        0     1666 2023-04-04 13:06:07.319201 redditwarp-1.0.0rc0/redditwarp/dark/auth/token_obtainment_client_ASYNC.py
--rw-r--r--   0        0        0     1641 2023-04-04 13:06:07.319777 redditwarp-1.0.0rc0/redditwarp/dark/auth/token_obtainment_client_SYNC.py
--rw-r--r--   0        0        0      732 2023-04-04 13:06:07.320330 redditwarp-1.0.0rc0/redditwarp/dark/client_ASYNC.py
--rw-r--r--   0        0        0      729 2023-04-04 13:06:07.320901 redditwarp-1.0.0rc0/redditwarp/dark/client_SYNC.py
--rw-r--r--   0        0        0       35 2023-04-04 13:06:07.321198 redditwarp-1.0.0rc0/redditwarp/dark/core/__init__.py
--rw-r--r--   0        0        0     4294 2023-04-04 13:06:07.321810 redditwarp-1.0.0rc0/redditwarp/dark/core/authorizer_ASYNC.py
--rw-r--r--   0        0        0     3876 2023-04-04 13:06:07.322596 redditwarp-1.0.0rc0/redditwarp/dark/core/authorizer_SYNC.py
--rw-r--r--   0        0        0      954 2023-04-04 13:06:07.323217 redditwarp-1.0.0rc0/redditwarp/dark/core/const.py
--rw-r--r--   0        0        0     2206 2023-04-04 13:06:07.323830 redditwarp-1.0.0rc0/redditwarp/dark/core/http_client_ASYNC.py
--rw-r--r--   0        0        0     2195 2023-04-04 13:06:07.324269 redditwarp-1.0.0rc0/redditwarp/dark/core/http_client_SYNC.py
--rw-r--r--   0        0        0      780 2023-04-04 13:06:07.324794 redditwarp-1.0.0rc0/redditwarp/dark/core/rate_limited_ASYNC.py
--rw-r--r--   0        0        0      658 2023-04-04 13:06:07.325055 redditwarp-1.0.0rc0/redditwarp/dark/core/rate_limited_SYNC.py
--rw-r--r--   0        0        0      916 2023-04-04 13:06:07.325788 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/ASYNC.py
--rw-r--r--   0        0        0      890 2023-04-04 13:06:07.326405 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.326579 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/__init__.py
--rw-r--r--   0        0        0     4112 2023-04-04 13:06:07.327590 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/login/ASYNC.py
--rw-r--r--   0        0        0     4069 2023-04-04 13:06:07.328253 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/login/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.328441 redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/login/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.328755 redditwarp-1.0.0rc0/redditwarp/dark/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-04-04 13:06:07.329910 redditwarp-1.0.0rc0/redditwarp/dark/util/request_signing.py
--rw-r--r--   0        0        0      101 2023-04-04 13:06:07.331734 redditwarp-1.0.0rc0/redditwarp/dtos/__init__.py
--rw-r--r--   0        0        0      124 2023-04-04 13:06:07.332098 redditwarp-1.0.0rc0/redditwarp/dtos/submission.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.332427 redditwarp-1.0.0rc0/redditwarp/dtos/widget/__init__.py
--rw-r--r--   0        0        0      775 2023-04-04 13:06:07.332708 redditwarp-1.0.0rc0/redditwarp/dtos/widget/button.py
--rw-r--r--   0        0        0      228 2023-04-04 13:06:07.332947 redditwarp-1.0.0rc0/redditwarp/dtos/widget/custom_css.py
--rw-r--r--   0        0        0      175 2023-04-04 13:06:07.333448 redditwarp-1.0.0rc0/redditwarp/dtos/widget/image.py
--rw-r--r--   0        0        0      400 2023-04-04 13:06:07.334101 redditwarp-1.0.0rc0/redditwarp/dtos/widget/menu_bar.py
--rw-r--r--   0        0        0     6794 2023-04-04 13:06:07.335705 redditwarp-1.0.0rc0/redditwarp/exceptions.py
--rw-r--r--   0        0        0      363 2023-04-04 13:06:07.336448 redditwarp-1.0.0rc0/redditwarp/http/ASYNC.py
--rw-r--r--   0        0        0      357 2023-04-04 13:06:07.336790 redditwarp-1.0.0rc0/redditwarp/http/SYNC.py
--rw-r--r--   0        0        0      725 2023-04-04 13:06:07.337267 redditwarp-1.0.0rc0/redditwarp/http/__init__.py
--rw-r--r--   0        0        0      498 2023-04-04 13:06:07.337671 redditwarp-1.0.0rc0/redditwarp/http/delegating_handler_ASYNC.py
--rw-r--r--   0        0        0      473 2023-04-04 13:06:07.338009 redditwarp-1.0.0rc0/redditwarp/http/delegating_handler_SYNC.py
--rw-r--r--   0        0        0     4709 2023-04-04 13:06:07.339047 redditwarp-1.0.0rc0/redditwarp/http/exceptions.py
--rw-r--r--   0        0        0      397 2023-04-04 13:06:07.339783 redditwarp-1.0.0rc0/redditwarp/http/exchange.py
--rw-r--r--   0        0        0      317 2023-04-04 13:06:07.340179 redditwarp-1.0.0rc0/redditwarp/http/handler_ASYNC.py
--rw-r--r--   0        0        0      305 2023-04-04 13:06:07.340525 redditwarp-1.0.0rc0/redditwarp/http/handler_SYNC.py
--rw-r--r--   0        0        0     4205 2023-04-04 13:06:07.341213 redditwarp-1.0.0rc0/redditwarp/http/http_client_ASYNC.py
--rw-r--r--   0        0        0     4123 2023-04-04 13:06:07.341953 redditwarp-1.0.0rc0/redditwarp/http/http_client_SYNC.py
--rw-r--r--   0        0        0      407 2023-04-04 13:06:07.342251 redditwarp-1.0.0rc0/redditwarp/http/invoker_ASYNC.py
--rw-r--r--   0        0        0      382 2023-04-04 13:06:07.342512 redditwarp-1.0.0rc0/redditwarp/http/invoker_SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.342743 redditwarp-1.0.0rc0/redditwarp/http/misc/__init__.py
--rw-r--r--   0        0        0     3315 2023-04-04 13:06:07.343244 redditwarp-1.0.0rc0/redditwarp/http/misc/apply_params_and_headers_ASYNC.py
--rw-r--r--   0        0        0     3241 2023-04-04 13:06:07.343771 redditwarp-1.0.0rc0/redditwarp/http/misc/apply_params_and_headers_SYNC.py
--rw-r--r--   0        0        0      145 2023-04-04 13:06:07.344026 redditwarp-1.0.0rc0/redditwarp/http/misc/block_close_ASYNC.py
--rw-r--r--   0        0        0      138 2023-04-04 13:06:07.344231 redditwarp-1.0.0rc0/redditwarp/http/misc/block_close_SYNC.py
--rw-r--r--   0        0        0     1651 2023-04-04 13:06:07.344678 redditwarp-1.0.0rc0/redditwarp/http/misc/demultiplexer_ASYNC.py
--rw-r--r--   0        0        0     1759 2023-04-04 13:06:07.345171 redditwarp-1.0.0rc0/redditwarp/http/misc/demultiplexer_SYNC.py
--rw-r--r--   0        0        0     3958 2023-04-04 13:06:07.345971 redditwarp-1.0.0rc0/redditwarp/http/payload.py
--rw-r--r--   0        0        0      378 2023-04-04 13:06:07.346229 redditwarp-1.0.0rc0/redditwarp/http/request.py
--rw-r--r--   0        0        0     1376 2023-04-04 13:06:07.346420 redditwarp-1.0.0rc0/redditwarp/http/requisition.py
--rw-r--r--   0        0        0     1104 2023-04-04 13:06:07.347100 redditwarp-1.0.0rc0/redditwarp/http/response.py
--rw-r--r--   0        0        0      323 2023-04-04 13:06:07.347405 redditwarp-1.0.0rc0/redditwarp/http/send_params.py
--rw-r--r--   0        0        0       31 2023-04-04 13:06:07.347734 redditwarp-1.0.0rc0/redditwarp/http/transport/__init__.py
--rw-r--r--   0        0        0      109 2023-04-04 13:06:07.347946 redditwarp-1.0.0rc0/redditwarp/http/transport/connector_ASYNC.py
--rw-r--r--   0        0        0      108 2023-04-04 13:06:07.348134 redditwarp-1.0.0rc0/redditwarp/http/transport/connector_SYNC.py
--rw-r--r--   0        0        0      805 2023-04-04 13:06:07.348422 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/__init__.py
--rw-r--r--   0        0        0     4600 2023-04-04 13:06:07.349059 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/aiohttp.py
--rw-r--r--   0        0        0      125 2023-04-04 13:06:07.349434 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/httpx.py
--rw-r--r--   0        0        0     4210 2023-04-04 13:06:07.350583 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/httpx_async.py
--rw-r--r--   0        0        0     4161 2023-04-04 13:06:07.351484 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/httpx_sync.py
--rw-r--r--   0        0        0     3557 2023-04-04 13:06:07.352004 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/python_urllib.py
--rw-r--r--   0        0        0     4227 2023-04-04 13:06:07.352620 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/requests.py
--rw-r--r--   0        0        0     5291 2023-04-04 13:06:07.353291 redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/urllib3.py
--rw-r--r--   0        0        0     1677 2023-04-04 13:06:07.353942 redditwarp-1.0.0rc0/redditwarp/http/transport/reg_ASYNC.py
--rw-r--r--   0        0        0     1784 2023-04-04 13:06:07.354400 redditwarp-1.0.0rc0/redditwarp/http/transport/reg_SYNC.py
--rw-r--r--   0        0        0      258 2023-04-04 13:06:07.354780 redditwarp-1.0.0rc0/redditwarp/http/types.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.355117 redditwarp-1.0.0rc0/redditwarp/http/util/__init__.py
--rw-r--r--   0        0        0     2794 2023-04-04 13:06:07.355373 redditwarp-1.0.0rc0/redditwarp/http/util/case_insensitive_dict.py
--rw-r--r--   0        0        0      204 2023-04-04 13:06:07.355685 redditwarp-1.0.0rc0/redditwarp/http/util/guess_filename_mimetype.py
--rw-r--r--   0        0        0     1265 2023-04-04 13:06:07.356239 redditwarp-1.0.0rc0/redditwarp/http/util/json_loading.py
--rw-r--r--   0        0        0     1915 2023-04-04 13:06:07.356780 redditwarp-1.0.0rc0/redditwarp/http/util/locked_keys_mapping_proxy.py
--rw-r--r--   0        0        0      980 2023-04-04 13:06:07.357017 redditwarp-1.0.0rc0/redditwarp/http/util/merge_query_params.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.357314 redditwarp-1.0.0rc0/redditwarp/iterators/__init__.py
--rw-r--r--   0        0        0      612 2023-04-04 13:06:07.357985 redditwarp-1.0.0rc0/redditwarp/iterators/async_call_chunk.py
--rw-r--r--   0        0        0      562 2023-04-04 13:06:07.358395 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk.py
--rw-r--r--   0        0        0     1216 2023-04-04 13:06:07.358630 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_calling_async_iterator.py
--rw-r--r--   0        0        0     1084 2023-04-04 13:06:07.358953 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_calling_iterator.py
--rw-r--r--   0        0        0     1746 2023-04-04 13:06:07.359237 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_chaining_async_iterator.py
--rw-r--r--   0        0        0     1593 2023-04-04 13:06:07.359491 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_chaining_iterator.py
--rw-r--r--   0        0        0      329 2023-04-04 13:06:07.359760 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunking_async1.py
--rw-r--r--   0        0        0      281 2023-04-04 13:06:07.360024 redditwarp-1.0.0rc0/redditwarp/iterators/call_chunking_sync1.py
--rw-r--r--   0        0        0      800 2023-04-04 13:06:07.362384 redditwarp-1.0.0rc0/redditwarp/iterators/chunking.py
--rw-r--r--   0        0        0     1027 2023-04-04 13:06:07.363641 redditwarp-1.0.0rc0/redditwarp/iterators/stubborn_caller_async_iterator.py
--rw-r--r--   0        0        0      864 2023-04-04 13:06:07.364342 redditwarp-1.0.0rc0/redditwarp/iterators/stubborn_caller_iterator.py
--rw-r--r--   0        0        0      965 2023-04-04 13:06:07.364948 redditwarp-1.0.0rc0/redditwarp/iterators/unfaltering_chaining_async_iterator.py
--rw-r--r--   0        0        0      773 2023-04-04 13:06:07.365486 redditwarp-1.0.0rc0/redditwarp/iterators/unfaltering_chaining_iterator.py
--rw-r--r--   0        0        0       21 2023-04-04 13:06:07.366224 redditwarp-1.0.0rc0/redditwarp/model_loaders/__init__.py
--rw-r--r--   0        0        0      422 2023-04-04 13:06:07.366561 redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_ASYNC.py
--rw-r--r--   0        0        0      420 2023-04-04 13:06:07.366876 redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_SYNC.py
--rw-r--r--   0        0        0     4087 2023-04-04 13:06:07.367246 redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_tree_ASYNC.py
--rw-r--r--   0        0        0     4080 2023-04-04 13:06:07.367601 redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_tree_SYNC.py
--rw-r--r--   0        0        0      298 2023-04-04 13:06:07.367907 redditwarp-1.0.0rc0/redditwarp/model_loaders/custom_feed_ASYNC.py
--rw-r--r--   0        0        0      296 2023-04-04 13:06:07.368169 redditwarp-1.0.0rc0/redditwarp/model_loaders/custom_feed_SYNC.py
--rw-r--r--   0        0        0     2116 2023-04-04 13:06:07.368497 redditwarp-1.0.0rc0/redditwarp/model_loaders/flair.py
--rw-r--r--   0        0        0     1068 2023-04-04 13:06:07.368825 redditwarp-1.0.0rc0/redditwarp/model_loaders/flair_emoji.py
--rw-r--r--   0        0        0      346 2023-04-04 13:06:07.369134 redditwarp-1.0.0rc0/redditwarp/model_loaders/karma_breakdown_entry.py
--rw-r--r--   0        0        0      418 2023-04-04 13:06:07.369417 redditwarp-1.0.0rc0/redditwarp/model_loaders/live_thread_ASYNC.py
--rw-r--r--   0        0        0      416 2023-04-04 13:06:07.369707 redditwarp-1.0.0rc0/redditwarp/model_loaders/live_thread_SYNC.py
--rw-r--r--   0        0        0      730 2023-04-04 13:06:07.370001 redditwarp-1.0.0rc0/redditwarp/model_loaders/media_upload_lease.py
--rw-r--r--   0        0        0     3906 2023-04-04 13:06:07.370720 redditwarp-1.0.0rc0/redditwarp/model_loaders/message.py
--rw-r--r--   0        0        0     1920 2023-04-04 13:06:07.371113 redditwarp-1.0.0rc0/redditwarp/model_loaders/message_ASYNC.py
--rw-r--r--   0        0        0     1918 2023-04-04 13:06:07.371441 redditwarp-1.0.0rc0/redditwarp/model_loaders/message_SYNC.py
--rw-r--r--   0        0        0      237 2023-04-04 13:06:07.371739 redditwarp-1.0.0rc0/redditwarp/model_loaders/moderated_subreddit.py
--rw-r--r--   0        0        0      582 2023-04-04 13:06:07.372054 redditwarp-1.0.0rc0/redditwarp/model_loaders/moderation_action_log_entry.py
--rw-r--r--   0        0        0     2199 2023-04-04 13:06:07.372453 redditwarp-1.0.0rc0/redditwarp/model_loaders/moderation_note.py
--rw-r--r--   0        0        0      229 2023-04-04 13:06:07.372747 redditwarp-1.0.0rc0/redditwarp/model_loaders/moderator_list.py
--rw-r--r--   0        0        0      334 2023-04-04 13:06:07.373054 redditwarp-1.0.0rc0/redditwarp/model_loaders/modmail.py
--rw-r--r--   0        0        0     4832 2023-04-04 13:06:07.373395 redditwarp-1.0.0rc0/redditwarp/model_loaders/modmail_ASYNC.py
--rw-r--r--   0        0        0     4830 2023-04-04 13:06:07.373806 redditwarp-1.0.0rc0/redditwarp/model_loaders/modmail_SYNC.py
--rw-r--r--   0        0        0      290 2023-04-04 13:06:07.374115 redditwarp-1.0.0rc0/redditwarp/model_loaders/my_account_ASYNC.py
--rw-r--r--   0        0        0      288 2023-04-04 13:06:07.374413 redditwarp-1.0.0rc0/redditwarp/model_loaders/my_account_SYNC.py
--rw-r--r--   0        0        0      517 2023-04-04 13:06:07.374911 redditwarp-1.0.0rc0/redditwarp/model_loaders/report.py
--rw-r--r--   0        0        0      432 2023-04-04 13:06:07.375224 redditwarp-1.0.0rc0/redditwarp/model_loaders/stylesheet.py
--rw-r--r--   0        0        0     1131 2023-04-04 13:06:07.375542 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission.py
--rw-r--r--   0        0        0     1357 2023-04-04 13:06:07.375831 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_ASYNC.py
--rw-r--r--   0        0        0     1354 2023-04-04 13:06:07.376120 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_SYNC.py
--rw-r--r--   0        0        0      525 2023-04-04 13:06:07.376438 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_collection_ASYNC.py
--rw-r--r--   0        0        0      523 2023-04-04 13:06:07.376837 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_collection_SYNC.py
--rw-r--r--   0        0        0     5355 2023-04-04 13:06:07.377173 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft.py
--rw-r--r--   0        0        0      576 2023-04-04 13:06:07.377519 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft_ASYNC.py
--rw-r--r--   0        0        0      573 2023-04-04 13:06:07.377830 redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft_SYNC.py
--rw-r--r--   0        0        0      524 2023-04-04 13:06:07.378147 redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_ASYNC.py
--rw-r--r--   0        0        0      522 2023-04-04 13:06:07.378472 redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_SYNC.py
--rw-r--r--   0        0        0      217 2023-04-04 13:06:07.378784 redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_rules.py
--rw-r--r--   0        0        0      687 2023-04-04 13:06:07.379098 redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_style_asset_upload_lease.py
--rw-r--r--   0        0        0      508 2023-04-04 13:06:07.379484 redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_user.py
--rw-r--r--   0        0        0      320 2023-04-04 13:06:07.379816 redditwarp-1.0.0rc0/redditwarp/model_loaders/trophy.py
--rw-r--r--   0        0        0      472 2023-04-04 13:06:07.380120 redditwarp-1.0.0rc0/redditwarp/model_loaders/user_ASYNC.py
--rw-r--r--   0        0        0      470 2023-04-04 13:06:07.380816 redditwarp-1.0.0rc0/redditwarp/model_loaders/user_SYNC.py
--rw-r--r--   0        0        0      533 2023-04-04 13:06:07.381102 redditwarp-1.0.0rc0/redditwarp/model_loaders/user_relationship.py
--rw-r--r--   0        0        0      219 2023-04-04 13:06:07.381403 redditwarp-1.0.0rc0/redditwarp/model_loaders/user_summary.py
--rw-r--r--   0        0        0      652 2023-04-04 13:06:07.381705 redditwarp-1.0.0rc0/redditwarp/model_loaders/widget.py
--rw-r--r--   0        0        0    10188 2023-04-04 13:06:07.382033 redditwarp-1.0.0rc0/redditwarp/model_loaders/widget_ASYNC.py
--rw-r--r--   0        0        0    10187 2023-04-04 13:06:07.382378 redditwarp-1.0.0rc0/redditwarp/model_loaders/widget_SYNC.py
--rw-r--r--   0        0        0     1320 2023-04-04 13:06:07.382683 redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki.py
--rw-r--r--   0        0        0     2017 2023-04-04 13:06:07.382997 redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki_ASYNC.py
--rw-r--r--   0        0        0     2015 2023-04-04 13:06:07.383480 redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki_SYNC.py
--rw-r--r--   0        0        0       86 2023-04-04 13:06:07.383973 redditwarp-1.0.0rc0/redditwarp/models/__init__.py
--rw-r--r--   0        0        0    14381 2023-04-04 13:06:07.384750 redditwarp-1.0.0rc0/redditwarp/models/comment.py
--rw-r--r--   0        0        0     2262 2023-04-04 13:06:07.385456 redditwarp-1.0.0rc0/redditwarp/models/comment_ASYNC.py
--rw-r--r--   0        0        0     2093 2023-04-04 13:06:07.386214 redditwarp-1.0.0rc0/redditwarp/models/comment_SYNC.py
--rw-r--r--   0        0        0      712 2023-04-04 13:06:07.386907 redditwarp-1.0.0rc0/redditwarp/models/comment_tree_ASYNC.py
--rw-r--r--   0        0        0      709 2023-04-04 13:06:07.387193 redditwarp-1.0.0rc0/redditwarp/models/comment_tree_SYNC.py
--rw-r--r--   0        0        0     2454 2023-04-04 13:06:07.387860 redditwarp-1.0.0rc0/redditwarp/models/custom_feed.py
--rw-r--r--   0        0        0     1185 2023-04-04 13:06:07.388480 redditwarp-1.0.0rc0/redditwarp/models/custom_feed_ASYNC.py
--rw-r--r--   0        0        0     1120 2023-04-04 13:06:07.389113 redditwarp-1.0.0rc0/redditwarp/models/custom_feed_SYNC.py
--rw-r--r--   0        0        0      780 2023-04-04 13:06:07.389813 redditwarp-1.0.0rc0/redditwarp/models/datamemento.py
--rw-r--r--   0        0        0     2499 2023-04-04 13:06:07.390313 redditwarp-1.0.0rc0/redditwarp/models/flair.py
--rw-r--r--   0        0        0     1575 2023-04-04 13:06:07.390954 redditwarp-1.0.0rc0/redditwarp/models/flair_emoji.py
--rw-r--r--   0        0        0      165 2023-04-04 13:06:07.391343 redditwarp-1.0.0rc0/redditwarp/models/karma_breakdown_entry.py
--rw-r--r--   0        0        0     4205 2023-04-04 13:06:07.391736 redditwarp-1.0.0rc0/redditwarp/models/live_thread.py
--rw-r--r--   0        0        0     1325 2023-04-04 13:06:07.392489 redditwarp-1.0.0rc0/redditwarp/models/live_thread_ASYNC.py
--rw-r--r--   0        0        0     1264 2023-04-04 13:06:07.393320 redditwarp-1.0.0rc0/redditwarp/models/live_thread_SYNC.py
--rw-r--r--   0        0        0      391 2023-04-04 13:06:07.393635 redditwarp-1.0.0rc0/redditwarp/models/media_upload_lease.py
--rw-r--r--   0        0        0     4213 2023-04-04 13:06:07.394324 redditwarp-1.0.0rc0/redditwarp/models/message.py
--rw-r--r--   0        0        0     1135 2023-04-04 13:06:07.394633 redditwarp-1.0.0rc0/redditwarp/models/message_ASYNC.py
--rw-r--r--   0        0        0     1074 2023-04-04 13:06:07.394903 redditwarp-1.0.0rc0/redditwarp/models/message_SYNC.py
--rw-r--r--   0        0        0     2228 2023-04-04 13:06:07.395644 redditwarp-1.0.0rc0/redditwarp/models/moderated_subreddit.py
--rw-r--r--   0        0        0      826 2023-04-04 13:06:07.396027 redditwarp-1.0.0rc0/redditwarp/models/moderation_action_log_entry.py
--rw-r--r--   0        0        0     2267 2023-04-04 13:06:07.396339 redditwarp-1.0.0rc0/redditwarp/models/moderation_note.py
--rw-r--r--   0        0        0     1549 2023-04-04 13:06:07.396650 redditwarp-1.0.0rc0/redditwarp/models/moderator_list.py
--rw-r--r--   0        0        0    12891 2023-04-04 13:06:07.397427 redditwarp-1.0.0rc0/redditwarp/models/modmail.py
--rw-r--r--   0        0        0     2107 2023-04-04 13:06:07.398388 redditwarp-1.0.0rc0/redditwarp/models/modmail_ASYNC.py
--rw-r--r--   0        0        0     2070 2023-04-04 13:06:07.399203 redditwarp-1.0.0rc0/redditwarp/models/modmail_SYNC.py
--rw-r--r--   0        0        0     2281 2023-04-04 13:06:07.400038 redditwarp-1.0.0rc0/redditwarp/models/more_comments_ASYNC.py
--rw-r--r--   0        0        0     2249 2023-04-04 13:06:07.401365 redditwarp-1.0.0rc0/redditwarp/models/more_comments_SYNC.py
--rw-r--r--   0        0        0     3187 2023-04-04 13:06:07.401744 redditwarp-1.0.0rc0/redditwarp/models/my_account.py
--rw-r--r--   0        0        0      372 2023-04-04 13:06:07.402406 redditwarp-1.0.0rc0/redditwarp/models/my_account_ASYNC.py
--rw-r--r--   0        0        0      371 2023-04-04 13:06:07.404060 redditwarp-1.0.0rc0/redditwarp/models/my_account_SYNC.py
--rw-r--r--   0        0        0      933 2023-04-04 13:06:07.404342 redditwarp-1.0.0rc0/redditwarp/models/report.py
--rw-r--r--   0        0        0      319 2023-04-04 13:06:07.404570 redditwarp-1.0.0rc0/redditwarp/models/stylesheet.py
--rw-r--r--   0        0        0    20016 2023-04-04 13:06:07.405284 redditwarp-1.0.0rc0/redditwarp/models/submission.py
--rw-r--r--   0        0        0     3134 2023-04-04 13:06:07.405894 redditwarp-1.0.0rc0/redditwarp/models/submission_ASYNC.py
--rw-r--r--   0        0        0     2963 2023-04-04 13:06:07.406568 redditwarp-1.0.0rc0/redditwarp/models/submission_SYNC.py
--rw-r--r--   0        0        0     3965 2023-04-04 13:06:07.406842 redditwarp-1.0.0rc0/redditwarp/models/submission_collection.py
--rw-r--r--   0        0        0     1797 2023-04-04 13:06:07.407316 redditwarp-1.0.0rc0/redditwarp/models/submission_collection_ASYNC.py
--rw-r--r--   0        0        0     1722 2023-04-04 13:06:07.407827 redditwarp-1.0.0rc0/redditwarp/models/submission_collection_SYNC.py
--rw-r--r--   0        0        0     3238 2023-04-04 13:06:07.408090 redditwarp-1.0.0rc0/redditwarp/models/submission_draft.py
--rw-r--r--   0        0        0      575 2023-04-04 13:06:07.408314 redditwarp-1.0.0rc0/redditwarp/models/submission_draft_ASYNC.py
--rw-r--r--   0        0        0      574 2023-04-04 13:06:07.408540 redditwarp-1.0.0rc0/redditwarp/models/submission_draft_SYNC.py
--rw-r--r--   0        0        0    11175 2023-04-04 13:06:07.409478 redditwarp-1.0.0rc0/redditwarp/models/subreddit.py
--rw-r--r--   0        0        0      711 2023-04-04 13:06:07.410306 redditwarp-1.0.0rc0/redditwarp/models/subreddit_ASYNC.py
--rw-r--r--   0        0        0      710 2023-04-04 13:06:07.410914 redditwarp-1.0.0rc0/redditwarp/models/subreddit_SYNC.py
--rw-r--r--   0        0        0     2150 2023-04-04 13:06:07.411231 redditwarp-1.0.0rc0/redditwarp/models/subreddit_rules.py
--rw-r--r--   0        0        0      337 2023-04-04 13:06:07.411518 redditwarp-1.0.0rc0/redditwarp/models/subreddit_style_asset_upload_lease.py
--rw-r--r--   0        0        0     4051 2023-04-04 13:06:07.412109 redditwarp-1.0.0rc0/redditwarp/models/subreddit_user.py
--rw-r--r--   0        0        0      677 2023-04-04 13:06:07.412394 redditwarp-1.0.0rc0/redditwarp/models/trophy.py
--rw-r--r--   0        0        0     3857 2023-04-04 13:06:07.413181 redditwarp-1.0.0rc0/redditwarp/models/user.py
--rw-r--r--   0        0        0      584 2023-04-04 13:06:07.413751 redditwarp-1.0.0rc0/redditwarp/models/user_ASYNC.py
--rw-r--r--   0        0        0      583 2023-04-04 13:06:07.415888 redditwarp-1.0.0rc0/redditwarp/models/user_SYNC.py
--rw-r--r--   0        0        0     1651 2023-04-04 13:06:07.416214 redditwarp-1.0.0rc0/redditwarp/models/user_relationship.py
--rw-r--r--   0        0        0     1062 2023-04-04 13:06:07.416504 redditwarp-1.0.0rc0/redditwarp/models/user_summary.py
--rw-r--r--   0        0        0      983 2023-04-04 13:06:07.416805 redditwarp-1.0.0rc0/redditwarp/models/widget/ASYNC.py
--rw-r--r--   0        0        0      970 2023-04-04 13:06:07.417012 redditwarp-1.0.0rc0/redditwarp/models/widget/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.417111 redditwarp-1.0.0rc0/redditwarp/models/widget/__init__.py
--rw-r--r--   0        0        0      846 2023-04-04 13:06:07.417317 redditwarp-1.0.0rc0/redditwarp/models/widget/button.py
--rw-r--r--   0        0        0      336 2023-04-04 13:06:07.417504 redditwarp-1.0.0rc0/redditwarp/models/widget/button_ASYNC.py
--rw-r--r--   0        0        0      335 2023-04-04 13:06:07.417687 redditwarp-1.0.0rc0/redditwarp/models/widget/button_SYNC.py
--rw-r--r--   0        0        0      272 2023-04-04 13:06:07.417860 redditwarp-1.0.0rc0/redditwarp/models/widget/calendar.py
--rw-r--r--   0        0        0      373 2023-04-04 13:06:07.418087 redditwarp-1.0.0rc0/redditwarp/models/widget/calendar_ASYNC.py
--rw-r--r--   0        0        0      372 2023-04-04 13:06:07.418317 redditwarp-1.0.0rc0/redditwarp/models/widget/calendar_SYNC.py
--rw-r--r--   0        0        0      301 2023-04-04 13:06:07.418515 redditwarp-1.0.0rc0/redditwarp/models/widget/community_details_ASYNC.py
--rw-r--r--   0        0        0      300 2023-04-04 13:06:07.418708 redditwarp-1.0.0rc0/redditwarp/models/widget/community_details_SYNC.py
--rw-r--r--   0        0        0      251 2023-04-04 13:06:07.418902 redditwarp-1.0.0rc0/redditwarp/models/widget/community_list.py
--rw-r--r--   0        0        0      336 2023-04-04 13:06:07.419090 redditwarp-1.0.0rc0/redditwarp/models/widget/community_list_ASYNC.py
--rw-r--r--   0        0        0      335 2023-04-04 13:06:07.419275 redditwarp-1.0.0rc0/redditwarp/models/widget/community_list_SYNC.py
--rw-r--r--   0        0        0      243 2023-04-04 13:06:07.419463 redditwarp-1.0.0rc0/redditwarp/models/widget/custom_css.py
--rw-r--r--   0        0        0      398 2023-04-04 13:06:07.419641 redditwarp-1.0.0rc0/redditwarp/models/widget/custom_css_ASYNC.py
--rw-r--r--   0        0        0      397 2023-04-04 13:06:07.419881 redditwarp-1.0.0rc0/redditwarp/models/widget/custom_css_SYNC.py
--rw-r--r--   0        0        0      276 2023-04-04 13:06:07.420208 redditwarp-1.0.0rc0/redditwarp/models/widget/image.py
--rw-r--r--   0        0        0      303 2023-04-04 13:06:07.420446 redditwarp-1.0.0rc0/redditwarp/models/widget/image_ASYNC.py
--rw-r--r--   0        0        0      302 2023-04-04 13:06:07.420725 redditwarp-1.0.0rc0/redditwarp/models/widget/image_SYNC.py
--rw-r--r--   0        0        0       92 2023-04-04 13:06:07.420899 redditwarp-1.0.0rc0/redditwarp/models/widget/image_size_named_tuple.py
--rw-r--r--   0        0        0      400 2023-04-04 13:06:07.421075 redditwarp-1.0.0rc0/redditwarp/models/widget/menu_bar.py
--rw-r--r--   0        0        0      321 2023-04-04 13:06:07.421369 redditwarp-1.0.0rc0/redditwarp/models/widget/menu_bar_ASYNC.py
--rw-r--r--   0        0        0      321 2023-04-04 13:06:07.421706 redditwarp-1.0.0rc0/redditwarp/models/widget/menu_bar_SYNC.py
--rw-r--r--   0        0        0      361 2023-04-04 13:06:07.421996 redditwarp-1.0.0rc0/redditwarp/models/widget/moderator_list.py
--rw-r--r--   0        0        0      332 2023-04-04 13:06:07.422263 redditwarp-1.0.0rc0/redditwarp/models/widget/moderator_list_ASYNC.py
--rw-r--r--   0        0        0      331 2023-04-04 13:06:07.422482 redditwarp-1.0.0rc0/redditwarp/models/widget/moderator_list_SYNC.py
--rw-r--r--   0        0        0      279 2023-04-04 13:06:07.422708 redditwarp-1.0.0rc0/redditwarp/models/widget/post_flair.py
--rw-r--r--   0        0        0      366 2023-04-04 13:06:07.422882 redditwarp-1.0.0rc0/redditwarp/models/widget/post_flair_ASYNC.py
--rw-r--r--   0        0        0      365 2023-04-04 13:06:07.423048 redditwarp-1.0.0rc0/redditwarp/models/widget/post_flair_SYNC.py
--rw-r--r--   0        0        0      230 2023-04-04 13:06:07.423230 redditwarp-1.0.0rc0/redditwarp/models/widget/rules.py
--rw-r--r--   0        0        0      298 2023-04-04 13:06:07.423403 redditwarp-1.0.0rc0/redditwarp/models/widget/rules_ASYNC.py
--rw-r--r--   0        0        0      297 2023-04-04 13:06:07.423569 redditwarp-1.0.0rc0/redditwarp/models/widget/rules_SYNC.py
--rw-r--r--   0        0        0      202 2023-04-04 13:06:07.423869 redditwarp-1.0.0rc0/redditwarp/models/widget/text_area_ASYNC.py
--rw-r--r--   0        0        0      201 2023-04-04 13:06:07.424111 redditwarp-1.0.0rc0/redditwarp/models/widget/text_area_SYNC.py
--rw-r--r--   0        0        0      350 2023-04-04 13:06:07.424312 redditwarp-1.0.0rc0/redditwarp/models/widget/widget_ASYNC.py
--rw-r--r--   0        0        0      350 2023-04-04 13:06:07.424549 redditwarp-1.0.0rc0/redditwarp/models/widget/widget_SYNC.py
--rw-r--r--   0        0        0      365 2023-04-04 13:06:07.424839 redditwarp-1.0.0rc0/redditwarp/models/widget/widget_image_upload_lease.py
--rw-r--r--   0        0        0     1757 2023-04-04 13:06:07.425160 redditwarp-1.0.0rc0/redditwarp/models/widget/widget_list_ASYNC.py
--rw-r--r--   0        0        0     1752 2023-04-04 13:06:07.425472 redditwarp-1.0.0rc0/redditwarp/models/widget/widget_list_SYNC.py
--rw-r--r--   0        0        0     4192 2023-04-04 13:06:07.426128 redditwarp-1.0.0rc0/redditwarp/models/wiki.py
--rw-r--r--   0        0        0      838 2023-04-04 13:06:07.426947 redditwarp-1.0.0rc0/redditwarp/models/wiki_ASYNC.py
--rw-r--r--   0        0        0      837 2023-04-04 13:06:07.427642 redditwarp-1.0.0rc0/redditwarp/models/wiki_SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.427979 redditwarp-1.0.0rc0/redditwarp/pagination/__init__.py
--rw-r--r--   0        0        0     1528 2023-04-04 13:06:07.428574 redditwarp-1.0.0rc0/redditwarp/pagination/async_paginator.py
--rw-r--r--   0        0        0     1440 2023-04-04 13:06:07.429338 redditwarp-1.0.0rc0/redditwarp/pagination/paginator.py
--rw-r--r--   0        0        0     1818 2023-04-04 13:06:07.430443 redditwarp-1.0.0rc0/redditwarp/pagination/paginator_chaining_async_iterator.py
--rw-r--r--   0        0        0     1681 2023-04-04 13:06:07.431128 redditwarp-1.0.0rc0/redditwarp/pagination/paginator_chaining_iterator.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.431444 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/__init__.py
--rw-r--r--   0        0        0      588 2023-04-04 13:06:07.431772 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/account_async1.py
--rw-r--r--   0        0        0      545 2023-04-04 13:06:07.432133 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/account_sync1.py
--rw-r--r--   0        0        0     2602 2023-04-04 13:06:07.432836 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/flair_async1.py
--rw-r--r--   0        0        0     2546 2023-04-04 13:06:07.433508 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/flair_sync1.py
--rw-r--r--   0        0        0     1268 2023-04-04 13:06:07.434006 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/front_async1.py
--rw-r--r--   0        0        0     1173 2023-04-04 13:06:07.434369 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/front_sync1.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.434761 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/__init__.py
--rw-r--r--   0        0        0      495 2023-04-04 13:06:07.435146 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/comment_listing_async_paginator.py
--rw-r--r--   0        0        0      460 2023-04-04 13:06:07.435441 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/comment_listing_paginator.py
--rw-r--r--   0        0        0     3410 2023-04-04 13:06:07.436043 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/listing_async_paginator.py
--rw-r--r--   0        0        0     3366 2023-04-04 13:06:07.436637 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/listing_paginator.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.436939 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/__init__.py
--rw-r--r--   0        0        0      858 2023-04-04 13:06:07.437469 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/sort_ASYNC.py
--rw-r--r--   0        0        0      841 2023-04-04 13:06:07.437950 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/sort_SYNC.py
--rw-r--r--   0        0        0      882 2023-04-04 13:06:07.438454 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_ASYNC.py
--rw-r--r--   0        0        0      865 2023-04-04 13:06:07.443200 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_SYNC.py
--rw-r--r--   0        0        0      855 2023-04-04 13:06:07.443938 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/time_ASYNC.py
--rw-r--r--   0        0        0      838 2023-04-04 13:06:07.444437 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/time_SYNC.py
--rw-r--r--   0        0        0      981 2023-04-04 13:06:07.444688 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_async_paginator.py
--rw-r--r--   0        0        0      946 2023-04-04 13:06:07.444929 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_paginator.py
--rw-r--r--   0        0        0      496 2023-04-04 13:06:07.445145 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_listing_async_paginator.py
--rw-r--r--   0        0        0      461 2023-04-04 13:06:07.445453 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_listing_paginator.py
--rw-r--r--   0        0        0      488 2023-04-04 13:06:07.445712 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/subreddit_listing_async_paginator.py
--rw-r--r--   0        0        0      453 2023-04-04 13:06:07.445928 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/subreddit_listing_paginator.py
--rw-r--r--   0        0        0      497 2023-04-04 13:06:07.446159 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/live_thread_async1.py
--rw-r--r--   0        0        0      462 2023-04-04 13:06:07.446373 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/live_thread_sync1.py
--rw-r--r--   0        0        0     1474 2023-04-04 13:06:07.446586 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/message_async1.py
--rw-r--r--   0        0        0     1373 2023-04-04 13:06:07.446784 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/message_sync1.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.446991 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/__init__.py
--rw-r--r--   0        0        0     1709 2023-04-04 13:06:07.447259 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/async1.py
--rw-r--r--   0        0        0     1355 2023-04-04 13:06:07.447524 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/legacy_pull_users_async1.py
--rw-r--r--   0        0        0     1289 2023-04-04 13:06:07.447760 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/legacy_pull_users_sync1.py
--rw-r--r--   0        0        0     3297 2023-04-04 13:06:07.448365 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/note_pulls_async1.py
--rw-r--r--   0        0        0     3221 2023-04-04 13:06:07.448902 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/note_pulls_sync1.py
--rw-r--r--   0        0        0     1402 2023-04-04 13:06:07.449395 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_actions_async1.py
--rw-r--r--   0        0        0     1368 2023-04-04 13:06:07.449812 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_actions_sync1.py
--rw-r--r--   0        0        0     4025 2023-04-04 13:06:07.450043 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_async1.py
--rw-r--r--   0        0        0     3842 2023-04-04 13:06:07.450245 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_sync1.py
--rw-r--r--   0        0        0     3627 2023-04-04 13:06:07.450708 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_users_async1.py
--rw-r--r--   0        0        0     3495 2023-04-04 13:06:07.451327 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_users_sync1.py
--rw-r--r--   0        0        0     1505 2023-04-04 13:06:07.451646 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/sync1.py
--rw-r--r--   0        0        0     2917 2023-04-04 13:06:07.452358 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/modmail_async1.py
--rw-r--r--   0        0        0     2869 2023-04-04 13:06:07.452959 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/modmail_sync1.py
--rw-r--r--   0        0        0     3679 2023-04-04 13:06:07.453854 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/submission_async1.py
--rw-r--r--   0        0        0     3608 2023-04-04 13:06:07.454568 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/submission_sync1.py
--rw-r--r--   0        0        0      892 2023-04-04 13:06:07.455117 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/subreddit_async1.py
--rw-r--r--   0        0        0      868 2023-04-04 13:06:07.455740 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/subreddit_sync1.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.455972 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/__init__.py
--rw-r--r--   0        0        0      961 2023-04-04 13:06:07.459228 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/async1.py
--rw-r--r--   0        0        0      922 2023-04-04 13:06:07.459886 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/explore_async1.py
--rw-r--r--   0        0        0      885 2023-04-04 13:06:07.463298 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/explore_sync1.py
--rw-r--r--   0        0        0     2263 2023-04-04 13:06:07.463852 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_async1.py
--rw-r--r--   0        0        0     2126 2023-04-04 13:06:07.464216 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_sync1.py
--rw-r--r--   0        0        0      360 2023-04-04 13:06:07.464702 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_user_subreddits_async1.py
--rw-r--r--   0        0        0      337 2023-04-04 13:06:07.465097 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_user_subreddits_sync1.py
--rw-r--r--   0        0        0      838 2023-04-04 13:06:07.465335 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/sync1.py
--rw-r--r--   0        0        0      868 2023-04-04 13:06:07.465535 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/wiki_async1.py
--rw-r--r--   0        0        0      832 2023-04-04 13:06:07.465822 redditwarp-1.0.0rc0/redditwarp/pagination/paginators/wiki_sync1.py
--rw-r--r--   0        0        0      176 2023-04-04 13:06:07.466072 redditwarp-1.0.0rc0/redditwarp/pushshift/ASYNC.py
--rw-r--r--   0        0        0      174 2023-04-04 13:06:07.466255 redditwarp-1.0.0rc0/redditwarp/pushshift/SYNC.py
--rw-r--r--   0        0        0      335 2023-04-04 13:06:07.467067 redditwarp-1.0.0rc0/redditwarp/pushshift/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-04 13:06:07.467786 redditwarp-1.0.0rc0/redditwarp/pushshift/client_ASYNC.py
--rw-r--r--   0        0        0     1810 2023-04-04 13:06:07.468455 redditwarp-1.0.0rc0/redditwarp/pushshift/client_SYNC.py
--rw-r--r--   0        0        0       35 2023-04-04 13:06:07.468901 redditwarp-1.0.0rc0/redditwarp/pushshift/core/__init__.py
--rw-r--r--   0        0        0       48 2023-04-04 13:06:07.469629 redditwarp-1.0.0rc0/redditwarp/pushshift/core/const.py
--rw-r--r--   0        0        0      758 2023-04-04 13:06:07.470229 redditwarp-1.0.0rc0/redditwarp/pushshift/core/http_client_ASYNC.py
--rw-r--r--   0        0        0      753 2023-04-04 13:06:07.470800 redditwarp-1.0.0rc0/redditwarp/pushshift/core/http_client_SYNC.py
--rw-r--r--   0        0        0      778 2023-04-04 13:06:07.471458 redditwarp-1.0.0rc0/redditwarp/pushshift/core/rate_limited_ASYNC.py
--rw-r--r--   0        0        0      656 2023-04-04 13:06:07.472135 redditwarp-1.0.0rc0/redditwarp/pushshift/core/rate_limited_SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.472367 redditwarp-1.0.0rc0/redditwarp/pushshift/models/__init__.py
--rw-r--r--   0        0        0      497 2023-04-04 13:06:07.472903 redditwarp-1.0.0rc0/redditwarp/pushshift/models/document.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.473126 redditwarp-1.0.0rc0/redditwarp/pushshift/paginators/__init__.py
--rw-r--r--   0        0        0     2955 2023-04-04 13:06:07.473648 redditwarp-1.0.0rc0/redditwarp/pushshift/paginators/document_async_paginator.py
--rw-r--r--   0        0        0     2921 2023-04-04 13:06:07.474662 redditwarp-1.0.0rc0/redditwarp/pushshift/paginators/document_paginator.py
--rw-r--r--   0        0        0    12170 2023-04-04 13:06:07.475772 redditwarp-1.0.0rc0/redditwarp/pushshift/siteprocs/ASYNC.py
--rw-r--r--   0        0        0    11988 2023-04-04 13:06:07.476550 redditwarp-1.0.0rc0/redditwarp/pushshift/siteprocs/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.476729 redditwarp-1.0.0rc0/redditwarp/pushshift/siteprocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.476897 redditwarp-1.0.0rc0/redditwarp/py.typed
--rw-r--r--   0        0        0     3151 2023-04-04 13:06:07.477683 redditwarp-1.0.0rc0/redditwarp/siteprocs/ASYNC.py
--rw-r--r--   0        0        0     3117 2023-04-04 13:06:07.478327 redditwarp-1.0.0rc0/redditwarp/siteprocs/SYNC.py
--rw-r--r--   0        0        0       38 2023-04-04 13:06:07.478617 redditwarp-1.0.0rc0/redditwarp/siteprocs/__init__.py
--rw-r--r--   0        0        0    14353 2023-04-04 13:06:07.479746 redditwarp-1.0.0rc0/redditwarp/siteprocs/account/ASYNC.py
--rw-r--r--   0        0        0    14131 2023-04-04 13:06:07.480518 redditwarp-1.0.0rc0/redditwarp/siteprocs/account/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.480668 redditwarp-1.0.0rc0/redditwarp/siteprocs/account/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-04 13:06:07.481519 redditwarp-1.0.0rc0/redditwarp/siteprocs/account/pull_subreddits_ASYNC.py
--rw-r--r--   0        0        0     1607 2023-04-04 13:06:07.481858 redditwarp-1.0.0rc0/redditwarp/siteprocs/account/pull_subreddits_SYNC.py
--rw-r--r--   0        0        0    16360 2023-04-04 13:06:07.482662 redditwarp-1.0.0rc0/redditwarp/siteprocs/collection/ASYNC.py
--rw-r--r--   0        0        0    16191 2023-04-04 13:06:07.483353 redditwarp-1.0.0rc0/redditwarp/siteprocs/collection/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.483483 redditwarp-1.0.0rc0/redditwarp/siteprocs/collection/__init__.py
--rw-r--r--   0        0        0    24087 2023-04-04 13:06:07.484409 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/ASYNC.py
--rw-r--r--   0        0        0    23737 2023-04-04 13:06:07.486754 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.487033 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/__init__.py
--rw-r--r--   0        0        0      947 2023-04-04 13:06:07.487382 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/fetch_ASYNC.py
--rw-r--r--   0        0        0      908 2023-04-04 13:06:07.487610 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/fetch_SYNC.py
--rw-r--r--   0        0        0     1016 2023-04-04 13:06:07.487789 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/get_ASYNC.py
--rw-r--r--   0        0        0      977 2023-04-04 13:06:07.487965 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/get_SYNC.py
--rw-r--r--   0        0        0     7237 2023-04-04 13:06:07.491422 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/ASYNC.py
--rw-r--r--   0        0        0     7184 2023-04-04 13:06:07.492161 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.492281 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/__init__.py
--rw-r--r--   0        0        0     3729 2023-04-04 13:06:07.492541 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/low_ASYNC.py
--rw-r--r--   0        0        0     3676 2023-04-04 13:06:07.492775 redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/low_SYNC.py
--rw-r--r--   0        0        0    14034 2023-04-04 13:06:07.493843 redditwarp-1.0.0rc0/redditwarp/siteprocs/custom_feed/ASYNC.py
--rw-r--r--   0        0        0    13804 2023-04-04 13:06:07.494821 redditwarp-1.0.0rc0/redditwarp/siteprocs/custom_feed/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.494975 redditwarp-1.0.0rc0/redditwarp/siteprocs/custom_feed/__init__.py
--rw-r--r--   0        0        0     6763 2023-04-04 13:06:07.496151 redditwarp-1.0.0rc0/redditwarp/siteprocs/draft/ASYNC.py
--rw-r--r--   0        0        0     6699 2023-04-04 13:06:07.499819 redditwarp-1.0.0rc0/redditwarp/siteprocs/draft/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.499956 redditwarp-1.0.0rc0/redditwarp/siteprocs/draft/__init__.py
--rw-r--r--   0        0        0    31100 2023-04-04 13:06:07.500816 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair/ASYNC.py
--rw-r--r--   0        0        0    30693 2023-04-04 13:06:07.506833 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.507170 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair/__init__.py
--rw-r--r--   0        0        0     8523 2023-04-04 13:06:07.510927 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair_emoji/ASYNC.py
--rw-r--r--   0        0        0     8390 2023-04-04 13:06:07.514782 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair_emoji/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.515009 redditwarp-1.0.0rc0/redditwarp/siteprocs/flair_emoji/__init__.py
--rw-r--r--   0        0        0      987 2023-04-04 13:06:07.518741 redditwarp-1.0.0rc0/redditwarp/siteprocs/front/ASYNC.py
--rw-r--r--   0        0        0      942 2023-04-04 13:06:07.524050 redditwarp-1.0.0rc0/redditwarp/siteprocs/front/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.524401 redditwarp-1.0.0rc0/redditwarp/siteprocs/front/__init__.py
--rw-r--r--   0        0        0     2696 2023-04-04 13:06:07.525138 redditwarp-1.0.0rc0/redditwarp/siteprocs/front/pull_ASYNC.py
--rw-r--r--   0        0        0     2507 2023-04-04 13:06:07.525836 redditwarp-1.0.0rc0/redditwarp/siteprocs/front/pull_SYNC.py
--rw-r--r--   0        0        0    19365 2023-04-04 13:06:07.527781 redditwarp-1.0.0rc0/redditwarp/siteprocs/live_thread/ASYNC.py
--rw-r--r--   0        0        0    19053 2023-04-04 13:06:07.533029 redditwarp-1.0.0rc0/redditwarp/siteprocs/live_thread/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.533386 redditwarp-1.0.0rc0/redditwarp/siteprocs/live_thread/__init__.py
--rw-r--r--   0        0        0    10103 2023-04-04 13:06:07.534700 redditwarp-1.0.0rc0/redditwarp/siteprocs/message/ASYNC.py
--rw-r--r--   0        0        0     9905 2023-04-04 13:06:07.535298 redditwarp-1.0.0rc0/redditwarp/siteprocs/message/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.535477 redditwarp-1.0.0rc0/redditwarp/siteprocs/message/__init__.py
--rw-r--r--   0        0        0     2727 2023-04-04 13:06:07.535906 redditwarp-1.0.0rc0/redditwarp/siteprocs/message/pulls_ASYNC.py
--rw-r--r--   0        0        0     2553 2023-04-04 13:06:07.536477 redditwarp-1.0.0rc0/redditwarp/siteprocs/message/pulls_SYNC.py
--rw-r--r--   0        0        0      938 2023-04-04 13:06:07.537722 redditwarp-1.0.0rc0/redditwarp/siteprocs/misc/ASYNC.py
--rw-r--r--   0        0        0      913 2023-04-04 13:06:07.538074 redditwarp-1.0.0rc0/redditwarp/siteprocs/misc/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.538298 redditwarp-1.0.0rc0/redditwarp/siteprocs/misc/__init__.py
--rw-r--r--   0        0        0    29926 2023-04-04 13:06:07.539554 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/ASYNC.py
--rw-r--r--   0        0        0    29625 2023-04-04 13:06:07.540389 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.540561 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/__init__.py
--rw-r--r--   0        0        0     4474 2023-04-04 13:06:07.541229 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_ASYNC.py
--rw-r--r--   0        0        0     4400 2023-04-04 13:06:07.541886 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_SYNC.py
--rw-r--r--   0        0        0     2394 2023-04-04 13:06:07.542212 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_pull_users_ASYNC.py
--rw-r--r--   0        0        0     2271 2023-04-04 13:06:07.542513 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_pull_users_SYNC.py
--rw-r--r--   0        0        0     9715 2023-04-04 13:06:07.543069 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/note_ASYNC.py
--rw-r--r--   0        0        0     9539 2023-04-04 13:06:07.543517 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/note_SYNC.py
--rw-r--r--   0        0        0     7419 2023-04-04 13:06:07.544196 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_ASYNC.py
--rw-r--r--   0        0        0     7060 2023-04-04 13:06:07.544791 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_SYNC.py
--rw-r--r--   0        0        0     3596 2023-04-04 13:06:07.545570 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_users_ASYNC.py
--rw-r--r--   0        0        0     3426 2023-04-04 13:06:07.545876 redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_users_SYNC.py
--rw-r--r--   0        0        0     1862 2023-04-04 13:06:07.546710 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/ASYNC.py
--rw-r--r--   0        0        0     1835 2023-04-04 13:06:07.547298 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.547436 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/__init__.py
--rw-r--r--   0        0        0    21467 2023-04-04 13:06:07.548132 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/conversation_ASYNC.py
--rw-r--r--   0        0        0    21114 2023-04-04 13:06:07.548850 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/conversation_SYNC.py
--rw-r--r--   0        0        0     4741 2023-04-04 13:06:07.549174 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/pull_ASYNC.py
--rw-r--r--   0        0        0     4592 2023-04-04 13:06:07.549363 redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/pull_SYNC.py
--rw-r--r--   0        0        0    59233 2023-04-04 13:06:07.550265 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/ASYNC.py
--rw-r--r--   0        0        0    58402 2023-04-04 13:06:07.551167 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.551313 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-04 13:06:07.551884 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/fetch_ASYNC.py
--rw-r--r--   0        0        0     2258 2023-04-04 13:06:07.552140 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/fetch_SYNC.py
--rw-r--r--   0        0        0     2088 2023-04-04 13:06:07.552441 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/get_ASYNC.py
--rw-r--r--   0        0        0     2049 2023-04-04 13:06:07.552856 redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/get_SYNC.py
--rw-r--r--   0        0        0    18879 2023-04-04 13:06:07.553946 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/ASYNC.py
--rw-r--r--   0        0        0    18420 2023-04-04 13:06:07.554323 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.554520 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-04 13:06:07.554899 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pull_ASYNC.py
--rw-r--r--   0        0        0     2343 2023-04-04 13:06:07.555273 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pull_SYNC.py
--rw-r--r--   0        0        0     1674 2023-04-04 13:06:07.555680 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pulls_ASYNC.py
--rw-r--r--   0        0        0     1570 2023-04-04 13:06:07.556034 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pulls_SYNC.py
--rw-r--r--   0        0        0     9395 2023-04-04 13:06:07.557332 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_new/ASYNC.py
--rw-r--r--   0        0        0     9238 2023-04-04 13:06:07.558204 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_new/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.558390 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_new/__init__.py
--rw-r--r--   0        0        0     8021 2023-04-04 13:06:07.559588 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_old/ASYNC.py
--rw-r--r--   0        0        0     7900 2023-04-04 13:06:07.560151 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_old/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.560328 redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_old/__init__.py
--rw-r--r--   0        0        0     7671 2023-04-04 13:06:07.561211 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/ASYNC.py
--rw-r--r--   0        0        0     7519 2023-04-04 13:06:07.563392 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.563537 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/__init__.py
--rw-r--r--   0        0        0     2149 2023-04-04 13:06:07.563883 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/bulk_fetch_user_summary_ASYNC.py
--rw-r--r--   0        0        0     2072 2023-04-04 13:06:07.564177 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/bulk_fetch_user_summary_SYNC.py
--rw-r--r--   0        0        0     1017 2023-04-04 13:06:07.564499 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/get_user_summary_ASYNC.py
--rw-r--r--   0        0        0      992 2023-04-04 13:06:07.564813 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/get_user_summary_SYNC.py
--rw-r--r--   0        0        0     4702 2023-04-04 13:06:07.565101 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_ASYNC.py
--rw-r--r--   0        0        0     4417 2023-04-04 13:06:07.565437 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_SYNC.py
--rw-r--r--   0        0        0     1065 2023-04-04 13:06:07.565744 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_subreddits_ASYNC.py
--rw-r--r--   0        0        0     1006 2023-04-04 13:06:07.566061 redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_subreddits_SYNC.py
--rw-r--r--   0        0        0    24334 2023-04-04 13:06:07.566976 redditwarp-1.0.0rc0/redditwarp/siteprocs/widget/ASYNC.py
--rw-r--r--   0        0        0    23988 2023-04-04 13:06:07.567788 redditwarp-1.0.0rc0/redditwarp/siteprocs/widget/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.567931 redditwarp-1.0.0rc0/redditwarp/siteprocs/widget/__init__.py
--rw-r--r--   0        0        0    13377 2023-04-04 13:06:07.568686 redditwarp-1.0.0rc0/redditwarp/siteprocs/wiki/ASYNC.py
--rw-r--r--   0        0        0    13120 2023-04-04 13:06:07.569265 redditwarp-1.0.0rc0/redditwarp/siteprocs/wiki/SYNC.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.569403 redditwarp-1.0.0rc0/redditwarp/siteprocs/wiki/__init__.py
--rw-r--r--   0        0        0       96 2023-04-04 13:06:07.569846 redditwarp-1.0.0rc0/redditwarp/streaming/ASYNC.py
--rw-r--r--   0        0        0       95 2023-04-04 13:06:07.570089 redditwarp-1.0.0rc0/redditwarp/streaming/SYNC.py
--rw-r--r--   0        0        0       48 2023-04-04 13:06:07.570321 redditwarp-1.0.0rc0/redditwarp/streaming/__init__.py
--rw-r--r--   0        0        0       82 2023-04-04 13:06:07.570566 redditwarp-1.0.0rc0/redditwarp/streaming/async1.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.570809 redditwarp-1.0.0rc0/redditwarp/streaming/makers/__init__.py
--rw-r--r--   0        0        0     2009 2023-04-04 13:06:07.571112 redditwarp-1.0.0rc0/redditwarp/streaming/makers/message_ASYNC.py
--rw-r--r--   0        0        0     1973 2023-04-04 13:06:07.571514 redditwarp-1.0.0rc0/redditwarp/streaming/makers/message_SYNC.py
--rw-r--r--   0        0        0     1158 2023-04-04 13:06:07.571844 redditwarp-1.0.0rc0/redditwarp/streaming/makers/moderation_ASYNC.py
--rw-r--r--   0        0        0     1134 2023-04-04 13:06:07.572164 redditwarp-1.0.0rc0/redditwarp/streaming/makers/moderation_SYNC.py
--rw-r--r--   0        0        0     2244 2023-04-04 13:06:07.572502 redditwarp-1.0.0rc0/redditwarp/streaming/makers/modmail_ASYNC.py
--rw-r--r--   0        0        0     2209 2023-04-04 13:06:07.572808 redditwarp-1.0.0rc0/redditwarp/streaming/makers/modmail_SYNC.py
--rw-r--r--   0        0        0     2515 2023-04-04 13:06:07.573127 redditwarp-1.0.0rc0/redditwarp/streaming/makers/subreddit_ASYNC.py
--rw-r--r--   0        0        0     2468 2023-04-04 13:06:07.573744 redditwarp-1.0.0rc0/redditwarp/streaming/makers/subreddit_SYNC.py
--rw-r--r--   0        0        0     1058 2023-04-04 13:06:07.574095 redditwarp-1.0.0rc0/redditwarp/streaming/makers/user_ASYNC.py
--rw-r--r--   0        0        0     1033 2023-04-04 13:06:07.574464 redditwarp-1.0.0rc0/redditwarp/streaming/makers/user_SYNC.py
--rw-r--r--   0        0        0     1028 2023-04-04 13:06:07.575152 redditwarp-1.0.0rc0/redditwarp/streaming/runners_ASYNC.py
--rw-r--r--   0        0        0      576 2023-04-04 13:06:07.575653 redditwarp-1.0.0rc0/redditwarp/streaming/runners_SYNC.py
--rw-r--r--   0        0        0     6706 2023-04-04 13:06:07.576604 redditwarp-1.0.0rc0/redditwarp/streaming/stream_ASYNC.py
--rw-r--r--   0        0        0     6167 2023-04-04 13:06:07.577540 redditwarp-1.0.0rc0/redditwarp/streaming/stream_SYNC.py
--rw-r--r--   0        0        0      294 2023-04-04 13:06:07.578070 redditwarp-1.0.0rc0/redditwarp/types.py
--rw-r--r--   0        0        0       17 2023-04-04 13:06:07.578643 redditwarp-1.0.0rc0/redditwarp/util/__init__.py
--rw-r--r--   0        0        0     4988 2023-04-04 13:06:07.579063 redditwarp-1.0.0rc0/redditwarp/util/attribute_mapping_proxy.py
--rw-r--r--   0        0        0     1451 2023-04-04 13:06:07.579414 redditwarp-1.0.0rc0/redditwarp/util/base_conversion.py
--rw-r--r--   0        0        0      778 2023-04-04 13:06:07.579730 redditwarp-1.0.0rc0/redditwarp/util/booleanify.py
--rw-r--r--   0        0        0      353 2023-04-04 13:06:07.580006 redditwarp-1.0.0rc0/redditwarp/util/bot_user_agent.py
--rw-r--r--   0        0        0     3784 2023-04-04 13:06:07.580319 redditwarp-1.0.0rc0/redditwarp/util/data_members_namespace.py
--rw-r--r--   0        0        0     2430 2023-04-04 13:06:07.580620 redditwarp-1.0.0rc0/redditwarp/util/event_dispatcher.py
--rw-r--r--   0        0        0     2054 2023-04-04 13:06:07.581231 redditwarp-1.0.0rc0/redditwarp/util/except_without_context.py
--rw-r--r--   0        0        0     2040 2023-04-04 13:06:07.581546 redditwarp-1.0.0rc0/redditwarp/util/extract_id_from_url.py
--rw-r--r--   0        0        0     1996 2023-04-04 13:06:07.581835 redditwarp-1.0.0rc0/redditwarp/util/imports.py
--rw-r--r--   0        0        0     2050 2023-04-04 13:06:07.582161 redditwarp-1.0.0rc0/redditwarp/util/ordered_set.py
--rw-r--r--   0        0        0      660 2023-04-04 13:06:07.582456 redditwarp-1.0.0rc0/redditwarp/util/passthru.py
--rw-r--r--   0        0        0     1272 2023-04-04 13:06:07.582764 redditwarp-1.0.0rc0/redditwarp/util/praw_config.py
--rw-r--r--   0        0        0     1238 2023-04-04 13:06:07.583371 redditwarp-1.0.0rc0/redditwarp/util/praw_config_ASYNC.py
--rw-r--r--   0        0        0     1236 2023-04-04 13:06:07.583687 redditwarp-1.0.0rc0/redditwarp/util/praw_config_SYNC.py
--rw-r--r--   0        0        0      336 2023-04-04 13:06:07.583987 redditwarp-1.0.0rc0/redditwarp/util/redditwarp_installed_client_credentials.py
--rw-r--r--   0        0        0     3788 2023-04-04 13:06:07.584574 redditwarp-1.0.0rc0/redditwarp/util/shdlr.py
--rw-r--r--   0        0        0      638 2023-04-04 13:06:07.584923 redditwarp-1.0.0rc0/redditwarp/util/shdlr_ctx.py
--rw-r--r--   0        0        0     2141 2023-04-04 13:06:07.585584 redditwarp-1.0.0rc0/redditwarp/util/token_bucket.py
--rw-r--r--   0        0        0      479 2023-04-04 13:06:07.585917 redditwarp-1.0.0rc0/redditwarp/util/tree_node.py
--rw-r--r--   0        0        0       45 2023-04-04 13:06:07.586243 redditwarp-1.0.0rc0/redditwarp/websocket/ASYNC.py
--rw-r--r--   0        0        0       44 2023-04-04 13:06:07.586523 redditwarp-1.0.0rc0/redditwarp/websocket/SYNC.py
--rw-r--r--   0        0        0      205 2023-04-04 13:06:07.586811 redditwarp-1.0.0rc0/redditwarp/websocket/__init__.py
--rw-r--r--   0        0        0      753 2023-04-04 13:06:07.587063 redditwarp-1.0.0rc0/redditwarp/websocket/const.py
--rw-r--r--   0        0        0      562 2023-04-04 13:06:07.587275 redditwarp-1.0.0rc0/redditwarp/websocket/events.py
--rw-r--r--   0        0        0      399 2023-04-04 13:06:07.587495 redditwarp-1.0.0rc0/redditwarp/websocket/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.587613 redditwarp-1.0.0rc0/redditwarp/websocket/transport/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 13:06:07.587905 redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/__init__.py
--rw-r--r--   0        0        0     5317 2023-04-04 13:06:07.588623 redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/aiohttp.py
--rw-r--r--   0        0        0     4420 2023-04-04 13:06:07.589210 redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/websocket.py
--rw-r--r--   0        0        0     4489 2023-04-04 13:06:07.589724 redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/websockets.py
--rw-r--r--   0        0        0     2066 2023-04-04 13:06:07.590579 redditwarp-1.0.0rc0/redditwarp/websocket/transport/reg_ASYNC.py
--rw-r--r--   0        0        0     1997 2023-04-04 13:06:07.591233 redditwarp-1.0.0rc0/redditwarp/websocket/transport/reg_SYNC.py
--rw-r--r--   0        0        0      760 2023-04-04 13:06:07.591485 redditwarp-1.0.0rc0/redditwarp/websocket/utils.py
--rw-r--r--   0        0        0     8179 2023-04-04 13:06:07.592130 redditwarp-1.0.0rc0/redditwarp/websocket/websocket_ASYNC.py
--rw-r--r--   0        0        0     8118 2023-04-04 13:06:07.593085 redditwarp-1.0.0rc0/redditwarp/websocket/websocket_SYNC.py
--rw-r--r--   0        0        0     8611 1970-01-01 00:00:00.000000 redditwarp-1.0.0rc0/setup.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 redditwarp-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-14 14:05:01.076388 redditwarp-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5947 2023-05-14 14:05:01.079641 redditwarp-1.1.0/README.md
+-rw-r--r--   0        0        0     1218 2023-05-14 14:07:55.893028 redditwarp-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-04-04 13:11:30.907895 redditwarp-1.1.0/redditwarp/ASYNC.py
+-rw-r--r--   0        0        0      192 2023-04-04 13:11:30.908245 redditwarp-1.1.0/redditwarp/SYNC.py
+-rw-r--r--   0        0        0     3308 2023-05-14 14:07:55.893763 redditwarp-1.1.0/redditwarp/__about__.py
+-rw-r--r--   0        0        0      883 2023-04-04 13:11:30.909087 redditwarp-1.1.0/redditwarp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.909438 redditwarp-1.1.0/redditwarp/_cli/__init__.pyi
+-rw-r--r--   0        0        0      227 2023-04-04 13:11:30.909869 redditwarp-1.1.0/redditwarp/_cli/access_token.py
+-rw-r--r--   0        0        0     8020 2023-05-14 14:05:01.116376 redditwarp-1.1.0/redditwarp/_cli/comment_tree.py
+-rw-r--r--   0        0        0     3201 2023-04-04 13:11:30.910600 redditwarp-1.1.0/redditwarp/_cli/exchange_authorization_code.py
+-rw-r--r--   0        0        0     3901 2023-04-04 13:11:30.910827 redditwarp-1.1.0/redditwarp/_cli/implicit_flow.py
+-rw-r--r--   0        0        0     5909 2023-04-04 13:11:30.911063 redditwarp-1.1.0/redditwarp/_cli/refresh_token.py
+-rw-r--r--   0        0        0     3045 2023-04-04 13:11:30.911302 redditwarp-1.1.0/redditwarp/_cli/revoke_token.py
+-rw-r--r--   0        0        0      325 2023-04-04 13:11:30.911869 redditwarp-1.1.0/redditwarp/auth/ASYNC.py
+-rw-r--r--   0        0        0      321 2023-04-04 13:11:30.912197 redditwarp-1.1.0/redditwarp/auth/SYNC.py
+-rw-r--r--   0        0        0      313 2023-04-04 13:11:30.912474 redditwarp-1.1.0/redditwarp/auth/__init__.py
+-rw-r--r--   0        0        0     5356 2023-04-04 13:11:30.912770 redditwarp-1.1.0/redditwarp/auth/exceptions.py
+-rw-r--r--   0        0        0     2067 2023-04-04 13:11:30.913022 redditwarp-1.1.0/redditwarp/auth/grants.py
+-rw-r--r--   0        0        0     1142 2023-04-04 13:11:30.913266 redditwarp-1.1.0/redditwarp/auth/token.py
+-rw-r--r--   0        0        0     3120 2023-04-04 13:11:30.914074 redditwarp-1.1.0/redditwarp/auth/token_obtainment_client_ASYNC.py
+-rw-r--r--   0        0        0     3094 2023-04-04 13:11:30.915197 redditwarp-1.1.0/redditwarp/auth/token_obtainment_client_SYNC.py
+-rw-r--r--   0        0        0     2617 2023-04-04 13:11:30.915952 redditwarp-1.1.0/redditwarp/auth/token_revocation_client_ASYNC.py
+-rw-r--r--   0        0        0     2579 2023-04-04 13:11:30.916642 redditwarp-1.1.0/redditwarp/auth/token_revocation_client_SYNC.py
+-rw-r--r--   0        0        0      111 2023-04-04 13:11:30.916992 redditwarp-1.1.0/redditwarp/auth/types.py
+-rw-r--r--   0        0        0     1413 2023-04-04 13:11:30.917248 redditwarp-1.1.0/redditwarp/auth/utils.py
+-rw-r--r--   0        0        0     5519 2023-04-04 13:11:30.918327 redditwarp-1.1.0/redditwarp/client_ASYNC.py
+-rw-r--r--   0        0        0     9566 2023-04-04 13:11:30.919378 redditwarp-1.1.0/redditwarp/client_SYNC.py
+-rw-r--r--   0        0        0      565 2023-04-04 13:11:30.919943 redditwarp-1.1.0/redditwarp/core/ASYNC.py
+-rw-r--r--   0        0        0      557 2023-04-04 13:11:30.920258 redditwarp-1.1.0/redditwarp/core/SYNC.py
+-rw-r--r--   0        0        0      247 2023-04-04 13:11:30.920566 redditwarp-1.1.0/redditwarp/core/__init__.py
+-rw-r--r--   0        0        0     6813 2023-04-04 13:11:30.921421 redditwarp-1.1.0/redditwarp/core/authorizer_ASYNC.py
+-rw-r--r--   0        0        0     6395 2023-04-04 13:11:30.922285 redditwarp-1.1.0/redditwarp/core/authorizer_SYNC.py
+-rw-r--r--   0        0        0      957 2023-04-04 13:11:30.922665 redditwarp-1.1.0/redditwarp/core/const.py
+-rw-r--r--   0        0        0      885 2023-04-04 13:11:30.923294 redditwarp-1.1.0/redditwarp/core/direct_by_origin_ASYNC.py
+-rw-r--r--   0        0        0      865 2023-04-04 13:11:30.924281 redditwarp-1.1.0/redditwarp/core/direct_by_origin_SYNC.py
+-rw-r--r--   0        0        0     4146 2023-04-04 13:11:30.924648 redditwarp-1.1.0/redditwarp/core/exceptions.py
+-rw-r--r--   0        0        0      362 2023-04-04 13:11:30.924914 redditwarp-1.1.0/redditwarp/core/grants.py
+-rw-r--r--   0        0        0     5574 2023-05-14 14:05:01.117545 redditwarp-1.1.0/redditwarp/core/http_client_ASYNC.py
+-rw-r--r--   0        0        0     5525 2023-05-14 14:05:01.118534 redditwarp-1.1.0/redditwarp/core/http_client_SYNC.py
+-rw-r--r--   0        0        0     2746 2023-04-04 13:11:30.927605 redditwarp-1.1.0/redditwarp/core/rate_limited_ASYNC.py
+-rw-r--r--   0        0        0     2030 2023-04-04 13:11:30.928400 redditwarp-1.1.0/redditwarp/core/rate_limited_SYNC.py
+-rw-r--r--   0        0        0     4078 2023-04-04 13:11:30.929289 redditwarp-1.1.0/redditwarp/core/recorded_ASYNC.py
+-rw-r--r--   0        0        0     4064 2023-04-04 13:11:30.931004 redditwarp-1.1.0/redditwarp/core/recorded_SYNC.py
+-rw-r--r--   0        0        0      859 2023-04-04 13:11:30.931735 redditwarp-1.1.0/redditwarp/core/reddit_please_send_json_ASYNC.py
+-rw-r--r--   0        0        0      845 2023-04-04 13:11:30.932362 redditwarp-1.1.0/redditwarp/core/reddit_please_send_json_SYNC.py
+-rw-r--r--   0        0        0     1186 2023-04-04 13:11:30.933141 redditwarp-1.1.0/redditwarp/core/reddit_token_obtainment_client_ASYNC.py
+-rw-r--r--   0        0        0     1173 2023-04-04 13:11:30.933979 redditwarp-1.1.0/redditwarp/core/reddit_token_obtainment_client_SYNC.py
+-rw-r--r--   0        0        0      524 2023-04-04 13:11:30.934633 redditwarp-1.1.0/redditwarp/core/user_agent_ASYNC.py
+-rw-r--r--   0        0        0      523 2023-04-04 13:11:30.935020 redditwarp-1.1.0/redditwarp/core/user_agent_SYNC.py
+-rw-r--r--   0        0        0      138 2023-05-14 14:05:01.119637 redditwarp-1.1.0/redditwarp/dark/ASYNC.py
+-rw-r--r--   0        0        0      136 2023-05-14 14:05:01.120538 redditwarp-1.1.0/redditwarp/dark/SYNC.py
+-rw-r--r--   0        0        0       67 2023-04-04 13:11:30.935825 redditwarp-1.1.0/redditwarp/dark/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-04 13:11:30.936470 redditwarp-1.1.0/redditwarp/dark/auth/ASYNC.py
+-rw-r--r--   0        0        0      161 2023-04-04 13:11:30.937342 redditwarp-1.1.0/redditwarp/dark/auth/SYNC.py
+-rw-r--r--   0        0        0      122 2023-04-04 13:11:30.938545 redditwarp-1.1.0/redditwarp/dark/auth/__init__.py
+-rw-r--r--   0        0        0     1166 2023-04-04 13:11:30.939597 redditwarp-1.1.0/redditwarp/dark/auth/exceptions.py
+-rw-r--r--   0        0        0      821 2023-04-04 13:11:30.940049 redditwarp-1.1.0/redditwarp/dark/auth/token.py
+-rw-r--r--   0        0        0     1666 2023-04-04 13:11:30.940911 redditwarp-1.1.0/redditwarp/dark/auth/token_obtainment_client_ASYNC.py
+-rw-r--r--   0        0        0     1641 2023-04-04 13:11:30.941582 redditwarp-1.1.0/redditwarp/dark/auth/token_obtainment_client_SYNC.py
+-rw-r--r--   0        0        0      753 2023-05-14 14:05:01.121472 redditwarp-1.1.0/redditwarp/dark/client_ASYNC.py
+-rw-r--r--   0        0        0      750 2023-05-14 14:05:01.122292 redditwarp-1.1.0/redditwarp/dark/client_SYNC.py
+-rw-r--r--   0        0        0       35 2023-04-04 13:11:30.943321 redditwarp-1.1.0/redditwarp/dark/core/__init__.py
+-rw-r--r--   0        0        0     4286 2023-05-14 14:05:01.127857 redditwarp-1.1.0/redditwarp/dark/core/authorizer_ASYNC.py
+-rw-r--r--   0        0        0     3868 2023-05-14 14:05:01.129070 redditwarp-1.1.0/redditwarp/dark/core/authorizer_SYNC.py
+-rw-r--r--   0        0        0      954 2023-04-04 13:11:30.945781 redditwarp-1.1.0/redditwarp/dark/core/const.py
+-rw-r--r--   0        0        0     2206 2023-04-04 13:11:30.946390 redditwarp-1.1.0/redditwarp/dark/core/http_client_ASYNC.py
+-rw-r--r--   0        0        0     2195 2023-04-04 13:11:30.946932 redditwarp-1.1.0/redditwarp/dark/core/http_client_SYNC.py
+-rw-r--r--   0        0        0      780 2023-04-04 13:11:30.947199 redditwarp-1.1.0/redditwarp/dark/core/rate_limited_ASYNC.py
+-rw-r--r--   0        0        0      658 2023-04-04 13:11:30.947428 redditwarp-1.1.0/redditwarp/dark/core/rate_limited_SYNC.py
+-rw-r--r--   0        0        0      916 2023-04-04 13:11:30.948066 redditwarp-1.1.0/redditwarp/dark/siteprocs/ASYNC.py
+-rw-r--r--   0        0        0      890 2023-04-04 13:11:30.948648 redditwarp-1.1.0/redditwarp/dark/siteprocs/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.948776 redditwarp-1.1.0/redditwarp/dark/siteprocs/__init__.py
+-rw-r--r--   0        0        0     4112 2023-04-04 13:11:30.949571 redditwarp-1.1.0/redditwarp/dark/siteprocs/login/ASYNC.py
+-rw-r--r--   0        0        0     4069 2023-04-04 13:11:30.950273 redditwarp-1.1.0/redditwarp/dark/siteprocs/login/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.950389 redditwarp-1.1.0/redditwarp/dark/siteprocs/login/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.950673 redditwarp-1.1.0/redditwarp/dark/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-04-04 13:11:30.951267 redditwarp-1.1.0/redditwarp/dark/util/request_signing.py
+-rw-r--r--   0        0        0      101 2023-04-04 13:11:30.951635 redditwarp-1.1.0/redditwarp/dtos/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-04 13:11:30.951925 redditwarp-1.1.0/redditwarp/dtos/submission.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.952144 redditwarp-1.1.0/redditwarp/dtos/widget/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-04 13:11:30.952389 redditwarp-1.1.0/redditwarp/dtos/widget/button.py
+-rw-r--r--   0        0        0      228 2023-04-04 13:11:30.952613 redditwarp-1.1.0/redditwarp/dtos/widget/custom_css.py
+-rw-r--r--   0        0        0      175 2023-04-04 13:11:30.952814 redditwarp-1.1.0/redditwarp/dtos/widget/image.py
+-rw-r--r--   0        0        0      400 2023-04-04 13:11:30.953029 redditwarp-1.1.0/redditwarp/dtos/widget/menu_bar.py
+-rw-r--r--   0        0        0     6794 2023-04-04 13:11:30.953599 redditwarp-1.1.0/redditwarp/exceptions.py
+-rw-r--r--   0        0        0      484 2023-05-14 14:05:01.130347 redditwarp-1.1.0/redditwarp/http/ASYNC.py
+-rw-r--r--   0        0        0      477 2023-05-14 14:05:01.131391 redditwarp-1.1.0/redditwarp/http/SYNC.py
+-rw-r--r--   0        0        0      725 2023-04-04 13:11:30.954510 redditwarp-1.1.0/redditwarp/http/__init__.py
+-rw-r--r--   0        0        0      498 2023-04-04 13:11:30.954697 redditwarp-1.1.0/redditwarp/http/delegating_handler_ASYNC.py
+-rw-r--r--   0        0        0      473 2023-04-04 13:11:30.954909 redditwarp-1.1.0/redditwarp/http/delegating_handler_SYNC.py
+-rw-r--r--   0        0        0     4709 2023-04-04 13:11:30.955536 redditwarp-1.1.0/redditwarp/http/exceptions.py
+-rw-r--r--   0        0        0      397 2023-04-04 13:11:30.955889 redditwarp-1.1.0/redditwarp/http/exchange.py
+-rw-r--r--   0        0        0      317 2023-04-04 13:11:30.956117 redditwarp-1.1.0/redditwarp/http/handler_ASYNC.py
+-rw-r--r--   0        0        0      305 2023-04-04 13:11:30.956358 redditwarp-1.1.0/redditwarp/http/handler_SYNC.py
+-rw-r--r--   0        0        0     4205 2023-04-04 13:11:30.957116 redditwarp-1.1.0/redditwarp/http/http_client_ASYNC.py
+-rw-r--r--   0        0        0     4123 2023-04-04 13:11:30.957677 redditwarp-1.1.0/redditwarp/http/http_client_SYNC.py
+-rw-r--r--   0        0        0      407 2023-04-04 13:11:30.957946 redditwarp-1.1.0/redditwarp/http/invoker_ASYNC.py
+-rw-r--r--   0        0        0      382 2023-04-04 13:11:30.958175 redditwarp-1.1.0/redditwarp/http/invoker_SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.958392 redditwarp-1.1.0/redditwarp/http/misc/__init__.py
+-rw-r--r--   0        0        0     3315 2023-04-04 13:11:30.958872 redditwarp-1.1.0/redditwarp/http/misc/apply_params_and_headers_ASYNC.py
+-rw-r--r--   0        0        0     3241 2023-04-04 13:11:30.959586 redditwarp-1.1.0/redditwarp/http/misc/apply_params_and_headers_SYNC.py
+-rw-r--r--   0        0        0      145 2023-04-04 13:11:30.959853 redditwarp-1.1.0/redditwarp/http/misc/block_close_ASYNC.py
+-rw-r--r--   0        0        0      138 2023-04-04 13:11:30.960049 redditwarp-1.1.0/redditwarp/http/misc/block_close_SYNC.py
+-rw-r--r--   0        0        0     1651 2023-04-04 13:11:30.960982 redditwarp-1.1.0/redditwarp/http/misc/demultiplexer_ASYNC.py
+-rw-r--r--   0        0        0     1759 2023-04-04 13:11:30.961621 redditwarp-1.1.0/redditwarp/http/misc/demultiplexer_SYNC.py
+-rw-r--r--   0        0        0     3958 2023-04-04 13:11:30.962231 redditwarp-1.1.0/redditwarp/http/payload.py
+-rw-r--r--   0        0        0      378 2023-04-04 13:11:30.962469 redditwarp-1.1.0/redditwarp/http/request.py
+-rw-r--r--   0        0        0     1376 2023-04-04 13:11:30.962650 redditwarp-1.1.0/redditwarp/http/requisition.py
+-rw-r--r--   0        0        0     1104 2023-04-04 13:11:30.963138 redditwarp-1.1.0/redditwarp/http/response.py
+-rw-r--r--   0        0        0      323 2023-04-04 13:11:30.963356 redditwarp-1.1.0/redditwarp/http/send_params.py
+-rw-r--r--   0        0        0      116 2023-05-14 14:05:01.132251 redditwarp-1.1.0/redditwarp/http/transport/ASYNC.py
+-rw-r--r--   0        0        0      115 2023-05-14 14:05:01.133053 redditwarp-1.1.0/redditwarp/http/transport/SYNC.py
+-rw-r--r--   0        0        0       31 2023-04-04 13:11:30.963616 redditwarp-1.1.0/redditwarp/http/transport/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-04 13:11:30.963802 redditwarp-1.1.0/redditwarp/http/transport/connector_ASYNC.py
+-rw-r--r--   0        0        0      108 2023-04-04 13:11:30.963996 redditwarp-1.1.0/redditwarp/http/transport/connector_SYNC.py
+-rw-r--r--   0        0        0      805 2023-04-04 13:11:30.964363 redditwarp-1.1.0/redditwarp/http/transport/connectors/__init__.py
+-rw-r--r--   0        0        0     4600 2023-04-04 13:11:30.964963 redditwarp-1.1.0/redditwarp/http/transport/connectors/aiohttp.py
+-rw-r--r--   0        0        0      125 2023-04-04 13:11:30.965178 redditwarp-1.1.0/redditwarp/http/transport/connectors/httpx.py
+-rw-r--r--   0        0        0     4210 2023-04-04 13:11:30.965772 redditwarp-1.1.0/redditwarp/http/transport/connectors/httpx_async.py
+-rw-r--r--   0        0        0     4161 2023-04-04 13:11:30.966222 redditwarp-1.1.0/redditwarp/http/transport/connectors/httpx_sync.py
+-rw-r--r--   0        0        0     3557 2023-04-04 13:11:30.966447 redditwarp-1.1.0/redditwarp/http/transport/connectors/python_urllib.py
+-rw-r--r--   0        0        0     4227 2023-04-04 13:11:30.966922 redditwarp-1.1.0/redditwarp/http/transport/connectors/requests.py
+-rw-r--r--   0        0        0     5291 2023-04-04 13:11:30.967397 redditwarp-1.1.0/redditwarp/http/transport/connectors/urllib3.py
+-rw-r--r--   0        0        0     1677 2023-04-04 13:11:30.967702 redditwarp-1.1.0/redditwarp/http/transport/reg_ASYNC.py
+-rw-r--r--   0        0        0     1784 2023-04-04 13:11:30.968128 redditwarp-1.1.0/redditwarp/http/transport/reg_SYNC.py
+-rw-r--r--   0        0        0      258 2023-04-04 13:11:30.968488 redditwarp-1.1.0/redditwarp/http/types.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.968773 redditwarp-1.1.0/redditwarp/http/util/__init__.py
+-rw-r--r--   0        0        0     2794 2023-04-04 13:11:30.969091 redditwarp-1.1.0/redditwarp/http/util/case_insensitive_dict.py
+-rw-r--r--   0        0        0      204 2023-04-04 13:11:30.969360 redditwarp-1.1.0/redditwarp/http/util/guess_filename_mimetype.py
+-rw-r--r--   0        0        0     1265 2023-04-04 13:11:30.970022 redditwarp-1.1.0/redditwarp/http/util/json_loading.py
+-rw-r--r--   0        0        0     1915 2023-04-04 13:11:30.970713 redditwarp-1.1.0/redditwarp/http/util/locked_keys_mapping_proxy.py
+-rw-r--r--   0        0        0      980 2023-04-04 13:11:30.971076 redditwarp-1.1.0/redditwarp/http/util/merge_query_params.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:30.971467 redditwarp-1.1.0/redditwarp/iterators/__init__.py
+-rw-r--r--   0        0        0      612 2023-04-04 13:11:30.972162 redditwarp-1.1.0/redditwarp/iterators/async_call_chunk.py
+-rw-r--r--   0        0        0      562 2023-04-04 13:11:30.972813 redditwarp-1.1.0/redditwarp/iterators/call_chunk.py
+-rw-r--r--   0        0        0     1216 2023-04-04 13:11:30.973245 redditwarp-1.1.0/redditwarp/iterators/call_chunk_calling_async_iterator.py
+-rw-r--r--   0        0        0     1084 2023-04-04 13:11:30.973613 redditwarp-1.1.0/redditwarp/iterators/call_chunk_calling_iterator.py
+-rw-r--r--   0        0        0     1746 2023-04-04 13:11:30.973928 redditwarp-1.1.0/redditwarp/iterators/call_chunk_chaining_async_iterator.py
+-rw-r--r--   0        0        0     1593 2023-04-04 13:11:30.974197 redditwarp-1.1.0/redditwarp/iterators/call_chunk_chaining_iterator.py
+-rw-r--r--   0        0        0      329 2023-04-04 13:11:30.974510 redditwarp-1.1.0/redditwarp/iterators/call_chunking_async1.py
+-rw-r--r--   0        0        0      281 2023-04-04 13:11:30.974794 redditwarp-1.1.0/redditwarp/iterators/call_chunking_sync1.py
+-rw-r--r--   0        0        0      800 2023-04-04 13:11:30.975897 redditwarp-1.1.0/redditwarp/iterators/chunking.py
+-rw-r--r--   0        0        0     1027 2023-04-04 13:11:30.977014 redditwarp-1.1.0/redditwarp/iterators/stubborn_caller_async_iterator.py
+-rw-r--r--   0        0        0      864 2023-04-04 13:11:30.977795 redditwarp-1.1.0/redditwarp/iterators/stubborn_caller_iterator.py
+-rw-r--r--   0        0        0      965 2023-04-04 13:11:30.978856 redditwarp-1.1.0/redditwarp/iterators/unfaltering_chaining_async_iterator.py
+-rw-r--r--   0        0        0      773 2023-04-04 13:11:30.979791 redditwarp-1.1.0/redditwarp/iterators/unfaltering_chaining_iterator.py
+-rw-r--r--   0        0        0       21 2023-04-04 13:11:30.980437 redditwarp-1.1.0/redditwarp/model_loaders/__init__.py
+-rw-r--r--   0        0        0      422 2023-04-04 13:11:30.980743 redditwarp-1.1.0/redditwarp/model_loaders/comment_ASYNC.py
+-rw-r--r--   0        0        0      420 2023-04-04 13:11:30.980989 redditwarp-1.1.0/redditwarp/model_loaders/comment_SYNC.py
+-rw-r--r--   0        0        0     3902 2023-05-14 14:05:01.134273 redditwarp-1.1.0/redditwarp/model_loaders/comment_tree_ASYNC.py
+-rw-r--r--   0        0        0     3895 2023-05-14 14:05:01.135288 redditwarp-1.1.0/redditwarp/model_loaders/comment_tree_SYNC.py
+-rw-r--r--   0        0        0      298 2023-04-04 13:11:30.981651 redditwarp-1.1.0/redditwarp/model_loaders/custom_feed_ASYNC.py
+-rw-r--r--   0        0        0      296 2023-04-04 13:11:30.981860 redditwarp-1.1.0/redditwarp/model_loaders/custom_feed_SYNC.py
+-rw-r--r--   0        0        0     2116 2023-04-04 13:11:30.982096 redditwarp-1.1.0/redditwarp/model_loaders/flair.py
+-rw-r--r--   0        0        0      684 2023-05-14 14:05:01.136463 redditwarp-1.1.0/redditwarp/model_loaders/flair_emoji.py
+-rw-r--r--   0        0        0      346 2023-04-04 13:11:30.982476 redditwarp-1.1.0/redditwarp/model_loaders/karma_breakdown_entry.py
+-rw-r--r--   0        0        0      418 2023-04-04 13:11:30.982677 redditwarp-1.1.0/redditwarp/model_loaders/live_thread_ASYNC.py
+-rw-r--r--   0        0        0      416 2023-04-04 13:11:30.982852 redditwarp-1.1.0/redditwarp/model_loaders/live_thread_SYNC.py
+-rw-r--r--   0        0        0      120 2023-05-14 14:05:01.137678 redditwarp-1.1.0/redditwarp/model_loaders/media_upload_lease.py
+-rw-r--r--   0        0        0     3981 2023-05-14 14:05:01.138717 redditwarp-1.1.0/redditwarp/model_loaders/message.py
+-rw-r--r--   0        0        0     1920 2023-04-04 13:11:30.984103 redditwarp-1.1.0/redditwarp/model_loaders/message_ASYNC.py
+-rw-r--r--   0        0        0     1918 2023-04-04 13:11:30.984406 redditwarp-1.1.0/redditwarp/model_loaders/message_SYNC.py
+-rw-r--r--   0        0        0      237 2023-04-04 13:11:30.984678 redditwarp-1.1.0/redditwarp/model_loaders/moderated_subreddit.py
+-rw-r--r--   0        0        0      582 2023-04-04 13:11:30.985036 redditwarp-1.1.0/redditwarp/model_loaders/moderation_action_log_entry.py
+-rw-r--r--   0        0        0     2199 2023-04-04 13:11:30.985292 redditwarp-1.1.0/redditwarp/model_loaders/moderation_note.py
+-rw-r--r--   0        0        0      229 2023-04-04 13:11:30.985516 redditwarp-1.1.0/redditwarp/model_loaders/moderator_list.py
+-rw-r--r--   0        0        0      334 2023-04-04 13:11:30.985741 redditwarp-1.1.0/redditwarp/model_loaders/modmail.py
+-rw-r--r--   0        0        0     4832 2023-04-04 13:11:30.985988 redditwarp-1.1.0/redditwarp/model_loaders/modmail_ASYNC.py
+-rw-r--r--   0        0        0     4830 2023-04-04 13:11:30.986279 redditwarp-1.1.0/redditwarp/model_loaders/modmail_SYNC.py
+-rw-r--r--   0        0        0      290 2023-04-04 13:11:30.986581 redditwarp-1.1.0/redditwarp/model_loaders/my_account_ASYNC.py
+-rw-r--r--   0        0        0      288 2023-04-04 13:11:30.986783 redditwarp-1.1.0/redditwarp/model_loaders/my_account_SYNC.py
+-rw-r--r--   0        0        0      517 2023-04-04 13:11:30.986962 redditwarp-1.1.0/redditwarp/model_loaders/report.py
+-rw-r--r--   0        0        0      432 2023-04-04 13:11:30.987145 redditwarp-1.1.0/redditwarp/model_loaders/stylesheet.py
+-rw-r--r--   0        0        0     1228 2023-05-14 14:05:01.139758 redditwarp-1.1.0/redditwarp/model_loaders/submission.py
+-rw-r--r--   0        0        0     1478 2023-05-14 14:05:01.140725 redditwarp-1.1.0/redditwarp/model_loaders/submission_ASYNC.py
+-rw-r--r--   0        0        0     1475 2023-05-14 14:05:01.141951 redditwarp-1.1.0/redditwarp/model_loaders/submission_SYNC.py
+-rw-r--r--   0        0        0      525 2023-04-04 13:11:30.987884 redditwarp-1.1.0/redditwarp/model_loaders/submission_collection_ASYNC.py
+-rw-r--r--   0        0        0      523 2023-04-04 13:11:30.988138 redditwarp-1.1.0/redditwarp/model_loaders/submission_collection_SYNC.py
+-rw-r--r--   0        0        0     5355 2023-04-04 13:11:30.988368 redditwarp-1.1.0/redditwarp/model_loaders/submission_draft.py
+-rw-r--r--   0        0        0      576 2023-04-04 13:11:30.988618 redditwarp-1.1.0/redditwarp/model_loaders/submission_draft_ASYNC.py
+-rw-r--r--   0        0        0      573 2023-04-04 13:11:30.988812 redditwarp-1.1.0/redditwarp/model_loaders/submission_draft_SYNC.py
+-rw-r--r--   0        0        0      782 2023-05-14 14:05:01.142922 redditwarp-1.1.0/redditwarp/model_loaders/submission_media_upload_lease.py
+-rw-r--r--   0        0        0      524 2023-04-04 13:11:30.988997 redditwarp-1.1.0/redditwarp/model_loaders/subreddit_ASYNC.py
+-rw-r--r--   0        0        0      522 2023-04-04 13:11:30.989195 redditwarp-1.1.0/redditwarp/model_loaders/subreddit_SYNC.py
+-rw-r--r--   0        0        0      217 2023-04-04 13:11:30.989380 redditwarp-1.1.0/redditwarp/model_loaders/subreddit_rules.py
+-rw-r--r--   0        0        0      102 2023-05-14 14:05:01.144135 redditwarp-1.1.0/redditwarp/model_loaders/subreddit_style_asset_upload_lease.py
+-rw-r--r--   0        0        0      508 2023-04-04 13:11:30.989807 redditwarp-1.1.0/redditwarp/model_loaders/subreddit_user.py
+-rw-r--r--   0        0        0      320 2023-04-04 13:11:30.990123 redditwarp-1.1.0/redditwarp/model_loaders/trophy.py
+-rw-r--r--   0        0        0      586 2023-05-14 14:05:01.144826 redditwarp-1.1.0/redditwarp/model_loaders/upload_lease.py
+-rw-r--r--   0        0        0      472 2023-04-04 13:11:30.990314 redditwarp-1.1.0/redditwarp/model_loaders/user_ASYNC.py
+-rw-r--r--   0        0        0      470 2023-04-04 13:11:30.990510 redditwarp-1.1.0/redditwarp/model_loaders/user_SYNC.py
+-rw-r--r--   0        0        0      533 2023-04-04 13:11:30.990742 redditwarp-1.1.0/redditwarp/model_loaders/user_relationship.py
+-rw-r--r--   0        0        0      219 2023-04-04 13:11:30.990992 redditwarp-1.1.0/redditwarp/model_loaders/user_summary.py
+-rw-r--r--   0        0        0       93 2023-05-14 14:05:01.145687 redditwarp-1.1.0/redditwarp/model_loaders/widget.py
+-rw-r--r--   0        0        0    10188 2023-04-04 13:11:30.991410 redditwarp-1.1.0/redditwarp/model_loaders/widget_ASYNC.py
+-rw-r--r--   0        0        0    10187 2023-04-04 13:11:30.991692 redditwarp-1.1.0/redditwarp/model_loaders/widget_SYNC.py
+-rw-r--r--   0        0        0     1320 2023-04-04 13:11:30.991947 redditwarp-1.1.0/redditwarp/model_loaders/wiki.py
+-rw-r--r--   0        0        0     2017 2023-04-04 13:11:30.992200 redditwarp-1.1.0/redditwarp/model_loaders/wiki_ASYNC.py
+-rw-r--r--   0        0        0     2015 2023-04-04 13:11:30.992503 redditwarp-1.1.0/redditwarp/model_loaders/wiki_SYNC.py
+-rw-r--r--   0        0        0       86 2023-04-04 13:11:30.992868 redditwarp-1.1.0/redditwarp/models/__init__.py
+-rw-r--r--   0        0        0    14731 2023-05-14 14:05:01.146718 redditwarp-1.1.0/redditwarp/models/comment.py
+-rw-r--r--   0        0        0     2262 2023-04-04 13:11:30.994154 redditwarp-1.1.0/redditwarp/models/comment_ASYNC.py
+-rw-r--r--   0        0        0     2093 2023-04-04 13:11:30.994910 redditwarp-1.1.0/redditwarp/models/comment_SYNC.py
+-rw-r--r--   0        0        0      712 2023-04-04 13:11:30.995164 redditwarp-1.1.0/redditwarp/models/comment_tree_ASYNC.py
+-rw-r--r--   0        0        0      709 2023-04-04 13:11:30.995361 redditwarp-1.1.0/redditwarp/models/comment_tree_SYNC.py
+-rw-r--r--   0        0        0     2512 2023-05-14 14:05:01.147659 redditwarp-1.1.0/redditwarp/models/custom_feed.py
+-rw-r--r--   0        0        0     1185 2023-04-04 13:11:30.996455 redditwarp-1.1.0/redditwarp/models/custom_feed_ASYNC.py
+-rw-r--r--   0        0        0     1120 2023-04-04 13:11:30.997014 redditwarp-1.1.0/redditwarp/models/custom_feed_SYNC.py
+-rw-r--r--   0        0        0      780 2023-04-04 13:11:30.997481 redditwarp-1.1.0/redditwarp/models/datamemento.py
+-rw-r--r--   0        0        0     2499 2023-04-04 13:11:30.997709 redditwarp-1.1.0/redditwarp/models/flair.py
+-rw-r--r--   0        0        0     1480 2023-05-14 14:05:01.148505 redditwarp-1.1.0/redditwarp/models/flair_emoji.py
+-rw-r--r--   0        0        0      165 2023-04-04 13:11:30.998165 redditwarp-1.1.0/redditwarp/models/karma_breakdown_entry.py
+-rw-r--r--   0        0        0     4306 2023-05-14 14:05:01.149315 redditwarp-1.1.0/redditwarp/models/live_thread.py
+-rw-r--r--   0        0        0     1325 2023-04-04 13:11:30.998762 redditwarp-1.1.0/redditwarp/models/live_thread_ASYNC.py
+-rw-r--r--   0        0        0     1264 2023-04-04 13:11:30.999249 redditwarp-1.1.0/redditwarp/models/live_thread_SYNC.py
+-rw-r--r--   0        0        0      105 2023-05-14 14:05:01.150207 redditwarp-1.1.0/redditwarp/models/media_upload_lease.py
+-rw-r--r--   0        0        0     4245 2023-05-14 14:05:01.151319 redditwarp-1.1.0/redditwarp/models/message.py
+-rw-r--r--   0        0        0     1135 2023-04-04 13:11:31.000678 redditwarp-1.1.0/redditwarp/models/message_ASYNC.py
+-rw-r--r--   0        0        0     1074 2023-04-04 13:11:31.001059 redditwarp-1.1.0/redditwarp/models/message_SYNC.py
+-rw-r--r--   0        0        0     2324 2023-05-14 14:05:01.152380 redditwarp-1.1.0/redditwarp/models/moderated_subreddit.py
+-rw-r--r--   0        0        0      826 2023-04-04 13:11:31.002487 redditwarp-1.1.0/redditwarp/models/moderation_action_log_entry.py
+-rw-r--r--   0        0        0     2267 2023-04-04 13:11:31.002768 redditwarp-1.1.0/redditwarp/models/moderation_note.py
+-rw-r--r--   0        0        0     1645 2023-05-14 14:05:01.153315 redditwarp-1.1.0/redditwarp/models/moderator_list.py
+-rw-r--r--   0        0        0    13116 2023-05-14 14:05:01.154457 redditwarp-1.1.0/redditwarp/models/modmail.py
+-rw-r--r--   0        0        0     2107 2023-04-04 13:11:31.004285 redditwarp-1.1.0/redditwarp/models/modmail_ASYNC.py
+-rw-r--r--   0        0        0     2070 2023-04-04 13:11:31.004896 redditwarp-1.1.0/redditwarp/models/modmail_SYNC.py
+-rw-r--r--   0        0        0     2361 2023-05-14 14:05:01.155374 redditwarp-1.1.0/redditwarp/models/more_comments_ASYNC.py
+-rw-r--r--   0        0        0     2329 2023-05-14 14:05:01.156297 redditwarp-1.1.0/redditwarp/models/more_comments_SYNC.py
+-rw-r--r--   0        0        0     3283 2023-05-14 14:05:01.157224 redditwarp-1.1.0/redditwarp/models/my_account.py
+-rw-r--r--   0        0        0      372 2023-04-04 13:11:31.010886 redditwarp-1.1.0/redditwarp/models/my_account_ASYNC.py
+-rw-r--r--   0        0        0      371 2023-04-04 13:11:31.012150 redditwarp-1.1.0/redditwarp/models/my_account_SYNC.py
+-rw-r--r--   0        0        0      933 2023-04-04 13:11:31.012387 redditwarp-1.1.0/redditwarp/models/report.py
+-rw-r--r--   0        0        0      319 2023-04-04 13:11:31.012582 redditwarp-1.1.0/redditwarp/models/stylesheet.py
+-rw-r--r--   0        0        0    20554 2023-05-14 14:05:01.158280 redditwarp-1.1.0/redditwarp/models/submission.py
+-rw-r--r--   0        0        0     3257 2023-05-14 14:05:01.159208 redditwarp-1.1.0/redditwarp/models/submission_ASYNC.py
+-rw-r--r--   0        0        0     3086 2023-05-14 14:05:01.160125 redditwarp-1.1.0/redditwarp/models/submission_SYNC.py
+-rw-r--r--   0        0        0     4355 2023-05-14 14:05:01.161059 redditwarp-1.1.0/redditwarp/models/submission_collection.py
+-rw-r--r--   0        0        0     1797 2023-04-04 13:11:31.015780 redditwarp-1.1.0/redditwarp/models/submission_collection_ASYNC.py
+-rw-r--r--   0        0        0     1722 2023-04-04 13:11:31.016275 redditwarp-1.1.0/redditwarp/models/submission_collection_SYNC.py
+-rw-r--r--   0        0        0     3238 2023-04-04 13:11:31.016518 redditwarp-1.1.0/redditwarp/models/submission_draft.py
+-rw-r--r--   0        0        0      575 2023-04-04 13:11:31.016719 redditwarp-1.1.0/redditwarp/models/submission_draft_ASYNC.py
+-rw-r--r--   0        0        0      574 2023-04-04 13:11:31.016911 redditwarp-1.1.0/redditwarp/models/submission_draft_SYNC.py
+-rw-r--r--   0        0        0      223 2023-05-14 14:05:01.161850 redditwarp-1.1.0/redditwarp/models/submission_media_upload_lease.py
+-rw-r--r--   0        0        0    11317 2023-05-14 14:05:01.162808 redditwarp-1.1.0/redditwarp/models/subreddit.py
+-rw-r--r--   0        0        0      711 2023-04-04 13:11:31.020117 redditwarp-1.1.0/redditwarp/models/subreddit_ASYNC.py
+-rw-r--r--   0        0        0      710 2023-04-04 13:11:31.020769 redditwarp-1.1.0/redditwarp/models/subreddit_SYNC.py
+-rw-r--r--   0        0        0     2150 2023-04-04 13:11:31.021099 redditwarp-1.1.0/redditwarp/models/subreddit_rules.py
+-rw-r--r--   0        0        0       87 2023-05-14 14:05:01.163886 redditwarp-1.1.0/redditwarp/models/subreddit_style_asset_upload_lease.py
+-rw-r--r--   0        0        0     4147 2023-05-14 14:05:01.164794 redditwarp-1.1.0/redditwarp/models/subreddit_user.py
+-rw-r--r--   0        0        0      677 2023-04-04 13:11:31.022738 redditwarp-1.1.0/redditwarp/models/trophy.py
+-rw-r--r--   0        0        0      353 2023-05-14 14:05:01.165506 redditwarp-1.1.0/redditwarp/models/upload_lease.py
+-rw-r--r--   0        0        0     3953 2023-05-14 14:05:01.166435 redditwarp-1.1.0/redditwarp/models/user.py
+-rw-r--r--   0        0        0      584 2023-04-04 13:11:31.024287 redditwarp-1.1.0/redditwarp/models/user_ASYNC.py
+-rw-r--r--   0        0        0      583 2023-04-04 13:11:31.024934 redditwarp-1.1.0/redditwarp/models/user_SYNC.py
+-rw-r--r--   0        0        0     1747 2023-05-14 14:05:01.167365 redditwarp-1.1.0/redditwarp/models/user_relationship.py
+-rw-r--r--   0        0        0     1158 2023-05-14 14:05:01.168164 redditwarp-1.1.0/redditwarp/models/user_summary.py
+-rw-r--r--   0        0        0      983 2023-04-04 13:11:31.026014 redditwarp-1.1.0/redditwarp/models/widget/ASYNC.py
+-rw-r--r--   0        0        0      970 2023-04-04 13:11:31.026314 redditwarp-1.1.0/redditwarp/models/widget/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.026446 redditwarp-1.1.0/redditwarp/models/widget/__init__.py
+-rw-r--r--   0        0        0      846 2023-04-04 13:11:31.026744 redditwarp-1.1.0/redditwarp/models/widget/button.py
+-rw-r--r--   0        0        0      336 2023-04-04 13:11:31.027044 redditwarp-1.1.0/redditwarp/models/widget/button_ASYNC.py
+-rw-r--r--   0        0        0      335 2023-04-04 13:11:31.027326 redditwarp-1.1.0/redditwarp/models/widget/button_SYNC.py
+-rw-r--r--   0        0        0      272 2023-04-04 13:11:31.027589 redditwarp-1.1.0/redditwarp/models/widget/calendar.py
+-rw-r--r--   0        0        0      373 2023-04-04 13:11:31.027857 redditwarp-1.1.0/redditwarp/models/widget/calendar_ASYNC.py
+-rw-r--r--   0        0        0      372 2023-04-04 13:11:31.028128 redditwarp-1.1.0/redditwarp/models/widget/calendar_SYNC.py
+-rw-r--r--   0        0        0      301 2023-04-04 13:11:31.028381 redditwarp-1.1.0/redditwarp/models/widget/community_details_ASYNC.py
+-rw-r--r--   0        0        0      300 2023-04-04 13:11:31.028645 redditwarp-1.1.0/redditwarp/models/widget/community_details_SYNC.py
+-rw-r--r--   0        0        0      251 2023-04-04 13:11:31.028904 redditwarp-1.1.0/redditwarp/models/widget/community_list.py
+-rw-r--r--   0        0        0      336 2023-04-04 13:11:31.029144 redditwarp-1.1.0/redditwarp/models/widget/community_list_ASYNC.py
+-rw-r--r--   0        0        0      335 2023-04-04 13:11:31.029407 redditwarp-1.1.0/redditwarp/models/widget/community_list_SYNC.py
+-rw-r--r--   0        0        0      243 2023-04-04 13:11:31.029658 redditwarp-1.1.0/redditwarp/models/widget/custom_css.py
+-rw-r--r--   0        0        0      398 2023-04-04 13:11:31.029919 redditwarp-1.1.0/redditwarp/models/widget/custom_css_ASYNC.py
+-rw-r--r--   0        0        0      397 2023-04-04 13:11:31.030216 redditwarp-1.1.0/redditwarp/models/widget/custom_css_SYNC.py
+-rw-r--r--   0        0        0      276 2023-04-04 13:11:31.030578 redditwarp-1.1.0/redditwarp/models/widget/image.py
+-rw-r--r--   0        0        0      303 2023-04-04 13:11:31.030821 redditwarp-1.1.0/redditwarp/models/widget/image_ASYNC.py
+-rw-r--r--   0        0        0      302 2023-04-04 13:11:31.031037 redditwarp-1.1.0/redditwarp/models/widget/image_SYNC.py
+-rw-r--r--   0        0        0       92 2023-04-04 13:11:31.031235 redditwarp-1.1.0/redditwarp/models/widget/image_size_named_tuple.py
+-rw-r--r--   0        0        0      400 2023-04-04 13:11:31.031451 redditwarp-1.1.0/redditwarp/models/widget/menu_bar.py
+-rw-r--r--   0        0        0      321 2023-04-04 13:11:31.031959 redditwarp-1.1.0/redditwarp/models/widget/menu_bar_ASYNC.py
+-rw-r--r--   0        0        0      321 2023-04-04 13:11:31.032212 redditwarp-1.1.0/redditwarp/models/widget/menu_bar_SYNC.py
+-rw-r--r--   0        0        0      361 2023-04-04 13:11:31.032437 redditwarp-1.1.0/redditwarp/models/widget/moderator_list.py
+-rw-r--r--   0        0        0      332 2023-04-04 13:11:31.032701 redditwarp-1.1.0/redditwarp/models/widget/moderator_list_ASYNC.py
+-rw-r--r--   0        0        0      331 2023-04-04 13:11:31.032900 redditwarp-1.1.0/redditwarp/models/widget/moderator_list_SYNC.py
+-rw-r--r--   0        0        0      279 2023-04-04 13:11:31.033092 redditwarp-1.1.0/redditwarp/models/widget/post_flair.py
+-rw-r--r--   0        0        0      366 2023-04-04 13:11:31.033269 redditwarp-1.1.0/redditwarp/models/widget/post_flair_ASYNC.py
+-rw-r--r--   0        0        0      365 2023-04-04 13:11:31.033459 redditwarp-1.1.0/redditwarp/models/widget/post_flair_SYNC.py
+-rw-r--r--   0        0        0      230 2023-04-04 13:11:31.033631 redditwarp-1.1.0/redditwarp/models/widget/rules.py
+-rw-r--r--   0        0        0      298 2023-04-04 13:11:31.033804 redditwarp-1.1.0/redditwarp/models/widget/rules_ASYNC.py
+-rw-r--r--   0        0        0      297 2023-04-04 13:11:31.033975 redditwarp-1.1.0/redditwarp/models/widget/rules_SYNC.py
+-rw-r--r--   0        0        0      202 2023-04-04 13:11:31.034147 redditwarp-1.1.0/redditwarp/models/widget/text_area_ASYNC.py
+-rw-r--r--   0        0        0      201 2023-04-04 13:11:31.034457 redditwarp-1.1.0/redditwarp/models/widget/text_area_SYNC.py
+-rw-r--r--   0        0        0      350 2023-04-04 13:11:31.034675 redditwarp-1.1.0/redditwarp/models/widget/widget_ASYNC.py
+-rw-r--r--   0        0        0      350 2023-04-04 13:11:31.034858 redditwarp-1.1.0/redditwarp/models/widget/widget_SYNC.py
+-rw-r--r--   0        0        0       80 2023-05-14 14:05:01.169116 redditwarp-1.1.0/redditwarp/models/widget/widget_image_upload_lease.py
+-rw-r--r--   0        0        0     1757 2023-04-04 13:11:31.035254 redditwarp-1.1.0/redditwarp/models/widget/widget_list_ASYNC.py
+-rw-r--r--   0        0        0     1752 2023-04-04 13:11:31.035439 redditwarp-1.1.0/redditwarp/models/widget/widget_list_SYNC.py
+-rw-r--r--   0        0        0     4238 2023-05-14 14:05:01.170009 redditwarp-1.1.0/redditwarp/models/wiki.py
+-rw-r--r--   0        0        0      838 2023-04-04 13:11:31.038742 redditwarp-1.1.0/redditwarp/models/wiki_ASYNC.py
+-rw-r--r--   0        0        0      837 2023-04-04 13:11:31.042322 redditwarp-1.1.0/redditwarp/models/wiki_SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.042700 redditwarp-1.1.0/redditwarp/pagination/__init__.py
+-rw-r--r--   0        0        0     1528 2023-04-04 13:11:31.043311 redditwarp-1.1.0/redditwarp/pagination/async_paginator.py
+-rw-r--r--   0        0        0     1440 2023-04-04 13:11:31.044320 redditwarp-1.1.0/redditwarp/pagination/paginator.py
+-rw-r--r--   0        0        0     1818 2023-04-04 13:11:31.045063 redditwarp-1.1.0/redditwarp/pagination/paginator_chaining_async_iterator.py
+-rw-r--r--   0        0        0     1681 2023-04-04 13:11:31.047451 redditwarp-1.1.0/redditwarp/pagination/paginator_chaining_iterator.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.047803 redditwarp-1.1.0/redditwarp/pagination/paginators/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-04 13:11:31.048134 redditwarp-1.1.0/redditwarp/pagination/paginators/account_async1.py
+-rw-r--r--   0        0        0      545 2023-04-04 13:11:31.048399 redditwarp-1.1.0/redditwarp/pagination/paginators/account_sync1.py
+-rw-r--r--   0        0        0     2602 2023-04-04 13:11:31.049152 redditwarp-1.1.0/redditwarp/pagination/paginators/flair_async1.py
+-rw-r--r--   0        0        0     2546 2023-04-04 13:11:31.049862 redditwarp-1.1.0/redditwarp/pagination/paginators/flair_sync1.py
+-rw-r--r--   0        0        0     1268 2023-04-04 13:11:31.050200 redditwarp-1.1.0/redditwarp/pagination/paginators/front_async1.py
+-rw-r--r--   0        0        0     1173 2023-04-04 13:11:31.050459 redditwarp-1.1.0/redditwarp/pagination/paginators/front_sync1.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.050673 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-04 13:11:31.050998 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/comment_listing_async_paginator.py
+-rw-r--r--   0        0        0      460 2023-04-04 13:11:31.051282 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/comment_listing_paginator.py
+-rw-r--r--   0        0        0     3410 2023-04-04 13:11:31.051888 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/listing_async_paginator.py
+-rw-r--r--   0        0        0     3366 2023-04-04 13:11:31.052530 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/listing_paginator.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.052824 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-04 13:11:31.053429 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/sort_ASYNC.py
+-rw-r--r--   0        0        0      841 2023-04-04 13:11:31.053969 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/sort_SYNC.py
+-rw-r--r--   0        0        0      882 2023-04-04 13:11:31.054554 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_ASYNC.py
+-rw-r--r--   0        0        0      865 2023-04-04 13:11:31.055069 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_SYNC.py
+-rw-r--r--   0        0        0      855 2023-04-04 13:11:31.055596 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/time_ASYNC.py
+-rw-r--r--   0        0        0      838 2023-04-04 13:11:31.056184 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/time_SYNC.py
+-rw-r--r--   0        0        0      981 2023-04-04 13:11:31.056438 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_async_paginator.py
+-rw-r--r--   0        0        0      946 2023-04-04 13:11:31.056828 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_paginator.py
+-rw-r--r--   0        0        0      496 2023-04-04 13:11:31.057076 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_listing_async_paginator.py
+-rw-r--r--   0        0        0      461 2023-04-04 13:11:31.057285 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_listing_paginator.py
+-rw-r--r--   0        0        0      488 2023-04-04 13:11:31.057501 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/subreddit_listing_async_paginator.py
+-rw-r--r--   0        0        0      453 2023-04-04 13:11:31.057722 redditwarp-1.1.0/redditwarp/pagination/paginators/listing/subreddit_listing_paginator.py
+-rw-r--r--   0        0        0      497 2023-04-04 13:11:31.057942 redditwarp-1.1.0/redditwarp/pagination/paginators/live_thread_async1.py
+-rw-r--r--   0        0        0      462 2023-04-04 13:11:31.058152 redditwarp-1.1.0/redditwarp/pagination/paginators/live_thread_sync1.py
+-rw-r--r--   0        0        0     1474 2023-04-04 13:11:31.058352 redditwarp-1.1.0/redditwarp/pagination/paginators/message_async1.py
+-rw-r--r--   0        0        0     1373 2023-04-04 13:11:31.058560 redditwarp-1.1.0/redditwarp/pagination/paginators/message_sync1.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.058817 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/__init__.py
+-rw-r--r--   0        0        0     1709 2023-04-04 13:11:31.059058 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/async1.py
+-rw-r--r--   0        0        0     1355 2023-04-04 13:11:31.059287 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/legacy_pull_users_async1.py
+-rw-r--r--   0        0        0     1289 2023-04-04 13:11:31.059528 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/legacy_pull_users_sync1.py
+-rw-r--r--   0        0        0     3297 2023-04-04 13:11:31.059994 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/note_pulls_async1.py
+-rw-r--r--   0        0        0     3221 2023-04-04 13:11:31.060517 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/note_pulls_sync1.py
+-rw-r--r--   0        0        0     1402 2023-04-04 13:11:31.061023 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_actions_async1.py
+-rw-r--r--   0        0        0     1368 2023-04-04 13:11:31.061540 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_actions_sync1.py
+-rw-r--r--   0        0        0     4025 2023-04-04 13:11:31.061923 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_async1.py
+-rw-r--r--   0        0        0     3842 2023-04-04 13:11:31.062159 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_sync1.py
+-rw-r--r--   0        0        0     3627 2023-04-04 13:11:31.062635 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_users_async1.py
+-rw-r--r--   0        0        0     3495 2023-04-04 13:11:31.063253 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_users_sync1.py
+-rw-r--r--   0        0        0     1505 2023-04-04 13:11:31.063509 redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/sync1.py
+-rw-r--r--   0        0        0     2917 2023-04-04 13:11:31.064033 redditwarp-1.1.0/redditwarp/pagination/paginators/modmail_async1.py
+-rw-r--r--   0        0        0     2869 2023-04-04 13:11:31.064526 redditwarp-1.1.0/redditwarp/pagination/paginators/modmail_sync1.py
+-rw-r--r--   0        0        0     3679 2023-04-04 13:11:31.065037 redditwarp-1.1.0/redditwarp/pagination/paginators/submission_async1.py
+-rw-r--r--   0        0        0     3608 2023-04-04 13:11:31.065526 redditwarp-1.1.0/redditwarp/pagination/paginators/submission_sync1.py
+-rw-r--r--   0        0        0      892 2023-04-04 13:11:31.065941 redditwarp-1.1.0/redditwarp/pagination/paginators/subreddit_async1.py
+-rw-r--r--   0        0        0      868 2023-04-04 13:11:31.066403 redditwarp-1.1.0/redditwarp/pagination/paginators/subreddit_sync1.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.066698 redditwarp-1.1.0/redditwarp/pagination/paginators/user/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-04 13:11:31.066974 redditwarp-1.1.0/redditwarp/pagination/paginators/user/async1.py
+-rw-r--r--   0        0        0      922 2023-04-04 13:11:31.067458 redditwarp-1.1.0/redditwarp/pagination/paginators/user/explore_async1.py
+-rw-r--r--   0        0        0      885 2023-04-04 13:11:31.068012 redditwarp-1.1.0/redditwarp/pagination/paginators/user/explore_sync1.py
+-rw-r--r--   0        0        0     2263 2023-04-04 13:11:31.068405 redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_async1.py
+-rw-r--r--   0        0        0     2126 2023-04-04 13:11:31.068759 redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_sync1.py
+-rw-r--r--   0        0        0      360 2023-04-04 13:11:31.069104 redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_user_subreddits_async1.py
+-rw-r--r--   0        0        0      337 2023-04-04 13:11:31.069431 redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_user_subreddits_sync1.py
+-rw-r--r--   0        0        0      838 2023-04-04 13:11:31.069738 redditwarp-1.1.0/redditwarp/pagination/paginators/user/sync1.py
+-rw-r--r--   0        0        0      868 2023-04-04 13:11:31.070133 redditwarp-1.1.0/redditwarp/pagination/paginators/wiki_async1.py
+-rw-r--r--   0        0        0      832 2023-04-04 13:11:31.070452 redditwarp-1.1.0/redditwarp/pagination/paginators/wiki_sync1.py
+-rw-r--r--   0        0        0      176 2023-04-04 13:11:31.070798 redditwarp-1.1.0/redditwarp/pushshift/ASYNC.py
+-rw-r--r--   0        0        0      174 2023-04-04 13:11:31.071078 redditwarp-1.1.0/redditwarp/pushshift/SYNC.py
+-rw-r--r--   0        0        0      335 2023-04-04 13:11:31.072959 redditwarp-1.1.0/redditwarp/pushshift/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-04 13:11:31.073738 redditwarp-1.1.0/redditwarp/pushshift/client_ASYNC.py
+-rw-r--r--   0        0        0     1810 2023-04-04 13:11:31.076116 redditwarp-1.1.0/redditwarp/pushshift/client_SYNC.py
+-rw-r--r--   0        0        0       35 2023-04-04 13:11:31.076611 redditwarp-1.1.0/redditwarp/pushshift/core/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-04 13:11:31.077771 redditwarp-1.1.0/redditwarp/pushshift/core/const.py
+-rw-r--r--   0        0        0      758 2023-04-04 13:11:31.078527 redditwarp-1.1.0/redditwarp/pushshift/core/http_client_ASYNC.py
+-rw-r--r--   0        0        0      753 2023-04-04 13:11:31.081240 redditwarp-1.1.0/redditwarp/pushshift/core/http_client_SYNC.py
+-rw-r--r--   0        0        0      778 2023-04-08 04:38:51.432432 redditwarp-1.1.0/redditwarp/pushshift/core/rate_limited_ASYNC.py
+-rw-r--r--   0        0        0      656 2023-04-08 04:38:52.852763 redditwarp-1.1.0/redditwarp/pushshift/core/rate_limited_SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.086019 redditwarp-1.1.0/redditwarp/pushshift/models/__init__.py
+-rw-r--r--   0        0        0      497 2023-04-04 13:11:31.086800 redditwarp-1.1.0/redditwarp/pushshift/models/document.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.087125 redditwarp-1.1.0/redditwarp/pushshift/paginators/__init__.py
+-rw-r--r--   0        0        0     2955 2023-04-04 13:11:31.087867 redditwarp-1.1.0/redditwarp/pushshift/paginators/document_async_paginator.py
+-rw-r--r--   0        0        0     2921 2023-04-04 13:11:31.088483 redditwarp-1.1.0/redditwarp/pushshift/paginators/document_paginator.py
+-rw-r--r--   0        0        0    12170 2023-04-04 13:11:31.089355 redditwarp-1.1.0/redditwarp/pushshift/siteprocs/ASYNC.py
+-rw-r--r--   0        0        0    11988 2023-04-04 13:11:31.093658 redditwarp-1.1.0/redditwarp/pushshift/siteprocs/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.093927 redditwarp-1.1.0/redditwarp/pushshift/siteprocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.094219 redditwarp-1.1.0/redditwarp/py.typed
+-rw-r--r--   0        0        0     3212 2023-05-14 14:05:01.171181 redditwarp-1.1.0/redditwarp/siteprocs/ASYNC.py
+-rw-r--r--   0        0        0     3178 2023-05-14 14:05:01.172257 redditwarp-1.1.0/redditwarp/siteprocs/SYNC.py
+-rw-r--r--   0        0        0       38 2023-04-04 13:11:31.097052 redditwarp-1.1.0/redditwarp/siteprocs/__init__.py
+-rw-r--r--   0        0        0    14694 2023-05-14 14:05:01.173596 redditwarp-1.1.0/redditwarp/siteprocs/account/ASYNC.py
+-rw-r--r--   0        0        0    14472 2023-05-14 14:05:01.174648 redditwarp-1.1.0/redditwarp/siteprocs/account/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.099680 redditwarp-1.1.0/redditwarp/siteprocs/account/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-04 13:11:31.100428 redditwarp-1.1.0/redditwarp/siteprocs/account/pull_subreddits_ASYNC.py
+-rw-r--r--   0        0        0     1607 2023-04-04 13:11:31.100846 redditwarp-1.1.0/redditwarp/siteprocs/account/pull_subreddits_SYNC.py
+-rw-r--r--   0        0        0    16659 2023-05-14 14:05:01.175782 redditwarp-1.1.0/redditwarp/siteprocs/collection/ASYNC.py
+-rw-r--r--   0        0        0    16490 2023-05-14 14:05:01.176869 redditwarp-1.1.0/redditwarp/siteprocs/collection/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.103131 redditwarp-1.1.0/redditwarp/siteprocs/collection/__init__.py
+-rw-r--r--   0        0        0    26162 2023-05-14 14:05:01.178240 redditwarp-1.1.0/redditwarp/siteprocs/comment/ASYNC.py
+-rw-r--r--   0        0        0    25724 2023-05-14 14:05:01.179625 redditwarp-1.1.0/redditwarp/siteprocs/comment/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.109830 redditwarp-1.1.0/redditwarp/siteprocs/comment/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-14 14:05:01.180697 redditwarp-1.1.0/redditwarp/siteprocs/comment/fetch_ASYNC.py
+-rw-r--r--   0        0        0      963 2023-05-14 14:05:01.181613 redditwarp-1.1.0/redditwarp/siteprocs/comment/fetch_SYNC.py
+-rw-r--r--   0        0        0     1071 2023-05-14 14:05:01.182531 redditwarp-1.1.0/redditwarp/siteprocs/comment/get_ASYNC.py
+-rw-r--r--   0        0        0     1032 2023-05-14 14:05:01.183509 redditwarp-1.1.0/redditwarp/siteprocs/comment/get_SYNC.py
+-rw-r--r--   0        0        0     8304 2023-05-14 14:05:01.184715 redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/ASYNC.py
+-rw-r--r--   0        0        0     8251 2023-05-14 14:05:01.185747 redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.113657 redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/__init__.py
+-rw-r--r--   0        0        0     3729 2023-04-04 13:11:31.114049 redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/low_ASYNC.py
+-rw-r--r--   0        0        0     3676 2023-04-04 13:11:31.114340 redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/low_SYNC.py
+-rw-r--r--   0        0        0    14034 2023-04-04 13:11:31.115879 redditwarp-1.1.0/redditwarp/siteprocs/custom_feed/ASYNC.py
+-rw-r--r--   0        0        0    13804 2023-04-04 13:11:31.116737 redditwarp-1.1.0/redditwarp/siteprocs/custom_feed/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.116900 redditwarp-1.1.0/redditwarp/siteprocs/custom_feed/__init__.py
+-rw-r--r--   0        0        0     6959 2023-05-14 14:05:01.186926 redditwarp-1.1.0/redditwarp/siteprocs/draft/ASYNC.py
+-rw-r--r--   0        0        0     6895 2023-05-14 14:05:01.187890 redditwarp-1.1.0/redditwarp/siteprocs/draft/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.120842 redditwarp-1.1.0/redditwarp/siteprocs/draft/__init__.py
+-rw-r--r--   0        0        0    37848 2023-05-14 14:05:01.189350 redditwarp-1.1.0/redditwarp/siteprocs/flair/ASYNC.py
+-rw-r--r--   0        0        0    37333 2023-05-14 14:05:01.190592 redditwarp-1.1.0/redditwarp/siteprocs/flair/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.123851 redditwarp-1.1.0/redditwarp/siteprocs/flair/__init__.py
+-rw-r--r--   0        0        0     8534 2023-05-14 14:05:01.192207 redditwarp-1.1.0/redditwarp/siteprocs/flair_emoji/ASYNC.py
+-rw-r--r--   0        0        0     8401 2023-05-14 14:05:01.193399 redditwarp-1.1.0/redditwarp/siteprocs/flair_emoji/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.126011 redditwarp-1.1.0/redditwarp/siteprocs/flair_emoji/__init__.py
+-rw-r--r--   0        0        0      987 2023-04-04 13:11:31.127009 redditwarp-1.1.0/redditwarp/siteprocs/front/ASYNC.py
+-rw-r--r--   0        0        0      942 2023-04-04 13:11:31.127307 redditwarp-1.1.0/redditwarp/siteprocs/front/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.127414 redditwarp-1.1.0/redditwarp/siteprocs/front/__init__.py
+-rw-r--r--   0        0        0     2696 2023-04-04 13:11:31.127814 redditwarp-1.1.0/redditwarp/siteprocs/front/pull_ASYNC.py
+-rw-r--r--   0        0        0     2507 2023-04-04 13:11:31.128168 redditwarp-1.1.0/redditwarp/siteprocs/front/pull_SYNC.py
+-rw-r--r--   0        0        0    19432 2023-05-14 14:05:01.194958 redditwarp-1.1.0/redditwarp/siteprocs/live_thread/ASYNC.py
+-rw-r--r--   0        0        0    19120 2023-05-14 14:05:01.196104 redditwarp-1.1.0/redditwarp/siteprocs/live_thread/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.134358 redditwarp-1.1.0/redditwarp/siteprocs/live_thread/__init__.py
+-rw-r--r--   0        0        0    11002 2023-05-14 14:05:01.197378 redditwarp-1.1.0/redditwarp/siteprocs/message/ASYNC.py
+-rw-r--r--   0        0        0    10804 2023-05-14 14:05:01.198531 redditwarp-1.1.0/redditwarp/siteprocs/message/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.135754 redditwarp-1.1.0/redditwarp/siteprocs/message/__init__.py
+-rw-r--r--   0        0        0     2727 2023-04-04 13:11:31.136069 redditwarp-1.1.0/redditwarp/siteprocs/message/pulls_ASYNC.py
+-rw-r--r--   0        0        0     2553 2023-04-04 13:11:31.136436 redditwarp-1.1.0/redditwarp/siteprocs/message/pulls_SYNC.py
+-rw-r--r--   0        0        0      938 2023-04-04 13:11:31.137306 redditwarp-1.1.0/redditwarp/siteprocs/misc/ASYNC.py
+-rw-r--r--   0        0        0      913 2023-04-04 13:11:31.137729 redditwarp-1.1.0/redditwarp/siteprocs/misc/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.137862 redditwarp-1.1.0/redditwarp/siteprocs/misc/__init__.py
+-rw-r--r--   0        0        0    30093 2023-05-14 14:05:01.199766 redditwarp-1.1.0/redditwarp/siteprocs/moderation/ASYNC.py
+-rw-r--r--   0        0        0    29792 2023-05-14 14:05:01.200878 redditwarp-1.1.0/redditwarp/siteprocs/moderation/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.143474 redditwarp-1.1.0/redditwarp/siteprocs/moderation/__init__.py
+-rw-r--r--   0        0        0     4474 2023-04-04 13:11:31.144640 redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_ASYNC.py
+-rw-r--r--   0        0        0     4400 2023-04-04 13:11:31.145718 redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_SYNC.py
+-rw-r--r--   0        0        0     2394 2023-04-04 13:11:31.146283 redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_pull_users_ASYNC.py
+-rw-r--r--   0        0        0     2271 2023-04-04 13:11:31.146843 redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_pull_users_SYNC.py
+-rw-r--r--   0        0        0     9715 2023-04-04 13:11:31.147624 redditwarp-1.1.0/redditwarp/siteprocs/moderation/note_ASYNC.py
+-rw-r--r--   0        0        0     9539 2023-04-04 13:11:31.148070 redditwarp-1.1.0/redditwarp/siteprocs/moderation/note_SYNC.py
+-rw-r--r--   0        0        0     7419 2023-04-04 13:11:31.148822 redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_ASYNC.py
+-rw-r--r--   0        0        0     7060 2023-04-04 13:11:31.149710 redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_SYNC.py
+-rw-r--r--   0        0        0     3596 2023-04-04 13:11:31.150909 redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_users_ASYNC.py
+-rw-r--r--   0        0        0     3426 2023-04-04 13:11:31.151314 redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_users_SYNC.py
+-rw-r--r--   0        0        0     1862 2023-04-04 13:11:31.152261 redditwarp-1.1.0/redditwarp/siteprocs/modmail/ASYNC.py
+-rw-r--r--   0        0        0     1835 2023-04-04 13:11:31.157549 redditwarp-1.1.0/redditwarp/siteprocs/modmail/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.157756 redditwarp-1.1.0/redditwarp/siteprocs/modmail/__init__.py
+-rw-r--r--   0        0        0    24848 2023-05-14 14:05:01.202284 redditwarp-1.1.0/redditwarp/siteprocs/modmail/conversation_ASYNC.py
+-rw-r--r--   0        0        0    24268 2023-05-14 14:05:01.203438 redditwarp-1.1.0/redditwarp/siteprocs/modmail/conversation_SYNC.py
+-rw-r--r--   0        0        0     4741 2023-04-04 13:11:31.159875 redditwarp-1.1.0/redditwarp/siteprocs/modmail/pull_ASYNC.py
+-rw-r--r--   0        0        0     4592 2023-04-04 13:11:31.160159 redditwarp-1.1.0/redditwarp/siteprocs/modmail/pull_SYNC.py
+-rw-r--r--   0        0        0    55156 2023-05-14 14:05:01.204977 redditwarp-1.1.0/redditwarp/siteprocs/submission/ASYNC.py
+-rw-r--r--   0        0        0    54068 2023-05-14 14:05:01.206415 redditwarp-1.1.0/redditwarp/siteprocs/submission/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.166481 redditwarp-1.1.0/redditwarp/siteprocs/submission/__init__.py
+-rw-r--r--   0        0        0     8063 2023-05-14 14:05:01.207616 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/ASYNC.py
+-rw-r--r--   0        0        0     8055 2023-05-14 14:05:01.209340 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/SYNC.py
+-rw-r--r--   0        0        0     5906 2023-05-14 14:05:01.212558 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/cross_ASYNC.py
+-rw-r--r--   0        0        0     5851 2023-05-14 14:05:01.213431 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/cross_SYNC.py
+-rw-r--r--   0        0        0     6109 2023-05-14 14:05:01.214112 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/gallery_ASYNC.py
+-rw-r--r--   0        0        0     6054 2023-05-14 14:05:01.214865 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/gallery_SYNC.py
+-rw-r--r--   0        0        0     2314 2023-05-14 14:05:01.219293 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/image_ASYNC.py
+-rw-r--r--   0        0        0     2295 2023-05-14 14:05:01.221473 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/image_SYNC.py
+-rw-r--r--   0        0        0     5975 2023-05-14 14:05:01.222272 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/link_ASYNC.py
+-rw-r--r--   0        0        0     5920 2023-05-14 14:05:01.223042 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/link_SYNC.py
+-rw-r--r--   0        0        0     6003 2023-05-14 14:05:01.223780 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/poll_ASYNC.py
+-rw-r--r--   0        0        0     5948 2023-05-14 14:05:01.224525 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/poll_SYNC.py
+-rw-r--r--   0        0        0     6007 2023-05-14 14:05:01.225319 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/text_ASYNC.py
+-rw-r--r--   0        0        0     5952 2023-05-14 14:05:01.225977 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/text_SYNC.py
+-rw-r--r--   0        0        0     2522 2023-05-14 14:05:01.226958 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/video_ASYNC.py
+-rw-r--r--   0        0        0     2503 2023-05-14 14:05:01.227710 redditwarp-1.1.0/redditwarp/siteprocs/submission/create/video_SYNC.py
+-rw-r--r--   0        0        0     2353 2023-05-14 14:05:01.228904 redditwarp-1.1.0/redditwarp/siteprocs/submission/fetch_ASYNC.py
+-rw-r--r--   0        0        0     2313 2023-05-14 14:05:01.229834 redditwarp-1.1.0/redditwarp/siteprocs/submission/fetch_SYNC.py
+-rw-r--r--   0        0        0     2143 2023-05-14 14:05:01.235356 redditwarp-1.1.0/redditwarp/siteprocs/submission/get_ASYNC.py
+-rw-r--r--   0        0        0     2104 2023-05-14 14:05:01.236467 redditwarp-1.1.0/redditwarp/siteprocs/submission/get_SYNC.py
+-rw-r--r--   0        0        0    19996 2023-05-14 14:05:01.237680 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/ASYNC.py
+-rw-r--r--   0        0        0    19443 2023-05-14 14:05:01.242436 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.172458 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/__init__.py
+-rw-r--r--   0        0        0     2507 2023-04-04 13:11:31.173120 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pull_ASYNC.py
+-rw-r--r--   0        0        0     2343 2023-04-04 13:11:31.173740 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pull_SYNC.py
+-rw-r--r--   0        0        0     1674 2023-04-04 13:11:31.174299 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pulls_ASYNC.py
+-rw-r--r--   0        0        0     1570 2023-04-04 13:11:31.174749 redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pulls_SYNC.py
+-rw-r--r--   0        0        0     9066 2023-05-14 14:05:01.244680 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_new/ASYNC.py
+-rw-r--r--   0        0        0     8909 2023-05-14 14:05:01.246234 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_new/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.177192 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_new/__init__.py
+-rw-r--r--   0        0        0     8021 2023-04-04 13:11:31.178309 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_old/ASYNC.py
+-rw-r--r--   0        0        0     7900 2023-04-04 13:11:31.178710 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_old/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.178877 redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_old/__init__.py
+-rw-r--r--   0        0        0     9471 2023-05-14 14:05:01.247530 redditwarp-1.1.0/redditwarp/siteprocs/user/ASYNC.py
+-rw-r--r--   0        0        0     9085 2023-05-14 14:05:01.249880 redditwarp-1.1.0/redditwarp/siteprocs/user/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.180916 redditwarp-1.1.0/redditwarp/siteprocs/user/__init__.py
+-rw-r--r--   0        0        0     4702 2023-04-04 13:11:31.182343 redditwarp-1.1.0/redditwarp/siteprocs/user/pull_ASYNC.py
+-rw-r--r--   0        0        0     4417 2023-04-04 13:11:31.182652 redditwarp-1.1.0/redditwarp/siteprocs/user/pull_SYNC.py
+-rw-r--r--   0        0        0     1065 2023-04-04 13:11:31.182886 redditwarp-1.1.0/redditwarp/siteprocs/user/pull_subreddits_ASYNC.py
+-rw-r--r--   0        0        0     1006 2023-04-04 13:11:31.183138 redditwarp-1.1.0/redditwarp/siteprocs/user/pull_subreddits_SYNC.py
+-rw-r--r--   0        0        0    24239 2023-05-14 14:05:01.255452 redditwarp-1.1.0/redditwarp/siteprocs/widget/ASYNC.py
+-rw-r--r--   0        0        0    23893 2023-05-14 14:05:01.256737 redditwarp-1.1.0/redditwarp/siteprocs/widget/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.185080 redditwarp-1.1.0/redditwarp/siteprocs/widget/__init__.py
+-rw-r--r--   0        0        0    13377 2023-04-04 13:11:31.185907 redditwarp-1.1.0/redditwarp/siteprocs/wiki/ASYNC.py
+-rw-r--r--   0        0        0    13120 2023-04-04 13:11:31.188415 redditwarp-1.1.0/redditwarp/siteprocs/wiki/SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.188605 redditwarp-1.1.0/redditwarp/siteprocs/wiki/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-04 13:11:31.189052 redditwarp-1.1.0/redditwarp/streaming/ASYNC.py
+-rw-r--r--   0        0        0       95 2023-04-04 13:11:31.189312 redditwarp-1.1.0/redditwarp/streaming/SYNC.py
+-rw-r--r--   0        0        0       48 2023-04-04 13:11:31.189570 redditwarp-1.1.0/redditwarp/streaming/__init__.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:11:31.190047 redditwarp-1.1.0/redditwarp/streaming/async1.py
+-rw-r--r--   0        0        0     1590 2023-05-14 14:05:01.258003 redditwarp-1.1.0/redditwarp/streaming/impls/modmail_stream_ASYNC.py
+-rw-r--r--   0        0        0     1572 2023-05-14 14:05:01.258892 redditwarp-1.1.0/redditwarp/streaming/impls/modmail_stream_SYNC.py
+-rw-r--r--   0        0        0     7181 2023-05-14 14:05:01.264845 redditwarp-1.1.0/redditwarp/streaming/impls/stream_ASYNC.py
+-rw-r--r--   0        0        0     6641 2023-05-14 14:05:01.265696 redditwarp-1.1.0/redditwarp/streaming/impls/stream_SYNC.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.190342 redditwarp-1.1.0/redditwarp/streaming/makers/__init__.py
+-rw-r--r--   0        0        0     2013 2023-05-14 14:05:01.266688 redditwarp-1.1.0/redditwarp/streaming/makers/message_ASYNC.py
+-rw-r--r--   0        0        0     1977 2023-05-14 14:05:01.267723 redditwarp-1.1.0/redditwarp/streaming/makers/message_SYNC.py
+-rw-r--r--   0        0        0     1169 2023-05-14 14:05:01.268641 redditwarp-1.1.0/redditwarp/streaming/makers/moderation_ASYNC.py
+-rw-r--r--   0        0        0     1145 2023-05-14 14:05:01.270157 redditwarp-1.1.0/redditwarp/streaming/makers/moderation_SYNC.py
+-rw-r--r--   0        0        0     4406 2023-05-14 14:05:01.271084 redditwarp-1.1.0/redditwarp/streaming/makers/modmail_ASYNC.py
+-rw-r--r--   0        0        0     4331 2023-05-14 14:05:01.271888 redditwarp-1.1.0/redditwarp/streaming/makers/modmail_SYNC.py
+-rw-r--r--   0        0        0     2480 2023-05-14 14:05:01.272668 redditwarp-1.1.0/redditwarp/streaming/makers/subreddit_ASYNC.py
+-rw-r--r--   0        0        0     2433 2023-05-14 14:05:01.273462 redditwarp-1.1.0/redditwarp/streaming/makers/subreddit_SYNC.py
+-rw-r--r--   0        0        0     1069 2023-05-14 14:05:01.274260 redditwarp-1.1.0/redditwarp/streaming/makers/user_ASYNC.py
+-rw-r--r--   0        0        0     1044 2023-05-14 14:05:01.275148 redditwarp-1.1.0/redditwarp/streaming/makers/user_SYNC.py
+-rw-r--r--   0        0        0     1028 2023-04-04 13:11:31.194300 redditwarp-1.1.0/redditwarp/streaming/runners_ASYNC.py
+-rw-r--r--   0        0        0      576 2023-04-04 13:11:31.194524 redditwarp-1.1.0/redditwarp/streaming/runners_SYNC.py
+-rw-r--r--   0        0        0      294 2023-04-04 13:11:31.196358 redditwarp-1.1.0/redditwarp/types.py
+-rw-r--r--   0        0        0       17 2023-04-04 13:11:31.196787 redditwarp-1.1.0/redditwarp/util/__init__.py
+-rw-r--r--   0        0        0     4988 2023-04-04 13:11:31.197039 redditwarp-1.1.0/redditwarp/util/attribute_mapping_proxy.py
+-rw-r--r--   0        0        0     1451 2023-04-04 13:11:31.197265 redditwarp-1.1.0/redditwarp/util/base_conversion.py
+-rw-r--r--   0        0        0      778 2023-04-04 13:11:31.197473 redditwarp-1.1.0/redditwarp/util/booleanify.py
+-rw-r--r--   0        0        0      353 2023-04-04 13:11:31.197677 redditwarp-1.1.0/redditwarp/util/bot_user_agent.py
+-rw-r--r--   0        0        0      894 2023-05-14 14:05:01.275959 redditwarp-1.1.0/redditwarp/util/ctx_var_ctx_mgr.py
+-rw-r--r--   0        0        0     3784 2023-04-04 13:11:31.197916 redditwarp-1.1.0/redditwarp/util/data_members_namespace.py
+-rw-r--r--   0        0        0     2430 2023-04-04 13:11:31.198127 redditwarp-1.1.0/redditwarp/util/event_dispatcher.py
+-rw-r--r--   0        0        0     2054 2023-04-04 13:11:31.198662 redditwarp-1.1.0/redditwarp/util/except_without_context.py
+-rw-r--r--   0        0        0     2562 2023-05-14 14:05:01.276873 redditwarp-1.1.0/redditwarp/util/extract_id_from_url.py
+-rw-r--r--   0        0        0     1996 2023-04-04 13:11:31.199126 redditwarp-1.1.0/redditwarp/util/imports.py
+-rw-r--r--   0        0        0     2163 2023-05-14 14:05:01.277931 redditwarp-1.1.0/redditwarp/util/ordered_set.py
+-rw-r--r--   0        0        0      660 2023-04-04 13:11:31.199556 redditwarp-1.1.0/redditwarp/util/passthru.py
+-rw-r--r--   0        0        0     1272 2023-04-04 13:11:31.199822 redditwarp-1.1.0/redditwarp/util/praw_config.py
+-rw-r--r--   0        0        0     1238 2023-04-04 13:11:31.200297 redditwarp-1.1.0/redditwarp/util/praw_config_ASYNC.py
+-rw-r--r--   0        0        0     1236 2023-04-04 13:11:31.200534 redditwarp-1.1.0/redditwarp/util/praw_config_SYNC.py
+-rw-r--r--   0        0        0      336 2023-04-04 13:11:31.200745 redditwarp-1.1.0/redditwarp/util/redditwarp_installed_client_credentials.py
+-rw-r--r--   0        0        0     3788 2023-04-04 13:11:31.201240 redditwarp-1.1.0/redditwarp/util/shdlr.py
+-rw-r--r--   0        0        0      638 2023-04-04 13:11:31.201470 redditwarp-1.1.0/redditwarp/util/shdlr_ctx.py
+-rw-r--r--   0        0        0     2141 2023-04-04 13:11:31.201970 redditwarp-1.1.0/redditwarp/util/token_bucket.py
+-rw-r--r--   0        0        0      479 2023-04-04 13:11:31.202190 redditwarp-1.1.0/redditwarp/util/tree_node.py
+-rw-r--r--   0        0        0       45 2023-04-04 13:11:31.202405 redditwarp-1.1.0/redditwarp/websocket/ASYNC.py
+-rw-r--r--   0        0        0       44 2023-04-04 13:11:31.202582 redditwarp-1.1.0/redditwarp/websocket/SYNC.py
+-rw-r--r--   0        0        0      205 2023-04-04 13:11:31.202831 redditwarp-1.1.0/redditwarp/websocket/__init__.py
+-rw-r--r--   0        0        0      753 2023-04-04 13:11:31.203039 redditwarp-1.1.0/redditwarp/websocket/const.py
+-rw-r--r--   0        0        0      562 2023-04-04 13:11:31.203264 redditwarp-1.1.0/redditwarp/websocket/events.py
+-rw-r--r--   0        0        0      399 2023-04-04 13:11:31.203504 redditwarp-1.1.0/redditwarp/websocket/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.203621 redditwarp-1.1.0/redditwarp/websocket/transport/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:11:31.203817 redditwarp-1.1.0/redditwarp/websocket/transport/carriers/__init__.py
+-rw-r--r--   0        0        0     5306 2023-05-14 14:05:01.279293 redditwarp-1.1.0/redditwarp/websocket/transport/carriers/aiohttp.py
+-rw-r--r--   0        0        0     4536 2023-05-14 14:05:01.280281 redditwarp-1.1.0/redditwarp/websocket/transport/carriers/websocket.py
+-rw-r--r--   0        0        0     4478 2023-05-14 14:05:01.281101 redditwarp-1.1.0/redditwarp/websocket/transport/carriers/websockets.py
+-rw-r--r--   0        0        0     2066 2023-04-04 13:11:31.206455 redditwarp-1.1.0/redditwarp/websocket/transport/reg_ASYNC.py
+-rw-r--r--   0        0        0     1997 2023-04-04 13:11:31.207153 redditwarp-1.1.0/redditwarp/websocket/transport/reg_SYNC.py
+-rw-r--r--   0        0        0      760 2023-04-04 13:11:31.207411 redditwarp-1.1.0/redditwarp/websocket/utils.py
+-rw-r--r--   0        0        0     8179 2023-04-04 13:11:31.208003 redditwarp-1.1.0/redditwarp/websocket/websocket_ASYNC.py
+-rw-r--r--   0        0        0     8118 2023-04-04 13:11:31.208629 redditwarp-1.1.0/redditwarp/websocket/websocket_SYNC.py
+-rw-r--r--   0        0        0     8702 1970-01-01 00:00:00.000000 redditwarp-1.1.0/setup.py
+-rw-r--r--   0        0        0     6863 1970-01-01 00:00:00.000000 redditwarp-1.1.0/PKG-INFO
```

### Comparing `redditwarp-1.0.0rc0/LICENSE` & `redditwarp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/README.md` & `redditwarp-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ## Features
 
 * A consistent and easy-to-use programming interface.
 * Modern type-complete codebase.
 * Sync and asynchronous IO support.
 * Automatic rate limit handling.
 * A comprehensive and discoverable index of API procedures.
-* Model classes that sensibly wrap API structures.
+* Model classes that are fully typed and sensibly wrap API structures.
 * Formal data structures to facilitate comment tree traversals and pagination.
 * HTTP transport library agnosticism.
 * OAuth2 tooling and CLI utilities to help manage auth tokens.
 * A simple event-based listing endpoint streaming framework.
 
 ## Installation
```

### Comparing `redditwarp-1.0.0rc0/pyproject.toml` & `redditwarp-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = 'redditwarp'
-version = "1.0.0rc"
+version = "1.1.0"
 description = "A library for interacting with the Reddit API."
 authors = ["Pyprohly <pyprohly@gmail.com>"]
 readme = "README.md"
 license = 'MIT'
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/__about__.py` & `redditwarp-1.1.0/redditwarp/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 #
 #
 #############################################################################
 
 from __future__ import annotations
 
 version_major: int = 1
-version_minor: int = 0
+version_minor: int = 1
 version_micro: int = 0
-version_extra: str = 'rc'
+version_extra: str = ''
 
 version_patch: int = version_micro
 version_triad: tuple[int, int, int] = (version_major, version_minor, version_micro)
 version_string: str = '.'.join(map(str, version_triad)) + version_extra
 
 __version__: str = version_string
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/__init__.py` & `redditwarp-1.1.0/redditwarp/__init__.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/_cli/comment_tree.py` & `redditwarp-1.1.0/redditwarp/_cli/comment_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,17 +149,17 @@
         node_batch = deque(node_queue)
         more_batch = deque(more_queue)
         queue.clear()
         node_queue.clear()
         more_queue.clear()
         while batch:
             if batch.popleft():
-                node = node_batch.pop()
+                node = node_batch.popleft()
             else:
-                node = more_batch.pop()()
+                node = more_batch.popleft()()
 
             if node.value is None:
                 if node.more:
                     batch.appendleft(False)
                     more_batch.appendleft(node.more)
                 batch.extendleft([True] * len(node.children))
                 node_batch.extendleft(reversed(node.children))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/_cli/exchange_authorization_code.py` & `redditwarp-1.1.0/redditwarp/_cli/exchange_authorization_code.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/_cli/implicit_flow.py` & `redditwarp-1.1.0/redditwarp/_cli/implicit_flow.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/_cli/refresh_token.py` & `redditwarp-1.1.0/redditwarp/_cli/refresh_token.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/_cli/revoke_token.py` & `redditwarp-1.1.0/redditwarp/_cli/revoke_token.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/exceptions.py` & `redditwarp-1.1.0/redditwarp/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/grants.py` & `redditwarp-1.1.0/redditwarp/auth/grants.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/token.py` & `redditwarp-1.1.0/redditwarp/auth/token.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/token_obtainment_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/auth/token_obtainment_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/token_obtainment_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/auth/token_obtainment_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/token_revocation_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/auth/token_revocation_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/token_revocation_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/auth/token_revocation_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/auth/utils.py` & `redditwarp-1.1.0/redditwarp/auth/utils.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/client_SYNC.py` & `redditwarp-1.1.0/redditwarp/client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/SYNC.py` & `redditwarp-1.1.0/redditwarp/core/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/authorizer_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/authorizer_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/authorizer_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/authorizer_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/const.py` & `redditwarp-1.1.0/redditwarp/core/const.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/direct_by_origin_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/direct_by_origin_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/direct_by_origin_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/direct_by_origin_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/exceptions.py` & `redditwarp-1.1.0/redditwarp/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/http_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/http_client_ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, MutableMapping
+from typing import TYPE_CHECKING, Optional, MutableMapping, Callable, ContextManager
 if TYPE_CHECKING:
-    from ..http.handler_ASYNC import Handler
+    from ..http.send_params import SendParams
+    from ..http.exchange import Exchange
+
+from contextvars import ContextVar
 
 from .const import RESOURCE_BASE_URL, TOKEN_OBTAINMENT_URL, TRUSTED_ORIGINS
 from ..http.http_client_ASYNC import HTTPClient as BaseHTTPClient
 from ..auth.types import AuthorizationGrant
 from .authorizer_ASYNC import Authorized
 from .rate_limited_ASYNC import RateLimited
 from .recorded_ASYNC import Recorded
@@ -15,34 +18,46 @@
 from ..http.transport.reg_ASYNC import new_connector
 from ..http.util.case_insensitive_dict import CaseInsensitiveDict
 from ..http.misc.apply_params_and_headers_ASYNC import ApplyDefaultHeaders
 from .user_agent_ASYNC import get_user_agent
 from ..auth.token import Token
 from .recorded_ASYNC import Last
 from .authorizer_ASYNC import Authorizer
-from ..http.send_params import SendParams
-from ..http.exchange import Exchange
 from .direct_by_origin_ASYNC import DirectByOrigin
+from ..http.handler_ASYNC import Handler
+from ..util.ctx_var_ctx_mgr import ContextVarContextManager
 
 
 DEFAULT_TIMEOUT: float = 8
 
 
 class HTTPClient(BaseHTTPClient):
     """An HTTP client specialised for the purposes of this library."""
 
+    class _MyHandler(Handler):
+        def __init__(self, active_handler_var: ContextVar[Handler]) -> None:
+            super().__init__()
+            self._active_handler_var: ContextVar[Handler] = active_handler_var
+
+        async def _send(self, p: SendParams) -> Exchange:
+            return await self._active_handler_var.get()._send(p)
+
+        async def _close(self) -> None:
+            await self._active_handler_var.get()._close()
+
     @property
     def last(self) -> Last:
         return self._last
 
     def __init__(self, handler: Handler, *,
         headers: Optional[MutableMapping[str, str]] = None,
     ) -> None:
         recorder = Recorded(handler)
-        super().__init__(recorder)
+        self._active_handler_var: ContextVar[Handler] = ContextVar('active_handler', default=recorder)
+        super().__init__(self._MyHandler(self._active_handler_var))
         self.base_url: str = RESOURCE_BASE_URL
         ("")
         self.timeout: float = DEFAULT_TIMEOUT
         ("")
         self.user_agent_base: str = ''
         ("")
         self.headers: MutableMapping[str, str] = CaseInsensitiveDict() if headers is None else headers
@@ -58,14 +73,17 @@
 
     def set_user_agent(self, value: Optional[str]) -> None:
         if value is None:
             self.headers.pop('User-Agent', None)
         else:
             self.headers['User-Agent'] = value
 
+    def having_additional_middleware(self, f: Callable[[Handler], Handler]) -> ContextManager[None]:
+        return ContextVarContextManager(self._active_handler_var, f(self._active_handler_var.get()))
+
 
 class RedditHTTPClient(HTTPClient):
     """An HTTP client for making requests to the public Reddit API."""
 
     @property
     def authorizer(self) -> Authorizer:
         return self.fetch_authorizer()
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/http_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/http_client_SYNC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, MutableMapping
+from typing import TYPE_CHECKING, Optional, MutableMapping, Callable, ContextManager
 if TYPE_CHECKING:
-    from ..http.handler_SYNC import Handler
+    from ..http.send_params import SendParams
+    from ..http.exchange import Exchange
+
+from contextvars import ContextVar
 
 from .const import RESOURCE_BASE_URL, TOKEN_OBTAINMENT_URL, TRUSTED_ORIGINS
 from ..http.http_client_SYNC import HTTPClient as BaseHTTPClient
 from ..auth.types import AuthorizationGrant
 from .authorizer_SYNC import Authorized
 from .rate_limited_SYNC import RateLimited
 from .recorded_SYNC import Recorded
@@ -15,34 +18,46 @@
 from ..http.transport.reg_SYNC import new_connector
 from ..http.util.case_insensitive_dict import CaseInsensitiveDict
 from ..http.misc.apply_params_and_headers_SYNC import ApplyDefaultHeaders
 from .user_agent_SYNC import get_user_agent
 from ..auth.token import Token
 from .recorded_SYNC import Last
 from .authorizer_SYNC import Authorizer
-from ..http.send_params import SendParams
-from ..http.exchange import Exchange
 from .direct_by_origin_SYNC import DirectByOrigin
+from ..http.handler_SYNC import Handler
+from ..util.ctx_var_ctx_mgr import ContextVarContextManager
 
 
 DEFAULT_TIMEOUT: float = 8
 
 
 class HTTPClient(BaseHTTPClient):
     """An HTTP client specialised for the purposes of this library."""
 
+    class _MyHandler(Handler):
+        def __init__(self, active_handler_var: ContextVar[Handler]) -> None:
+            super().__init__()
+            self._active_handler_var: ContextVar[Handler] = active_handler_var
+
+        def _send(self, p: SendParams) -> Exchange:
+            return self._active_handler_var.get()._send(p)
+
+        def _close(self) -> None:
+            self._active_handler_var.get()._close()
+
     @property
     def last(self) -> Last:
         return self._last
 
     def __init__(self, handler: Handler, *,
         headers: Optional[MutableMapping[str, str]] = None,
     ) -> None:
         recorder = Recorded(handler)
-        super().__init__(recorder)
+        self._active_handler_var: ContextVar[Handler] = ContextVar('active_handler', default=recorder)
+        super().__init__(self._MyHandler(self._active_handler_var))
         self.base_url: str = RESOURCE_BASE_URL
         ("")
         self.timeout: float = DEFAULT_TIMEOUT
         ("")
         self.user_agent_base: str = ''
         ("")
         self.headers: MutableMapping[str, str] = CaseInsensitiveDict() if headers is None else headers
@@ -58,14 +73,17 @@
 
     def set_user_agent(self, value: Optional[str]) -> None:
         if value is None:
             self.headers.pop('User-Agent', None)
         else:
             self.headers['User-Agent'] = value
 
+    def having_additional_middleware(self, f: Callable[[Handler], Handler]) -> ContextManager[None]:
+        return ContextVarContextManager(self._active_handler_var, f(self._active_handler_var.get()))
+
 
 class RedditHTTPClient(HTTPClient):
     """An HTTP client for making requests to the public Reddit API."""
 
     @property
     def authorizer(self) -> Authorizer:
         return self.fetch_authorizer()
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/rate_limited_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/rate_limited_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/rate_limited_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/rate_limited_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/recorded_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/recorded_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/recorded_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/recorded_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/reddit_please_send_json_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/reddit_please_send_json_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/reddit_please_send_json_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/reddit_please_send_json_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/reddit_token_obtainment_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/reddit_token_obtainment_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/reddit_token_obtainment_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/reddit_token_obtainment_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/user_agent_ASYNC.py` & `redditwarp-1.1.0/redditwarp/core/user_agent_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/core/user_agent_SYNC.py` & `redditwarp-1.1.0/redditwarp/core/user_agent_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/auth/exceptions.py` & `redditwarp-1.1.0/redditwarp/dark/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/auth/token.py` & `redditwarp-1.1.0/redditwarp/dark/auth/token.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/auth/token_obtainment_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/auth/token_obtainment_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/auth/token_obtainment_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/auth/token_obtainment_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/client_ASYNC.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 
     def _init(self, http: HTTPClient) -> None:
         self.http: HTTPClient = http
         ("")
 
         from .siteprocs.ASYNC import Procedures
         self.p: Procedures = Procedures(self.http)
+
+DarkClient = Client
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/client_SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/client_SYNC.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 
     def _init(self, http: HTTPClient) -> None:
         self.http: HTTPClient = http
         ("")
 
         from .siteprocs.SYNC import Procedures
         self.p: Procedures = Procedures(self.http)
+
+DarkClient = Client
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/authorizer_ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/authorizer_ASYNC.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,52 +21,52 @@
 
 
 class Authorizer:
     def __init__(self,
         token_client: Optional[TokenObtainmentClient] = None,
         token: Optional[Token] = None,
     ) -> None:
-        self._token_client: Optional[TokenObtainmentClient] = token_client
+        self.token_client: Optional[TokenObtainmentClient] = token_client
         ("")
-        self._token: Optional[Token] = token
+        self.token: Optional[Token] = token
         ("")
         self.renewal_time: Optional[float] = None
         ("")
         self.renewal_skew: float = 30
         ("")
         self.expires_in_fallback: Optional[int] = None
         ("")
         self.time_func: Callable[[], float] = time.monotonic
         ("")
         self.authorization_header_name: str = 'Authorization'
         ("")
 
     def has_token_client(self) -> bool:
-        return self._token_client is not None
+        return self.token_client is not None
 
     def fetch_token_client(self) -> TokenObtainmentClient:
-        v = self._token_client
+        v = self.token_client
         if v is None:
             raise RuntimeError('token client not set')
         return v
 
     def set_token_client(self, value: Optional[TokenObtainmentClient]) -> None:
-        self._token_client = value
+        self.token_client = value
 
     def has_token(self) -> bool:
-        return self._token is not None
+        return self.token is not None
 
     def fetch_token(self) -> Token:
-        v = self._token
+        v = self.token
         if v is None:
             raise RuntimeError('token not set')
         return v
 
     def set_token(self, value: Optional[Token]) -> None:
-        self._token = value
+        self.token = value
 
     async def renew_token(self) -> None:
         tc = self.fetch_token_client()
         tk = await tc.fetch_token()
 
         self.set_token(tk)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/authorizer_SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/authorizer_SYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,52 +15,52 @@
 
 
 class Authorizer:
     def __init__(self,
         token_client: Optional[TokenObtainmentClient] = None,
         token: Optional[Token] = None,
     ) -> None:
-        self._token_client: Optional[TokenObtainmentClient] = token_client
+        self.token_client: Optional[TokenObtainmentClient] = token_client
         ("")
-        self._token: Optional[Token] = token
+        self.token: Optional[Token] = token
         ("")
         self.renewal_time: Optional[float] = None
         ("")
         self.renewal_skew: float = 30
         ("")
         self.expires_in_fallback: Optional[int] = None
         ("")
         self.time_func: Callable[[], float] = time.monotonic
         ("")
         self.authorization_header_name: str = 'Authorization'
         ("")
 
     def has_token_client(self) -> bool:
-        return self._token_client is not None
+        return self.token_client is not None
 
     def fetch_token_client(self) -> TokenObtainmentClient:
-        v = self._token_client
+        v = self.token_client
         if v is None:
             raise RuntimeError('token client not set')
         return v
 
     def set_token_client(self, value: Optional[TokenObtainmentClient]) -> None:
-        self._token_client = value
+        self.token_client = value
 
     def has_token(self) -> bool:
-        return self._token is not None
+        return self.token is not None
 
     def fetch_token(self) -> Token:
-        v = self._token
+        v = self.token
         if v is None:
             raise RuntimeError('token not set')
         return v
 
     def set_token(self, value: Optional[Token]) -> None:
-        self._token = value
+        self.token = value
 
     def renew_token(self) -> None:
         tc = self.fetch_token_client()
         tk = tc.fetch_token()
 
         self.set_token(tk)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/const.py` & `redditwarp-1.1.0/redditwarp/dark/core/const.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/http_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/http_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/http_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/http_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/rate_limited_ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/rate_limited_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/core/rate_limited_SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/core/rate_limited_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/siteprocs/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/siteprocs/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/login/ASYNC.py` & `redditwarp-1.1.0/redditwarp/dark/siteprocs/login/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/siteprocs/login/SYNC.py` & `redditwarp-1.1.0/redditwarp/dark/siteprocs/login/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dark/util/request_signing.py` & `redditwarp-1.1.0/redditwarp/dark/util/request_signing.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/dtos/widget/button.py` & `redditwarp-1.1.0/redditwarp/dtos/widget/button.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/exceptions.py` & `redditwarp-1.1.0/redditwarp/exceptions.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/__init__.py` & `redditwarp-1.1.0/redditwarp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/exceptions.py` & `redditwarp-1.1.0/redditwarp/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/http_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/http/http_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/http_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/http/http_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/misc/apply_params_and_headers_ASYNC.py` & `redditwarp-1.1.0/redditwarp/http/misc/apply_params_and_headers_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/misc/apply_params_and_headers_SYNC.py` & `redditwarp-1.1.0/redditwarp/http/misc/apply_params_and_headers_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/misc/demultiplexer_ASYNC.py` & `redditwarp-1.1.0/redditwarp/http/misc/demultiplexer_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/misc/demultiplexer_SYNC.py` & `redditwarp-1.1.0/redditwarp/http/misc/demultiplexer_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/payload.py` & `redditwarp-1.1.0/redditwarp/http/payload.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/requisition.py` & `redditwarp-1.1.0/redditwarp/http/requisition.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/response.py` & `redditwarp-1.1.0/redditwarp/http/response.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/__init__.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/aiohttp.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/httpx_async.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/httpx_async.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/httpx_sync.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/httpx_sync.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/python_urllib.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/python_urllib.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/requests.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/requests.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/connectors/urllib3.py` & `redditwarp-1.1.0/redditwarp/http/transport/connectors/urllib3.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/reg_ASYNC.py` & `redditwarp-1.1.0/redditwarp/http/transport/reg_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/transport/reg_SYNC.py` & `redditwarp-1.1.0/redditwarp/http/transport/reg_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/util/case_insensitive_dict.py` & `redditwarp-1.1.0/redditwarp/http/util/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/util/json_loading.py` & `redditwarp-1.1.0/redditwarp/http/util/json_loading.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/util/locked_keys_mapping_proxy.py` & `redditwarp-1.1.0/redditwarp/http/util/locked_keys_mapping_proxy.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/http/util/merge_query_params.py` & `redditwarp-1.1.0/redditwarp/http/util/merge_query_params.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/async_call_chunk.py` & `redditwarp-1.1.0/redditwarp/iterators/async_call_chunk.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk.py` & `redditwarp-1.1.0/redditwarp/iterators/call_chunk.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_calling_async_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/call_chunk_calling_async_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_calling_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/call_chunk_calling_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_chaining_async_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/call_chunk_chaining_async_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/call_chunk_chaining_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/call_chunk_chaining_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/chunking.py` & `redditwarp-1.1.0/redditwarp/iterators/chunking.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/stubborn_caller_async_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/stubborn_caller_async_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/stubborn_caller_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/stubborn_caller_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/unfaltering_chaining_async_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/unfaltering_chaining_async_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/iterators/unfaltering_chaining_iterator.py` & `redditwarp-1.1.0/redditwarp/iterators/unfaltering_chaining_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_tree_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/comment_tree_ASYNC.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,46 +77,40 @@
             node = load_comment_tree_node(m['data'], client, submission_id36, sort)
             children.append(node)
 
     return SubmissionTreeNode(value, children, more)
 
 
 def load_more_comments_tree_node(d: Any, client: Client, submission_id36: str, sort: str) -> MoreCommentsTreeNode:
-    value_lookup: dict[str, Comment] = {}
-    children_lookup: dict[str, list[CommentTreeNode]] = {}
-    more_lookup: dict[str, MoreComments] = {}
+    value_lookup: dict[object, Comment] = {}
+    children_lookup: dict[object, list[CommentTreeNode]] = {}
+    more_lookup: dict[object, MoreComments] = {}
 
     elements = d['json']['data']['things']
     for m in elements:
         data = m['data']
-        kind = m['kind']
-        if kind == 'more':
-            more = load_more_comments(data, client, submission_id36, sort)
-            parent_idt = data['parent_id']
-            more_lookup[parent_idt] = more
+        if m['kind'] == 'more':
+            more_lookup[data['parent_id']] = load_more_comments(data, client, submission_id36, sort)
         else:
-            value = load_comment(data, client)
-            children: list[CommentTreeNode] = []
             idt = data['name']
-            value_lookup[idt] = value
-            children_lookup[idt] = children
+            value_lookup[idt] = load_comment(data, client)
+            children_lookup[idt] = []
 
     root_children: list[CommentTreeNode] = []
     for m in elements:
         data = m['data']
-        kind = m['kind']
-        if kind != 'more':
+        if m['kind'] != 'more':
             idt = data['name']
-            node = CommentTreeNode(
-                value_lookup[idt],
-                children_lookup[idt],
-                more_lookup.pop(idt, None),
+            children_lookup.get(data['parent_id'], root_children).append(
+                CommentTreeNode(
+                    value_lookup[idt],
+                    children_lookup[idt],
+                    more_lookup.pop(idt, None),
+                ),
             )
-            parent_idt = data['parent_id']
-            children_lookup.get(parent_idt, root_children).append(node)
 
     root_more = None
     if more_lookup:
         root_more = more_lookup.popitem()[1]
     if more_lookup:
         raise Exception
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/comment_tree_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/comment_tree_SYNC.py`

 * *Files 26% similar despite different names*

```diff
@@ -77,46 +77,40 @@
             node = load_comment_tree_node(m['data'], client, submission_id36, sort)
             children.append(node)
 
     return SubmissionTreeNode(value, children, more)
 
 
 def load_more_comments_tree_node(d: Any, client: Client, submission_id36: str, sort: str) -> MoreCommentsTreeNode:
-    value_lookup: dict[str, Comment] = {}
-    children_lookup: dict[str, list[CommentTreeNode]] = {}
-    more_lookup: dict[str, MoreComments] = {}
+    value_lookup: dict[object, Comment] = {}
+    children_lookup: dict[object, list[CommentTreeNode]] = {}
+    more_lookup: dict[object, MoreComments] = {}
 
     elements = d['json']['data']['things']
     for m in elements:
         data = m['data']
-        kind = m['kind']
-        if kind == 'more':
-            more = load_more_comments(data, client, submission_id36, sort)
-            parent_idt = data['parent_id']
-            more_lookup[parent_idt] = more
+        if m['kind'] == 'more':
+            more_lookup[data['parent_id']] = load_more_comments(data, client, submission_id36, sort)
         else:
-            value = load_comment(data, client)
-            children: list[CommentTreeNode] = []
             idt = data['name']
-            value_lookup[idt] = value
-            children_lookup[idt] = children
+            value_lookup[idt] = load_comment(data, client)
+            children_lookup[idt] = []
 
     root_children: list[CommentTreeNode] = []
     for m in elements:
         data = m['data']
-        kind = m['kind']
-        if kind != 'more':
+        if m['kind'] != 'more':
             idt = data['name']
-            node = CommentTreeNode(
-                value_lookup[idt],
-                children_lookup[idt],
-                more_lookup.pop(idt, None),
+            children_lookup.get(data['parent_id'], root_children).append(
+                CommentTreeNode(
+                    value_lookup[idt],
+                    children_lookup[idt],
+                    more_lookup.pop(idt, None),
+                ),
             )
-            parent_idt = data['parent_id']
-            children_lookup.get(parent_idt, root_children).append(node)
 
     root_more = None
     if more_lookup:
         root_more = more_lookup.popitem()[1]
     if more_lookup:
         raise Exception
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/flair.py` & `redditwarp-1.1.0/redditwarp/model_loaders/flair.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/message.py` & `redditwarp-1.1.0/redditwarp/model_loaders/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,15 +81,16 @@
             author_id=int(d['author_fullname'].partition('_')[2], 36),
             subreddit_name=d['subreddit'],
             permalink_path=(permalink_path := context.partition('?')[0]),
             permalink=AUTHORIZATION_BASE_URL + permalink_path,
             is_top_level=(is_top_level := (parent_id := d['parent_id']).startswith('t3_')),
             has_parent_comment=(has_parent_comment := not is_top_level),
             parent_comment_id36=(parent_comment_id36 := parent_id.partition('_')[2] if has_parent_comment else ''),
-            parent_comment_id=int(parent_comment_id36, 36) if has_parent_comment else 0,
+            parent_comment_idn=(parent_comment_idn := int(parent_comment_id36, 36) if has_parent_comment else 0),
+            parent_comment_id=parent_comment_idn,
             score=d['score'],
             body=d['body'],
             body_html=d['body_html'],
             voted={False: -1, None: 0, True: 1}[d['likes']],
         ),
     )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/message_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/message_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/message_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/message_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/moderation_action_log_entry.py` & `redditwarp-1.1.0/redditwarp/model_loaders/moderation_action_log_entry.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/moderation_note.py` & `redditwarp-1.1.0/redditwarp/model_loaders/moderation_note.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/modmail_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/modmail_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/modmail_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/modmail_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/report.py` & `redditwarp-1.1.0/redditwarp/model_loaders/report.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 
 def load_submission(d: Mapping[str, Any]) -> Submission:
     if d.get('is_gallery', False):
         return load_gallery_post(d)
     if 'poll_data' in d:
         return load_poll_post(d)
     if 'crosspost_parent' in d:
-        return load_crosspost_submission(d)
+        return load_cross_post(d)
     if d['is_self']:
         return load_text_post(d)
     if 'url_overridden_by_dest' in d:
         return load_link_post(d)
     raise Exception('unknown post type')
 
 
-def load_text_post(d: Mapping[str, Any]) -> TextPost:
-    return TextPost(d)
-
 def load_link_post(d: Mapping[str, Any]) -> LinkPost:
     return LinkPost(d)
 
+def load_text_post(d: Mapping[str, Any]) -> TextPost:
+    return TextPost(d)
+
 def load_gallery_post(d: Mapping[str, Any]) -> GalleryPost:
     return GalleryPost(d)
 
 def load_poll_post(d: Mapping[str, Any]) -> PollPost:
     return PollPost(d)
 
 def load_crosspost_submission(d: Mapping[str, Any]) -> CrosspostSubmission:
     return CrosspostSubmission(d)
+
+def load_cross_post(d: Mapping[str, Any]) -> CrosspostSubmission:
+    return load_crosspost_submission(d)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_ASYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 
 def load_submission(d: Mapping[str, Any], client: Client) -> Submission:
     if d.get('is_gallery', False):
         return load_gallery_post(d, client)
     if 'poll_data' in d:
         return load_poll_post(d, client)
     if 'crosspost_parent' in d:
-        return load_crosspost_submission(d, client)
+        return load_cross_post(d, client)
     if d['is_self']:
         return load_text_post(d, client)
     if 'url_overridden_by_dest' in d:
         return load_link_post(d, client)
     raise Exception('unknown post type')
 
 
-def load_text_post(d: Mapping[str, Any], client: Client) -> TextPost:
-    return TextPost(d, client)
-
 def load_link_post(d: Mapping[str, Any], client: Client) -> LinkPost:
     return LinkPost(d, client)
 
+def load_text_post(d: Mapping[str, Any], client: Client) -> TextPost:
+    return TextPost(d, client)
+
 def load_gallery_post(d: Mapping[str, Any], client: Client) -> GalleryPost:
     return GalleryPost(d, client)
 
 def load_poll_post(d: Mapping[str, Any], client: Client) -> PollPost:
     return PollPost(d, client)
 
 def load_crosspost_submission(d: Mapping[str, Any], client: Client) -> CrosspostSubmission:
     return CrosspostSubmission(d, client)
+
+def load_cross_post(d: Mapping[str, Any], client: Client) -> CrosspostSubmission:
+    return load_crosspost_submission(d, client)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_SYNC.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 
 def load_submission(d: Mapping[str, Any], client: Client) -> Submission:
     if d.get('is_gallery', False):
         return load_gallery_post(d, client)
     if 'poll_data' in d:
         return load_poll_post(d, client)
     if 'crosspost_parent' in d:
-        return load_crosspost_submission(d, client)
+        return load_cross_post(d, client)
     if d['is_self']:
         return load_text_post(d, client)
     if 'url_overridden_by_dest' in d:
         return load_link_post(d, client)
     raise Exception('unknown post type')
 
 
-def load_text_post(d: Mapping[str, Any], client: Client) -> TextPost:
-    return TextPost(d, client)
-
 def load_link_post(d: Mapping[str, Any], client: Client) -> LinkPost:
     return LinkPost(d, client)
 
+def load_text_post(d: Mapping[str, Any], client: Client) -> TextPost:
+    return TextPost(d, client)
+
 def load_gallery_post(d: Mapping[str, Any], client: Client) -> GalleryPost:
     return GalleryPost(d, client)
 
 def load_poll_post(d: Mapping[str, Any], client: Client) -> PollPost:
     return PollPost(d, client)
 
 def load_crosspost_submission(d: Mapping[str, Any], client: Client) -> CrosspostSubmission:
     return CrosspostSubmission(d, client)
+
+def load_cross_post(d: Mapping[str, Any], client: Client) -> CrosspostSubmission:
+    return load_crosspost_submission(d, client)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_collection_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_collection_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_collection_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_collection_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_draft.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_draft_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/submission_draft_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/submission_draft_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/subreddit_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/subreddit_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/subreddit_style_asset_upload_lease.py` & `redditwarp-1.1.0/redditwarp/model_loaders/upload_lease.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from __future__ import annotations
 from typing import Mapping, Any
 
-from ..models.subreddit_style_asset_upload_lease import SubredditStyleAssetUploadLease
+from ..models.upload_lease import UploadLease
 
-def load_subreddit_style_asset_upload_lease(d: Mapping[str, Any]) -> SubredditStyleAssetUploadLease:
+def load_upload_lease(d: Mapping[str, Any]) -> UploadLease:
     lease_data = d['s3UploadLease']
     endpoint = f'https:{x}' if (x := lease_data['action']).startswith('//') else x
     fields = {field['name']: field['value'] for field in lease_data['fields']}
     s3_object_key = fields['key']
-    return SubredditStyleAssetUploadLease(
+    return UploadLease(
         d=d,
         endpoint=endpoint,
         fields=fields,
         s3_object_key=s3_object_key,
         location=f"{endpoint}/{s3_object_key}",
     )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/user_relationship.py` & `redditwarp-1.1.0/redditwarp/model_loaders/user_relationship.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/widget_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/widget_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/widget_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/widget_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki.py` & `redditwarp-1.1.0/redditwarp/model_loaders/wiki.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki_ASYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/wiki_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/model_loaders/wiki_SYNC.py` & `redditwarp-1.1.0/redditwarp/model_loaders/wiki_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/comment.py` & `redditwarp-1.1.0/redditwarp/models/comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,42 +98,48 @@
                     """)
 
         def __init__(self, d: Mapping[str, Any]) -> None:
             self.name: str = d['author']
             ("")
             self.id36: str = d['author_fullname'].split('_', 1)[-1]
             ("")
-            self.id: int = int(self.id36, 36)
+            self.idn: int = int(self.id36, 36)
+            ("")
+            self.id: int = self.idn
             ("")
             self.has_premium: bool = d['author_premium']
             ("")
             self.flair: Comment.Author.AuthorFlair = self.AuthorFlair(d)
             ("""
                 Attributes related to the author's flair.
                 """)
 
     class Submission:
         def __init__(self, d: Mapping[str, Any]) -> None:
             self.id36: str = d['link_id'].split('_', 1)[-1]
             ("")
-            self.id: int = int(self.id36, 36)
+            self.idn: int = int(self.id36, 36)
+            ("")
+            self.id: int = self.idn
             ("")
             self.archived: bool = d['archived']
             ("""
                 Whether the post is archived.
 
                 Archived posts cannot be commented on,
                 but the author can still edit the OP.
                 """)
 
     class Subreddit:
         def __init__(self, d: Mapping[str, Any]) -> None:
             self.id36: str = d['subreddit_id'].split('_', 1)[-1]
             ("")
-            self.id: int = int(self.id36, 36)
+            self.idn: int = int(self.id36, 36)
+            ("")
+            self.id: int = self.idn
             ("")
             self.name: str = d['subreddit']
             ("")
             self.openness: str = d['subreddit_type']
             ("""
                 One of: `public`, `private`, `restricted`, `archived`,
                 `employees_only`, `gold_only`, `gold_restricted`, or `user`.
@@ -213,15 +219,17 @@
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         super().__init__(d)
         self.id36: str = d['id']
         ("""
             ID of the comment as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         self.created_ut: int = int(d['created_utc'])
         ("""
             Unix timestamp of when the comment was made.
             """)
         self.created_at: datetime = datetime.fromtimestamp(self.created_ut, timezone.utc)
         ("""
@@ -309,23 +317,27 @@
             """)
         self.parent_comment_id36: str = ''
         ("""
             Parent comment ID36.
 
             Empty string if not applicable.
             """)
-        self.parent_comment_id: int = 0
+        self.parent_comment_idn: int = 0
         ("""
             Parent comment ID.
 
             Value is `0` if not applicable.
             """)
         if self.has_parent_comment:
             self.parent_comment_id36 = parent_id.partition('_')[2]
-            self.parent_comment_id = int(self.parent_comment_id36, 36)
+            self.parent_comment_idn = int(self.parent_comment_id36, 36)
+        self.parent_comment_id: int = self.parent_comment_idn
+        ("""
+            Same as :attr:`parent_comment_idn`.
+            """)
 
         self.me: Comment.Me = self.Me(d)
         ("""
             Attributes relating to the current user.
 
             If there is no user context, these values contain nonsense.
             """)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/comment_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/comment_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/comment_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/comment_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/comment_tree_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/comment_tree_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/comment_tree_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/comment_tree_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/custom_feed.py` & `redditwarp-1.1.0/redditwarp/models/custom_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
         ("""
             The curator of the custom feed.
             """)
         full_id36: str = d['owner_id']
         _, _, id36 = full_id36.partition('_')
         self.owner_id36: str = id36
         ("")
-        self.owner_id: int = int(id36, 36)
+        self.owner_idn: int = int(id36, 36)
+        ("")
+        self.owner_id: int = self.owner_idn
         ("")
         self.name: str = d['name']
         ("")
         self.title: str = d['display_name']
         ("")
         self.description: str = d['description_md']
         ("")
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/custom_feed_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/custom_feed_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/custom_feed_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/custom_feed_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/datamemento.py` & `redditwarp-1.1.0/redditwarp/models/datamemento.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/flair.py` & `redditwarp-1.1.0/redditwarp/models/flair.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/flair_emoji.py` & `redditwarp-1.1.0/redditwarp/models/flair_emoji.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 
 from __future__ import annotations
 from typing import Mapping, Any, Iterator
 
 from dataclasses import dataclass
 
-from .datamemento import DatamementoDataclassesMixin
+from .upload_lease import UploadLease as FlairEmojiUploadLease  # noqa: F401
 
 
 @dataclass(repr=False, eq=False)
-class FlairEmojiUploadLease(DatamementoDataclassesMixin):
-    d: Mapping[str, Any]
-    endpoint: str
-    fields: Mapping[str, str]
-    s3_object_key: str
-    location: str
-
-@dataclass(repr=False, eq=False)
 class FlairEmoji:
     d: Mapping[str, Any]
     name: str
     image_url: str
+    creator_idn: int
     creator_id: int
     creator_id36: str
     post_enabled: bool
     user_enabled: bool
     mod_only: bool
 
 
@@ -39,15 +32,17 @@
         ("")
         self.reddit_emojis: Mapping[str, FlairEmoji] = reddit_emojis
         ("")
         self.all_emojis: Mapping[str, FlairEmoji] = all_emojis
         ("")
         self.subreddit_id36: str = subreddit_id36
         ("")
-        self.subreddit_id: int = int(subreddit_id36, 36)
+        self.subreddit_idn: int = int(subreddit_id36, 36)
+        ("")
+        self.subreddit_id: int = self.subreddit_idn
         ("")
 
     def __contains__(self, item: object) -> bool:
         return item in self.all_emojis
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.all_emojis)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/live_thread.py` & `redditwarp-1.1.0/redditwarp/models/live_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,18 +92,22 @@
             """)
         full_id36: str = d['id']
         _, _, id36 = full_id36.partition('_')
         self.id36: str = id36
         ("""
             Contributor's user ID as a base 36 number.
             """)
-        self.id: int = int(id36, 36)
+        self.idn: int = int(self.id36, 36)
         ("""
             Contributor's user ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.permissions: Sequence[str] = d['permissions']
         ("""
             Values: `all`, `close`, `discussions`, `edit`, `manage`, `settings`, `update`.
 
             Can be empty. This means no permissions.
             """)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/live_thread_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/live_thread_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/live_thread_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/live_thread_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/message.py` & `redditwarp-1.1.0/redditwarp/models/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
             `<https://github.com/Pyprohly/redditwarp/issues>`_.
             """)
         permalink_path: str
         permalink: str
         is_top_level: bool
         has_parent_comment: bool
         parent_comment_id36: str
+        parent_comment_idn: int
         parent_comment_id: int
         score: int
         body: str
         body_html: str
         voted: int
 
     cause: CommentMessageCause
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/message_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/message_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/message_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/message_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/moderated_subreddit.py` & `redditwarp-1.1.0/redditwarp/models/moderated_subreddit.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,22 @@
         self.d: Mapping[str, Any] = d
         ("")
         full_id36: str = d['name']
         self.id36: str = full_id36[3:]
         ("""
             The ID of the subreddit as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
         ("""
             The subreddit ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['display_name']
         ("""
             The name of the subreddit.
             """)
         self.openness: str = d['subreddit_type']
         ("""
             Either: `public`, `private`, `restricted`, `archived`,
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/moderation_action_log_entry.py` & `redditwarp-1.1.0/redditwarp/models/moderation_action_log_entry.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/moderation_note.py` & `redditwarp-1.1.0/redditwarp/models/moderation_note.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/moderator_list.py` & `redditwarp-1.1.0/redditwarp/models/moderator_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,22 @@
         ("")
         full_id36: str = d['id']
         _, _, id36 = full_id36.partition('_')
         self.id36: str = id36
         ("""
             User ID of the moderator as a base 36 number.
             """)
-        self.id: int = int(id36, 36)
+        self.idn: int = int(id36, 36)
         ("""
             User ID of the moderator.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['name']
         ("""
             The moderator's user name.
             """)
         #self.rel_id: str = d['rel_id']
         self.added_ut: int = int(d['date'])
         ("""
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/modmail.py` & `redditwarp-1.1.0/redditwarp/models/modmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     subscriber_count: int
 
 
 class ConversationInfo(DatamementoPropertiesMixin):
     @dataclass(repr=False, eq=False)
     class LegacyMessage:
         id: int
+        idn: int
         id36: str
         link: str
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("")
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         self.subject: str = d['subject']
         ("")
         self.progress: int = d['state']
         ("""
             Enum: :class:`.ConversationProgress`
             """)
@@ -85,15 +88,17 @@
             The underlying data can be null in rare cases, such as in the
             "r/{subreddit} is now enrolled in the New Modmail"
             modmail message from u/reddit.
             """)
         if (x := d['legacyFirstMessageId']) is not None:
             self.legacy_message = self.LegacyMessage(
                 id36=x,
-                id=int(x, 36),
+                idn=(idn := int(x, 36)),
+                # https://github.com/python/mypy/issues
+                id=idn,  # type: ignore[has-type]
                 link="https://www.reddit.com/message/messages/" + x,
             )
 
         self.last_updated_by_user_at: Optional[datetime] = (x := d['lastUserUpdate']) and datetime.fromisoformat(x)
         ("""
             If :attr:`internal` is true this should always be null.
             """)
@@ -119,15 +124,17 @@
 
 class Message(DatamementoPropertiesMixin):
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("")
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         author = d['author']
         self.author_name: str = author['name']
         ("""
             User name of the author of the message.
 
             Unknown what happens if the user is deleted.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/modmail_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/modmail_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/modmail_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/modmail_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/more_comments_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/more_comments_ASYNC.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 class ContinueThisThread(MoreComments):
     async def __call__(self, *,
         depth: Optional[int] = None,
     ) -> MoreCommentsTreeNode:
         node = await self.client.p.comment_tree.low.fetch(self.submission_id36, self.comment_id36)
         return MoreCommentsTreeNode(None, node.children[0].children, node.more)
 
+DepthMoreComments = ContinueThisThread
+
 class LoadMoreComments(MoreComments):
     def __init__(self,
         *,
         submission_id36: str,
         comment_id36: str,
         child_id36s: Sequence[str],
         sort: str,
@@ -78,7 +80,9 @@
         return await self.client.p.comment_tree.low.more_children(
             self.submission_id36,
             self.child_id36s,
             sort=self.sort,
             depth=depth,
             exact=exact,
         )
+
+BreadthMoreComments = LoadMoreComments
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/more_comments_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/more_comments_SYNC.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 class ContinueThisThread(MoreComments):
     def __call__(self, *,
         depth: Optional[int] = None,
     ) -> MoreCommentsTreeNode:
         node = self.client.p.comment_tree.low.fetch(self.submission_id36, self.comment_id36)
         return MoreCommentsTreeNode(None, node.children[0].children, node.more)
 
+DepthMoreComments = ContinueThisThread
+
 class LoadMoreComments(MoreComments):
     def __init__(self,
         *,
         submission_id36: str,
         comment_id36: str,
         child_id36s: Sequence[str],
         sort: str,
@@ -78,7 +80,9 @@
         return self.client.p.comment_tree.low.more_children(
             self.submission_id36,
             self.child_id36s,
             sort=self.sort,
             depth=depth,
             exact=exact,
         )
+
+BreadthMoreComments = LoadMoreComments
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/my_account.py` & `redditwarp-1.1.0/redditwarp/models/my_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,22 @@
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         super().__init__(d)
         self.id36: str = d['id']
         ("""
             User ID of the current user account as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
         ("""
             User ID of the current user account.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['name']
         ("""
             Username of the current user account.
             """)
         self.created_ut: int = int(d['created_utc'])
         ("""
             Unix timestamp of when the current user account was created.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/report.py` & `redditwarp-1.1.0/redditwarp/models/report.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission.py` & `redditwarp-1.1.0/redditwarp/models/submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,26 +101,30 @@
                     """)
 
         def __init__(self, d: Mapping[str, Any]) -> None:
             self.name: str = d['author']
             ("")
             self.id36: str = d['author_fullname'].split('_', 1)[-1]
             ("")
-            self.id: int = int(self.id36, 36)
+            self.idn: int = int(self.id36, 36)
+            ("")
+            self.id: int = self.idn
             ("")
             self.has_premium: bool = d['author_premium']
             ("")
             self.flair: Submission.Author.AuthorFlair = self.AuthorFlair(d)
             ("")
 
     class Subreddit:
         def __init__(self, d: Mapping[str, Any]) -> None:
             self.id36: str = d['subreddit_id'].split('_', 1)[-1]
             ("")
-            self.id: int = int(self.id36, 36)
+            self.idn: int = int(self.id36, 36)
+            ("")
+            self.id: int = self.idn
             ("")
             self.name: str = d['subreddit']
             ("")
             self.openness: str = d['subreddit_type']
             ("""
                 Either: `public`, `private`, `restricted`, `archived`,
                 `employees_only`, `gold_only`, `gold_restricted`, or `user`.
@@ -267,15 +271,17 @@
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         super().__init__(d)
         self.id36: str = d['id']
         ("""
             The ID of the submission as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         self.created_ut: int = int(d['created_utc'])
         ("""
             Unix timestamp of when the submission was made.
             """)
         self.created_at: datetime = datetime.fromtimestamp(self.created_ut, timezone.utc)
         ("""
@@ -522,27 +528,41 @@
         now banned and the submission is no longer accessible.
         """
         return self.__original
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         super().__init__(d)
         self.original_id36: str = d['crosspost_parent'][3:]
-        ("")
-        self.original_id: int = int(self.original_id36, 36)
-        ("")
+        ("""
+            The ID36 of the original submission.
+            """)
+        self.original_idn: int = int(self.original_id36, 36)
+        ("""
+            The ID of the original submission.
+            """)
+        self.original_id: int = self.original_idn
+        ("""
+            Same as :attr:`original_idn`.
+            """)
 
         self.__original: Optional[Submission] = None
         # https://github.com/python/mypy/issues/4177
         if self.__class__.original == __class__.original:  # type: ignore[name-defined]
             from ..model_loaders.submission import load_submission  # Avoid cyclic import
-            self.__original = self._load_original(d, load_submission)
+            self.__original = self._load_original(
+                d=d,
+                load_submission=load_submission,
+            )
 
     _TSubmission = TypeVar('_TSubmission', bound=Submission)
 
     @final
     def _load_original(self,
+        *,
         d: Mapping[str, Any],
-        load: Callable[[Mapping[str, Any]], _TSubmission],
+        load_submission: Callable[[Mapping[str, Any]], _TSubmission],
     ) -> Optional[_TSubmission]:
         if crosspost_parent_list := d['crosspost_parent_list']:
-            return load(crosspost_parent_list[0])
+            return load_submission(crosspost_parent_list[0])
         return None
+
+CrossPost = CrosspostSubmission
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_ASYNC.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,9 +85,14 @@
     @property
     def original(self) -> Optional[Submission]:
         return self.__original
 
     def __init__(self, d: Mapping[str, Any], client: Client) -> None:
         super().__init__(d, client)
         from ..model_loaders.submission_ASYNC import load_submission  # Avoid cyclic import
-        load = lambda d: load_submission(d, client)
-        self.__original: Optional[Submission] = self._load_original(d, load)
+        my_load_submission = lambda d: load_submission(d=d, client=client)
+        self.__original: Optional[Submission] = self._load_original(
+            d=d,
+            load_submission=my_load_submission,
+        )
+
+CrossPost = CrosspostSubmission
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_SYNC.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,9 +85,14 @@
     @property
     def original(self) -> Optional[Submission]:
         return self.__original
 
     def __init__(self, d: Mapping[str, Any], client: Client) -> None:
         super().__init__(d, client)
         from ..model_loaders.submission_SYNC import load_submission  # Avoid cyclic import
-        load = lambda d: load_submission(d, client)
-        self.__original: Optional[Submission] = self._load_original(d, load)
+        my_load_submission = lambda d: load_submission(d=d, client=client)
+        self.__original: Optional[Submission] = self._load_original(
+            d=d,
+            load_submission=my_load_submission,
+        )
+
+CrossPost = CrosspostSubmission
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_collection.py` & `redditwarp-1.1.0/redditwarp/models/submission_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,31 @@
         self.uuid: str = d['collection_id']
         ("")
 
         full_id36: str = d['subreddit_id']
         _, _, id36 = full_id36.partition('_')
         self.subreddit_id36: str = id36
         ("")
-        self.subreddit_id: int = int(id36, 36)
+        self.subreddit_idn: int = int(id36, 36)
         ("")
+        self.subreddit_id: int = self.subreddit_idn
+        ("""
+            Same as :attr:`subreddit_idn`.
+            """)
 
         full_id36 = d['author_id']
         _, _, id36 = full_id36.partition('_')
         self.author_id36: str = id36
         ("")
-        self.author_id: int = int(id36, 36)
+        self.author_idn: int = int(id36, 36)
         ("")
+        self.author_id: int = self.author_idn
+        ("""
+            Same as :attr:`author_idn`.
+            """)
 
         self.author_display_name: str = d['author_name']
         ("")
         self.title: str = d['title']
         ("")
         self.description: str = d['description']
         ("")
@@ -61,18 +69,22 @@
             self.layout = self.display_layout
 
         submission_full_id36s: Sequence[str] = d['link_ids']
         self.submission_id36s: Sequence[str] = [s[3:] for s in submission_full_id36s]
         ("""
             List of submission ID36s contained in the collection.
             """)
-        self.submission_ids: Sequence[int] = [int(s, 36) for s in self.submission_id36s]
+        self.submission_idns: Sequence[int] = [int(s, 36) for s in self.submission_id36s]
         ("""
             List of submission IDs contained in the collection.
             """)
+        self.submission_ids: Sequence[int] = self.submission_idns
+        ("""
+            Same as :attr:`self.submission_idns`.
+            """)
 
 class SubmissionCollection(SubmissionCollectionInfo, Sequence[Submission]):
     @property
     def submissions(self) -> Sequence[Submission]:
         """List of submission objects contained in the collection."""
         return self.__submissions
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_collection_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_collection_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_collection_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_collection_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_draft.py` & `redditwarp-1.1.0/redditwarp/models/submission_draft.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_draft_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_draft_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/submission_draft_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/submission_draft_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/subreddit.py` & `redditwarp-1.1.0/redditwarp/models/subreddit.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,18 +149,22 @@
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("""
             The ID of the subreddit as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
         ("""
             The subreddit ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['display_name']
         ("""
             The name of the subreddit.
             """)
         self.openness: str = d['subreddit_type']
         ("""
             Either: `public`, `private`, `restricted`, `archived`,
@@ -258,15 +262,17 @@
 
 class InaccessibleSubreddit(DatamementoPropertiesMixin):
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("")
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         self.created_ut: int = int(d['created_utc'])
         ("")
         self.created_at: datetime = datetime.fromtimestamp(self.created_ut, timezone.utc)
         ("")
 
         self.name: str = d['display_name']
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/subreddit_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/subreddit_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/subreddit_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/subreddit_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/subreddit_rules.py` & `redditwarp-1.1.0/redditwarp/models/subreddit_rules.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/subreddit_user.py` & `redditwarp-1.1.0/redditwarp/models/subreddit_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,22 @@
         ("")
         full_id36: str = d['id']
         _, _, id36 = full_id36.partition('_')
         self.id36: str = id36
         ("""
             User ID as a base 36 number.
             """)
-        self.id: int = int(id36, 36)
+        self.idn: int = int(id36, 36)
         ("""
             User ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['username']
         ("""
             Username.
             """)
         self.account_icon: str = d['accountIcon']
         ("""
             URL of the user account's icon.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/trophy.py` & `redditwarp-1.1.0/redditwarp/models/trophy.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/user.py` & `redditwarp-1.1.0/redditwarp/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,22 @@
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("""
             User ID as a base 36 number.
             """)
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
         ("""
             User ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['name']
         ("""
             Username.
             """)
         self.created_ut: int = int(d['created_utc'])
         ("""
             Unix timestamp of when the user account was created.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/user_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/user_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/user_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/user_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/user_relationship.py` & `redditwarp-1.1.0/redditwarp/models/user_relationship.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,22 @@
         ("")
         full_id36: str = d['id']
         _, _, id36 = full_id36.partition('_')
         self.id36: str = id36
         ("""
             User ID as a base 36 number.
             """)
-        self.id: int = int(id36, 36)
+        self.idn: int = int(id36, 36)
         ("""
             User ID.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['name']
         ("""
             Username.
             """)
         #self.rel_id: str = d['rel_id']
         self.added_ut: int = int(d['date'])
         ("""
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/user_summary.py` & `redditwarp-1.1.0/redditwarp/models/user_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,22 @@
     def __init__(self, d: Mapping[str, Any], id36: str) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = id36
         ("""
             ID of the user account as a base 36 number.
             """)
-        self.id: int = int(id36, 36)
+        self.idn: int = int(id36, 36)
         ("""
             ID of the user account.
             """)
+        self.id: int = self.idn
+        ("""
+            Same as :attr:`idn`.
+            """)
         self.name: str = d['name']
         ("""
             Name of the user.
             """)
         self.created_ut: int = int(d['created_utc'])
         ("""
             Unix timestamp of when the user account was created.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/widget/ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/widget/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/widget/SYNC.py` & `redditwarp-1.1.0/redditwarp/models/widget/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/widget/button.py` & `redditwarp-1.1.0/redditwarp/models/widget/button.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/widget/widget_list_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/widget/widget_list_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/widget/widget_list_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/widget/widget_list_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/wiki.py` & `redditwarp-1.1.0/redditwarp/models/wiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
             ("")
 
     def __init__(self, d: Mapping[str, Any]) -> None:
         self.d: Mapping[str, Any] = d
         ("")
         self.id36: str = d['id']
         ("")
-        self.id: int = int(self.id36, 36)
+        self.idn: int = int(self.id36, 36)
+        ("")
+        self.id: int = self.idn
         ("")
         self.name: str = d['name']
         ("")
         self.created_ut: int = int(d['created_utc'])
         ("")
         self.created_at: datetime = datetime.fromtimestamp(self.created_ut, timezone.utc)
         ("")
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/wiki_ASYNC.py` & `redditwarp-1.1.0/redditwarp/models/wiki_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/models/wiki_SYNC.py` & `redditwarp-1.1.0/redditwarp/models/wiki_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/async_paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/async_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginator_chaining_async_iterator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginator_chaining_async_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginator_chaining_iterator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginator_chaining_iterator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/account_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/account_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/account_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/account_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/flair_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/flair_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/flair_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/flair_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/front_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/front_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/front_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/front_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/listing_async_paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/listing_async_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/listing_paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/listing_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/sort_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/sort_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/sort_SYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/sort_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_SYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/subreddit_detail_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/time_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/time_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/mixins/time_SYNC.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/mixins/time_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_async_paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_async_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_paginator.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/listing/submission_and_comment_listing_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/message_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/message_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/message_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/message_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/legacy_pull_users_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/legacy_pull_users_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/legacy_pull_users_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/legacy_pull_users_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/note_pulls_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/note_pulls_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/note_pulls_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/note_pulls_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_actions_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_actions_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_actions_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_actions_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_users_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_users_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/pull_users_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/pull_users_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/moderation/sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/moderation/sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/modmail_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/modmail_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/modmail_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/modmail_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/submission_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/submission_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/submission_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/submission_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/subreddit_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/subreddit_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/subreddit_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/subreddit_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/explore_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/explore_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/explore_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/explore_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/pull_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/pull_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/user/sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/user/sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/wiki_async1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/wiki_async1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pagination/paginators/wiki_sync1.py` & `redditwarp-1.1.0/redditwarp/pagination/paginators/wiki_sync1.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/client_SYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/core/http_client_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/core/http_client_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/core/http_client_SYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/core/http_client_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/core/rate_limited_ASYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/core/rate_limited_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/core/rate_limited_SYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/core/rate_limited_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/paginators/document_async_paginator.py` & `redditwarp-1.1.0/redditwarp/pushshift/paginators/document_async_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/paginators/document_paginator.py` & `redditwarp-1.1.0/redditwarp/pushshift/paginators/document_paginator.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/siteprocs/ASYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/siteprocs/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/pushshift/siteprocs/SYNC.py` & `redditwarp-1.1.0/redditwarp/pushshift/siteprocs/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/ASYNC.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,8 +69,9 @@
         ("")
         self.subreddit_style_old: SubredditStyleOldProcedures = SubredditStyleOldProcedures(client)
         ("")
         self.subreddit_style_new: SubredditStyleNewProcedures = SubredditStyleNewProcedures(client)
         ("")
 
     async def ping(self) -> None:
+        """Make a request to the server having no effect."""
         await self._client.request('GET', '/api/v1/scopes', params={'scopes': 'read'})
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/SYNC.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,8 +69,9 @@
         ("")
         self.subreddit_style_old: SubredditStyleOldProcedures = SubredditStyleOldProcedures(client)
         ("")
         self.subreddit_style_new: SubredditStyleNewProcedures = SubredditStyleNewProcedures(client)
         ("")
 
     def ping(self) -> None:
+        """Make a request to the server having no effect."""
         self._client.request('GET', '/api/v1/scopes', params={'scopes': 'read'})
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/account/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/account/ASYNC.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Mapping, Any
+from typing import TYPE_CHECKING, Optional, Sequence, Mapping, Any, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.my_account_ASYNC import MyAccount
     from ...models.user_relationship import UserRelationship, FriendRelationship
     from ...models.trophy import Trophy
     from ...models.karma_breakdown_entry import KarmaBreakdownEntry
     from ...types import JSON_ro
@@ -250,20 +250,20 @@
             raise
         if isinstance(root, str):
             raise exceptions.OperationException('no user context')
 
         entries = root['data']['children']
         return [load_user_relationship(d) for d in entries]
 
-    async def block_user_by_id(self, idn: int) -> None:
+    async def block_user_by_id(self, idy: Union[int, str]) -> None:
         """Block a user by ID.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `int | str` idy:
             The ID of the user to block.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -272,15 +272,16 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                - The username or user ID given doesn't exist.
                - You tried to block yourself.
         """
-        await self._client.request('POST', '/api/block_user', data={'account_id': to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        await self._client.request('POST', '/api/block_user', data={'account_id': id36})
 
     async def block_user_by_name(self, name: str) -> None:
         """Block a user by name.
 
         .. .PARAMETERS
 
         :param `str` name:
@@ -292,22 +293,22 @@
         .. .RAISES
 
         :(raises):
             (Same as in :meth:`.block_user_by_id`.)
         """
         await self._client.request('POST', '/api/block_user', data={'name': name})
 
-    async def unblock_user_by_target_id(self, target_id: int, agent_id: int) -> None:
+    async def unblock_user_by_target_id(self, target_id: Union[int, str], agent_id: Union[int, str]) -> None:
         """Unblock a user by ID.
 
         .. .PARAMETERS
 
-        :param `int` target_id:
+        :param `int | str` target_id:
             The user ID in which to unblock.
-        :param `int` agent_id:
+        :param `int | str` agent_id:
             Your user account's ID.
 
             The endpoint needs this information for some dumb reason.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -317,47 +318,50 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 The target username or target user ID doesn't exist.
         """
+        target_id36 = x if isinstance((x := target_id), str) else to_base36(x)
+        agent_id36 = x if isinstance((x := agent_id), str) else to_base36(x)
         data = {
             'type': 'enemy',
-            'container': 't2_' + to_base36(agent_id),
-            'id': 't2_' + to_base36(target_id),
+            'container': 't2_' + agent_id36,
+            'id': 't2_' + target_id36,
         }
         await self._client.request('POST', '/api/unfriend', data=data)
 
-    async def unblock_user_by_target_name(self, target_name: str, agent_id: int) -> None:
+    async def unblock_user_by_target_name(self, target_name: str, agent_id: Union[int, str]) -> None:
         """Unblock a user by name.
 
         Behaves similarly to :meth:`.unblock_user_by_target_id`.
 
         .. .PARAMETERS
 
         :param `str` target_name:
             The username in which to unblock.
-        :param `int` agent_id:
+        :param `int | str` agent_id:
             Your user account's ID.
 
             The endpoint needs this information for some dumb reason.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :(raises):
             See :meth:`.unblock_user_by_target_id`.
         """
+        agent_id36 = x if isinstance((x := agent_id), str) else to_base36(x)
         data = {
             'type': 'enemy',
-            'container': 't2_' + to_base36(agent_id),
+            'container': 't2_' + agent_id36,
             'name': target_name,
         }
         await self._client.request('POST', '/api/unfriend', data=data)
 
     async def list_trusted_users(self) -> Sequence[UserRelationship]:
         """Get a list of trusted users.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/account/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/account/SYNC.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Mapping, Any
+from typing import TYPE_CHECKING, Optional, Sequence, Mapping, Any, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.my_account_SYNC import MyAccount
     from ...models.user_relationship import UserRelationship, FriendRelationship
     from ...models.trophy import Trophy
     from ...models.karma_breakdown_entry import KarmaBreakdownEntry
     from ...types import JSON_ro
@@ -249,20 +249,20 @@
             raise
         if isinstance(root, str):
             raise exceptions.OperationException('no user context')
 
         entries = root['data']['children']
         return [load_user_relationship(d) for d in entries]
 
-    def block_user_by_id(self, idn: int) -> None:
+    def block_user_by_id(self, idy: Union[int, str]) -> None:
         """Block a user by ID.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `int | str` idy:
             The ID of the user to block.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -271,15 +271,16 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                - The username or user ID given doesn't exist.
                - You tried to block yourself.
         """
-        self._client.request('POST', '/api/block_user', data={'account_id': to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/block_user', data={'account_id': id36})
 
     def block_user_by_name(self, name: str) -> None:
         """Block a user by name.
 
         .. .PARAMETERS
 
         :param `str` name:
@@ -291,22 +292,22 @@
         .. .RAISES
 
         :(raises):
             (Same as in :meth:`.block_user_by_id`.)
         """
         self._client.request('POST', '/api/block_user', data={'name': name})
 
-    def unblock_user_by_target_id(self, target_id: int, agent_id: int) -> None:
+    def unblock_user_by_target_id(self, target_id: Union[int, str], agent_id: Union[int, str]) -> None:
         """Unblock a user by ID.
 
         .. .PARAMETERS
 
-        :param `int` target_id:
+        :param `int | str` target_id:
             The user ID in which to unblock.
-        :param `int` agent_id:
+        :param `int | str` agent_id:
             Your user account's ID.
 
             The endpoint needs this information for some dumb reason.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -316,47 +317,50 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 The target username or target user ID doesn't exist.
         """
+        target_id36 = x if isinstance((x := target_id), str) else to_base36(x)
+        agent_id36 = x if isinstance((x := agent_id), str) else to_base36(x)
         data = {
             'type': 'enemy',
-            'container': 't2_' + to_base36(agent_id),
-            'id': 't2_' + to_base36(target_id),
+            'container': 't2_' + agent_id36,
+            'id': 't2_' + target_id36,
         }
         self._client.request('POST', '/api/unfriend', data=data)
 
-    def unblock_user_by_target_name(self, target_name: str, agent_id: int) -> None:
+    def unblock_user_by_target_name(self, target_name: str, agent_id: Union[int, str]) -> None:
         """Unblock a user by name.
 
         Behaves similarly to :meth:`.unblock_user_by_target_id`.
 
         .. .PARAMETERS
 
         :param `str` target_name:
             The username in which to unblock.
-        :param `int` agent_id:
+        :param `int | str` agent_id:
             Your user account's ID.
 
             The endpoint needs this information for some dumb reason.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :(raises):
             See :meth:`.unblock_user_by_target_id`.
         """
+        agent_id36 = x if isinstance((x := agent_id), str) else to_base36(x)
         data = {
             'type': 'enemy',
-            'container': 't2_' + to_base36(agent_id),
+            'container': 't2_' + agent_id36,
             'name': target_name,
         }
         self._client.request('POST', '/api/unfriend', data=data)
 
     def list_trusted_users(self) -> Sequence[UserRelationship]:
         """Get a list of trusted users.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/account/pull_subreddits_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/account/pull_subreddits_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/account/pull_subreddits_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/account/pull_subreddits_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/collection/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/collection/ASYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.submission_collection_ASYNC import SubmissionCollectionInfo, SubmissionCollection
 
 from ...model_loaders.submission_collection_ASYNC import load_submission_collection_info, load_submission_collection
 from ...util.base_conversion import to_base36
 
 
 class CollectionProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     async def create(self,
-        sr_id: int,
+        sr_id: Union[int, str],
         title: str,
         description: Optional[str] = None,
         display_layout: Optional[str] = None,
     ) -> SubmissionCollection:
         """
         Create a collection.
 
         Returns the newly created collection.
 
         .. .PARAMETERS
 
-        :param `int` sr_id:
+        :param `int | str` sr_id:
             Subreddit ID.
         :param `str` title:
             A string no longer than 300 characters.
         :param `Optional[str]` description:
             A string no longer than 500 characters.
         :param `Optional[str]` display_layout:
             Either `TIMELINE` or `GALLERY`.
@@ -55,34 +55,34 @@
                - The specified `description` was longer than 500 characters.
 
             + `INVALID_OPTION`:
                 The value specified for `display_layout` is not valid.
 
                 The options are case-sensitive.
         """
-        sr_id36 = to_base36(sr_id)
+        sr_id36 = x if isinstance((x := sr_id), str) else to_base36(x)
         params = {'sr_fullname': 't5_' + sr_id36, 'title': title}
         if description is not None:
             params['description'] = description
         if display_layout is not None:
             params['display_layout'] = display_layout
         data = await self._client.request('POST', '/api/v1/collections/create_collection', params=params)
         return load_submission_collection(data, self._client)
 
-    async def add_post(self, uuid: str, subm_id: int) -> None:
+    async def add_post(self, uuid: str, subm_id: Union[int, str]) -> None:
         """
         Add a submission to a collection.
 
         Collections have a capacity of 100 posts. Attempting to add to a full
         collection will result in an `INVALID_COLLECTION_UPDATE` API error.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `int` subm_id:
+        :param `int | str` subm_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -107,26 +107,26 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The submission specified by `subm_id` does not exist.
             + `500`:
                 The value specified by `uuid` is not a valid UUID.
         """
-        id36 = to_base36(subm_id)
+        id36 = x if isinstance((x := subm_id), str) else to_base36(x)
         params = {'collection_id': uuid, 'link_fullname': 't3_' + id36}
         await self._client.request('POST', '/api/v1/collections/add_post_to_collection', params=params)
 
-    async def remove_post(self, uuid: str, subm_id: int) -> None:
+    async def remove_post(self, uuid: str, subm_id: Union[int, str]) -> None:
         """
         Remove a submission from a collection.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `int` subm_id:
+        :param `int | str` subm_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -148,15 +148,15 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                The submission specified by `subm_id` does not exist.
             + `500`:
                The value specified by `uuid` is not a valid UUID.
         """
-        id36 = to_base36(subm_id)
+        id36 = x if isinstance((x := subm_id), str) else to_base36(x)
         params = {'collection_id': uuid, 'link_fullname': 't3_' + id36}
         await self._client.request('POST', '/api/v1/collections/remove_post_in_collection', params=params)
 
     async def get_full(self, uuid: str) -> Optional[SubmissionCollection]:
         """Get a collection, including its submissions.
 
         .. .PARAMETERS
@@ -206,34 +206,34 @@
         """
         params = {'collection_id': uuid, 'include_links': '0'}
         root = await self._client.request('GET', '/api/v1/collections/collection', params=params)
         if len(root) < 3:
             return None
         return load_submission_collection_info(root, self._client)
 
-    async def get_subreddit_collections_info(self, sr_id: int) -> Sequence[SubmissionCollectionInfo]:
+    async def get_subreddit_collections_info(self, sr_id: Union[int, str]) -> Sequence[SubmissionCollectionInfo]:
         """
         Get a list of collections' details from the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` id:
+        :param `int | str` id:
             Subreddit ID.
 
         .. .RETURNS
 
         :rtype: `Sequence`\\[:class:`~.models.submission_collection_ASYNC.SubmissionCollectionInfo`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `SUBREDDIT_NOEXIST`:
                 The specified subreddit could not be found.
         """
-        id36 = to_base36(sr_id)
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
         params = {'sr_fullname': 't5_' + id36}
         root = await self._client.request('GET', '/api/v1/collections/subreddit_collections', params=params)
         return [load_submission_collection_info(d, self._client) for d in root]
 
     async def delete(self, uuid: str) -> None:
         """Delete a collection.
 
@@ -258,29 +258,29 @@
                 The specified `uuid` was over 36 characters.
             + `INVALID_COLLECTION_ID`:
                 The specified does not exist.
         """
         params = {'collection_id': uuid}
         await self._client.request('POST', '/api/v1/collections/delete_collection', params=params)
 
-    async def reorder(self, uuid: str, subm_ids: Sequence[int]) -> None:
+    async def reorder(self, uuid: str, subm_ids: Union[Sequence[int], Sequence[str]]) -> None:
         """
         Reorder posts in a collection.
 
         An API error is returned (`INVALID_COLLECTION_UPDATE`) if an ID in
         the given list is not found in the collection.
 
         If only a subset of the IDs in the collection are specified then those
         submissions will be moved to the top of the collection in the order specified.
         The rest are moved down, maintaining their order.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `Sequence[int]` subm_ids:
+        :param `Sequence[int] | Sequence[str]` subm_ids:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -292,15 +292,15 @@
                 exist in the collection.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - The specified `uuid` was empty.
                - The specified `uuid` is invalid.
                - The specified `uuid` does not exist.
         """
-        id36s = [to_base36(i) for i in subm_ids]
+        id36s = [(x if isinstance((x := i), str) else to_base36(x)) for i in subm_ids]
         full_id36s = ['t3_' + s for s in id36s]
         params = {'collection_id': uuid, 'link_ids': ','.join(full_id36s)}
         await self._client.request('POST', '/api/v1/collections/reorder_collection', params=params)
 
     async def set_title(self, uuid: str, title: str) -> None:
         """Update a collection's title.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/collection/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/collection/SYNC.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.submission_collection_SYNC import SubmissionCollectionInfo, SubmissionCollection
 
 from ...model_loaders.submission_collection_SYNC import load_submission_collection_info, load_submission_collection
 from ...util.base_conversion import to_base36
 
 
 class CollectionProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     def create(self,
-        sr_id: int,
+        sr_id: Union[int, str],
         title: str,
         description: Optional[str] = None,
         display_layout: Optional[str] = None,
     ) -> SubmissionCollection:
         """
         Create a collection.
 
         Returns the newly created collection.
 
         .. .PARAMETERS
 
-        :param `int` sr_id:
+        :param `int | str` sr_id:
             Subreddit ID.
         :param `str` title:
             A string no longer than 300 characters.
         :param `Optional[str]` description:
             A string no longer than 500 characters.
         :param `Optional[str]` display_layout:
             Either `TIMELINE` or `GALLERY`.
@@ -55,34 +55,34 @@
                - The specified `description` was longer than 500 characters.
 
             + `INVALID_OPTION`:
                 The value specified for `display_layout` is not valid.
 
                 The options are case-sensitive.
         """
-        sr_id36 = to_base36(sr_id)
+        sr_id36 = x if isinstance((x := sr_id), str) else to_base36(x)
         params = {'sr_fullname': 't5_' + sr_id36, 'title': title}
         if description is not None:
             params['description'] = description
         if display_layout is not None:
             params['display_layout'] = display_layout
         data = self._client.request('POST', '/api/v1/collections/create_collection', params=params)
         return load_submission_collection(data, self._client)
 
-    def add_post(self, uuid: str, subm_id: int) -> None:
+    def add_post(self, uuid: str, subm_id: Union[int, str]) -> None:
         """
         Add a submission to a collection.
 
         Collections have a capacity of 100 posts. Attempting to add to a full
         collection will result in an `INVALID_COLLECTION_UPDATE` API error.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `int` subm_id:
+        :param `int | str` subm_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -107,26 +107,26 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The submission specified by `subm_id` does not exist.
             + `500`:
                 The value specified by `uuid` is not a valid UUID.
         """
-        id36 = to_base36(subm_id)
+        id36 = x if isinstance((x := subm_id), str) else to_base36(x)
         params = {'collection_id': uuid, 'link_fullname': 't3_' + id36}
         self._client.request('POST', '/api/v1/collections/add_post_to_collection', params=params)
 
-    def remove_post(self, uuid: str, subm_id: int) -> None:
+    def remove_post(self, uuid: str, subm_id: Union[int, str]) -> None:
         """
         Remove a submission from a collection.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `int` subm_id:
+        :param `int | str` subm_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -148,15 +148,15 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                The submission specified by `subm_id` does not exist.
             + `500`:
                The value specified by `uuid` is not a valid UUID.
         """
-        id36 = to_base36(subm_id)
+        id36 = x if isinstance((x := subm_id), str) else to_base36(x)
         params = {'collection_id': uuid, 'link_fullname': 't3_' + id36}
         self._client.request('POST', '/api/v1/collections/remove_post_in_collection', params=params)
 
     def get_full(self, uuid: str) -> Optional[SubmissionCollection]:
         """Get a collection, including its submissions.
 
         .. .PARAMETERS
@@ -206,34 +206,34 @@
         """
         params = {'collection_id': uuid, 'include_links': '0'}
         root = self._client.request('GET', '/api/v1/collections/collection', params=params)
         if len(root) < 3:
             return None
         return load_submission_collection_info(root, self._client)
 
-    def get_subreddit_collections_info(self, sr_id: int) -> Sequence[SubmissionCollectionInfo]:
+    def get_subreddit_collections_info(self, sr_id: Union[int, str]) -> Sequence[SubmissionCollectionInfo]:
         """
         Get a list of collections' details from the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` id:
+        :param `int | str` id:
             Subreddit ID.
 
         .. .RETURNS
 
         :rtype: `Sequence`\\[:class:`~.models.submission_collection_SYNC.SubmissionCollectionInfo`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `SUBREDDIT_NOEXIST`:
                 The specified subreddit could not be found.
         """
-        id36 = to_base36(sr_id)
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
         params = {'sr_fullname': 't5_' + id36}
         root = self._client.request('GET', '/api/v1/collections/subreddit_collections', params=params)
         return [load_submission_collection_info(d, self._client) for d in root]
 
     def delete(self, uuid: str) -> None:
         """Delete a collection.
 
@@ -258,29 +258,29 @@
                 The specified `uuid` was over 36 characters.
             + `INVALID_COLLECTION_ID`:
                 The specified does not exist.
         """
         params = {'collection_id': uuid}
         self._client.request('POST', '/api/v1/collections/delete_collection', params=params)
 
-    def reorder(self, uuid: str, subm_ids: Sequence[int]) -> None:
+    def reorder(self, uuid: str, subm_ids: Union[Sequence[int], Sequence[str]]) -> None:
         """
         Reorder posts in a collection.
 
         An API error is returned (`INVALID_COLLECTION_UPDATE`) if an ID in
         the given list is not found in the collection.
 
         If only a subset of the IDs in the collection are specified then those
         submissions will be moved to the top of the collection in the order specified.
         The rest are moved down, maintaining their order.
 
         .. .PARAMETERS
 
         :param `str` uuid:
-        :param `Sequence[int]` subm_ids:
+        :param `Sequence[int] | Sequence[str]` subm_ids:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -292,15 +292,15 @@
                 exist in the collection.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - The specified `uuid` was empty.
                - The specified `uuid` is invalid.
                - The specified `uuid` does not exist.
         """
-        id36s = [to_base36(i) for i in subm_ids]
+        id36s = [(x if isinstance((x := i), str) else to_base36(x)) for i in subm_ids]
         full_id36s = ['t3_' + s for s in id36s]
         params = {'collection_id': uuid, 'link_ids': ','.join(full_id36s)}
         self._client.request('POST', '/api/v1/collections/reorder_collection', params=params)
 
     def set_title(self, uuid: str, title: str) -> None:
         """Update a collection's title.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment/ASYNC.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Union, Mapping
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Union, Mapping, TypeVar
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.comment_ASYNC import Comment
     from ...types import JSON_ro
 
 import json
 
@@ -12,24 +12,26 @@
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_chaining_async_iterator import CallChunkChainingAsyncIterator
 from ...iterators.async_call_chunk import AsyncCallChunk
 from .fetch_ASYNC import Fetch
 from .get_ASYNC import Get
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class CommentProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.fetch: Fetch = Fetch(self, client)
         ("""
             Fetch a comment.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `int | str` idy:
                 Comment ID.
 
             .. .RETURNS
 
             :rtype: :class:`~.models.comment_ASYNC.Comment`
 
             .. .RAISES
@@ -39,51 +41,53 @@
             """)
         self.get: Get = Get(client)
         ("""
             Get a comment.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `int | str` idy:
                 Comment ID.
 
             .. .RETURNS
 
             :rtype: `Optional`\\[:class:`~.models.comment_ASYNC.Comment`]
             """)
 
-    def bulk_fetch(self, ids: Iterable[int]) -> CallChunkChainingAsyncIterator[Comment]:
+    def bulk_fetch(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingAsyncIterator[Comment]:
         """Bulk fetch comments.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
             Comment IDs.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[:class:`~.models.comment_ASYNC.Comment`]
         """
-        async def mass_fetch(ids: Sequence[int]) -> Sequence[Comment]:
-            id36s = map(to_base36, ids)
+        async def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[Comment]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t1_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = await self._client.request('GET', '/api/info', params={'id': ids_str})
-            return [load_comment(i['data'], self._client) for i in root['data']['children']]
+            # https://github.com/python/mypy/issues/13408
+            return [load_comment(i['data'], self._client) for i in root['data']['children']]  # type: ignore[return-value]
 
-        return CallChunkChainingAsyncIterator(AsyncCallChunk(mass_fetch, idfs) for idfs in chunked(ids, 100))
+        return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], Sequence[Comment]](mass_fetch, idfs) for idfs in chunked(ids, 100))
 
-    async def reply(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    async def reply(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Reply to a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_ASYNC.Comment`
@@ -120,32 +124,33 @@
             + `403`:
                 The target comment does not exist.
             + `500`:
                 The target comment is from a quarantined subreddit that the
                 current user has not opted in to.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't1_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't1_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = await self._client.request('POST', '/api/comment', files=dict(g()))
         return load_comment(result, self._client)
 
-    async def edit_body(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    async def edit_body(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Edit the body text of a comment.
 
         The target entity (with the new body text) is returned.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_ASYNC.Comment`
@@ -155,105 +160,109 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `NO_THING_ID`:
                 The target comment does not exist.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't1_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't1_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = await self._client.request('POST', '/api/editusertext', files=dict(g()))
         return load_comment(result, self._client)
 
-    async def delete(self, idn: int) -> None:
+    async def delete(self, idy: Union[int, str]) -> None:
         """Delete a comment.
 
         If the target doesn't exist or isn't valid, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         await self._client.request('POST', '/api/del', data=data)
 
-    async def lock(self, idn: int) -> None:
+    async def lock(self, idy: Union[int, str]) -> None:
         """Lock a comment.
 
         Nothing happens if the target is already locked.
 
         .. hint::
 
            Locking prevents a submission/comment from receiving new comments.
            A locked submission is unable to receive any new comments.
            Locking a comment only stops direct comments, but
            existing child comments can still receive replies.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target doesn't exist or you don't have permission to lock it.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         await self._client.request('POST', '/api/lock', data=data)
 
-    async def unlock(self, idn: int) -> None:
+    async def unlock(self, idy: Union[int, str]) -> None:
         """Unlock a comment.
 
         Behaves similarly to :meth:`.lock`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises:
             Similar to :meth:`.lock`.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         await self._client.request('POST', '/api/unlock', data=data)
 
-    async def vote(self, idn: int, direction: int) -> None:
+    async def vote(self, idy: Union[int, str], direction: int) -> None:
         """Cast a vote on a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` direction:
             Either: `1` (upvote), `0` unvote, `-1` downvote.
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -262,26 +271,27 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'dir': str(direction),
         }
         await self._client.request('POST', '/api/vote', data=data)
 
-    async def save(self, idn: int, category: Optional[str] = None) -> None:
+    async def save(self, idy: Union[int, str], category: Optional[str] = None) -> None:
         """Save a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` category:
             A category/label.
 
             Requires Reddit Premium. Ignored if no Reddit Premium.
 
         .. .RETURNS
 
@@ -292,51 +302,51 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The category name specified was invalid.
         """
-        data = {
-            'id': 't1_' + to_base36(idn),
-        }
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         if category is not None:
             data['category'] = category
         await self._client.request('POST', '/api/save', data=data)
 
-    async def unsave(self, idn: int) -> None:
+    async def unsave(self, idy: Union[int, str]) -> None:
         """Save a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         await self._client.request('POST', '/api/unsave', data=data)
 
-    async def distinguish(self, idn: int) -> Comment:
+    async def distinguish(self, idy: Union[int, str]) -> Comment:
         """Distinguish a comment.
 
         .. hint::
            Distinguishing decoratates the author's name by
            giving it a different color and putting a sigil beside it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_ASYNC.Comment`
 
         .. .RAISES
@@ -346,31 +356,32 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'yes',
         }
         root = await self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    async def distinguish_and_sticky(self, idn: int) -> Comment:
+    async def distinguish_and_sticky(self, idy: Union[int, str]) -> Comment:
         """Distinguish and sticky a comment.
 
         Only one comment may be stickied at a time. Attempting to sticky a comment
         when there is already a stickied comment will override that stickied comment.
         Only top-level comments may be stickied.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_ASYNC.Comment`
 
         .. .RAISES
@@ -380,28 +391,29 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'yes',
             'sticky': '1',
         }
         root = await self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    async def undistinguish(self, idn: int) -> Comment:
+    async def undistinguish(self, idy: Union[int, str]) -> Comment:
         """Undistinguish a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_ASYNC.Comment`
 
         .. .RAISES
@@ -411,73 +423,76 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'no',
         }
         root = await self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    async def enable_reply_notifications(self, idn: int) -> None:
+    async def enable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Enable inbox reply notifications for a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'state': '1'
         }
         await self._client.request('POST', '/api/sendreplies', data=data)
 
-    async def disable_reply_notifications(self, idn: int) -> None:
+    async def disable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Disable inbox reply notifications for a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'state': '0'
         }
         await self._client.request('POST', '/api/sendreplies', data=data)
 
-    async def approve(self, idn: int) -> None:
+    async def approve(self, idy: Union[int, str]) -> None:
         """Approve a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -487,25 +502,26 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         await self._client.request('POST', '/api/approve', data=data)
 
-    async def remove(self, idn: int) -> None:
+    async def remove(self, idy: Union[int, str]) -> None:
         """Remove a comment.
 
         This is a moderator action.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -515,43 +531,45 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'spam': '0',
         }
         await self._client.request('POST', '/api/remove', data=data)
 
-    async def remove_spam(self, idn: int) -> None:
+    async def remove_spam(self, idy: Union[int, str]) -> None:
         """Remove as spam.
 
         See :meth:`.remove`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'spam': '1',
         }
         await self._client.request('POST', '/api/remove', data=data)
 
-    async def ignore_reports(self, idn: int) -> None:
+    async def ignore_reports(self, idy: Union[int, str]) -> None:
         """Ignore reports on a comment.
 
         .. hint::
            If you ignore reports, you won't receive notifications and the
            ignored thing will be absent from moderation listings.
 
         Nothing happens if the target is already ignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -560,24 +578,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        await self._client.request('POST', '/api/ignore_reports', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        await self._client.request('POST', '/api/ignore_reports', data={'id': 't1_' + id36})
 
-    async def unignore_reports(self, idn: int) -> None:
+    async def unignore_reports(self, idy: Union[int, str]) -> None:
         """Unignore reports on a comment.
 
         Nothing happens if the target is already unignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -586,22 +605,23 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        await self._client.request('POST', '/api/unignore_reports', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        await self._client.request('POST', '/api/unignore_reports', data={'id': 't1_' + id36})
 
-    async def snooze_reports(self, idn: int, reason: str) -> None:
+    async def snooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Ignore a custom report reason in a subreddit for 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
         :param `str` reason:
             The custom report reason to snooze.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -612,36 +632,38 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't1_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36, 'reason': reason}
         await self._client.request('POST', '/api/snooze_reports', data=data)
 
-    async def unsnooze_reports(self, idn: int, reason: str) -> None:
+    async def unsnooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Unsnooze a custom report.
 
         See :meth:`.snooze_reports`.
         """
-        data = {'id': 't1_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36, 'reason': reason}
         await self._client.request('POST', '/api/unsnooze_reports', data=data)
 
     async def apply_removal_reason(self,
-            idn: int,
+            idy: Union[int, str],
             reason_id: Optional[str] = None,
             note: Optional[str] = None) -> None:
         """Set a removal reason on a removed comment.
 
         If the target is not a removed comment, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
         :param `Optional[int]` reason_id:
             A removal reason ID.
         :param `Optional[str]` note:
             A note.
 
         .. .RETURNS
@@ -662,20 +684,20 @@
                 The reason ID is invalid.
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't1_' + to_base36(idn)
-        json_data = {'item_ids': [target], 'reason_id': reason_id, 'mod_note': note}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        json_data = {'item_ids': ['t1_' + id36], 'reason_id': reason_id, 'mod_note': note}
         await self._client.request('POST', '/api/v1/modactions/removal_reasons', json=json_data)
 
     async def send_removal_comment(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False,
             locked: bool = False) -> Comment:
         """Send a removal comment.
 
@@ -685,15 +707,15 @@
         (The UI does not normally let you do this.)
 
         Unlike :meth:`.apply_removal_reason`, the target you specify must be a
         removed item otherwise an `INVALID_ID` API error is produced.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             This is ultimately unused for removal comments, but a non-empty
             string must be specified or you'll get a `NO_TEXT` API error.
 
@@ -729,38 +751,38 @@
 
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't1_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'public' + ('' if exposed else '_as_subreddit'),
-            'item_id': [target],
+            'item_id': ['t1_' + id36],
             'title': title,
             'message': message,
             'lock_comment': '01'[locked],
         }
         root = await self._client.request('POST', '/api/v1/modactions/removal_comment_message', json=json_data)
         return load_comment(root, self._client)
 
     async def send_removal_message(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False) -> None:
         """Send a removal message.
 
         Behaves similarly to :meth:`.send_removal_comment`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             A non-empty string must be specified or you'll get a `NO_TEXT` API error.
 
             The UI sends the title of the selected removal reason.
@@ -777,15 +799,15 @@
 
         :returns: `None`
 
         .. .RAISES
 
         :(raises): See :meth:`.send_removal_comment`.
         """
-        target = 't1_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'private' + ('_exposed' if exposed else ''),
-            'item_id': [target],
+            'item_id': ['t1_' + id36],
             'title': title,
             'message': message,
         }
         await self._client.request('POST', '/api/v1/modactions/removal_comment_message', json=json_data)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment/SYNC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Union, Mapping
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Union, Mapping, TypeVar
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.comment_SYNC import Comment
     from ...types import JSON_ro
 
 import json
 
@@ -12,24 +12,26 @@
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
 from ...iterators.call_chunk import CallChunk
 from .fetch_SYNC import Fetch
 from .get_SYNC import Get
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class CommentProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.fetch: Fetch = Fetch(self, client)
         ("""
             Fetch a comment.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `int | str` idy:
                 Comment ID.
 
             .. .RETURNS
 
             :rtype: :class:`~.models.comment_SYNC.Comment`
 
             .. .RAISES
@@ -39,51 +41,52 @@
             """)
         self.get: Get = Get(client)
         ("""
             Get a comment.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `int | str` idy:
                 Comment ID.
 
             .. .RETURNS
 
             :rtype: `Optional`\\[:class:`~.models.comment_SYNC.Comment`]
             """)
 
-    def bulk_fetch(self, ids: Iterable[int]) -> CallChunkChainingIterator[Comment]:
+    def bulk_fetch(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingIterator[Comment]:
         """Bulk fetch comments.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
             Comment IDs.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[:class:`~.models.comment_SYNC.Comment`]
         """
-        def mass_fetch(ids: Sequence[int]) -> Sequence[Comment]:
-            id36s = map(to_base36, ids)
+        def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[Comment]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t1_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = self._client.request('GET', '/api/info', params={'id': ids_str})
             return [load_comment(i['data'], self._client) for i in root['data']['children']]
 
-        return CallChunkChainingIterator(CallChunk(mass_fetch, idfs) for idfs in chunked(ids, 100))
+        return CallChunkChainingIterator(CallChunk[Sequence[_YIntOrStr], Sequence[Comment]](mass_fetch, idfs) for idfs in chunked(ids, 100))
 
-    def reply(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    def reply(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Reply to a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_SYNC.Comment`
@@ -120,32 +123,33 @@
             + `403`:
                 The target comment does not exist.
             + `500`:
                 The target comment is from a quarantined subreddit that the
                 current user has not opted in to.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't1_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't1_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = self._client.request('POST', '/api/comment', files=dict(g()))
         return load_comment(result, self._client)
 
-    def edit_body(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    def edit_body(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Edit the body text of a comment.
 
         The target entity (with the new body text) is returned.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_SYNC.Comment`
@@ -155,105 +159,109 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `NO_THING_ID`:
                 The target comment does not exist.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't1_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't1_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = self._client.request('POST', '/api/editusertext', files=dict(g()))
         return load_comment(result, self._client)
 
-    def delete(self, idn: int) -> None:
+    def delete(self, idy: Union[int, str]) -> None:
         """Delete a comment.
 
         If the target doesn't exist or isn't valid, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         self._client.request('POST', '/api/del', data=data)
 
-    def lock(self, idn: int) -> None:
+    def lock(self, idy: Union[int, str]) -> None:
         """Lock a comment.
 
         Nothing happens if the target is already locked.
 
         .. hint::
 
            Locking prevents a submission/comment from receiving new comments.
            A locked submission is unable to receive any new comments.
            Locking a comment only stops direct comments, but
            existing child comments can still receive replies.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target doesn't exist or you don't have permission to lock it.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         self._client.request('POST', '/api/lock', data=data)
 
-    def unlock(self, idn: int) -> None:
+    def unlock(self, idy: Union[int, str]) -> None:
         """Unlock a comment.
 
         Behaves similarly to :meth:`.lock`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises:
             Similar to :meth:`.lock`.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         self._client.request('POST', '/api/unlock', data=data)
 
-    def vote(self, idn: int, direction: int) -> None:
+    def vote(self, idy: Union[int, str], direction: int) -> None:
         """Cast a vote on a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` direction:
             Either: `1` (upvote), `0` unvote, `-1` downvote.
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -262,26 +270,27 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'dir': str(direction),
         }
         self._client.request('POST', '/api/vote', data=data)
 
-    def save(self, idn: int, category: Optional[str] = None) -> None:
+    def save(self, idy: Union[int, str], category: Optional[str] = None) -> None:
         """Save a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` category:
             A category/label.
 
             Requires Reddit Premium. Ignored if no Reddit Premium.
 
         .. .RETURNS
 
@@ -292,51 +301,51 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The category name specified was invalid.
         """
-        data = {
-            'id': 't1_' + to_base36(idn),
-        }
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         if category is not None:
             data['category'] = category
         self._client.request('POST', '/api/save', data=data)
 
-    def unsave(self, idn: int) -> None:
+    def unsave(self, idy: Union[int, str]) -> None:
         """Save a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         self._client.request('POST', '/api/unsave', data=data)
 
-    def distinguish(self, idn: int) -> Comment:
+    def distinguish(self, idy: Union[int, str]) -> Comment:
         """Distinguish a comment.
 
         .. hint::
            Distinguishing decoratates the author's name by
            giving it a different color and putting a sigil beside it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_SYNC.Comment`
 
         .. .RAISES
@@ -346,31 +355,32 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'yes',
         }
         root = self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    def distinguish_and_sticky(self, idn: int) -> Comment:
+    def distinguish_and_sticky(self, idy: Union[int, str]) -> Comment:
         """Distinguish and sticky a comment.
 
         Only one comment may be stickied at a time. Attempting to sticky a comment
         when there is already a stickied comment will override that stickied comment.
         Only top-level comments may be stickied.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_SYNC.Comment`
 
         .. .RAISES
@@ -380,28 +390,29 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'yes',
             'sticky': '1',
         }
         root = self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    def undistinguish(self, idn: int) -> Comment:
+    def undistinguish(self, idy: Union[int, str]) -> Comment:
         """Undistinguish a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target comment.
         :rtype: :class:`~.models.comment_SYNC.Comment`
 
         .. .RAISES
@@ -411,73 +422,76 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'how': 'no',
         }
         root = self._client.request('POST', '/api/distinguish', data=data)
         return load_comment(root['json']['data']['things'][0]['data'], self._client)
 
-    def enable_reply_notifications(self, idn: int) -> None:
+    def enable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Enable inbox reply notifications for a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'state': '1'
         }
         self._client.request('POST', '/api/sendreplies', data=data)
 
-    def disable_reply_notifications(self, idn: int) -> None:
+    def disable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Disable inbox reply notifications for a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'state': '0'
         }
         self._client.request('POST', '/api/sendreplies', data=data)
 
-    def approve(self, idn: int) -> None:
+    def approve(self, idy: Union[int, str]) -> None:
         """Approve a comment.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -487,25 +501,26 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't1_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36}
         self._client.request('POST', '/api/approve', data=data)
 
-    def remove(self, idn: int) -> None:
+    def remove(self, idy: Union[int, str]) -> None:
         """Remove a comment.
 
         This is a moderator action.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -515,43 +530,45 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'spam': '0',
         }
         self._client.request('POST', '/api/remove', data=data)
 
-    def remove_spam(self, idn: int) -> None:
+    def remove_spam(self, idy: Union[int, str]) -> None:
         """Remove as spam.
 
         See :meth:`.remove`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't1_' + to_base36(idn),
+            'id': 't1_' + id36,
             'spam': '1',
         }
         self._client.request('POST', '/api/remove', data=data)
 
-    def ignore_reports(self, idn: int) -> None:
+    def ignore_reports(self, idy: Union[int, str]) -> None:
         """Ignore reports on a comment.
 
         .. hint::
            If you ignore reports, you won't receive notifications and the
            ignored thing will be absent from moderation listings.
 
         Nothing happens if the target is already ignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -560,24 +577,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        self._client.request('POST', '/api/ignore_reports', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/ignore_reports', data={'id': 't1_' + id36})
 
-    def unignore_reports(self, idn: int) -> None:
+    def unignore_reports(self, idy: Union[int, str]) -> None:
         """Unignore reports on a comment.
 
         Nothing happens if the target is already unignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -586,22 +604,23 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        self._client.request('POST', '/api/unignore_reports', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/unignore_reports', data={'id': 't1_' + id36})
 
-    def snooze_reports(self, idn: int, reason: str) -> None:
+    def snooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Ignore a custom report reason in a subreddit for 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
         :param `str` reason:
             The custom report reason to snooze.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -612,36 +631,38 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't1_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36, 'reason': reason}
         self._client.request('POST', '/api/snooze_reports', data=data)
 
-    def unsnooze_reports(self, idn: int, reason: str) -> None:
+    def unsnooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Unsnooze a custom report.
 
         See :meth:`.snooze_reports`.
         """
-        data = {'id': 't1_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't1_' + id36, 'reason': reason}
         self._client.request('POST', '/api/unsnooze_reports', data=data)
 
     def apply_removal_reason(self,
-            idn: int,
+            idy: Union[int, str],
             reason_id: Optional[str] = None,
             note: Optional[str] = None) -> None:
         """Set a removal reason on a removed comment.
 
         If the target is not a removed comment, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Comment ID.
         :param `Optional[int]` reason_id:
             A removal reason ID.
         :param `Optional[str]` note:
             A note.
 
         .. .RETURNS
@@ -662,20 +683,20 @@
                 The reason ID is invalid.
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't1_' + to_base36(idn)
-        json_data = {'item_ids': [target], 'reason_id': reason_id, 'mod_note': note}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        json_data = {'item_ids': ['t1_' + id36], 'reason_id': reason_id, 'mod_note': note}
         self._client.request('POST', '/api/v1/modactions/removal_reasons', json=json_data)
 
     def send_removal_comment(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False,
             locked: bool = False) -> Comment:
         """Send a removal comment.
 
@@ -685,15 +706,15 @@
         (The UI does not normally let you do this.)
 
         Unlike :meth:`.apply_removal_reason`, the target you specify must be a
         removed item otherwise an `INVALID_ID` API error is produced.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             This is ultimately unused for removal comments, but a non-empty
             string must be specified or you'll get a `NO_TEXT` API error.
 
@@ -729,38 +750,38 @@
 
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't1_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'public' + ('' if exposed else '_as_subreddit'),
-            'item_id': [target],
+            'item_id': ['t1_' + id36],
             'title': title,
             'message': message,
             'lock_comment': '01'[locked],
         }
         root = self._client.request('POST', '/api/v1/modactions/removal_comment_message', json=json_data)
         return load_comment(root, self._client)
 
     def send_removal_message(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False) -> None:
         """Send a removal message.
 
         Behaves similarly to :meth:`.send_removal_comment`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             A non-empty string must be specified or you'll get a `NO_TEXT` API error.
 
             The UI sends the title of the selected removal reason.
@@ -777,15 +798,15 @@
 
         :returns: `None`
 
         .. .RAISES
 
         :(raises): See :meth:`.send_removal_comment`.
         """
-        target = 't1_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'private' + ('_exposed' if exposed else ''),
-            'item_id': [target],
+            'item_id': ['t1_' + id36],
             'title': title,
             'message': message,
         }
         self._client.request('POST', '/api/v1/modactions/removal_comment_message', json=json_data)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/fetch_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment/fetch_ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.comment_ASYNC import Comment
     from .ASYNC import CommentProcedures
 
 from ...util.base_conversion import to_base36
 from ...util.extract_id_from_url import extract_comment_id_from_url
 from ...exceptions import NoResultException
 
 class Fetch:
     def __init__(self, outer: CommentProcedures, client: Client) -> None:
         self._outer = outer
         self._client = client
 
-    async def __call__(self, idn: int) -> Comment:
-        id36 = to_base36(idn)
+    async def __call__(self, idy: Union[int, str]) -> Comment:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return await self.by_id36(id36)
 
     async def by_id36(self, id36: str) -> Comment:
         v = await self._outer.get.by_id36(id36)
         if v is None:
             raise NoResultException('target not found')
         return v
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/fetch_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment/fetch_SYNC.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.comment_SYNC import Comment
     from .SYNC import CommentProcedures
 
 from ...util.base_conversion import to_base36
 from ...util.extract_id_from_url import extract_comment_id_from_url
 from ...exceptions import NoResultException
 
 class Fetch:
     def __init__(self, outer: CommentProcedures, client: Client) -> None:
         self._outer = outer
         self._client = client
 
-    def __call__(self, idn: int) -> Comment:
-        id36 = to_base36(idn)
+    def __call__(self, idy: Union[int, str]) -> Comment:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return self.by_id36(id36)
 
     def by_id36(self, id36: str) -> Comment:
         v = self._outer.get.by_id36(id36)
         if v is None:
             raise NoResultException('target not found')
         return v
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment/get_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment/get_SYNC.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Union
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
-    from ...models.comment_ASYNC import Comment
+    from ...client_SYNC import Client
+    from ...models.comment_SYNC import Comment
 
-from ...model_loaders.comment_ASYNC import load_comment
+from ...model_loaders.comment_SYNC import load_comment
 from ...util.base_conversion import to_base36
 from ...util.extract_id_from_url import extract_comment_id_from_url
 
 class Get:
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    async def __call__(self, idn: int) -> Optional[Comment]:
-        id36 = to_base36(idn)
-        return await self.by_id36(id36)
+    def __call__(self, idy: Union[int, str]) -> Optional[Comment]:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        return self.by_id36(id36)
 
-    async def by_id36(self, id36: str) -> Optional[Comment]:
+    def by_id36(self, id36: str) -> Optional[Comment]:
         full_id36 = 't1_' + id36
-        root = await self._client.request('GET', '/api/info', params={'id': full_id36})
+        root = self._client.request('GET', '/api/info', params={'id': full_id36})
         if children := root['data']['children']:
             return load_comment(children[0]['data'], self._client)
         return None
 
-    async def by_url(self, url: str) -> Optional[Comment]:
-        return await self(extract_comment_id_from_url(url))
+    def by_url(self, url: str) -> Optional[Comment]:
+        return self(extract_comment_id_from_url(url))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/SYNC.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, Optional
+from typing import TYPE_CHECKING, Iterable, Optional, TypeVar
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
-    from ...models.comment_tree_ASYNC import MoreCommentsTreeNode, SubmissionTreeNode
+    from ...client_SYNC import Client
+    from ...models.comment_tree_SYNC import MoreCommentsTreeNode, SubmissionTreeNode
 
 from ...util.base_conversion import to_base36
-from .low_ASYNC import Low
+from .low_SYNC import Low
+
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
 
 class CommentTreeProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.low: Low = Low(self, client)
         ("""
             Low level calls for efficiency.
             """)
 
-    async def get(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    def get(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> Optional[SubmissionTreeNode]:
         """Get the comment tree for a submission.
 
         Behaves similarly to :meth:`.fetch`.
 
         Returns `None` instead of raises on `StatusCodeException(404)` and `RejectedResultException`.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return await self.low.get(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return self.low.get(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    async def fetch(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    def fetch(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> SubmissionTreeNode:
         """Get the comment tree for a submission.
 
         .. .PARAMETERS
 
-        :param `int` submission_id:
+        :param `_YIntOrStr` submission_id:
             Submission ID.
-        :param `Optional[int]` comment_id:
+        :param `Optional[_YIntOrStr]` comment_id:
             Optional comment ID to start the tree at that comment.
         :param `str` sort:
             Either: `confidence` ('best'), `top`, `new`, `controversial`, `old`, `random`, `qa`, `live`.
 
             If not given or not a valid sort value (including empty string), the default is the
             'sort comments by' preference of the logged in user. Otherwise, if there is no user
             context the default is `confidence`.
@@ -82,15 +86,15 @@
         :param `Optional[int]` context:
             If `comment_id` is specified, the number of parent comments to include.
 
             Specify an integer from 0 to 8. Any number higher than 8 is treated the same as 8.
 
         .. .RETURNS
 
-        :rtype: :class:`~.models.comment_tree_ASYNC.SubmissionTreeNode`
+        :rtype: :class:`~.models.comment_tree_SYNC.SubmissionTreeNode`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RejectedResultException:
             When specifying a comment using the `comment_id` parameter and the returned
             comment list is empty, so the specified comment was not returned.
 
@@ -100,56 +104,60 @@
             has a reference to the comment and tried to retrieve it.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - The specified submission ID does not exist.
                - The specified comment ID does not exist or the comment belongs
                  to a submission other than the one specified.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return await self.low.fetch(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return self.low.fetch(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    async def fetch_lenient(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    def fetch_lenient(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> SubmissionTreeNode:
         """Get the comment tree for a submission.
 
         Behaves similarly to :meth:`.fetch`.
 
         This method does the same thing as :meth:`.fetch` but doesn't reject
         with a `RejectedResultException` when the specified comment ID could
         not be retrieved.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return await self.low.fetch(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return self.low.fetch(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    async def more_children(self,
-        submission_id: int,
-        child_ids: Iterable[int],
+    def more_children(self,
+        submission_id: _YIntOrStr,
+        child_ids: Iterable[_YIntOrStr],
         *,
         sort: str = '',
         depth: Optional[int] = None,
         exact: bool = False,
     ) -> MoreCommentsTreeNode:
         """Retrieve comments omitted from a comment tree.
 
@@ -159,40 +167,42 @@
         is used to retrieve the comments represented by the 'load more comments' stubs.
 
         You may only make one request at a time to this API endpoint.
         Higher concurrency will result in an error being returned.
 
         .. .PARAMETERS
 
-        :param `int` submission_id:
-        :param `Iterable[int]` child_ids:
+        :param `_YIntOrStr` submission_id:
+        :param `Iterable[_YIntOrStr]` child_ids:
             A list of comment IDs.
         :param `str` sort:
             Same as on :meth:`.fetch`.
         :param `Optional[int]` depth:
             Same as on :meth:`.fetch`.
         :param `bool` exact:
             If true, only return the children requested, and not their sub-comments.
 
             This is kind of the same as specifying `depth=1` but more-comment objects won't be present.
 
             If this is specified with the `depth` parameter, this parameter will take precedence.
 
         .. .RETURNS
 
-        :rtype: :class:`~.models.comment_tree_ASYNC.MoreCommentsTreeNode`
+        :rtype: :class:`~.models.comment_tree_SYNC.MoreCommentsTreeNode`
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The specified submission does not exist.
         """
-        submission_id36 = to_base36(submission_id)
-        child_id36s = (to_base36(x) for x in child_ids)
-        return await self.low.more_children(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        child_id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in child_ids)  # type: ignore[arg-type]
+        return self.low.more_children(
             submission_id36,
             child_id36s,
             sort=sort,
             depth=depth,
             exact=exact,
         )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/ASYNC.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, Optional
+from typing import TYPE_CHECKING, Iterable, Optional, TypeVar
 if TYPE_CHECKING:
-    from ...client_SYNC import Client
-    from ...models.comment_tree_SYNC import MoreCommentsTreeNode, SubmissionTreeNode
+    from ...client_ASYNC import Client
+    from ...models.comment_tree_ASYNC import MoreCommentsTreeNode, SubmissionTreeNode
 
 from ...util.base_conversion import to_base36
-from .low_SYNC import Low
+from .low_ASYNC import Low
+
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
 
 class CommentTreeProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.low: Low = Low(self, client)
         ("""
             Low level calls for efficiency.
             """)
 
-    def get(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    async def get(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> Optional[SubmissionTreeNode]:
         """Get the comment tree for a submission.
 
         Behaves similarly to :meth:`.fetch`.
 
         Returns `None` instead of raises on `StatusCodeException(404)` and `RejectedResultException`.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return self.low.get(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return await self.low.get(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    def fetch(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    async def fetch(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> SubmissionTreeNode:
         """Get the comment tree for a submission.
 
         .. .PARAMETERS
 
-        :param `int` submission_id:
+        :param `_YIntOrStr` submission_id:
             Submission ID.
-        :param `Optional[int]` comment_id:
+        :param `Optional[_YIntOrStr]` comment_id:
             Optional comment ID to start the tree at that comment.
         :param `str` sort:
             Either: `confidence` ('best'), `top`, `new`, `controversial`, `old`, `random`, `qa`, `live`.
 
             If not given or not a valid sort value (including empty string), the default is the
             'sort comments by' preference of the logged in user. Otherwise, if there is no user
             context the default is `confidence`.
@@ -82,15 +86,15 @@
         :param `Optional[int]` context:
             If `comment_id` is specified, the number of parent comments to include.
 
             Specify an integer from 0 to 8. Any number higher than 8 is treated the same as 8.
 
         .. .RETURNS
 
-        :rtype: :class:`~.models.comment_tree_SYNC.SubmissionTreeNode`
+        :rtype: :class:`~.models.comment_tree_ASYNC.SubmissionTreeNode`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RejectedResultException:
             When specifying a comment using the `comment_id` parameter and the returned
             comment list is empty, so the specified comment was not returned.
 
@@ -100,56 +104,60 @@
             has a reference to the comment and tried to retrieve it.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - The specified submission ID does not exist.
                - The specified comment ID does not exist or the comment belongs
                  to a submission other than the one specified.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return self.low.fetch(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return await self.low.fetch(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    def fetch_lenient(self,
-        submission_id: int,
-        comment_id: Optional[int] = None,
+    async def fetch_lenient(self,
+        submission_id: _YIntOrStr,
+        comment_id: Optional[_YIntOrStr] = None,
         *,
         sort: str = 'confidence',
         limit: Optional[int] = None,
         depth: Optional[int] = None,
         context: Optional[int] = None,
     ) -> SubmissionTreeNode:
         """Get the comment tree for a submission.
 
         Behaves similarly to :meth:`.fetch`.
 
         This method does the same thing as :meth:`.fetch` but doesn't reject
         with a `RejectedResultException` when the specified comment ID could
         not be retrieved.
         """
-        submission_id36 = to_base36(submission_id)
-        comment_id36 = None if comment_id is None else to_base36(comment_id)
-        return self.low.fetch(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        comment_id36 = None if comment_id is None else (x if isinstance((x := comment_id), str) else to_base36(x))  # type: ignore[arg-type]
+        return await self.low.fetch(
             submission_id36,
             comment_id36,
             sort=sort,
             limit=limit,
             depth=depth,
             context=context,
         )
 
-    def more_children(self,
-        submission_id: int,
-        child_ids: Iterable[int],
+    async def more_children(self,
+        submission_id: _YIntOrStr,
+        child_ids: Iterable[_YIntOrStr],
         *,
         sort: str = '',
         depth: Optional[int] = None,
         exact: bool = False,
     ) -> MoreCommentsTreeNode:
         """Retrieve comments omitted from a comment tree.
 
@@ -159,40 +167,42 @@
         is used to retrieve the comments represented by the 'load more comments' stubs.
 
         You may only make one request at a time to this API endpoint.
         Higher concurrency will result in an error being returned.
 
         .. .PARAMETERS
 
-        :param `int` submission_id:
-        :param `Iterable[int]` child_ids:
+        :param `_YIntOrStr` submission_id:
+        :param `Iterable[_YIntOrStr]` child_ids:
             A list of comment IDs.
         :param `str` sort:
             Same as on :meth:`.fetch`.
         :param `Optional[int]` depth:
             Same as on :meth:`.fetch`.
         :param `bool` exact:
             If true, only return the children requested, and not their sub-comments.
 
             This is kind of the same as specifying `depth=1` but more-comment objects won't be present.
 
             If this is specified with the `depth` parameter, this parameter will take precedence.
 
         .. .RETURNS
 
-        :rtype: :class:`~.models.comment_tree_SYNC.MoreCommentsTreeNode`
+        :rtype: :class:`~.models.comment_tree_ASYNC.MoreCommentsTreeNode`
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The specified submission does not exist.
         """
-        submission_id36 = to_base36(submission_id)
-        child_id36s = (to_base36(x) for x in child_ids)
-        return self.low.more_children(
+        # https://github.com/python/mypy/issues/4134
+        submission_id36 = x if isinstance((x := submission_id), str) else to_base36(x)  # type: ignore[arg-type]
+        # https://github.com/python/mypy/issues/4134
+        child_id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in child_ids)  # type: ignore[arg-type]
+        return await self.low.more_children(
             submission_id36,
             child_id36s,
             sort=sort,
             depth=depth,
             exact=exact,
         )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/low_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/low_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/comment_tree/low_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/comment_tree/low_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/custom_feed/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/custom_feed/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/custom_feed/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/custom_feed/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/draft/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/draft/ASYNC.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         draft_data = root['drafts'][uuid]
         return load_public_submission_draft(draft_data)
 
     async def create(self,
         *,
         body: Union[str, Mapping[str, JSON_ro]],
         public: Optional[bool] = None,
-        subreddit_id: Optional[int] = None,
+        subreddit_id: Optional[Union[int, str]] = None,
         title: Optional[str] = None,
         reply_notifications: Optional[bool] = None,
         spoiler: Optional[bool] = None,
         nsfw: Optional[bool] = None,
         oc: Optional[bool] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
@@ -81,15 +81,15 @@
         """Create a draft.
 
         .. .PARAMETERS
 
         :param body:
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
         :param `Optional[bool]` public:
-        :param `Optional[int]` subreddit_id:
+        :param `Optional[Union[int, str]]` subreddit_id:
         :param `Optional[str]` title:
         :param `Optional[bool]` reply_notifications:
         :param `Optional[bool]` spoiler:
         :param `Optional[bool]` nsfw:
         :param `Optional[bool]` oc:
         :param `Optional[str]` flair_uuid:
         :param `Optional[str]` flair_text:
@@ -110,15 +110,17 @@
                 yield ('kind', 'markdown')
                 yield ('body', body)
             else:
                 yield ('kind', 'richtext')
                 yield ('body', json.dumps(body))
 
             if public is not None: yield ('is_public_link', '01'[public])
-            if subreddit_id is not None: yield ('subreddit', 't5_' + to_base36(subreddit_id))
+            if subreddit_id is not None:
+                id36 = x if isinstance((x := subreddit_id), str) else to_base36(x)
+                yield ('subreddit', 't5_' + id36)
             if title is not None: yield ('title', title)
             if reply_notifications is not None: yield ('send_replies', '01'[reply_notifications])
             if spoiler is not None: yield ('spoiler', '01'[spoiler])
             if nsfw is not None: yield ('nsfw', '01'[nsfw])
             if oc is not None: yield ('original_content', '01'[oc])
             if flair_uuid is not None: yield ('flair_id', flair_uuid)
             if flair_text is not None: yield ('flair_text', flair_text)
@@ -127,15 +129,15 @@
         return root['json']['data']['id']
 
     async def replace(self,
         uuid: str,
         *,
         body: Union[str, Mapping[str, JSON_ro]],
         public: Optional[bool] = None,
-        subreddit_id: Optional[int] = None,
+        subreddit_id: Optional[Union[int, str]] = None,
         title: Optional[str] = None,
         reply_notifications: Optional[bool] = None,
         spoiler: Optional[bool] = None,
         nsfw: Optional[bool] = None,
         oc: Optional[bool] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
@@ -151,15 +153,17 @@
                 yield ('kind', 'markdown')
                 yield ('body', body)
             else:
                 yield ('kind', 'richtext')
                 yield ('body', json.dumps(body))
 
             if public is not None: yield ('is_public_link', '01'[public])
-            if subreddit_id is not None: yield ('subreddit', 't5_' + to_base36(subreddit_id))
+            if subreddit_id is not None:
+                id36 = x if isinstance((x := subreddit_id), str) else to_base36(x)
+                yield ('subreddit', 't5_' + id36)
             if title is not None: yield ('title', title)
             if reply_notifications is not None: yield ('send_replies', '01'[reply_notifications])
             if spoiler is not None: yield ('spoiler', '01'[spoiler])
             if nsfw is not None: yield ('nsfw', '01'[nsfw])
             if oc is not None: yield ('original_content', '01'[oc])
             if flair_uuid is not None: yield ('flair_id', flair_uuid)
             if flair_text is not None: yield ('flair_text', flair_text)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/draft/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/draft/SYNC.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         draft_data = root['drafts'][uuid]
         return load_public_submission_draft(draft_data)
 
     def create(self,
         *,
         body: Union[str, Mapping[str, JSON_ro]],
         public: Optional[bool] = None,
-        subreddit_id: Optional[int] = None,
+        subreddit_id: Optional[Union[int, str]] = None,
         title: Optional[str] = None,
         reply_notifications: Optional[bool] = None,
         spoiler: Optional[bool] = None,
         nsfw: Optional[bool] = None,
         oc: Optional[bool] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
@@ -81,15 +81,15 @@
         """Create a draft.
 
         .. .PARAMETERS
 
         :param body:
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
         :param `Optional[bool]` public:
-        :param `Optional[int]` subreddit_id:
+        :param `Optional[Union[int, str]]` subreddit_id:
         :param `Optional[str]` title:
         :param `Optional[bool]` reply_notifications:
         :param `Optional[bool]` spoiler:
         :param `Optional[bool]` nsfw:
         :param `Optional[bool]` oc:
         :param `Optional[str]` flair_uuid:
         :param `Optional[str]` flair_text:
@@ -110,15 +110,17 @@
                 yield ('kind', 'markdown')
                 yield ('body', body)
             else:
                 yield ('kind', 'richtext')
                 yield ('body', json.dumps(body))
 
             if public is not None: yield ('is_public_link', '01'[public])
-            if subreddit_id is not None: yield ('subreddit', 't5_' + to_base36(subreddit_id))
+            if subreddit_id is not None:
+                id36 = x if isinstance((x := subreddit_id), str) else to_base36(x)
+                yield ('subreddit', 't5_' + id36)
             if title is not None: yield ('title', title)
             if reply_notifications is not None: yield ('send_replies', '01'[reply_notifications])
             if spoiler is not None: yield ('spoiler', '01'[spoiler])
             if nsfw is not None: yield ('nsfw', '01'[nsfw])
             if oc is not None: yield ('original_content', '01'[oc])
             if flair_uuid is not None: yield ('flair_id', flair_uuid)
             if flair_text is not None: yield ('flair_text', flair_text)
@@ -127,15 +129,15 @@
         return root['json']['data']['id']
 
     def replace(self,
         uuid: str,
         *,
         body: Union[str, Mapping[str, JSON_ro]],
         public: Optional[bool] = None,
-        subreddit_id: Optional[int] = None,
+        subreddit_id: Optional[Union[int, str]] = None,
         title: Optional[str] = None,
         reply_notifications: Optional[bool] = None,
         spoiler: Optional[bool] = None,
         nsfw: Optional[bool] = None,
         oc: Optional[bool] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
@@ -151,15 +153,17 @@
                 yield ('kind', 'markdown')
                 yield ('body', body)
             else:
                 yield ('kind', 'richtext')
                 yield ('body', json.dumps(body))
 
             if public is not None: yield ('is_public_link', '01'[public])
-            if subreddit_id is not None: yield ('subreddit', 't5_' + to_base36(subreddit_id))
+            if subreddit_id is not None:
+                id36 = x if isinstance((x := subreddit_id), str) else to_base36(x)
+                yield ('subreddit', 't5_' + id36)
             if title is not None: yield ('title', title)
             if reply_notifications is not None: yield ('send_replies', '01'[reply_notifications])
             if spoiler is not None: yield ('spoiler', '01'[spoiler])
             if nsfw is not None: yield ('nsfw', '01'[nsfw])
             if oc is not None: yield ('original_content', '01'[oc])
             if flair_uuid is not None: yield ('flair_id', flair_uuid)
             if flair_text is not None: yield ('flair_text', flair_text)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/flair/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/flair/SYNC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Tuple
+from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Tuple, Protocol, IO, Union
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
+    from ...client_SYNC import Client
     from ...models.flair import FlairTemplate, FlairTemplateChoices, UserFlairAssociation
+    from ...models.upload_lease import UploadLease
 
 import csv
 from io import StringIO
+from functools import cached_property
+import os.path as op
 
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
-from ...iterators.call_chunk_chaining_async_iterator import CallChunkChainingAsyncIterator
-from ...iterators.async_call_chunk import AsyncCallChunk
-from ...pagination.paginator_chaining_async_iterator import ImpartedPaginatorChainingAsyncIterator
-from ...pagination.paginators.flair_async1 import UserFlairAssociationAsyncPaginator
+from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
+from ...iterators.call_chunk import CallChunk
+from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
+from ...pagination.paginators.flair_sync1 import UserFlairAssociationPaginator
 from ...model_loaders.flair import (
     load_variant2_flair_template,
     load_variant1_flair_template,
     load_flair_template_choices,
     load_user_flair_association,
 )
+from ...http.util.guess_filename_mimetype import guess_filename_mimetype
+from ...model_loaders.upload_lease import load_upload_lease
 
 class FlairProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    async def set_user_flair(self,
+    def set_user_flair(self,
         sr: str,
         user: str,
         text: Optional[str],
         css_class: Optional[str] = None,
     ) -> None:
         """Set the flair information on a user.
 
@@ -80,19 +85,19 @@
                 The specified subreddit does not exist.
         """
         def g() -> Iterable[tuple[str, str]]:
             yield ('name', user)
             if text is not None: yield ('text', text)
             if css_class is not None: yield ('css_class', css_class)
 
-        await self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
+        self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
 
-    async def set_post_flair(self,
+    def set_post_flair(self,
         sr: str,
-        subm: int,
+        subm: Union[int, str],
         text: Optional[str],
         css_class: Optional[str] = None,
     ) -> None:
         """Set the flair information on a post.
 
         Any previously set flair information will be discarded.
 
@@ -102,15 +107,15 @@
         To revoke a flair, specify null or an empty string for the `text`
         and `css_class` parameters.
 
         .. .PARAMETERS
 
         :param `str` sr:
             Subreddit name.
-        :param `int` subm:
+        :param `Union[int, str]` subm:
             Submission ID.
         :param `Optional[str]` text:
             Flair text.
 
             Specify a string no longer than 64 characters.
             If longer than 64 characters then the parameter is ignored and an empty string is used.
         :param `Optional[str]` css_class:
@@ -137,27 +142,27 @@
                - There is no user context.
                - You do not have permission to set flairs in the specified subreddit.
                - The target submission does not belong to the specified subreddit.
 
             + `404`:
                 The specified subreddit does not exist.
         """
-        full_id36 = 't3_' + to_base36(subm)
+        id36 = x if isinstance((x := subm), str) else to_base36(x)
 
         def g() -> Iterable[tuple[str, str]]:
-            yield ('link', full_id36)
+            yield ('link', 't3_' + id36)
             if text is not None: yield ('text', text)
             if css_class is not None: yield ('css_class', css_class)
 
-        await self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
+        self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
 
     def bulk_set_user_flairs(self,
         sr: str,
         items: Iterable[Tuple[str, str, str]],
-    ) -> CallChunkChainingAsyncIterator[bool]:
+    ) -> CallChunkChainingIterator[bool]:
         """Bulk set flair information for users.
 
         The second parameter is an iterable of 3-element tuples:
         `(user, text, css_class)`: the target user name, the flair text,
         and CSS class to assign.
 
         .. .PARAMETERS
@@ -167,40 +172,40 @@
             An iterable of tuples consisting of `(user, text, css_class)`.
 
         .. .RETURNS
 
         :returns:
             For each input item, a boolean appears in the output indicating whether
             the flair assignment succeeded.
-        :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[`bool`]
+        :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`bool`]
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - There is no user context.
                - You do not have permission to set flairs in the specified subreddit.
 
             + `404`:
                 The specified subreddit does not exist.
         """
-        async def mass_update_user_flairs(items: Sequence[Tuple[str, str, str]]) -> Sequence[bool]:
+        def mass_update_user_flairs(items: Sequence[Tuple[str, str, str]]) -> Sequence[bool]:
             sio = StringIO()
             csv.writer(sio).writerows(items)
             s = sio.getvalue()
-            root = await self._client.request('POST', f'/r/{sr}/api/flaircsv', files={'flair_csv': s})
+            root = self._client.request('POST', f'/r/{sr}/api/flaircsv', files={'flair_csv': s})
             return [d['ok'] for d in root]
 
         itr = map(
-            lambda xs: AsyncCallChunk(mass_update_user_flairs, xs),
+            lambda xs: CallChunk(mass_update_user_flairs, xs),
             chunked(items, 100),
         )
-        return CallChunkChainingAsyncIterator(itr)
+        return CallChunkChainingIterator(itr)
 
-    async def _create_or_update_flair_template(self,
+    def _create_or_update_flair_template(self,
         sr: str,
         flair_type: str,
         *,
         uuid: Optional[str] = None,
         text: Optional[str] = None,
         css_class: Optional[str] = None,
         bg_color: Optional[str] = None,
@@ -220,18 +225,18 @@
             ('mod_only', None if mod_only is None else '01'[mod_only]),
             ('text_editable', None if text_editable is None else '01'[text_editable]),
             ('allowable_content', allowable_content),
             ('max_emojis', str(max_emojis)),
         ):
             if v is not None:
                 d[k] = v
-        root = await self._client.request('POST', f'/r/{sr}/api/flairtemplate_v2', data=d)
+        root = self._client.request('POST', f'/r/{sr}/api/flairtemplate_v2', data=d)
         return load_variant2_flair_template(root)
 
-    async def create_user_flair_template(self,
+    def create_user_flair_template(self,
         sr: str,
         *,
         text: Optional[str] = None,
         css_class: Optional[str] = None,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
         mod_only: Optional[bool] = None,
@@ -290,28 +295,28 @@
             + `403`:
                - There is no user context.
                - You do not have permission to set flairs in the specified subreddit.
 
             + `404`:
                 The specified subreddit does not exist.
         """
-        return await self._create_or_update_flair_template(
+        return self._create_or_update_flair_template(
             sr,
             flair_type='USER_FLAIR',
             text=text,
             css_class=css_class,
             bg_color=bg_color,
             fg_color_scheme=fg_color_scheme,
             mod_only=mod_only,
             text_editable=text_editable,
             allowable_content=allowable_content,
             max_emojis=max_emojis,
         )
 
-    async def create_post_flair_template(self,
+    def create_post_flair_template(self,
         sr: str,
         *,
         text: Optional[str] = None,
         css_class: Optional[str] = None,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
         mod_only: Optional[bool] = None,
@@ -336,28 +341,28 @@
 
         :(returns): Same as :meth:`.create_user_flair_template`.
 
         .. .RAISES
 
         :(raises): Same as :meth:`.create_user_flair_template`.
         """
-        return await self._create_or_update_flair_template(
+        return self._create_or_update_flair_template(
             sr,
             flair_type='LINK_FLAIR',
             text=text,
             css_class=css_class,
             bg_color=bg_color,
             fg_color_scheme=fg_color_scheme,
             mod_only=mod_only,
             text_editable=text_editable,
             allowable_content=allowable_content,
             max_emojis=max_emojis,
         )
 
-    async def update_user_flair_template(self,
+    def update_user_flair_template(self,
         sr: str,
         uuid: str,
         *,
         text: Optional[str] = None,
         css_class: Optional[str] = None,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
@@ -374,29 +379,29 @@
 
         :(parameters):
             Similar to :meth:`.create_user_flair_template`.
 
         :param `str` uuid:
             The flair template UUID.
         """
-        return await self._create_or_update_flair_template(
+        return self._create_or_update_flair_template(
             sr,
             flair_type='USER_FLAIR',
             uuid=uuid,
             text=text,
             css_class=css_class,
             bg_color=bg_color,
             fg_color_scheme=fg_color_scheme,
             mod_only=mod_only,
             text_editable=text_editable,
             allowable_content=allowable_content,
             max_emojis=max_emojis,
         )
 
-    async def update_post_flair_template(self,
+    def update_post_flair_template(self,
         sr: str,
         uuid: str,
         *,
         text: Optional[str] = None,
         css_class: Optional[str] = None,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
@@ -405,29 +410,29 @@
         allowable_content: Optional[str] = None,
         max_emojis: Optional[int] = None,
     ) -> FlairTemplate:
         """Update a post flair template.
 
         Behaves similarly to :meth:`.update_user_flair_template`.
         """
-        return await self._create_or_update_flair_template(
+        return self._create_or_update_flair_template(
             sr,
             flair_type='LINK_FLAIR',
             uuid=uuid,
             text=text,
             css_class=css_class,
             bg_color=bg_color,
             fg_color_scheme=fg_color_scheme,
             mod_only=mod_only,
             text_editable=text_editable,
             allowable_content=allowable_content,
             max_emojis=max_emojis,
         )
 
-    async def delete_flair_template(self, sr: str, uuid: str) -> None:
+    def delete_flair_template(self, sr: str, uuid: str) -> None:
         """Delete a user or post flair template.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` uuid:
 
@@ -442,17 +447,17 @@
                - There is no user context.
                - You do not have permission.
 
             + `404`:
                - The specified subreddit does not exist.
                - The specified flair UUID does not exist.
         """
-        await self._client.request('POST', f'/r/{sr}/api/deleteflairtemplate', data={'flair_template_id': uuid})
+        self._client.request('POST', f'/r/{sr}/api/deleteflairtemplate', data={'flair_template_id': uuid})
 
-    async def delete_all_user_flair_templates(self, sr: str) -> None:
+    def delete_all_user_flair_templates(self, sr: str) -> None:
         """Delete all user flair templates in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
@@ -465,21 +470,21 @@
             + `403`:
                - There is no user context.
                - You do not have permission.
 
             + `404`:
                 The specified subreddit does not exist.
         """
-        await self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'USER_FLAIR'})
+        self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'USER_FLAIR'})
 
-    async def delete_all_post_flair_templates(self, sr: str) -> None:
+    def delete_all_post_flair_templates(self, sr: str) -> None:
         """Delete all post flair templates in a subreddit."""
-        await self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'LINK_FLAIR'})
+        self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'LINK_FLAIR'})
 
-    async def retrieve_user_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
+    def retrieve_user_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
         """Return a list of available user flair templates in a subreddit.
 
         Current user must be a moderator of the subreddit
         (otherwise a 403 HTTP error is returned).
 
         For non-mods, there is :meth:`.get_post_flair_choices`.
 
@@ -498,26 +503,26 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `302`:
                 The specified subreddit does not exist.
             + `403`:
                 You do not have permission.
         """
-        root = await self._client.request('GET', f'/r/{sr}/api/user_flair_v2')
+        root = self._client.request('GET', f'/r/{sr}/api/user_flair_v2')
         return [load_variant1_flair_template(d) for d in root]
 
-    async def retrieve_post_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
+    def retrieve_post_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
         """Return a list of available post flair templates in a subreddit.
 
         Behaves similarly to :meth:`.retrieve_user_flair_templates`.
         """
-        root = await self._client.request('GET', f'/r/{sr}/api/link_flair_v2')
+        root = self._client.request('GET', f'/r/{sr}/api/link_flair_v2')
         return [load_variant1_flair_template(d) for d in root]
 
-    async def reorder_user_flair_templates(self, sr: str, order: Sequence[str]) -> None:
+    def reorder_user_flair_templates(self, sr: str, order: Sequence[str]) -> None:
         """Reorder user flair templates.
 
         Reorders the flair templates as shown in the UI.
 
         The list must contain every flair UUID, otherwise a 400 HTTP error is returned.
 
         If you duplicate an ID the flair will have multiple references in the UI.
@@ -537,25 +542,25 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 A flair template ID is missing from the provided list.
             + `500`:
                 The specified subreddit does not exist.
         """
         params = {'subreddit': sr, 'flair_type': 'USER_FLAIR'}
-        await self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
+        self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
 
-    async def reorder_post_flair_templates(self, sr: str, order: Sequence[str]) -> None:
+    def reorder_post_flair_templates(self, sr: str, order: Sequence[str]) -> None:
         """Reorder post flair templates.
 
         Behaves similarly to :meth:`.reorder_user_flair_templates`.
         """
         params = {'subreddit': sr, 'flair_type': 'LINK_FLAIR'}
-        await self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
+        self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
 
-    async def assign_user_flair_template(self,
+    def assign_user_flair_template(self,
         sr: str,
         user: str,
         uuid: str,
         *,
         text: Optional[str] = None,
     ) -> None:
         """Assign a user flair template.
@@ -587,19 +592,19 @@
         """
         d = {
             'name': user,
             'flair_template_id': uuid,
         }
         if text is not None:
             d['text'] = text
-        await self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
 
-    async def assign_post_flair_template(self,
+    def assign_post_flair_template(self,
         sr: str,
-        subm: int,
+        subm: Union[int, str],
         uuid: str,
         *,
         text: Optional[str] = None,
     ) -> None:
         """Assign a post flair template.
 
         .. .PARAMETERS
@@ -623,24 +628,24 @@
                - The specified flair UUID does not exist.
                - You do not have permission.
 
             + `404`:
                - The specified subreddit does not exist.
                - The specified submission does not exist.
         """
-        full_id36 = 't3_' + to_base36(subm)
+        id36 = x if isinstance((x := subm), str) else to_base36(x)
         d = {
-            'link': full_id36,
+            'link': 't3_' + id36,
             'flair_template_id': uuid,
         }
         if text is not None:
             d['text'] = text
-        await self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
 
-    async def assign_user_flair(self,
+    def assign_user_flair(self,
         sr: str,
         user: str,
         text: Optional[str],
         css_class: Optional[str] = None,
         *,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
@@ -681,33 +686,33 @@
             ('text', text),
             ('css_class', css_class),
             ('background_color', bg_color),
             ('text_color', fg_color_scheme),
         ):
             if v is not None:
                 d[k] = v
-        await self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
 
-    async def assign_post_flair(self,
+    def assign_post_flair(self,
         sr: str,
-        subm: int,
+        subm: Union[int, str],
         text: Optional[str],
         css_class: Optional[str] = None,
         *,
         bg_color: Optional[str] = None,
         fg_color_scheme: Optional[str] = None,
     ) -> None:
         """Assign a custom post flair.
 
         This is a newer version of :meth:`.set_user_flair`.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `int` subm:
+        :param `Union[int, str]` subm:
         :param `Optional[str]` text:
         :param `Optional[str]` css_class:
         :param `Optional[str]` bg_color:
         :param `Optional[str]` fg_color_scheme:
 
         .. .RETURNS
 
@@ -723,27 +728,27 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                - The specified subreddit does not exist.
                - The specified submission does not exist.
         """
-        full_id36 = 't3_' + to_base36(subm)
-        d = {'link': full_id36}
+        id36 = x if isinstance((x := subm), str) else to_base36(x)
+        d = {'link': 't3_' + id36}
         for k, v in (
             ('text', text),
             ('css_class', css_class),
             ('background_color', bg_color),
             ('text_color', fg_color_scheme),
         ):
             if v is not None:
                 d[k] = v
-        await self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
 
-    async def configure_subreddit_flair_settings(self,
+    def configure_subreddit_flair_settings(self,
         sr: str,
         *,
         user_enabled: Optional[bool] = False,
         user_position: Optional[str] = '',
         user_self_assign: Optional[bool] = False,
         post_position: Optional[str] = '',
         post_self_assign: Optional[bool] = False,
@@ -810,17 +815,17 @@
             if user_self_assign is not None:
                 yield ('flair_self_assign_enabled', '01'[user_self_assign])
             if post_position is not None:
                 yield ('link_flair_position', post_position)
             if post_self_assign is not None:
                 yield ('link_flair_self_assign_enabled', '01'[post_self_assign])
 
-        await self._client.request('POST', f'/r/{sr}/api/flairconfig', data=dict(g()))
+        self._client.request('POST', f'/r/{sr}/api/flairconfig', data=dict(g()))
 
-    async def get_user_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
+    def get_user_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
         """Get user flair template choices.
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
@@ -832,26 +837,26 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `302`:
                 There is no user context.
             + `404`:
                 The specified subreddit does not exist.
         """
-        root = await self._client.request('POST', f'/r/{sr}/api/flairselector')
+        root = self._client.request('POST', f'/r/{sr}/api/flairselector')
         return load_flair_template_choices(root)
 
-    async def get_post_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
+    def get_post_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
         """Get user flair template choices.
 
         Behaves similarly to :meth:`.get_user_flair_template_choices`.
         """
-        root = await self._client.request('POST', f'/r/{sr}/api/flairselector', data={'is_newlink': '1'})
+        root = self._client.request('POST', f'/r/{sr}/api/flairselector', data={'is_newlink': '1'})
         return load_flair_template_choices(root)
 
-    async def get_user_flair_association(self, sr: str, user: str) -> Optional[UserFlairAssociation]:
+    def get_user_flair_association(self, sr: str, user: str) -> Optional[UserFlairAssociation]:
         """Get a user flair association in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -865,56 +870,56 @@
             + `302`:
                 The specified subreddit does not exist.
             + `403`:
                - There is no user context.
                - You are not a moderator of the subreddit.
         """
         params = {'name': user, 'limit': '1'}
-        root = await self._client.request('GET', f'/r/{sr}/api/flairlist', params=params)
+        root = self._client.request('GET', f'/r/{sr}/api/flairlist', params=params)
         users_data = root['users']
         if not users_data:
             return None
         user_data = users_data[0]
         if user_data['user'].lower() != user.lower():
             return None
         return load_user_flair_association(user_data)
 
     def get_user_flair_associations(self,
         sr: str,
         amount: Optional[int] = None,
-    ) -> ImpartedPaginatorChainingAsyncIterator[UserFlairAssociationAsyncPaginator, UserFlairAssociation]:
+    ) -> ImpartedPaginatorChainingIterator[UserFlairAssociationPaginator, UserFlairAssociation]:
         """Get a user flair associations in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
         .. .RETURNS
 
-        :rtype: :class:`~.pagination.paginator_chaining_async_iterator.ImpartedPaginatorChainingAsyncIterator`\\[:class:`~.pagination.paginators.flair_async1.UserFlairAssociationAsyncPaginator`, :class:`~.models.flair.UserFlairAssociation`]
+        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.flair_sync1.UserFlairAssociationPaginator`, :class:`~.models.flair.UserFlairAssociation`]
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `302`:
                 The specified subreddit does not exist.
             + `403`:
                - There is no user context.
                - You are not a moderator of the subreddit.
         """
-        p = UserFlairAssociationAsyncPaginator(self._client, f'/r/{sr}/api/flairlist')
-        return ImpartedPaginatorChainingAsyncIterator(p, amount)
+        p = UserFlairAssociationPaginator(self._client, f'/r/{sr}/api/flairlist')
+        return ImpartedPaginatorChainingIterator(p, amount)
 
-    async def show_my_flair(self, sr: str) -> None:
+    def show_my_flair(self, sr: str) -> None:
         """Show the current user's flair in the subreddit.
 
         To tell if the current user's flair is shown::
 
-           subr = await client.p.subreddit.fetch_by_name('Python')
+           subr = client.p.subreddit.fetch_by_name('Python')
            print(subr.me.flair.shown)
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
@@ -928,12 +933,180 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                 The specified subreddit does not exist.
         """
-        await self._client.request('GET', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '1'})
+        self._client.request('POST', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '1'})
 
-    async def hide_my_flair(self, sr: str) -> None:
+    def hide_my_flair(self, sr: str) -> None:
         """Hide the current user's flair in the subreddit."""
-        await self._client.request('GET', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '0'})
+        self._client.request('POST', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '0'})
+
+    class PostAppearance:
+        def __init__(self, outer: FlairProcedures) -> None:
+            self._client = outer._client
+
+        def _obtain_upload_lease_helper(self,
+            *,
+            sr: str,
+            uuid: str,
+            imagetype: str,
+            filepath: str,
+            mimetype: Optional[str] = None,
+        ) -> UploadLease:
+            if mimetype is None:
+                mimetype = guess_filename_mimetype(filepath)
+            result = self._client.request('POST', f'/api/v1/{sr}/flair_style_asset_upload_s3/{uuid}',
+                    data={'imagetype': imagetype, 'filepath': filepath, 'mimetype': mimetype})
+            return load_upload_lease(result)
+
+        def obtain_thumbnail_upload_lease(self,
+            *,
+            sr: str,
+            uuid: str,
+            filepath: str,
+            mimetype: Optional[str] = None,
+        ) -> UploadLease:
+            return self._obtain_upload_lease_helper(
+                sr=sr,
+                uuid=uuid,
+                imagetype='postPlaceholderImage',
+                filepath=filepath,
+                mimetype=mimetype,
+            )
+
+        def obtain_background_upload_lease(self,
+            *,
+            sr: str,
+            uuid: str,
+            filepath: str,
+            mimetype: Optional[str] = None,
+        ) -> UploadLease:
+            return self._obtain_upload_lease_helper(
+                sr=sr,
+                uuid=uuid,
+                imagetype='postBackgroundImage',
+                filepath=filepath,
+                mimetype=mimetype,
+            )
+
+        def deposit_file(self,
+            file: IO[bytes],
+            upload_lease: UploadLease,
+            *,
+            timeout: float = 1000,
+        ) -> None:
+            resp = self._client.http.request('POST', upload_lease.endpoint,
+                    data=upload_lease.fields, files={'file': file}, timeout=timeout)
+            resp.ensure_successful_status()
+
+        class ObtainUploadLeaseFunction(Protocol):
+            def __call__(self,
+                *,
+                sr: str,
+                uuid: str,
+                filepath: str,
+                mimetype: Optional[str] = None,
+            ) -> UploadLease: ...
+
+        def _upload_helper(self,
+            file: IO[bytes],
+            *,
+            sr: str,
+            uuid: str,
+            filepath: Optional[str] = None,
+            timeout: float = 1000,
+            obtain_upload_lease: ObtainUploadLeaseFunction,
+        ) -> UploadLease:
+            if filepath is None:
+                filepath = op.basename(getattr(file, 'name', ''))
+                if not filepath:
+                    raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
+            upload_lease = obtain_upload_lease(sr=sr, uuid=uuid, filepath=filepath)
+            self.deposit_file(file, upload_lease, timeout=timeout)
+            return upload_lease
+
+        def upload_thumbnail(self,
+            file: IO[bytes],
+            *,
+            sr: str,
+            uuid: str,
+            filepath: Optional[str] = None,
+            timeout: float = 1000,
+        ) -> UploadLease:
+            return self._upload_helper(file=file, sr=sr, uuid=uuid, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_thumbnail_upload_lease)
+
+        def upload_background(self,
+            file: IO[bytes],
+            *,
+            sr: str,
+            uuid: str,
+            filepath: Optional[str] = None,
+            timeout: float = 1000,
+        ) -> UploadLease:
+            return self._upload_helper(file=file, sr=sr, uuid=uuid, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_background_upload_lease)
+
+        def config(self,
+            sr: str,
+            uuid: str,
+            *,
+            title_color: Optional[str] = '',
+            background_color: Optional[str] = '',
+            thumbnail_image_url: Optional[str] = '',
+            background_image_url: Optional[str] = '',
+        ) -> None:
+            """Configure a post flair's post appearance settings.
+
+            All parameters should be specified. If a parameter is not specified or is
+            an invalid value, its default will be used.
+
+            .. .PARAMETERS
+
+            :param `Optional[str]` title_color:
+                A hex color.
+
+                The default value will be used if an empty string or any other invalid value is specified.
+
+                Default: `#222222`.
+            :param `Optional[str]` background_color:
+                A hex color.
+
+                The default value will be used if an empty string or any other invalid value is specified.
+
+                Default: `#FFFFFF`.
+            :param `Optional[str]` thumbnail_image_url:
+                The URL location of a thumbnail image.
+
+                Specify an empty string to remove the image.
+            :param `Optional[str]` background_image_url:
+                The URL location of a background image.
+
+                Specify an empty string to remove the image.
+
+            .. .RETURNS
+
+            :rtype: `None`
+
+            .. .RAISES
+
+            :raises redditwarp.exceptions.RedditError:
+                + `USER_REQUIRED`:
+                    There is no user context.
+            """
+            def g() -> Iterable[tuple[str, str]]:
+                if title_color is not None: yield ('postTitleColor', title_color)
+                if background_color is not None: yield ('postBackgroundColor', background_color)
+                if thumbnail_image_url is not None: yield ('postPlaceholderImage', thumbnail_image_url)
+                if background_image_url is not None: yield ('postBackgroundImage', background_image_url)
+
+            self._client.request('PUT', f'/api/v1/{sr}/flair_styles/{uuid}', data=dict(g()))
+
+    post_appearance: cached_property[PostAppearance] = cached_property(PostAppearance)
+    ("""
+        When you edit a post flair template (through the new Reddit UI), there is a toggle at
+        the bottom of the menu that says "Edit post appearance". The methods on this object
+        relate to these settings.
+
+        The important method is :meth:`~PostAppearance.config`.
+        """)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/flair/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/ASYNC.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,939 +1,930 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Tuple
+from typing import TYPE_CHECKING, Sequence, Optional, Mapping, Union
 if TYPE_CHECKING:
-    from ...client_SYNC import Client
-    from ...models.flair import FlairTemplate, FlairTemplateChoices, UserFlairAssociation
-
-import csv
-from io import StringIO
-
-from ...util.base_conversion import to_base36
-from ...iterators.chunking import chunked
-from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
-from ...iterators.call_chunk import CallChunk
-from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
-from ...pagination.paginators.flair_sync1 import UserFlairAssociationPaginator
-from ...model_loaders.flair import (
-    load_variant2_flair_template,
-    load_variant1_flair_template,
-    load_flair_template_choices,
-    load_user_flair_association,
+    from ...client_ASYNC import Client
+    from ...models.subreddit_user import (
+        Moderator,
+        ApprovedUser,
+        BannedUser,
+        MutedUser,
+    )
+    from ...models.moderation_action_log_entry import ModerationActionLogEntry
+
+from functools import cached_property
+
+from ...model_loaders.subreddit_user import (
+    load_moderator,
+    load_approved_user,
+    load_banned_user,
+    load_muted_user,
 )
+from .pull_users_ASYNC import PullUsers
+from .legacy_ASYNC import Legacy
+from .pull_ASYNC import Pull
+from .note_ASYNC import Note
+from ...util.base_conversion import to_base36
+from ...pagination.paginator_chaining_async_iterator import ImpartedPaginatorChainingAsyncIterator
+from ...pagination.paginators.moderation.async1 import ModerationActionLogAsyncPaginator
 
-class FlairProcedures:
+class ModerationProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
+        self.legacy: Legacy = Legacy(client)
+        ("""
+            Legacy procedures for retrieving subreddit users.
+            """)
+        self.pull_users: PullUsers = PullUsers(client)
+        ("""
+            Procedures for retrieving subreddit users.
+            """)
+        self.pull: Pull = Pull(client)
+        ("""
+            Procedures for pulling moderation items.
+            """)
+        self.note: Note = Note(client)
+        ("""
+            Procedures for managing mod notes.
+            """)
 
-    def set_user_flair(self,
-        sr: str,
-        user: str,
-        text: Optional[str],
-        css_class: Optional[str] = None,
-    ) -> None:
-        """Set the flair information on a user.
+    def pull_actions(self, sr: str, amount: Optional[int] = None, *,
+            action: str = '', mod: str = '',
+            ) -> ImpartedPaginatorChainingAsyncIterator[ModerationActionLogAsyncPaginator, ModerationActionLogEntry]:
+        """Retrieve recent moderation actions from the mod log.
 
-        Any previously set flair information will be discarded.
+        .. hint::
 
-        A null argument means the field will not be sent in the request.
-        The API treats this as the same as supplying an empty string.
-
-        To revoke a flair, specify null or an empty string for the `text`
-        and `css_class` parameters.
+           Moderator actions taken within a subreddit are logged to a mod log.
+           Entries in the mod log last for 3 months before they become inaccessible.
 
         .. .PARAMETERS
 
         :param `str` sr:
-            Subreddit name.
-        :param `str` user:
-            User name.
-        :param `Optional[str]` text:
-            Flair text.
-
-            Specify a string no longer than 64 characters.
-            If longer than 64 characters then the parameter is ignored and an empty string is used.
-        :param `Optional[str]` css_class:
-            Flair CSS class.
-
-            Specify a string no longer than 100 characters.
-            If longer than 100 characters then a `BAD_CSS_NAME` API error is returned.
+            The target subreddit.
+        :param `Optional[int]` amount:
+            The number of items to retrieve.
+        :param `str` action:
+            Limit log entries to only those of a specified action.
+        :param `str` mod:
+            A comma-delimited list of moderator names to restrict the results to,
+            or use the string `a` to restrict the results to actions performed by administrators.
 
         .. .RETURNS
 
-        :rtype: `None`
+        :rtype: :class:`~.pagination.paginator_chaining_async_iterator.ImpartedPaginatorChainingAsyncIterator`\\[:class:`~.pagination.paginators.moderation.async1.ModerationActionLogAsyncPaginator`, :class:`~.models.moderation_action_log_entry.ModerationActionLogEntry`]
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `BAD_FLAIR_TARGET`:
-                The specified user doesn't exist.
-            + `BAD_CSS_NAME`:
-               - The specified CSS class was longer than 100 characters.
-               - The specified CSS class contained invalid characters.
-
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-               - There is no user context.
-               - You do not have permission to set flairs in the specified subreddit.
-
             + `404`:
-                The specified subreddit does not exist.
+                You do not have permission to view the mod log of the specified subreddit.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('name', user)
-            if text is not None: yield ('text', text)
-            if css_class is not None: yield ('css_class', css_class)
+        p = ModerationActionLogAsyncPaginator(self._client, f'/r/{sr}/about/log', action=action, mod=mod)
+        return ImpartedPaginatorChainingAsyncIterator(p, amount)
 
-        self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
 
-    def set_post_flair(self,
-        sr: str,
-        subm: int,
-        text: Optional[str],
-        css_class: Optional[str] = None,
-    ) -> None:
-        """Set the flair information on a post.
+    async def get_moderator(self, sr: str, user: str) -> Optional[Moderator]:
+        """
+        Behaves similarly to :meth:`.get_approved_user`.
+        """
+        root = await self._client.request('GET', f'/api/v1/{sr}/moderators', params={'username': user})
+        order = root['moderatorIds']
+        object_map = root['moderators']
+        return load_moderator(object_map[order[0]]) if order else None
 
-        Any previously set flair information will be discarded.
+    async def get_moderator_invitation(self, sr: str, user: str) -> Optional[Moderator]:
+        """
+        Behaves similarly to :meth:`.get_approved_user`.
+        """
+        root = await self._client.request('GET', f'/api/v1/{sr}/moderators_invited', params={'username': user})
+        order = root['moderatorIds']
+        object_map = root['moderators']
+        return load_moderator(object_map[order[0]]) if order else None
 
-        A null argument means the field will not be sent in the request.
-        The API treats this as the same as supplying an empty string.
+    async def get_editable_moderator(self, sr: str, user: str) -> Optional[Moderator]:
+        """
+        Behaves similarly to :meth:`.get_approved_user`.
+        """
+        root = await self._client.request('GET', f'/api/v1/{sr}/moderators_editable', params={'username': user})
+        order = root['moderatorIds']
+        object_map = root['moderators']
+        return load_moderator(object_map[order[0]]) if order else None
 
-        To revoke a flair, specify null or an empty string for the `text`
-        and `css_class` parameters.
+    async def get_approved_user(self, sr: str, user: str) -> Optional[ApprovedUser]:
+        """Get an approved user of a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
-            Subreddit name.
-        :param `int` subm:
-            Submission ID.
-        :param `Optional[str]` text:
-            Flair text.
-
-            Specify a string no longer than 64 characters.
-            If longer than 64 characters then the parameter is ignored and an empty string is used.
-        :param `Optional[str]` css_class:
-            Flair CSS class.
-
-            Specify a string no longer than 100 characters.
-            If longer than 100 characters then a `BAD_CSS_NAME` API error is returned.
+            Name of a subreddit.
+        :param `str` user:
+            Name of a user.
 
         .. .RETURNS
 
-        :rtype: `None`
+        :rtype: `Optional`\\[:class:`~.models.subreddit_user.ApprovedUser`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
-            + `BAD_FLAIR_TARGET`:
-                The specified submission doesn't exist.
-            + `BAD_CSS_NAME`:
-               - The specified CSS class was longer than 100 characters.
-               - The specified CSS class contained invalid characters.
-
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-               - There is no user context.
-               - You do not have permission to set flairs in the specified subreddit.
-               - The target submission does not belong to the specified subreddit.
+            + `SUBREDDIT_NOEXIST`:
+                The target subreddit does not exist.
+            + `SUBREDDIT_NO_ACCESS`:
+                The subreddit cannot be accessed.
+        """
+        root = await self._client.request('GET', f'/api/v1/{sr}/contributors', params={'username': user})
+        order = root['approvedSubmitterIds']
+        object_map = root['approvedSubmitters']
+        return load_approved_user(object_map[order[0]]) if order else None
 
-            + `404`:
-                The specified subreddit does not exist.
+    async def get_banned_user(self, sr: str, user: str) -> Optional[BannedUser]:
+        """
+        Behaves similarly to :meth:`.get_approved_user`.
         """
-        full_id36 = 't3_' + to_base36(subm)
+        root = await self._client.request('GET', f'/api/v1/{sr}/banned', params={'username': user})
+        order = root['bannedUserIds']
+        object_map = root['bannedUsers']
+        return load_banned_user(object_map[order[0]]) if order else None
 
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('link', full_id36)
-            if text is not None: yield ('text', text)
-            if css_class is not None: yield ('css_class', css_class)
+    async def get_muted_user(self, sr: str, user: str) -> Optional[MutedUser]:
+        """
+        Behaves similarly to :meth:`.get_approved_user`.
+        """
+        root = await self._client.request('GET', f'/api/v1/{sr}/muted', params={'username': user})
+        order = root['mutedUserIds']
+        object_map = root['mutedUsers']
+        return load_muted_user(object_map[order[0]]) if order else None
 
-        self._client.request('POST', f'/r/{sr}/api/flair', data=dict(g()))
 
-    def bulk_set_user_flairs(self,
-        sr: str,
-        items: Iterable[Tuple[str, str, str]],
-    ) -> CallChunkChainingIterator[bool]:
-        """Bulk set flair information for users.
+    async def send_moderator_invite(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+        """Send a moderator invite.
 
-        The second parameter is an iterable of 3-element tuples:
-        `(user, text, css_class)`: the target user name, the flair text,
-        and CSS class to assign.
+        If the user is already invited, nothing happens. The permissions won't change.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `Iterable[tuple[str, str, str]]` items:
-            An iterable of tuples consisting of `(user, text, css_class)`.
+        :param `str` user:
+        :param `Sequence[str]` permissions:
+            Values: `all`, `access`, `chat_config`, `chat_operator`, `config`,
+            `flair`, `mail`, `posts`, `wiki`.
+
+            Pass an empty sequence for no permissions.
 
         .. .RETURNS
 
-        :returns:
-            For each input item, a boolean appears in the output indicating whether
-            the flair assignment succeeded.
-        :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`bool`]
+        :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
+            + `INVALID_PERMISSIONS`:
+                An invalid permission was provided.
+            + `ALREADY_MODERATOR`:
+                The user is already a moderator.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-               - There is no user context.
-               - You do not have permission to set flairs in the specified subreddit.
+               - You don't have permission.
+               - The target subreddit specified was empty.
 
             + `404`:
                 The specified subreddit does not exist.
         """
-        def mass_update_user_flairs(items: Sequence[Tuple[str, str, str]]) -> Sequence[bool]:
-            sio = StringIO()
-            csv.writer(sio).writerows(items)
-            s = sio.getvalue()
-            root = self._client.request('POST', f'/r/{sr}/api/flaircsv', files={'flair_csv': s})
-            return [d['ok'] for d in root]
-
-        itr = map(
-            lambda xs: CallChunk(mass_update_user_flairs, xs),
-            chunked(items, 100),
-        )
-        return CallChunkChainingIterator(itr)
-
-    def _create_or_update_flair_template(self,
-        sr: str,
-        flair_type: str,
-        *,
-        uuid: Optional[str] = None,
-        text: Optional[str] = None,
-        css_class: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-        mod_only: Optional[bool] = None,
-        text_editable: Optional[bool] = None,
-        allowable_content: Optional[str] = None,
-        max_emojis: Optional[int] = None,
-    ) -> FlairTemplate:
-        d = {'flair_type': flair_type}
-        for k, v in (
-            ('flair_template_id', uuid),
-            ('text', text),
-            ('css_class', css_class),
-            ('background_color', bg_color),
-            ('text_color', fg_color_scheme),
-            ('mod_only', None if mod_only is None else '01'[mod_only]),
-            ('text_editable', None if text_editable is None else '01'[text_editable]),
-            ('allowable_content', allowable_content),
-            ('max_emojis', str(max_emojis)),
-        ):
-            if v is not None:
-                d[k] = v
-        root = self._client.request('POST', f'/r/{sr}/api/flairtemplate_v2', data=d)
-        return load_variant2_flair_template(root)
-
-    def create_user_flair_template(self,
-        sr: str,
-        *,
-        text: Optional[str] = None,
-        css_class: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-        mod_only: Optional[bool] = None,
-        text_editable: Optional[bool] = None,
-        allowable_content: Optional[str] = None,
-        max_emojis: Optional[int] = None,
-    ) -> FlairTemplate:
-        """Create a user flair template.
-
-        Any previously set flair information will be discarded.
-
-        A null argument means the field will not be sent in the request.
-        The API treats this as the same as supplying an empty string.
-
-        .. .PARAMETERS
-
-        :param `str` sr:
-        :param `Optional[str]` text:
-        :param `Optional[str]` css_class:
-        :param `Optional[str]` bg_color:
-            A 6-digit rgb hex color with an optional hash at the start. E.g. `#fb8559`.
-
-            For user flair templates, the background color can be unset, making it transparent.
-            (Post flairs cannot be transparent.)
-
-            Effective default: empty string. It will be transparent.
-        :param `Optional[str]` fg_color_scheme:
-            Either `dark` or `light`.
-
-            Effective default: `dark`.
-        :param `Optional[bool]` mod_only:
-            Whether flair is only available for mods to select.
-
-            Effective default: false.
-        :param `Optional[bool]` text_editable:
-            Whether users will be able to edit their flair text.
-
-            Effective default: false.
-        :param `Optional[str]` allowable_content:
-            Either: `all`, `emoji`, `text`.
-
-            Effective default: `all`.
-        :param `Optional[int]` max_emojis:
-            An integer from 1 to 10.
+        data = {
+            'type': 'moderator_invite',
+            'r': sr,
+            'name': user,
+            'permissions': ','.join('+' + p for p in permissions),
+        }
+        await self._client.request('POST', '/api/friend', data=data)
 
-            Effective default: `10`.
+    async def accept_moderator_invite(self, sr: str) -> None:
+        """Accept a moderator invite.
+
+        .. .PARAMETERS
+
+        :param `str` sr:
 
         .. .RETURNS
 
-        :returns: The newly created flair template.
-        :rtype: :class:`~.models.flair.FlairTemplate`
+        :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_INVITE_FOUND`:
+                You don't have a pendning invitation for the specified subreddit.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-               - There is no user context.
-               - You do not have permission to set flairs in the specified subreddit.
-
-            + `404`:
-                The specified subreddit does not exist.
+                The subreddit specified was empty.
         """
-        return self._create_or_update_flair_template(
-            sr,
-            flair_type='USER_FLAIR',
-            text=text,
-            css_class=css_class,
-            bg_color=bg_color,
-            fg_color_scheme=fg_color_scheme,
-            mod_only=mod_only,
-            text_editable=text_editable,
-            allowable_content=allowable_content,
-            max_emojis=max_emojis,
-        )
-
-    def create_post_flair_template(self,
-        sr: str,
-        *,
-        text: Optional[str] = None,
-        css_class: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-        mod_only: Optional[bool] = None,
-        text_editable: Optional[bool] = None,
-        allowable_content: Optional[str] = None,
-        max_emojis: Optional[int] = None,
-    ) -> FlairTemplate:
-        """Create a post flair template.
-
-        Behaves similarly to :meth:`.create_user_flair_template`.
-
-        .. .PARAMETERS
-
-        :(parameters):
-            Same as :meth:`.create_user_flair_template`,
-            but `bg_color` effective default is different.
-
-        :param `Optional[str]` bg_color:
-            Effective default: `#d3d6da`.
-
-        .. .RETURNS
-
-        :(returns): Same as :meth:`.create_user_flair_template`.
-
-        .. .RAISES
-
-        :(raises): Same as :meth:`.create_user_flair_template`.
-        """
-        return self._create_or_update_flair_template(
-            sr,
-            flair_type='LINK_FLAIR',
-            text=text,
-            css_class=css_class,
-            bg_color=bg_color,
-            fg_color_scheme=fg_color_scheme,
-            mod_only=mod_only,
-            text_editable=text_editable,
-            allowable_content=allowable_content,
-            max_emojis=max_emojis,
-        )
-
-    def update_user_flair_template(self,
-        sr: str,
-        uuid: str,
-        *,
-        text: Optional[str] = None,
-        css_class: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-        mod_only: Optional[bool] = None,
-        text_editable: Optional[bool] = None,
-        allowable_content: Optional[str] = None,
-        max_emojis: Optional[int] = None,
-    ) -> FlairTemplate:
-        """Update a user flair template.
-
-        Behaves similarly to :meth:`.create_user_flair_template`.
-
-        .. .PARAMETERS
-
-        :(parameters):
-            Similar to :meth:`.create_user_flair_template`.
-
-        :param `str` uuid:
-            The flair template UUID.
-        """
-        return self._create_or_update_flair_template(
-            sr,
-            flair_type='USER_FLAIR',
-            uuid=uuid,
-            text=text,
-            css_class=css_class,
-            bg_color=bg_color,
-            fg_color_scheme=fg_color_scheme,
-            mod_only=mod_only,
-            text_editable=text_editable,
-            allowable_content=allowable_content,
-            max_emojis=max_emojis,
-        )
-
-    def update_post_flair_template(self,
-        sr: str,
-        uuid: str,
-        *,
-        text: Optional[str] = None,
-        css_class: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-        mod_only: Optional[bool] = None,
-        text_editable: Optional[bool] = None,
-        allowable_content: Optional[str] = None,
-        max_emojis: Optional[int] = None,
-    ) -> FlairTemplate:
-        """Update a post flair template.
-
-        Behaves similarly to :meth:`.update_user_flair_template`.
-        """
-        return self._create_or_update_flair_template(
-            sr,
-            flair_type='LINK_FLAIR',
-            uuid=uuid,
-            text=text,
-            css_class=css_class,
-            bg_color=bg_color,
-            fg_color_scheme=fg_color_scheme,
-            mod_only=mod_only,
-            text_editable=text_editable,
-            allowable_content=allowable_content,
-            max_emojis=max_emojis,
-        )
+        await self._client.request('POST', '/api/accept_moderator_invite', data={'r': sr})
 
-    def delete_flair_template(self, sr: str, uuid: str) -> None:
-        """Delete a user or post flair template.
+    async def revoke_moderator_invite(self, sr: str, user: str) -> None:
+        """Revoke a moderator invite.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `str` uuid:
+        :param `str` user:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
+            + `400`:
+                The `user` parameter was empty or the user doesn't exist.
             + `403`:
-               - There is no user context.
-               - You do not have permission.
-
-            + `404`:
-               - The specified subreddit does not exist.
-               - The specified flair UUID does not exist.
+               - You don't have permission.
+               - The target subreddit specified was empty.
         """
-        self._client.request('POST', f'/r/{sr}/api/deleteflairtemplate', data={'flair_template_id': uuid})
+        data = {
+            'type': 'moderator_invite',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
+
+    async def remove_moderator(self, sr: str, user: str) -> None:
+        """Remove a moderator.
 
-    def delete_all_user_flair_templates(self, sr: str) -> None:
-        """Delete all user flair templates in a subreddit.
+        Nothing happens if the specified user is not a moderator of the subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
+        :param `str` user:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
+            + `400`:
+                The `user` parameter was empty or the user doesn't exist.
             + `403`:
-               - There is no user context.
-               - You do not have permission.
-
-            + `404`:
-                The specified subreddit does not exist.
+               - You don't have permission.
+               - The target subreddit specified was empty.
         """
-        self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'USER_FLAIR'})
+        data = {
+            'type': 'moderator',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
+
+    async def leave_moderator(self, sr_id: Union[int, str]) -> None:
+        """Abdicate moderator status in a subreddit.
 
-    def delete_all_post_flair_templates(self, sr: str) -> None:
-        """Delete all post flair templates in a subreddit."""
-        self._client.request('POST', f'/r/{sr}/api/clearflairtemplates', data={'flair_type': 'LINK_FLAIR'})
+        .. warning::
 
-    def retrieve_user_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
-        """Return a list of available user flair templates in a subreddit.
+            This action cannot be undone.
 
-        Current user must be a moderator of the subreddit
-        (otherwise a 403 HTTP error is returned).
+        Be careful with this endpoint. It's possible for a subreddit to not have any moderators.
 
-        For non-mods, there is :meth:`.get_post_flair_choices`.
+        Nothing happens if the specified subreddit ID is not valid or the
+        current user is not a moderator of the subreddit.
 
         .. .PARAMETERS
 
-        :param `str` sr:
+        :param `Union[int, str]` sr_id:
 
         .. .RETURNS
 
-        :rtype: `Sequence`\\[:class:`~.models.flair.FlairTemplate`]
+        :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `302`:
-                The specified subreddit does not exist.
-            + `403`:
-                You do not have permission.
         """
-        root = self._client.request('GET', f'/r/{sr}/api/user_flair_v2')
-        return [load_variant1_flair_template(d) for d in root]
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
+        await self._client.request('POST', '/api/leavemoderator', data={'id': 't5_' + id36})
 
-    def retrieve_post_flair_templates(self, sr: str) -> Sequence[FlairTemplate]:
-        """Return a list of available post flair templates in a subreddit.
+    async def set_moderator_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+        """Set the permissions of a moderator.
 
-        Behaves similarly to :meth:`.retrieve_user_flair_templates`.
-        """
-        root = self._client.request('GET', f'/r/{sr}/api/link_flair_v2')
-        return [load_variant1_flair_template(d) for d in root]
+        Be careful with this endpoint. It's possible for a subreddit to not have any moderators.
 
-    def reorder_user_flair_templates(self, sr: str, order: Sequence[str]) -> None:
-        """Reorder user flair templates.
-
-        Reorders the flair templates as shown in the UI.
-
-        The list must contain every flair UUID, otherwise a 400 HTTP error is returned.
-
-        If you duplicate an ID the flair will have multiple references in the UI.
+        Nothing happens if the current user is not a moderator of the subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `Sequence[str]` order:
-            A list of all flair UUIDs.
+        :param `str` user:
+        :param `Sequence[str]` permissions:
+            Values: `all`, `access`, `chat_config`, `chat_operator`, `config`,
+            `flair`, `mail`, `posts`, `wiki`.
+
+            Pass an empty sequence for no permissions.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
+            + `INVALID_PERMISSION_TYPE`:
+                The user specified by `user` isn't a moderator of the subreddit.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-                A flair template ID is missing from the provided list.
-            + `500`:
+                You don't have permission.
+            + `404`:
                 The specified subreddit does not exist.
         """
-        params = {'subreddit': sr, 'flair_type': 'USER_FLAIR'}
-        self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
-
-    def reorder_post_flair_templates(self, sr: str, order: Sequence[str]) -> None:
-        """Reorder post flair templates.
-
-        Behaves similarly to :meth:`.reorder_user_flair_templates`.
-        """
-        params = {'subreddit': sr, 'flair_type': 'LINK_FLAIR'}
-        self._client.request('PATCH', '/api/flair_template_order', params=params, json=order)
+        data = {
+            'type': 'moderator',
+            'r': sr,
+            'name': user,
+            'permissions': ','.join('+' + p for p in permissions) if permissions else '-access',
+        }
+        await self._client.request('POST', '/api/setpermissions', data=data)
 
-    def assign_user_flair_template(self,
-        sr: str,
-        user: str,
-        uuid: str,
-        *,
-        text: Optional[str] = None,
-    ) -> None:
-        """Assign a user flair template.
+    async def set_moderator_invite_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+        """Set the permissions on a moderator invite.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
-        :param `str` uuid:
-        :param `Optional[str]` text:
-            Custom text to override the template's text.
+        :param `Sequence[str]` permissions:
+            Values: `all`, `access`, `chat_config`, `chat_operator`, `config`,
+            `flair`, `mail`, `posts`, `wiki`.
 
-            Supply `None` or empty string to use the template's text.
+            Pass an empty sequence for no permissions.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
+            + `INVALID_PERMISSION_TYPE`:
+                The user specified by `user` doesn't have a moderator invite to the subreddit.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-               - The specified flair UUID does not exist.
-               - You do not have permission.
-
+                You don't have permission.
             + `404`:
-               - The specified subreddit does not exist.
-               - The specified user does not exist.
+                The specified subreddit does not exist.
         """
-        d = {
+        data = {
+            'type': 'moderator_invite',
+            'r': sr,
             'name': user,
-            'flair_template_id': uuid,
+            'permissions': ','.join('+' + p for p in permissions) if permissions else '-access',
         }
-        if text is not None:
-            d['text'] = text
-        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        await self._client.request('POST', '/api/setpermissions', data=data)
 
-    def assign_post_flair_template(self,
-        sr: str,
-        subm: int,
-        uuid: str,
-        *,
-        text: Optional[str] = None,
-    ) -> None:
-        """Assign a post flair template.
+    async def add_approved_user(self, sr: str, user: str) -> None:
+        """Add an approved user to a subreddit.
+
+        If the user is already an approved user, nothing happens.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
-        :param `str` uuid:
-        :param `Optional[str]` text:
-            Custom text to override the template's text.
-
-            Supply `None` or empty string to use the template's text.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-               - The specified flair UUID does not exist.
-               - You do not have permission.
+               - You don't have permission.
+               - The target subreddit specified was empty.
 
             + `404`:
-               - The specified subreddit does not exist.
-               - The specified submission does not exist.
+                The specified subreddit does not exist.
         """
-        full_id36 = 't3_' + to_base36(subm)
-        d = {
-            'link': full_id36,
-            'flair_template_id': uuid,
+        data = {
+            'type': 'contributor',
+            'r': sr,
+            'name': user,
         }
-        if text is not None:
-            d['text'] = text
-        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        await self._client.request('POST', '/api/friend', data=data)
 
-    def assign_user_flair(self,
-        sr: str,
-        user: str,
-        text: Optional[str],
-        css_class: Optional[str] = None,
-        *,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-    ) -> None:
-        """Assign a custom user flair.
+    async def remove_approved_user(self, sr: str, user: str) -> None:
+        """Remove an approved user of a subreddit.
 
-        This is a newer version of :meth:`.set_user_flair`.
+        If the user is already not an approved user, nothing happens.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
-        :param `Optional[str]` text:
-        :param `Optional[str]` css_class:
-        :param `Optional[str]` bg_color:
-        :param `Optional[str]` fg_color_scheme:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
-            + `BAD_CSS_NAME`:
-               - The specified CSS class was longer than 100 characters.
-               - The specified CSS class contained invalid characters.
-
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
+            + `400`:
+                The `user` parameter was empty or the user doesn't exist.
             + `403`:
-                You do not have permission.
+               - You don't have permission.
+               - The target subreddit specified was empty.
+
             + `404`:
-               - The specified subreddit does not exist.
-               - The specified user does not exist.
+                The specified subreddit does not exist.
         """
-        d = {'name': user}
-        for k, v in (
-            ('text', text),
-            ('css_class', css_class),
-            ('background_color', bg_color),
-            ('text_color', fg_color_scheme),
-        ):
-            if v is not None:
-                d[k] = v
-        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
+        data = {
+            'type': 'contributor',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
 
-    def assign_post_flair(self,
-        sr: str,
-        subm: int,
-        text: Optional[str],
-        css_class: Optional[str] = None,
-        *,
-        bg_color: Optional[str] = None,
-        fg_color_scheme: Optional[str] = None,
-    ) -> None:
-        """Assign a custom post flair.
+    async def leave_approved_user(self, sr_id: Union[int, str]) -> None:
+        """Abdicate approved user status in a subreddit.
 
-        This is a newer version of :meth:`.set_user_flair`.
+        Nothing happens if the specified subreddit ID is not valid or the
+        current user is not an approved user of the subreddit.
+
+        .. .PARAMETERS
+
+        :param `Union[int, str]` sr_id:
+
+        .. .RETURNS
+
+        :rtype: `None`
+
+        .. .RAISES
+
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_REQUIRED`:
+                There is no user context.
+        """
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
+        await self._client.request('POST', '/api/leavecontributor', data={'id': 't5_' + id36})
+
+    async def ban_user(self, sr: str, user: str, *,
+            duration: Optional[int] = None,
+            reason: str = '',
+            note: str = '',
+            message: str = '') -> None:
+        """Ban a user from a subreddit.
+
+        Banning an already banned user does nothing. However, when banning an already
+        banned user (as to change the ban reason or note), if the duration is changed
+        then a new direct message will be issued to the user informing them of the
+        duration change.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `int` subm:
-        :param `Optional[str]` text:
-        :param `Optional[str]` css_class:
-        :param `Optional[str]` bg_color:
-        :param `Optional[str]` fg_color_scheme:
+        :param `str` user:
+        :param `Optional[int]` duration:
+            Number of days they should be banned for, in the range of 1 to 999.
+
+            To change the duration of a ban, re-issue this procedure with a new duration.
+            A direct message is sent to the user informing them of the ban duration change.
+        :param `str` reason:
+            Ban reason. No longer than 100 characters.
+        :param `str` note:
+            A moderator note. No longer than 300 characters.
+        :param `str` message:
+            The message to include in the DM that is sent to the user.
+
+            Specify markdown text.
+
+            Note that a direct message is always sent to the banned user when a ban is issued.
+            The ban message shows in the DM under a section called "Note from the moderators:".
+
+            If empty string, no message or section "Note from the moderators:" is shown.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
-            + `BAD_CSS_NAME`:
-               - The specified CSS class was longer than 100 characters.
-               - The specified CSS class contained invalid characters.
+            + `USER_REQUIRED`:
+                There is no user context.
+            + `NO_USER`:
+                The `user` parameter was empty, or contains invalid characters.
+            + `USER_DOESNT_EXIST`:
+                The user specified by `user` does not exist.
+            + `BAD_NUMBER`:
+                When `type: banned` or `type: wikibanned`,
+                the number specified by `duration` is not within the range 1 to 999.
+            + `TOO_LONG`:
+               - The value specified by `reason` is over 100 characters.
+               - The value specified by `note` is over 300 characters.
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-                You do not have permission.
+               - You don't have permission.
+               - The target subreddit specified was empty.
+
             + `404`:
-               - The specified subreddit does not exist.
-               - The specified submission does not exist.
+                The specified subreddit does not exist.
         """
-        full_id36 = 't3_' + to_base36(subm)
-        d = {'link': full_id36}
-        for k, v in (
-            ('text', text),
-            ('css_class', css_class),
-            ('background_color', bg_color),
-            ('text_color', fg_color_scheme),
-        ):
-            if v is not None:
-                d[k] = v
-        self._client.request('POST', f'/r/{sr}/api/selectflair', data=d)
-
-    def configure_subreddit_flair_settings(self,
-        sr: str,
-        *,
-        user_enabled: Optional[bool] = False,
-        user_position: Optional[str] = '',
-        user_self_assign: Optional[bool] = False,
-        post_position: Optional[str] = '',
-        post_self_assign: Optional[bool] = False,
-    ) -> None:
-        """Configure subreddit flair settings.
-
-        All parameters should be specified. If a parameter is not specified or is
-        an invalid value, its default will be used.
+        data = {
+            'type': 'banned',
+            'r': sr,
+            'name': user,
+            'ban_reason': reason,
+            'ban_message': message,
+            'note': note,
+        }
+        if duration is not None:
+            data['duration'] = str(duration)
 
-        User flairs are disabled when either `user_enabled` is false
-        or `user_position` is an empty string.
+        await self._client.request('POST', '/api/friend', data=data)
 
-        Post flairs are disabled when `post_position` is an empty string.
+    async def unban_user(self, sr: str, user: str) -> None:
+        """Unban a user from a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
-        :param `Optional[bool]` user_enabled:
-            Whether user flairs are enabled in the subreddit.
+        :param `str` user:
 
-            Effective default: false.
-        :param `Optional[str]` user_position:
-            Either `left`, `right`, or empty string.
+        .. .RETURNS
 
-            An empty string value will disable user flairs even if
-            `user_enabled` is true.
+        :rtype: `None`
 
-            Effective default: empty string.
-        :param `Optional[bool]` user_self_assign:
-            Whether users are allowed to assign their own user flairs.
+        .. .RAISES
 
-            Value is forced false if `user_enabled` is false
-            (but not if `user_position` is an empty string).
+        :(raises): Same as :meth:`~.remove_approved_user`.
+        """
+        data = {
+            'type': 'banned',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
 
-            Effective default: false.
-        :param `Optional[str]` post_position:
-            Either `left`, `right`, or empty string.
+    async def mute_user(self, sr: str, user: str, *, note: str = '') -> None:
+        """Mute a user in a subreddit.
 
-            Effective default: empty string.
-        :param `Optional[bool]` post_self_assign:
-            Whether users are allowed to assign their own post flairs.
+        Muting an already muted user does nothing.
 
-            Value is forced false if `post_position` is an empty string.
+        .. .PARAMETERS
 
-            Effective default: false.
+        :param `str` sr:
+        :param `str` user:
+        :param `str` note:
+            A moderator note. No longer than 300 characters.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            In addition to :meth:`~.add_approved_user`:
+
+            + `TOO_LONG`:
+                The value specified by `note` is over 300 characters.
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-                You do not have permission.
-            + `404`:
-                The specified subreddit does not exist.
+            Same as :meth:`~.add_approved_user`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            if user_enabled is not None:
-                yield ('flair_enabled', '01'[user_enabled])
-            if user_position is not None:
-                yield ('flair_position', user_position)
-            if user_self_assign is not None:
-                yield ('flair_self_assign_enabled', '01'[user_self_assign])
-            if post_position is not None:
-                yield ('link_flair_position', post_position)
-            if post_self_assign is not None:
-                yield ('link_flair_self_assign_enabled', '01'[post_self_assign])
-
-        self._client.request('POST', f'/r/{sr}/api/flairconfig', data=dict(g()))
+        data = {
+            'type': 'muted',
+            'r': sr,
+            'name': user,
+            'note': note,
+        }
+        await self._client.request('POST', '/api/friend', data=data)
 
-    def get_user_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
-        """Get user flair template choices.
+    async def unmute_user(self, sr: str, user: str) -> None:
+        """Unmute a user in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
+        :param `str` user:
 
         .. .RETURNS
 
-        :returns: :class:`~.models.flair.FlairTemplateChoices`, a `Sequence`\\[:class:`~.models.flair.FlairTemplateChoice`]
-        :rtype: :class:`~.models.flair.FlairTemplateChoices`
+        :rtype: `None`
 
         .. .RAISES
 
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `302`:
-                There is no user context.
-            + `404`:
-                The specified subreddit does not exist.
+        :(raises): Same as :meth:`~.remove_approved_user`.
         """
-        root = self._client.request('POST', f'/r/{sr}/api/flairselector')
-        return load_flair_template_choices(root)
+        data = {
+            'type': 'muted',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
+
+    async def add_wiki_contributor(self, sr: str, user: str) -> None:
+        """Add a wiki contributor in a subreddit.
+
+        Adding a user who is already a wiki contributor does nothing.
+
+        .. .PARAMETERS
 
-    def get_post_flair_template_choices(self, sr: str) -> FlairTemplateChoices:
-        """Get user flair template choices.
+        :param `str` sr:
+        :param `str` user:
+
+        .. .RETURNS
+
+        :rtype: `None`
+
+        .. .RAISES
 
-        Behaves similarly to :meth:`.get_user_flair_template_choices`.
+        :(raises): Same as :meth:`~.add_approved_user`.
         """
-        root = self._client.request('POST', f'/r/{sr}/api/flairselector', data={'is_newlink': '1'})
-        return load_flair_template_choices(root)
+        data = {
+            'type': 'wikicontributor',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/friend', data=data)
 
-    def get_user_flair_association(self, sr: str, user: str) -> Optional[UserFlairAssociation]:
-        """Get a user flair association in a subreddit.
+    async def remove_wiki_contributor(self, sr: str, user: str) -> None:
+        """Remove a wiki contributor in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
         .. .RETURNS
 
-        :rtype: `Optional`\\[:class:`~.models.flair.UserFlairAssociation`]
+        :rtype: `None`
 
         .. .RAISES
 
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `302`:
-                The specified subreddit does not exist.
-            + `403`:
-               - There is no user context.
-               - You are not a moderator of the subreddit.
+        :(raises): Same as :meth:`~.remove_approved_user`.
         """
-        params = {'name': user, 'limit': '1'}
-        root = self._client.request('GET', f'/r/{sr}/api/flairlist', params=params)
-        users_data = root['users']
-        if not users_data:
-            return None
-        user_data = users_data[0]
-        if user_data['user'].lower() != user.lower():
-            return None
-        return load_user_flair_association(user_data)
+        data = {
+            'type': 'wikicontributor',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
+
+    async def ban_wiki_contributor(self, sr: str, user: str, *,
+            duration: Optional[int] = None,
+            reason: str = '',
+            note: str = '') -> None:
+        """Ban a wiki contributor in a subreddit.
 
-    def get_user_flair_associations(self,
-        sr: str,
-        amount: Optional[int] = None,
-    ) -> ImpartedPaginatorChainingIterator[UserFlairAssociationPaginator, UserFlairAssociation]:
-        """Get a user flair associations in a subreddit.
+        Adding a user who is already a wiki contributor does nothing.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
+        :param `Optional[int]` duration:
+            Number of days they should be banned for, in the range of 1 to 999.
+        :param `str` reason:
+            Ban reason. No longer than 100 characters.
+        :param `str` note:
+            A moderator note. No longer than 300 characters.
 
         .. .RETURNS
 
-        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.flair_sync1.UserFlairAssociationPaginator`, :class:`~.models.flair.UserFlairAssociation`]
+        :rtype: `None`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            In addition to :meth:`~.add_approved_user`:
+
+            + `TOO_LONG`:
+               - The value specified by `reason` is over 100 characters.
+               - The value specified by `note` is over 300 characters.
+
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `302`:
-                The specified subreddit does not exist.
-            + `403`:
-               - There is no user context.
-               - You are not a moderator of the subreddit.
+            Same as :meth:`~.add_approved_user`.
         """
-        p = UserFlairAssociationPaginator(self._client, f'/r/{sr}/api/flairlist')
-        return ImpartedPaginatorChainingIterator(p, amount)
-
-    def show_my_flair(self, sr: str) -> None:
-        """Show the current user's flair in the subreddit.
+        data = {
+            'type': 'banned',
+            'r': sr,
+            'name': user,
+            'ban_reason': reason,
+            'note': note,
+        }
+        if duration is not None:
+            data['duration'] = str(duration)
 
-        To tell if the current user's flair is shown::
+        await self._client.request('POST', '/api/friend', data=data)
 
-           subr = client.p.subreddit.fetch_by_name('Python')
-           print(subr.me.flair.shown)
+    async def unban_wiki_contributor(self, sr: str, user: str) -> None:
+        """Unban a wiki contributor in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
+        :param `str` user:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-                You do not have permission.
-            + `404`:
-                The specified subreddit does not exist.
+        :(raises): Same as :meth:`~.remove_approved_user`.
         """
-        self._client.request('POST', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '1'})
+        data = {
+            'type': 'wikibanned',
+            'r': sr,
+            'name': user,
+        }
+        await self._client.request('POST', '/api/unfriend', data=data)
+
+
+    class RemovalReason:
+        def __init__(self, outer: ModerationProcedures) -> None:
+            self._outer = outer
+            self._client = outer._client
+
+        async def create(self, sr: str, title: str, message: str) -> str:
+            """Create a removal reason.
+
+            .. .PARAMETERS
+
+            :param `str` sr:
+            :param `str` title:
+                A title for this removal reason.
+            :param `str` message:
+                The removal reason message.
+
+            .. .RETURNS
+
+            :returns: The newly created removal reason ID.
+            :rtype: `str`
+
+            .. .RAISES
+
+            :raises redditwarp.exceptions.RedditError:
+                + `MOD_REQUIRED`:
+                   - There is no user context.
+                   - The current user is not a moderator of the subreddit.
+
+                + `NO_TEXT`:
+                   - The `title` parameter was not specified or was empty.
+                   - The `message` parameter was not specified or was empty.
+
+                + `TOO_LONG`:
+                   - The value specified for `title` is over 50 characters.
+                   - The value specified for `message` is over 10000 characters.
+
+            :raises redditwarp.http.exceptions.StatusCodeException:
+                + `500`:
+                    The target subreddit does not exist.
+            """
+            data = {'title': title, 'message': message}
+            root = await self._client.request('POST', f'/api/v1/{sr}/removal_reasons', data=data)
+            return root['id']
+
+        async def retrieve(self, sr: str) -> Mapping[str, tuple[str, str]]:
+            """Get a list of removal reasons.
+
+            .. .PARAMETERS
+
+            :param `str` sr:
+
+            .. .RETURNS
+
+            :returns: A mapping of removal reason IDs to tuples of `(title, message)`.
+            :rtype: `Mapping`\\[`str`, `tuple`\\[`str`, `str`]]
+
+            .. .RAISES
+
+            :raises redditwarp.exceptions.RedditError:
+                + `MOD_REQUIRED`:
+                   - There is no user context.
+                   - The current user is not a moderator of the subreddit.
+
+                + `SUBREDDIT_NOEXIST`:
+                    The target subreddit does not exist.
+            """
+            root = await self._client.request('GET', f'/api/v1/{sr}/removal_reasons')
+            order = root['order']
+            object_map = root['data']
+            return {
+                y: (m['title'], m['message'])
+                for y in order for m in [object_map[y]]
+            }
+
+        async def replace(self, sr: str, idt: str, title: str, message: str) -> None:
+            """Update a removal reason's title and message.
+
+            Both parameters `title` and `message` must be specified otherwise
+            a `NO_TEXT` API error is returned.
+
+            .. .PARAMETERS
+
+            :param `str` sr:
+            :param `str` idt:
+                A removal reason ID.
+            :param `str` title:
+            :param `str` message:
+
+            .. .RETURNS
+
+            :rtype: `None`
+
+            .. .RAISES
+
+            :raises redditwarp.exceptions.RedditError:
+                + `MOD_REQUIRED`:
+                   - There is no user context.
+                   - The current user is not a moderator of the subreddit.
+
+                + `SUBREDDIT_NOEXIST`:
+                    The target subreddit does not exist.
+                + `INVALID_ID`:
+                    The specified removal reason ID was not found.
+                + `NO_TEXT`:
+                   - The `title` parameter was not specified or was empty.
+                   - The `message` parameter was not specified or was empty.
+
+                + `TOO_LONG`:
+                   - The value specified for `title` is over 50 characters.
+                   - The value specified for `message` is over 10000 characters.
+            """
+            data = {'title': title, 'message': message}
+            await self._client.request('PUT', f'/api/v1/{sr}/removal_reasons/{idt}', data=data)
+
+        async def delete(self, sr: str, idt: str) -> None:
+            """Delete a removal reason.
+
+            If the specified removal reason ID did not exist, nothing happens.
+
+            .. .PARAMETERS
+
+            :param `str` sr:
+            :param `str` idt:
+
+            .. .RETURNS
+
+            :rtype: `None`
+
+            .. .RAISES
+
+            :raises redditwarp.exceptions.RedditError:
+                + `MOD_REQUIRED`:
+                   - There is no user context.
+                   - The current user is not a moderator of the subreddit.
+
+                + `SUBREDDIT_NOEXIST`:
+                    The target subreddit does not exist.
+                + `INVALID_ID`:
+                    The specified removal reason ID was not found.
+            """
+            await self._client.request('DELETE', f'/api/v1/{sr}/removal_reasons/{idt}')
 
-    def hide_my_flair(self, sr: str) -> None:
-        """Hide the current user's flair in the subreddit."""
-        self._client.request('POST', f'/r/{sr}/api/setflairenabled', params={'flair_enabled': '0'})
+    removal_reason: cached_property[RemovalReason] = cached_property(RemovalReason)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/flair_emoji/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/flair_emoji/ASYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from typing import TYPE_CHECKING, IO, Optional
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
 
 import os.path as op
 from functools import cached_property
 
-from ...models.flair_emoji import FlairEmojiUploadLease, SubredditFlairEmojis
-from ...model_loaders.flair_emoji import load_flair_emoji_upload_lease, load_flair_emoji
+from ...models.flair_emoji import SubredditFlairEmojis
+from ...model_loaders.flair_emoji import load_flair_emoji
+from ...models.upload_lease import UploadLease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 
 class FlairEmojiProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     async def retrieve(self, sr: str) -> SubredditFlairEmojis:
@@ -77,38 +79,38 @@
                     mod_only=mod_only)
 
         async def obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> FlairEmojiUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = await self._client.request('POST', f'/api/v1/{sr}/emoji_asset_upload_s3',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_flair_emoji_upload_lease(result)
+            return load_upload_lease(result)
 
         async def deposit_file(self,
             file: IO[bytes],
-            upload_lease: FlairEmojiUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = await self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         async def upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> FlairEmojiUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = await self.obtain_upload_lease(sr=sr, filepath=filepath)
             await self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/flair_emoji/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/flair_emoji/SYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from typing import TYPE_CHECKING, IO, Optional
 if TYPE_CHECKING:
     from ...client_SYNC import Client
 
 import os.path as op
 from functools import cached_property
 
-from ...models.flair_emoji import FlairEmojiUploadLease, SubredditFlairEmojis
-from ...model_loaders.flair_emoji import load_flair_emoji_upload_lease, load_flair_emoji
+from ...models.flair_emoji import SubredditFlairEmojis
+from ...model_loaders.flair_emoji import load_flair_emoji
+from ...models.upload_lease import UploadLease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 
 class FlairEmojiProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     def retrieve(self, sr: str) -> SubredditFlairEmojis:
@@ -77,38 +79,38 @@
                     mod_only=mod_only)
 
         def obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> FlairEmojiUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = self._client.request('POST', f'/api/v1/{sr}/emoji_asset_upload_s3',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_flair_emoji_upload_lease(result)
+            return load_upload_lease(result)
 
         def deposit_file(self,
             file: IO[bytes],
-            upload_lease: FlairEmojiUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         def upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> FlairEmojiUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = self.obtain_upload_lease(sr=sr, filepath=filepath)
             self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/front/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/front/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/front/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/front/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/front/pull_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/front/pull_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/front/pull_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/front/pull_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/live_thread/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/live_thread/ASYNC.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Mapping
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Mapping, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.live_thread_ASYNC import LiveThread, LiveUpdate
 
 from ...models.live_thread import ContributorList, Contributor
 from ...model_loaders.live_thread_ASYNC import load_live_thread, load_live_update
 from ...iterators.chunking import chunked
@@ -416,40 +416,40 @@
                 You don't have an invitation for the specified live thread.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The specified live thread does not exist.
         """
         await self._client.request('POST', f'/api/live/{idt}/accept_contributor_invite')
 
-    async def revoke_contributor_invite(self, idt: str, user_id: int) -> None:
+    async def revoke_contributor_invite(self, idt: str, user_id: Union[int, str]) -> None:
         """Revoke an outstanding contributor invite.
 
         Requires the `manage` live thread permission.
 
         If attempting to remove the invite for a user that was not invited,
         the action is treated as a success.
 
         .. .PARAMETERS
 
         :param `str` idt:
-        :param `int` user_id:
+        :param `Union[int, str]` user_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - There is no user context.
                - You do not have the `manage` permission.
                - You do not have permission.
         """
-        id36 = to_base36(user_id)
+        id36 = x if isinstance((x := user_id), str) else to_base36(x)
         await self._client.request('POST', f'/api/live/{idt}/rm_contributor_invite', data={'id': 't2_' + id36})
 
     async def leave_contributor(self, idt: str) -> None:
         """Abdicate contributorship of the thread.
 
         It is possible to leave a live thread and not have any contributors to it.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/live_thread/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/live_thread/SYNC.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Mapping
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, Mapping, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.live_thread_SYNC import LiveThread, LiveUpdate
 
 from ...models.live_thread import ContributorList, Contributor
 from ...model_loaders.live_thread_SYNC import load_live_thread, load_live_update
 from ...iterators.chunking import chunked
@@ -416,40 +416,40 @@
                 You don't have an invitation for the specified live thread.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The specified live thread does not exist.
         """
         self._client.request('POST', f'/api/live/{idt}/accept_contributor_invite')
 
-    def revoke_contributor_invite(self, idt: str, user_id: int) -> None:
+    def revoke_contributor_invite(self, idt: str, user_id: Union[int, str]) -> None:
         """Revoke an outstanding contributor invite.
 
         Requires the `manage` live thread permission.
 
         If attempting to remove the invite for a user that was not invited,
         the action is treated as a success.
 
         .. .PARAMETERS
 
         :param `str` idt:
-        :param `int` user_id:
+        :param `Union[int, str]` user_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                - There is no user context.
                - You do not have the `manage` permission.
                - You do not have permission.
         """
-        id36 = to_base36(user_id)
+        id36 = x if isinstance((x := user_id), str) else to_base36(x)
         self._client.request('POST', f'/api/live/{idt}/rm_contributor_invite', data={'id': 't2_' + id36})
 
     def leave_contributor(self, idt: str) -> None:
         """Abdicate contributorship of the thread.
 
         It is possible to leave a live thread and not have any contributors to it.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/message/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/message/SYNC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Sequence, Union
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
-    from ...models.message_ASYNC import ComposedMessage
+    from ...client_SYNC import Client
+    from ...models.message_SYNC import ComposedMessage
 
 from functools import cached_property
 
 from ...util.base_conversion import to_base36
-from ...model_loaders.message_ASYNC import load_composed_message, load_composed_message_thread
-from .pulls_ASYNC import Pulls
+from ...model_loaders.message_SYNC import load_composed_message, load_composed_message_thread
+from .pulls_SYNC import Pulls
 
 class MessageProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.pulls: Pulls = Pulls(client)
         ("""
             Pull messages.
             """)
 
-    async def get_thread(self, idn: int) -> Sequence[ComposedMessage]:
+    def get_thread(self, idy: Union[int, str]) -> Sequence[ComposedMessage]:
         """Get a message thread.
 
         Specifying the ID of any message in the same thread gives you the same list.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
             Message ID.
 
         .. .RETURNS
 
-        :rtype: `Sequence`\\[:class:`~.models.message_ASYNC.ComposedMessage`]
+        :rtype: `Sequence`\\[:class:`~.models.message_SYNC.ComposedMessage`]
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target message specified does not exist or
                 you do not have permission to access it.
         """
-        id36 = to_base36(idn)
-        root = await self._client.request('GET', f'/message/messages/{id36}')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('GET', f'/message/messages/{id36}')
         obj_data = root['data']['children'][0]['data']
         return load_composed_message_thread(obj_data, self._client)
 
-    async def send(self, to: str, subject: str, body: str) -> None:
+    def send(self, to: str, subject: str, body: str) -> None:
         """Send a direct message to a user.
 
         .. .PARAMETERS
 
         :param `str` to:
             Name of user in which to send the message to.
         :param `str` subject:
@@ -81,17 +81,17 @@
                 by setting "Show private messages from" to "Only trusted users".
         """
         req_data = {
             'to': to,
             'subject': subject,
             'text': body,
         }
-        await self._client.request('POST', '/api/compose', data=req_data)
+        self._client.request('POST', '/api/compose', data=req_data)
 
-    async def send_from_sr(self, sr: str, to: str, subject: str, body: str) -> None:
+    def send_from_sr(self, sr: str, to: str, subject: str, body: str) -> None:
         """Send a direct message to a user on behalf of a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
             The name of a subreddit you moderate.
         :param `str` to:
@@ -127,175 +127,186 @@
         """
         req_data = {
             'from_sr': sr,
             'to': to,
             'subject': subject,
             'text': body,
         }
-        await self._client.request('POST', '/api/compose', data=req_data)
+        self._client.request('POST', '/api/compose', data=req_data)
 
-    async def reply(self, idn: int, body: str) -> ComposedMessage:
+    def reply(self, idy: Union[int, str], body: str) -> ComposedMessage:
         """Reply to a message
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
         :param `str` body:
 
         .. .RETURNS
 
         :returns: The newly created message.
-        :rtype: :class:`~.models.message_ASYNC.ComposedMessage`
+        :rtype: :class:`~.models.message_SYNC.ComposedMessage`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `NO_TEXT`:
                 The body text specified by `body` was empty.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The specified message ID does not exist.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'thing_id': 't4_' + to_base36(idn),
+            'thing_id': 't4_' + id36,
             'text': body,
             'return_rtjson': '1',
         }
-        result = await self._client.request('POST', '/api/comment', data=data)
+        result = self._client.request('POST', '/api/comment', data=data)
         root = result['json']['data']['things'][0]['data']
         return load_composed_message(root, self._client)
 
-    async def delete(self, idn: int) -> None:
+    def delete(self, idy: Union[int, str]) -> None:
         """Delete a message.
 
         If the message specified by the ID doesn't exist, or is invalid,
         the action is treated as a success.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        await self._client.request('POST', '/api/del_msg', data={'id': 't4_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/del_msg', data={'id': 't4_' + id36})
 
-    async def mark_read(self, idn: int) -> None:
+    def mark_read(self, idy: Union[int, str]) -> None:
         """Mark a message as read.
 
         Marking an already marked as read item is treated as a success.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 The message specified by the ID doesn't exist or is invalid.
         """
-        await self._client.request('POST', '/api/read_message', data={'id': 't4_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/read_message', data={'id': 't4_' + id36})
 
-    async def mark_unread(self, idn: int) -> None:
+    def mark_unread(self, idy: Union[int, str]) -> None:
         """Mark a message as unread.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        await self._client.request('POST', '/api/unread_message', data={'id': 't4_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/unread_message', data={'id': 't4_' + id36})
 
-    async def mark_all_read(self) -> None:
+    def mark_all_read(self) -> None:
         """Mark all messages as read.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        await self._client.request('POST', '/api/read_all_messages')
+        self._client.request('POST', '/api/read_all_messages')
 
-    async def mark_comment_read(self, idn: int) -> None:
+    def mark_comment_read(self, idy: Union[int, str]) -> None:
         """Mark a comment message as read.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        await self._client.request('POST', '/api/read_message', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/read_message', data={'id': 't1_' + id36})
 
-    async def mark_comment_unread(self, idn: int) -> None:
+    def mark_comment_unread(self, idy: Union[int, str]) -> None:
         """Mark a comment message as unread.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        await self._client.request('POST', '/api/read_message', data={'id': 't1_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/read_message', data={'id': 't1_' + id36})
 
-    async def collapse(self, idn: int) -> None:
+    def collapse(self, idy: Union[int, str]) -> None:
         """Collapse a message.
 
         If the specified message does not exist or is valid,
         the action is treated as a success.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        await self._client.request('POST', '/api/collapse_message', data={'id': 't4_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/collapse_message', data={'id': 't4_' + id36})
 
-    async def uncollapse(self, idn: int) -> None:
+    def uncollapse(self, idy: Union[int, str]) -> None:
         """Uncollapse a message.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        await self._client.request('POST', '/api/uncollapse_message', data={'id': 't4_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/uncollapse_message', data={'id': 't4_' + id36})
 
     class BlockAuthor:
         def __init__(self, outer: MessageProcedures) -> None:
             self._client = outer._client
 
-        async def __call__(self, idn: int) -> None:
-            await self.of_message(idn)
+        def __call__(self, idy: Union[int, str]) -> None:
+            self.of_message(idy)
 
-        async def of_message(self, idn: int) -> None:
-            await self._client.request('POST', '/api/block', data={'id': 't4_' + to_base36(idn)})
-
-        async def of_comment(self, idn: int) -> None:
-            await self._client.request('POST', '/api/block', data={'id': 't1_' + to_base36(idn)})
-
-        async def of_submission(self, idn: int) -> None:
-            await self._client.request('POST', '/api/block', data={'id': 't3_' + to_base36(idn)})
+        def of_message(self, idy: Union[int, str]) -> None:
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            self._client.request('POST', '/api/block', data={'id': 't4_' + id36})
+
+        def of_comment(self, idy: Union[int, str]) -> None:
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            self._client.request('POST', '/api/block', data={'id': 't1_' + id36})
+
+        def of_submission(self, idy: Union[int, str]) -> None:
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            self._client.request('POST', '/api/block', data={'id': 't3_' + id36})
 
     block_author: cached_property[BlockAuthor] = cached_property(BlockAuthor)
     ("""
         Block the author of a message, comment, or submission.
 
         - Use :meth:`~.BlockAuthor.__call__` to block the author of a message.
         - Use :meth:`~.BlockAuthor.of_comment` to block the author of a comment.
@@ -303,15 +314,15 @@
 
         To block a user directly by ID or name, see
         :meth:`~.AccountProcedures.block_user_by_id` and :meth:`~.AccountProcedures.block_user_by_name`
         instead.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idn:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/message/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/note_SYNC.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,321 +1,260 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable
 if TYPE_CHECKING:
     from ...client_SYNC import Client
-    from ...models.message_SYNC import ComposedMessage
+    from ...models.moderation_note import (
+        ModerationNote,
+        ModerationUserNote,
+    )
+
+from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
+from ...pagination.paginators.moderation.note_pulls_sync1 import (
+    ModerationNotePaginator,
+    ModerationUserNotePaginator,
+)
+from ...iterators.chunking import chunked
+from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
+from ...iterators.call_chunk import CallChunk
+from ...model_loaders.moderation_note import load_moderation_user_note
+from ... import http
 
-from functools import cached_property
-
-from ...util.base_conversion import to_base36
-from ...model_loaders.message_SYNC import load_composed_message, load_composed_message_thread
-from .pulls_SYNC import Pulls
-
-class MessageProcedures:
+class Note:
     def __init__(self, client: Client) -> None:
         self._client = client
-        self.pulls: Pulls = Pulls(client)
-        ("""
-            Pull messages.
-            """)
 
-    def get_thread(self, idn: int) -> Sequence[ComposedMessage]:
-        """Get a message thread.
-
-        Specifying the ID of any message in the same thread gives you the same list.
+    def create_user_note(self, sr: str, user: str, content: str, *,
+            label: str = '',
+            anchor_submission_id: Optional[int] = None,
+            anchor_comment_id: Optional[int] = None) -> ModerationUserNote:
+        """Create a user note.
 
         .. .PARAMETERS
 
-        :param `int` idn:
-            Message ID.
+        :param `str` sr:
+            Subreddit name.
+        :param `str` user:
+            User name.
+        :param `str` content:
+            Content of the note. Max 250 characters.
+        :param `str` label:
+            Either: `BOT_BAN`, `PERMA_BAN`, `BAN`, `ABUSE_WARNING`, `SPAM_WARNING`,
+            `SPAM_WATCH`, `SOLID_CONTRIBUTOR`, `HELPFUL_USER`.
+        :param `Optional[str]` anchor_submission_id:
+            A submission ID to link the note to.
+
+            Mutually exclusive with `anchor_comment_id`.
+        :param `Optional[str]` anchor_comment_id:
+            A comment ID to link the note to.
+
+            Mutually exclusive with `anchor_submission_id`.
 
         .. .RETURNS
 
-        :rtype: `Sequence`\\[:class:`~.models.message_SYNC.ComposedMessage`]
+        :rtype: :class:`~.models.moderation_note.ModerationUserNote`
 
         .. .RAISES
 
+        :raises redditwarp.exceptions.RedditError:
+            + `USER_DOESNT_EXIST`:
+                The specified user does not exist.
+            + `BAD_SR_NAME`:
+                The specified subreddit does not exist.
+            + `NO_TEXT`:
+                The content of the note was empty.
+            + `TOO_LONG`:
+                The content of the note was too long, over 250 characters.
+            + `INVALID_OPTION`:
+                The label specified was invalid.
+            + `NO_THING_ID`:
+                The linked submission or comment does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
-                The target message specified does not exist or
-                you do not have permission to access it.
+                You are not a moderator of the target subreddit.
         """
-        id36 = to_base36(idn)
-        root = self._client.request('GET', f'/message/messages/{id36}')
-        obj_data = root['data']['children'][0]['data']
-        return load_composed_message_thread(obj_data, self._client)
-
-    def send(self, to: str, subject: str, body: str) -> None:
-        """Send a direct message to a user.
-
-        .. .PARAMETERS
-
-        :param `str` to:
-            Name of user in which to send the message to.
-        :param `str` subject:
-            The subject of the message.
-        :param `str` body:
-            The body text of the message.
-
-        .. .RETURNS
+        mxp = (anchor_submission_id, anchor_comment_id)
+        if len(mxp) - mxp.count(None) > 1:
+            raise TypeError("mutually exclusive parameters: `anchor_submission_id`, `anchor_comment_id`.")
 
-        :rtype: `None`
+        params = {'subreddit': sr, 'user': user, 'note': content, 'label': label}
+        root = self._client.request('POST', '/api/mod/notes', params=params)
+        return load_moderation_user_note(root['created'])
 
-        .. .RAISES
+    def delete(self, sr: str, user: str, uuid: str) -> None:
+        """Delete a moderation note.
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `NO_USER`:
-                The user specified by `to` was empty.
-            + `NO_SUBJECT`:
-                The subject specified by `subject` was empty.
-            + `NO_TEXT`:
-                The body text specified by `body` was empty.
-            + `USER_DOESNT_EXIST`:
-                The user specified by `to` does not exist.
-            + `NOT_WHITELISTED_BY_USER_MESSAGE`:
-                The target user has direct messages from strangers disabled.
-
-                On old Reddit, this setting can be configured at `<https://old.reddit.com/prefs/blocked>`_
-                by setting "Show private messages from" to "Only trusted users".
-        """
-        req_data = {
-            'to': to,
-            'subject': subject,
-            'text': body,
-        }
-        self._client.request('POST', '/api/compose', data=req_data)
+        This procedure can be used to delete either a user or action type note.
 
-    def send_from_sr(self, sr: str, to: str, subject: str, body: str) -> None:
-        """Send a direct message to a user on behalf of a subreddit.
+        In addition to the note ID, the endpoint must be given the subreddit and
+        user name in which the note belongs. If either information is incorrect,
+        the endpoint will raise a 500 HTTP error.
 
         .. .PARAMETERS
 
         :param `str` sr:
-            The name of a subreddit you moderate.
-        :param `str` to:
-            Name of user in which to send the message to.
-        :param `str` subject:
-            The subject of the message.
-        :param `str` body:
-            The body text of the message.
+        :param `str` user:
+        :param `str` uuid:
+            UUID of a note.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
-            + `NO_USER`:
-                The user specified by `to` was empty.
-            + `NO_SUBJECT`:
-                The subject specified by `subject` was empty.
-            + `NO_TEXT`:
-                The body text specified by `body` was empty.
+            + `BAD_SR_NAME`:
+                The `sr` parameter was empty.
             + `SUBREDDIT_NOEXIST`:
-                The subreddit specified by `sr` does not exist.
-            + `NO_SR_TO_SR_MESSAGE`:
-                Both `sr` and `to` refer to subreddits.
-                Subreddit to subreddit messages is not allowed.
+                The target subreddit does not exist.
+            + `USER_DOESNT_EXIST`:
+               - The specified user does not exist.
+               - The `user` parameter was empty.
+            + `PARAMETER_REQUIRED`:
+                The `uuid` parameter was empty.
+            + `INVALID_ID`:
+                The specified user does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-                The current user is not a moderator of the specified subreddit.
-        """
-        req_data = {
-            'from_sr': sr,
-            'to': to,
-            'subject': subject,
-            'text': body,
-        }
-        self._client.request('POST', '/api/compose', data=req_data)
-
-    def reply(self, idn: int, body: str) -> ComposedMessage:
-        """Reply to a message
+            + `500`:
+               - The subreddit or user specified is incorrect for the given note ID.
+               - The given note ID was invalid.
+        """
+        params = {'subreddit': sr, 'user': user, 'note_id': 'ModNote_' + uuid}
+        self._client.request('DELETE', '/api/mod/notes', params=params)
+
+    def pull_notes(self,
+        sr: str,
+        user: str,
+        amount: Optional[int] = None,
+        *,
+        label: Optional[str] = None,
+    ) -> ImpartedPaginatorChainingIterator[ModerationNotePaginator, ModerationNote]:
+        """Get moderation notes of a user in a subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
-        :param `str` body:
-
-        .. .RETURNS
-
-        :returns: The newly created message.
-        :rtype: :class:`~.models.message_SYNC.ComposedMessage`
-
-        .. .RAISES
-
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `NO_TEXT`:
-                The body text specified by `body` was empty.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-                The specified message ID does not exist.
-        """
-        data = {
-            'thing_id': 't4_' + to_base36(idn),
-            'text': body,
-            'return_rtjson': '1',
-        }
-        result = self._client.request('POST', '/api/comment', data=data)
-        root = result['json']['data']['things'][0]['data']
-        return load_composed_message(root, self._client)
-
-    def delete(self, idn: int) -> None:
-        """Delete a message.
-
-        If the message specified by the ID doesn't exist, or is invalid,
-        the action is treated as a success.
-
-        .. .PARAMETERS
+        :param `str` sr:
+        :param `str` user:
+        :param `Optional[int]` amount:
+        :param `Optional[str]` label:
+            Filter by note type.
 
-        :param `int` idn:
+            Either: `ALL`, `NOTE`, `APPROVAL`, `REMOVAL`, `BAN`, `MUTE`,
+            `INVITE`, `SPAM`, `CONTENT_CHANGE`.
 
         .. .RETURNS
 
-        :rtype: `None`
+        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.moderation.note_pulls_sync1.ModerationNotePaginator`, :class:`~.models.moderation_note.ModerationNote`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
-        """
-        self._client.request('POST', '/api/del_msg', data={'id': 't4_' + to_base36(idn)})
-
-    def mark_read(self, idn: int) -> None:
-        """Mark a message as read.
+            + `BAD_SR_NAME`:
+                The `sr` parameter was empty.
+            + `SUBREDDIT_NOEXIST`:
+                The target subreddit does not exist.
+            + `USER_DOESNT_EXIST`:
+               - The specified user does not exist.
+               - The `user` parameter was empty.
+            + `INVALID_ID`:
+                An invalid value was specified for the `label` parameter.
+                Values are case-sensitive.
+        """
+        p = ModerationNotePaginator(
+            client=self._client,
+            url='/api/mod/notes',
+            subreddit=sr,
+            user=user,
+            type=label,
+        )
+        return ImpartedPaginatorChainingIterator(p, amount)
+
+    def pull_user_notes(self,
+        sr: str,
+        user: str,
+        amount: Optional[int] = None,
+    ) -> ImpartedPaginatorChainingIterator[ModerationUserNotePaginator, ModerationUserNote]:
+        """
+        Behaves similarly to :meth:`.pull_notes`.
+        """
+        p = ModerationUserNotePaginator(
+            client=self._client,
+            url='/api/mod/notes',
+            subreddit=sr,
+            user=user,
+            type='NOTE',
+        )
+        return ImpartedPaginatorChainingIterator(p, amount)
 
-        Marking an already marked as read item is treated as a success.
+    def get_latest_user_note(self, sr: str, user: str) -> Optional[ModerationUserNote]:
+        """Get the most recently written user note for some user.
 
         .. .PARAMETERS
 
-        :param `int` idn:
-
-        .. .RETURNS
-
-        :rtype: `None`
-
-        .. .RAISES
-
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `400`:
-                The message specified by the ID doesn't exist or is invalid.
-        """
-        self._client.request('POST', '/api/read_message', data={'id': 't4_' + to_base36(idn)})
-
-    def mark_unread(self, idn: int) -> None:
-        """Mark a message as unread.
-
-        Behaves similarly to :meth:`.mark_read`.
-        """
-        self._client.request('POST', '/api/unread_message', data={'id': 't4_' + to_base36(idn)})
-
-    def mark_all_read(self) -> None:
-        """Mark all messages as read.
+        :param `str` sr:
+        :param `str` user:
 
         .. .RETURNS
 
-        :rtype: `None`
+        :rtype: `Optional`\\[:class:`~.models.moderation_note.ModerationUserNote`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
-        """
-        self._client.request('POST', '/api/read_all_messages')
-
-    def mark_comment_read(self, idn: int) -> None:
-        """Mark a comment message as read.
+            + `PARAMETER_REQUIRED`:
+               - The `sr` parameter was empty.
+               - The `user` parameter was empty.
+        """
+        params = {'subreddits': sr, 'users': user}
+        try:
+            root = self._client.request('GET', '/api/mod/notes/recent', params=params)
+        except http.exceptions.StatusCodeException as e:
+            if e.status_code == 400:
+                return None
+            raise
+        note_obj = root['mod_notes'][0]
+        if note_obj is None:
+            return None
+        return load_moderation_user_note(note_obj)
 
-        Behaves similarly to :meth:`.mark_read`.
-        """
-        self._client.request('POST', '/api/read_message', data={'id': 't1_' + to_base36(idn)})
+    def bulk_get_latest_user_note(self, pairs: Iterable[tuple[str, str]]) -> CallChunkChainingIterator[Optional[ModerationUserNote]]:
+        """Bulk fetch the most recently written user notes for users.
 
-    def mark_comment_unread(self, idn: int) -> None:
-        """Mark a comment message as unread.
-
-        Behaves similarly to :meth:`.mark_read`.
-        """
-        self._client.request('POST', '/api/read_message', data={'id': 't1_' + to_base36(idn)})
-
-    def collapse(self, idn: int) -> None:
-        """Collapse a message.
-
-        If the specified message does not exist or is valid,
-        the action is treated as a success.
+        The response contains a list of mod notes in the order that subreddits and users were given.
+        If no note exists for a given pair, `None` will take its place in the list.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Iterable[tuple[str, str]]` pairs:
 
         .. .RETURNS
 
-        :rtype: `None`
+        :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`Optional`\\[:class:`~.models.moderation_note.ModerationUserNote`]]
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
+        :(raises): Same as :meth:`.get_latest_user_note`.
         """
-        self._client.request('POST', '/api/collapse_message', data={'id': 't4_' + to_base36(idn)})
-
-    def uncollapse(self, idn: int) -> None:
-        """Uncollapse a message.
-
-        Behaves similarly to :meth:`.mark_read`.
-        """
-        self._client.request('POST', '/api/uncollapse_message', data={'id': 't4_' + to_base36(idn)})
-
-    class BlockAuthor:
-        def __init__(self, outer: MessageProcedures) -> None:
-            self._client = outer._client
-
-        def __call__(self, idn: int) -> None:
-            self.of_message(idn)
-
-        def of_message(self, idn: int) -> None:
-            self._client.request('POST', '/api/block', data={'id': 't4_' + to_base36(idn)})
-
-        def of_comment(self, idn: int) -> None:
-            self._client.request('POST', '/api/block', data={'id': 't1_' + to_base36(idn)})
-
-        def of_submission(self, idn: int) -> None:
-            self._client.request('POST', '/api/block', data={'id': 't3_' + to_base36(idn)})
-
-    block_author: cached_property[BlockAuthor] = cached_property(BlockAuthor)
-    ("""
-        Block the author of a message, comment, or submission.
-
-        - Use :meth:`~.BlockAuthor.__call__` to block the author of a message.
-        - Use :meth:`~.BlockAuthor.of_comment` to block the author of a comment.
-        - Use :meth:`~.BlockAuthor.of_submission` to block the author of a submission.
-
-        To block a user directly by ID or name, see
-        :meth:`~.AccountProcedures.block_user_by_id` and :meth:`~.AccountProcedures.block_user_by_name`
-        instead.
+        def mass_get_latest_user_note(pairs: Sequence[tuple[str, str]]) -> Sequence[Optional[ModerationUserNote]]:
+            subreddits, users = tuple(zip(*pairs))
+            subreddits_str = ','.join(subreddits)
+            users_str = ','.join(users)
+            params = {'subreddits': subreddits_str, 'users': users_str}
+            try:
+                root = self._client.request('GET', '/api/mod/notes/recent', params=params)
+            except http.exceptions.StatusCodeException as e:
+                if e.status_code == 400:
+                    return [None]
+                raise
+            return [
+                (None if note_obj is None else load_moderation_user_note(note_obj))
+                for note_obj in root['mod_notes']
+            ]
 
-        .. .PARAMETERS
-
-        :param `int` idn:
-
-        .. .RETURNS
-
-        :rtype: `None`
-
-        .. .RAISES
-
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-        """)
+        return CallChunkChainingIterator(CallChunk(mass_get_latest_user_note, chunk) for chunk in chunked(pairs, 500))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/message/pulls_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/message/pulls_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/message/pulls_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/message/pulls_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/misc/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/misc/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/misc/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/misc/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/SYNC.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence, Optional, Mapping
+from typing import TYPE_CHECKING, Sequence, Optional, Mapping, Union
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
+    from ...client_SYNC import Client
     from ...models.subreddit_user import (
         Moderator,
         ApprovedUser,
         BannedUser,
         MutedUser,
     )
     from ...models.moderation_action_log_entry import ModerationActionLogEntry
@@ -15,21 +15,21 @@
 
 from ...model_loaders.subreddit_user import (
     load_moderator,
     load_approved_user,
     load_banned_user,
     load_muted_user,
 )
-from .pull_users_ASYNC import PullUsers
-from .legacy_ASYNC import Legacy
-from .pull_ASYNC import Pull
-from .note_ASYNC import Note
+from .pull_users_SYNC import PullUsers
+from .legacy_SYNC import Legacy
+from .pull_SYNC import Pull
+from .note_SYNC import Note
 from ...util.base_conversion import to_base36
-from ...pagination.paginator_chaining_async_iterator import ImpartedPaginatorChainingAsyncIterator
-from ...pagination.paginators.moderation.async1 import ModerationActionLogAsyncPaginator
+from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
+from ...pagination.paginators.moderation.sync1 import ModerationActionLogPaginator
 
 class ModerationProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.legacy: Legacy = Legacy(client)
         ("""
             Legacy procedures for retrieving subreddit users.
@@ -45,15 +45,15 @@
         self.note: Note = Note(client)
         ("""
             Procedures for managing mod notes.
             """)
 
     def pull_actions(self, sr: str, amount: Optional[int] = None, *,
             action: str = '', mod: str = '',
-            ) -> ImpartedPaginatorChainingAsyncIterator[ModerationActionLogAsyncPaginator, ModerationActionLogEntry]:
+            ) -> ImpartedPaginatorChainingIterator[ModerationActionLogPaginator, ModerationActionLogEntry]:
         """Retrieve recent moderation actions from the mod log.
 
         .. hint::
 
            Moderator actions taken within a subreddit are logged to a mod log.
            Entries in the mod log last for 3 months before they become inaccessible.
 
@@ -67,54 +67,54 @@
             Limit log entries to only those of a specified action.
         :param `str` mod:
             A comma-delimited list of moderator names to restrict the results to,
             or use the string `a` to restrict the results to actions performed by administrators.
 
         .. .RETURNS
 
-        :rtype: :class:`~.pagination.paginator_chaining_async_iterator.ImpartedPaginatorChainingAsyncIterator`\\[:class:`~.pagination.paginators.moderation.async1.ModerationActionLogAsyncPaginator`, :class:`~.models.moderation_action_log_entry.ModerationActionLogEntry`]
+        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.moderation.sync1.ModerationActionLogPaginator`, :class:`~.models.moderation_action_log_entry.ModerationActionLogEntry`]
 
         .. .RAISES
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 You do not have permission to view the mod log of the specified subreddit.
         """
-        p = ModerationActionLogAsyncPaginator(self._client, f'/r/{sr}/about/log', action=action, mod=mod)
-        return ImpartedPaginatorChainingAsyncIterator(p, amount)
+        p = ModerationActionLogPaginator(self._client, f'/r/{sr}/about/log', action=action, mod=mod)
+        return ImpartedPaginatorChainingIterator(p, amount)
 
 
-    async def get_moderator(self, sr: str, user: str) -> Optional[Moderator]:
+    def get_moderator(self, sr: str, user: str) -> Optional[Moderator]:
         """
         Behaves similarly to :meth:`.get_approved_user`.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/moderators', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/moderators', params={'username': user})
         order = root['moderatorIds']
         object_map = root['moderators']
         return load_moderator(object_map[order[0]]) if order else None
 
-    async def get_moderator_invitation(self, sr: str, user: str) -> Optional[Moderator]:
+    def get_moderator_invitation(self, sr: str, user: str) -> Optional[Moderator]:
         """
         Behaves similarly to :meth:`.get_approved_user`.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/moderators_invited', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/moderators_invited', params={'username': user})
         order = root['moderatorIds']
         object_map = root['moderators']
         return load_moderator(object_map[order[0]]) if order else None
 
-    async def get_editable_moderator(self, sr: str, user: str) -> Optional[Moderator]:
+    def get_editable_moderator(self, sr: str, user: str) -> Optional[Moderator]:
         """
         Behaves similarly to :meth:`.get_approved_user`.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/moderators_editable', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/moderators_editable', params={'username': user})
         order = root['moderatorIds']
         object_map = root['moderators']
         return load_moderator(object_map[order[0]]) if order else None
 
-    async def get_approved_user(self, sr: str, user: str) -> Optional[ApprovedUser]:
+    def get_approved_user(self, sr: str, user: str) -> Optional[ApprovedUser]:
         """Get an approved user of a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
             Name of a subreddit.
         :param `str` user:
@@ -128,39 +128,39 @@
 
         :raises redditwarp.exceptions.RedditError:
             + `SUBREDDIT_NOEXIST`:
                 The target subreddit does not exist.
             + `SUBREDDIT_NO_ACCESS`:
                 The subreddit cannot be accessed.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/contributors', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/contributors', params={'username': user})
         order = root['approvedSubmitterIds']
         object_map = root['approvedSubmitters']
         return load_approved_user(object_map[order[0]]) if order else None
 
-    async def get_banned_user(self, sr: str, user: str) -> Optional[BannedUser]:
+    def get_banned_user(self, sr: str, user: str) -> Optional[BannedUser]:
         """
         Behaves similarly to :meth:`.get_approved_user`.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/banned', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/banned', params={'username': user})
         order = root['bannedUserIds']
         object_map = root['bannedUsers']
         return load_banned_user(object_map[order[0]]) if order else None
 
-    async def get_muted_user(self, sr: str, user: str) -> Optional[MutedUser]:
+    def get_muted_user(self, sr: str, user: str) -> Optional[MutedUser]:
         """
         Behaves similarly to :meth:`.get_approved_user`.
         """
-        root = await self._client.request('GET', f'/api/v1/{sr}/muted', params={'username': user})
+        root = self._client.request('GET', f'/api/v1/{sr}/muted', params={'username': user})
         order = root['mutedUserIds']
         object_map = root['mutedUsers']
         return load_muted_user(object_map[order[0]]) if order else None
 
 
-    async def send_moderator_invite(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+    def send_moderator_invite(self, sr: str, user: str, permissions: Sequence[str]) -> None:
         """Send a moderator invite.
 
         If the user is already invited, nothing happens. The permissions won't change.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -196,19 +196,19 @@
             + `404`:
                 The specified subreddit does not exist.
         """
         data = {
             'type': 'moderator_invite',
             'r': sr,
             'name': user,
-            'permissions': ','.join('+' + p for p in permissions),
+            'permissions': ','.join('+' + p for p in permissions) if permissions else '-access',
         }
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def accept_moderator_invite(self, sr: str) -> None:
+    def accept_moderator_invite(self, sr: str) -> None:
         """Accept a moderator invite.
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
@@ -222,17 +222,17 @@
                 There is no user context.
             + `NO_INVITE_FOUND`:
                 You don't have a pendning invitation for the specified subreddit.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The subreddit specified was empty.
         """
-        await self._client.request('POST', '/api/accept_moderator_invite', data={'r': sr})
+        self._client.request('POST', '/api/accept_moderator_invite', data={'r': sr})
 
-    async def revoke_moderator_invite(self, sr: str, user: str) -> None:
+    def revoke_moderator_invite(self, sr: str, user: str) -> None:
         """Revoke a moderator invite.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -253,17 +253,17 @@
                - The target subreddit specified was empty.
         """
         data = {
             'type': 'moderator_invite',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def remove_moderator(self, sr: str, user: str) -> None:
+    def remove_moderator(self, sr: str, user: str) -> None:
         """Remove a moderator.
 
         Nothing happens if the specified user is not a moderator of the subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -286,45 +286,46 @@
                - The target subreddit specified was empty.
         """
         data = {
             'type': 'moderator',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def leave_moderator(self, sr_id: int) -> None:
+    def leave_moderator(self, sr_id: Union[int, str]) -> None:
         """Abdicate moderator status in a subreddit.
 
         .. warning::
 
             This action cannot be undone.
 
         Be careful with this endpoint. It's possible for a subreddit to not have any moderators.
 
         Nothing happens if the specified subreddit ID is not valid or the
         current user is not a moderator of the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` sr_id:
+        :param `Union[int, str]` sr_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        await self._client.request('POST', '/api/leavemoderator', data={'id': 't5_' + to_base36(sr_id)})
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
+        self._client.request('POST', '/api/leavemoderator', data={'id': 't5_' + id36})
 
-    async def set_moderator_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+    def set_moderator_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
         """Set the permissions of a moderator.
 
         Be careful with this endpoint. It's possible for a subreddit to not have any moderators.
 
         Nothing happens if the current user is not a moderator of the subreddit.
 
         .. .PARAMETERS
@@ -360,17 +361,17 @@
         """
         data = {
             'type': 'moderator',
             'r': sr,
             'name': user,
             'permissions': ','.join('+' + p for p in permissions) if permissions else '-access',
         }
-        await self._client.request('POST', '/api/setpermissions', data=data)
+        self._client.request('POST', '/api/setpermissions', data=data)
 
-    async def set_moderator_invite_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
+    def set_moderator_invite_permissions(self, sr: str, user: str, permissions: Sequence[str]) -> None:
         """Set the permissions on a moderator invite.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
         :param `Sequence[str]` permissions:
@@ -402,17 +403,17 @@
         """
         data = {
             'type': 'moderator_invite',
             'r': sr,
             'name': user,
             'permissions': ','.join('+' + p for p in permissions) if permissions else '-access',
         }
-        await self._client.request('POST', '/api/setpermissions', data=data)
+        self._client.request('POST', '/api/setpermissions', data=data)
 
-    async def add_approved_user(self, sr: str, user: str) -> None:
+    def add_approved_user(self, sr: str, user: str) -> None:
         """Add an approved user to a subreddit.
 
         If the user is already an approved user, nothing happens.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -440,17 +441,17 @@
                 The specified subreddit does not exist.
         """
         data = {
             'type': 'contributor',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def remove_approved_user(self, sr: str, user: str) -> None:
+    def remove_approved_user(self, sr: str, user: str) -> None:
         """Remove an approved user of a subreddit.
 
         If the user is already not an approved user, nothing happens.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -480,39 +481,40 @@
                 The specified subreddit does not exist.
         """
         data = {
             'type': 'contributor',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def leave_approved_user(self, sr_id: int) -> None:
+    def leave_approved_user(self, sr_id: Union[int, str]) -> None:
         """Abdicate approved user status in a subreddit.
 
         Nothing happens if the specified subreddit ID is not valid or the
         current user is not an approved user of the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` sr_id:
+        :param `Union[int, str]` sr_id:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        await self._client.request('POST', '/api/leavecontributor', data={'id': 't5_' + to_base36(sr_id)})
+        id36 = x if isinstance((x := sr_id), str) else to_base36(x)
+        self._client.request('POST', '/api/leavecontributor', data={'id': 't5_' + id36})
 
-    async def ban_user(self, sr: str, user: str, *,
+    def ban_user(self, sr: str, user: str, *,
             duration: Optional[int] = None,
             reason: str = '',
             note: str = '',
             message: str = '') -> None:
         """Ban a user from a subreddit.
 
         Banning an already banned user does nothing. However, when banning an already
@@ -578,17 +580,17 @@
             'ban_reason': reason,
             'ban_message': message,
             'note': note,
         }
         if duration is not None:
             data['duration'] = str(duration)
 
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def unban_user(self, sr: str, user: str) -> None:
+    def unban_user(self, sr: str, user: str) -> None:
         """Unban a user from a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -601,17 +603,17 @@
         :(raises): Same as :meth:`~.remove_approved_user`.
         """
         data = {
             'type': 'banned',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def mute_user(self, sr: str, user: str, *, note: str = '') -> None:
+    def mute_user(self, sr: str, user: str, *, note: str = '') -> None:
         """Mute a user in a subreddit.
 
         Muting an already muted user does nothing.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -635,17 +637,17 @@
         """
         data = {
             'type': 'muted',
             'r': sr,
             'name': user,
             'note': note,
         }
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def unmute_user(self, sr: str, user: str) -> None:
+    def unmute_user(self, sr: str, user: str) -> None:
         """Unmute a user in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -658,17 +660,17 @@
         :(raises): Same as :meth:`~.remove_approved_user`.
         """
         data = {
             'type': 'muted',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def add_wiki_contributor(self, sr: str, user: str) -> None:
+    def add_wiki_contributor(self, sr: str, user: str) -> None:
         """Add a wiki contributor in a subreddit.
 
         Adding a user who is already a wiki contributor does nothing.
 
         .. .PARAMETERS
 
         :param `str` sr:
@@ -683,17 +685,17 @@
         :(raises): Same as :meth:`~.add_approved_user`.
         """
         data = {
             'type': 'wikicontributor',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def remove_wiki_contributor(self, sr: str, user: str) -> None:
+    def remove_wiki_contributor(self, sr: str, user: str) -> None:
         """Remove a wiki contributor in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -706,17 +708,17 @@
         :(raises): Same as :meth:`~.remove_approved_user`.
         """
         data = {
             'type': 'wikicontributor',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
-    async def ban_wiki_contributor(self, sr: str, user: str, *,
+    def ban_wiki_contributor(self, sr: str, user: str, *,
             duration: Optional[int] = None,
             reason: str = '',
             note: str = '') -> None:
         """Ban a wiki contributor in a subreddit.
 
         Adding a user who is already a wiki contributor does nothing.
 
@@ -753,17 +755,17 @@
             'name': user,
             'ban_reason': reason,
             'note': note,
         }
         if duration is not None:
             data['duration'] = str(duration)
 
-        await self._client.request('POST', '/api/friend', data=data)
+        self._client.request('POST', '/api/friend', data=data)
 
-    async def unban_wiki_contributor(self, sr: str, user: str) -> None:
+    def unban_wiki_contributor(self, sr: str, user: str) -> None:
         """Unban a wiki contributor in a subreddit.
 
         .. .PARAMETERS
 
         :param `str` sr:
         :param `str` user:
 
@@ -776,23 +778,23 @@
         :(raises): Same as :meth:`~.remove_approved_user`.
         """
         data = {
             'type': 'wikibanned',
             'r': sr,
             'name': user,
         }
-        await self._client.request('POST', '/api/unfriend', data=data)
+        self._client.request('POST', '/api/unfriend', data=data)
 
 
     class RemovalReason:
         def __init__(self, outer: ModerationProcedures) -> None:
             self._outer = outer
             self._client = outer._client
 
-        async def create(self, sr: str, title: str, message: str) -> str:
+        def create(self, sr: str, title: str, message: str) -> str:
             """Create a removal reason.
 
             .. .PARAMETERS
 
             :param `str` sr:
             :param `str` title:
                 A title for this removal reason.
@@ -820,18 +822,18 @@
                    - The value specified for `message` is over 10000 characters.
 
             :raises redditwarp.http.exceptions.StatusCodeException:
                 + `500`:
                     The target subreddit does not exist.
             """
             data = {'title': title, 'message': message}
-            root = await self._client.request('POST', f'/api/v1/{sr}/removal_reasons', data=data)
+            root = self._client.request('POST', f'/api/v1/{sr}/removal_reasons', data=data)
             return root['id']
 
-        async def retrieve(self, sr: str) -> Mapping[str, tuple[str, str]]:
+        def retrieve(self, sr: str) -> Mapping[str, tuple[str, str]]:
             """Get a list of removal reasons.
 
             .. .PARAMETERS
 
             :param `str` sr:
 
             .. .RETURNS
@@ -845,23 +847,23 @@
                 + `MOD_REQUIRED`:
                    - There is no user context.
                    - The current user is not a moderator of the subreddit.
 
                 + `SUBREDDIT_NOEXIST`:
                     The target subreddit does not exist.
             """
-            root = await self._client.request('GET', f'/api/v1/{sr}/removal_reasons')
+            root = self._client.request('GET', f'/api/v1/{sr}/removal_reasons')
             order = root['order']
             object_map = root['data']
             return {
                 y: (m['title'], m['message'])
                 for y in order for m in [object_map[y]]
             }
 
-        async def replace(self, sr: str, idt: str, title: str, message: str) -> None:
+        def replace(self, sr: str, idt: str, title: str, message: str) -> None:
             """Update a removal reason's title and message.
 
             Both parameters `title` and `message` must be specified otherwise
             a `NO_TEXT` API error is returned.
 
             .. .PARAMETERS
 
@@ -891,17 +893,17 @@
                    - The `message` parameter was not specified or was empty.
 
                 + `TOO_LONG`:
                    - The value specified for `title` is over 50 characters.
                    - The value specified for `message` is over 10000 characters.
             """
             data = {'title': title, 'message': message}
-            await self._client.request('PUT', f'/api/v1/{sr}/removal_reasons/{idt}', data=data)
+            self._client.request('PUT', f'/api/v1/{sr}/removal_reasons/{idt}', data=data)
 
-        async def delete(self, sr: str, idt: str) -> None:
+        def delete(self, sr: str, idt: str) -> None:
             """Delete a removal reason.
 
             If the specified removal reason ID did not exist, nothing happens.
 
             .. .PARAMETERS
 
             :param `str` sr:
@@ -919,10 +921,13 @@
                    - The current user is not a moderator of the subreddit.
 
                 + `SUBREDDIT_NOEXIST`:
                     The target subreddit does not exist.
                 + `INVALID_ID`:
                     The specified removal reason ID was not found.
             """
-            await self._client.request('DELETE', f'/api/v1/{sr}/removal_reasons/{idt}')
+            self._client.request('DELETE', f'/api/v1/{sr}/removal_reasons/{idt}')
 
     removal_reason: cached_property[RemovalReason] = cached_property(RemovalReason)
+    ("""
+        Manage subreddit removal reasons.
+        """)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_pull_users_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_pull_users_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/legacy_pull_users_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/legacy_pull_users_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/note_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/note_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/note_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/SYNC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,260 +1,262 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable
+from typing import TYPE_CHECKING, Optional, Sequence, Union, TypeVar, Iterable
 if TYPE_CHECKING:
     from ...client_SYNC import Client
-    from ...models.moderation_note import (
-        ModerationNote,
-        ModerationUserNote,
-    )
+    from ...models.user_SYNC import User
+    from ...models.moderated_subreddit import ModeratedSubreddit
 
+from .pull_SYNC import Pull
+from .pull_subreddits_SYNC import PullSubreddits
+from ...model_loaders.user_SYNC import load_user, load_potentially_suspended_user
+from ...model_loaders.moderated_subreddit import load_moderated_subreddit
+from ... import http
 from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
-from ...pagination.paginators.moderation.note_pulls_sync1 import (
-    ModerationNotePaginator,
-    ModerationUserNotePaginator,
-)
+from ...pagination.paginators.user.sync1 import UserSearchPaginator
+from ...exceptions import RejectedResultException
+from ...models.user_summary import UserSummary
+from ...model_loaders.user_summary import load_user_summary
+from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
 from ...iterators.call_chunk import CallChunk
-from ...model_loaders.moderation_note import load_moderation_user_note
-from ... import http
 
-class Note:
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
+class UserProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
+        self.pull: Pull = Pull(client)
+        ("""
+            Pull submissions and comments associated with a user.
+            """)
+        self.pull_subreddits: PullSubreddits = PullSubreddits(client)
+        ("""
+            Get user subreddits.
+            """)
 
-    def create_user_note(self, sr: str, user: str, content: str, *,
-            label: str = '',
-            anchor_submission_id: Optional[int] = None,
-            anchor_comment_id: Optional[int] = None) -> ModerationUserNote:
-        """Create a user note.
+    def get_by_name(self, name: str) -> Optional[User]:
+        """Get information about a user by name.
+
+        Returns `None` if the specified user was not found,
+        or is a suspended account.
 
         .. .PARAMETERS
 
-        :param `str` sr:
-            Subreddit name.
-        :param `str` user:
+        :param `str` name:
             User name.
-        :param `str` content:
-            Content of the note. Max 250 characters.
-        :param `str` label:
-            Either: `BOT_BAN`, `PERMA_BAN`, `BAN`, `ABUSE_WARNING`, `SPAM_WARNING`,
-            `SPAM_WATCH`, `SOLID_CONTRIBUTOR`, `HELPFUL_USER`.
-        :param `Optional[str]` anchor_submission_id:
-            A submission ID to link the note to.
-
-            Mutually exclusive with `anchor_comment_id`.
-        :param `Optional[str]` anchor_comment_id:
-            A comment ID to link the note to.
 
-            Mutually exclusive with `anchor_submission_id`.
+        .. .RETURNS
+
+        :rtype: `Optional`\\[:class:`~.models.user_SYNC.User`]
+        """
+        try:
+            root = self._client.request('GET', f'/user/{name}/about')
+        except http.exceptions.StatusCodeException as e:
+            if e.status_code == 404:
+                return None
+            raise
+        obj_data = root['data']
+        if obj_data.get('is_suspended', False):
+            return None
+        return load_user(obj_data, self._client)
+
+    def fetch_by_name(self, name: str) -> User:
+        """Fetch information about a user by name.
+
+        .. .PARAMETERS
+
+        :param `str` name:
+            User name.
 
         .. .RETURNS
 
-        :rtype: :class:`~.models.moderation_note.ModerationUserNote`
+        :rtype: :class:`~.models.user_SYNC.User`
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_DOESNT_EXIST`:
-                The specified user does not exist.
-            + `BAD_SR_NAME`:
-                The specified subreddit does not exist.
-            + `NO_TEXT`:
-                The content of the note was empty.
-            + `TOO_LONG`:
-                The content of the note was too long, over 250 characters.
-            + `INVALID_OPTION`:
-                The label specified was invalid.
-            + `NO_THING_ID`:
-                The linked submission or comment does not exist.
+        :raises redditwarp.exceptions.RejectedResultException:
+            The specified user account is suspended.
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `403`:
-                You are not a moderator of the target subreddit.
+            + `404`:
+                The specified user was not found.
         """
-        mxp = (anchor_submission_id, anchor_comment_id)
-        if len(mxp) - mxp.count(None) > 1:
-            raise TypeError("mutually exclusive parameters: `anchor_submission_id`, `anchor_comment_id`.")
+        root = self._client.request('GET', f'/user/{name}/about')
+        obj_data = root['data']
+        if obj_data.get('is_suspended', False):
+            raise RejectedResultException('user is suspended')
+        return load_user(obj_data, self._client)
 
-        params = {'subreddit': sr, 'user': user, 'note': content, 'label': label}
-        root = self._client.request('POST', '/api/mod/notes', params=params)
-        return load_moderation_user_note(root['created'])
+    def get_potentially_suspended_by_name(self, name: str) -> Optional[object]:
+        """Get information about a potentially suspended user, by name.
 
-    def delete(self, sr: str, user: str, uuid: str) -> None:
-        """Delete a moderation note.
+        Returns `None` if the specified user was not found.
 
-        This procedure can be used to delete either a user or action type note.
+        .. .PARAMETERS
 
-        In addition to the note ID, the endpoint must be given the subreddit and
-        user name in which the note belongs. If either information is incorrect,
-        the endpoint will raise a 500 HTTP error.
+        :param `str` name:
+
+        .. .RETURNS
+
+        :returns:
+            * :class:`~.models.user_SYNC.User` if the user exists.
+            * :class:`~.models.user_SYNC.SuspendedUser` if the user is suspended.
+            * `None` if the user was not found.
+        :rtype: `Optional`\\[`object`]
+        """
+        try:
+            root = self._client.request('GET', f'/user/{name}/about')
+        except http.exceptions.StatusCodeException as e:
+            if e.status_code == 404:
+                return None
+            raise
+        return load_potentially_suspended_user(root['data'], self._client)
+
+    def fetch_potentially_suspended_by_name(self, name: str) -> object:
+        """Fetch information about a potentially suspended user, by name.
 
         .. .PARAMETERS
 
-        :param `str` sr:
-        :param `str` user:
-        :param `str` uuid:
-            UUID of a note.
+        :param `str` name:
 
         .. .RETURNS
 
-        :rtype: `None`
+        :returns:
+            * :class:`~.models.user_SYNC.User` if the user exists.
+            * :class:`~.models.user_SYNC.SuspendedUser` if the user is suspended.
+        :rtype: `object`
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `BAD_SR_NAME`:
-                The `sr` parameter was empty.
-            + `SUBREDDIT_NOEXIST`:
-                The target subreddit does not exist.
-            + `USER_DOESNT_EXIST`:
-               - The specified user does not exist.
-               - The `user` parameter was empty.
-            + `PARAMETER_REQUIRED`:
-                The `uuid` parameter was empty.
-            + `INVALID_ID`:
-                The specified user does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
-            + `500`:
-               - The subreddit or user specified is incorrect for the given note ID.
-               - The given note ID was invalid.
-        """
-        params = {'subreddit': sr, 'user': user, 'note_id': 'ModNote_' + uuid}
-        self._client.request('DELETE', '/api/mod/notes', params=params)
-
-    def pull_notes(self,
-        sr: str,
-        user: str,
-        amount: Optional[int] = None,
-        *,
-        label: Optional[str] = None,
-    ) -> ImpartedPaginatorChainingIterator[ModerationNotePaginator, ModerationNote]:
-        """Get moderation notes of a user in a subreddit.
+            + `404`:
+                The specified user was not found.
+        """
+        root = self._client.request('GET', f'/user/{name}/about')
+        return load_potentially_suspended_user(root['data'], self._client)
+
+    def get_user_summary(self, idy: Union[int, str]) -> Optional[UserSummary]:
+        """
+        Get a partial user object by ID.
 
         .. .PARAMETERS
 
-        :param `str` sr:
-        :param `str` user:
-        :param `Optional[int]` amount:
-        :param `Optional[str]` label:
-            Filter by note type.
+        :param `Union[int, str]` idy:
 
-            Either: `ALL`, `NOTE`, `APPROVAL`, `REMOVAL`, `BAN`, `MUTE`,
-            `INVITE`, `SPAM`, `CONTENT_CHANGE`.
+        .. .RETURNS
+
+        :returns:
+            * :class:`~.models.user_summary.UserSummary`
+            * `None` if the user was not found.
+        :rtype: `Optional`\\[:class:`~.models.user_summary.UserSummary`]
+        """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        full_id36 = 't2_' + id36
+        try:
+            root = self._client.request('GET', '/api/user_data_by_account_ids',
+                    params={'ids': full_id36})
+        except http.exceptions.StatusCodeException as e:
+            if e.status_code == 404:
+                return None
+            raise
+        obj_data = root[full_id36]
+        return load_user_summary(obj_data, id36)
+
+    def bulk_fetch_user_summary(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingIterator[UserSummary]:
+        """
+        Bulk fetch partial user objects, by ID.
+
+        Any ID that can't be resolved will be ignored.
+        Duplicate IDs in a batch will be ignored.
+
+        .. .PARAMETERS
+
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
-        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.moderation.note_pulls_sync1.ModerationNotePaginator`, :class:`~.models.moderation_note.ModerationNote`]
+        :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[:class:`~.models.user_summary.UserSummary`]
+        """
+        def mass_fetch_by_id(ids: Sequence[_YIntOrStr]) -> Sequence[UserSummary]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
+            full_id36s = map('t2_'.__add__, id36s)
+            ids_str = ','.join(full_id36s)
 
-        .. .RAISES
+            try:
+                root = self._client.request('GET', '/api/user_data_by_account_ids', params={'ids': ids_str})
+            except http.exceptions.StatusCodeException as e:
+                if e.status_code == 404:
+                    return []
+                raise
+            return [load_user_summary(v, k) for k, v in root.items()]
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `BAD_SR_NAME`:
-                The `sr` parameter was empty.
-            + `SUBREDDIT_NOEXIST`:
-                The target subreddit does not exist.
-            + `USER_DOESNT_EXIST`:
-               - The specified user does not exist.
-               - The `user` parameter was empty.
-            + `INVALID_ID`:
-                An invalid value was specified for the `label` parameter.
-                Values are case-sensitive.
-        """
-        p = ModerationNotePaginator(
-            client=self._client,
-            url='/api/mod/notes',
-            subreddit=sr,
-            user=user,
-            type=label,
-        )
-        return ImpartedPaginatorChainingIterator(p, amount)
+        return CallChunkChainingIterator(CallChunk[Sequence[_YIntOrStr], Sequence[UserSummary]](mass_fetch_by_id, idfs) for idfs in chunked(ids, 100))
 
-    def pull_user_notes(self,
-        sr: str,
-        user: str,
-        amount: Optional[int] = None,
-    ) -> ImpartedPaginatorChainingIterator[ModerationUserNotePaginator, ModerationUserNote]:
-        """
-        Behaves similarly to :meth:`.pull_notes`.
-        """
-        p = ModerationUserNotePaginator(
-            client=self._client,
-            url='/api/mod/notes',
-            subreddit=sr,
-            user=user,
-            type='NOTE',
-        )
-        return ImpartedPaginatorChainingIterator(p, amount)
+    def moderating(self, name: str) -> Sequence[ModeratedSubreddit]:
+        """Get a list of partial subreddit objects the target user is a moderator of.
 
-    def get_latest_user_note(self, sr: str, user: str) -> Optional[ModerationUserNote]:
-        """Get the most recently written user note for some user.
+        This endpoint isn't very reliable on users with big lists.
+
+        The specified user's own user subreddit won't be returned, but any other user
+        subreddit they moderate will be.
+
+        .. seealso::
+
+           :meth:`p.account.pull_subreddits.moderating() <.pull_subreddits_SYNC.PullSubreddits.moderating>`
+              For obtaining a list of the current user's moderated subreddits.
 
         .. .PARAMETERS
 
-        :param `str` sr:
-        :param `str` user:
+        :param `str` name:
 
         .. .RETURNS
 
-        :rtype: `Optional`\\[:class:`~.models.moderation_note.ModerationUserNote`]
+        :rtype: `Sequence`\\[:class:`~.models.moderated_subreddit.ModeratedSubreddit`]
 
         .. .RAISES
 
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `PARAMETER_REQUIRED`:
-               - The `sr` parameter was empty.
-               - The `user` parameter was empty.
+        :raises redditwarp.http.exceptions.StatusCodeException:
+            + `404`:
+                The specified user was not found.
         """
-        params = {'subreddits': sr, 'users': user}
-        try:
-            root = self._client.request('GET', '/api/mod/notes/recent', params=params)
-        except http.exceptions.StatusCodeException as e:
-            if e.status_code == 400:
-                return None
-            raise
-        note_obj = root['mod_notes'][0]
-        if note_obj is None:
-            return None
-        return load_moderation_user_note(note_obj)
+        root = self._client.request('GET', f'/user/{name}/moderated_subreddits')
+        if not root:
+            return ()
+        return [load_moderated_subreddit(d) for d in root['data']]
+
+    def search(self, query: str, amount: Optional[int] = None,
+            ) -> ImpartedPaginatorChainingIterator[UserSearchPaginator, User]:
+        """Search users by name or description.
 
-    def bulk_get_latest_user_note(self, pairs: Iterable[tuple[str, str]]) -> CallChunkChainingIterator[Optional[ModerationUserNote]]:
-        """Bulk fetch the most recently written user notes for users.
+        .. .PARAMETERS
 
-        The response contains a list of mod notes in the order that subreddits and users were given.
-        If no note exists for a given pair, `None` will take its place in the list.
+        :param `str` query:
+        :param `Optional[int]` amount:
+
+        .. .RETURNS
+
+        :rtype: :class:`~.pagination.paginator_chaining_iterator.ImpartedPaginatorChainingIterator`\\[:class:`~.pagination.paginators.user.sync1.UserSearchPaginator`, :class:`~.models.user_SYNC.User`]
+        """
+        p = UserSearchPaginator(self._client, '/users/search', query)
+        return ImpartedPaginatorChainingIterator(p, amount)
+
+    def exists(self, name: str) -> bool:
+        """Check whether a user name exists.
 
         .. .PARAMETERS
 
-        :param `Iterable[tuple[str, str]]` pairs:
+        :param `str` name:
 
         .. .RETURNS
 
-        :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`Optional`\\[:class:`~.models.moderation_note.ModerationUserNote`]]
+        :rtype: `bool`
 
         .. .RAISES
 
-        :(raises): Same as :meth:`.get_latest_user_note`.
+        :raises redditwarp.exceptions.RedditError:
+            + `BAD_USERNAME`:
+                * The specified parameter is empty.
+                * The specified username contains illegal characters.
         """
-        def mass_get_latest_user_note(pairs: Sequence[tuple[str, str]]) -> Sequence[Optional[ModerationUserNote]]:
-            subreddits, users = tuple(zip(*pairs))
-            subreddits_str = ','.join(subreddits)
-            users_str = ','.join(users)
-            params = {'subreddits': subreddits_str, 'users': users_str}
-            try:
-                root = self._client.request('GET', '/api/mod/notes/recent', params=params)
-            except http.exceptions.StatusCodeException as e:
-                if e.status_code == 400:
-                    return [None]
-                raise
-            return [
-                (None if note_obj is None else load_moderation_user_note(note_obj))
-                for note_obj in root['mod_notes']
-            ]
-
-        return CallChunkChainingIterator(CallChunk(mass_get_latest_user_note, chunk) for chunk in chunked(pairs, 500))
+        return not self._client.request('GET', '/api/username_available', params={'user': name})
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_users_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_users_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/moderation/pull_users_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/moderation/pull_users_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/conversation_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/conversation_ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence, Iterable
+from typing import TYPE_CHECKING, Sequence, Iterable, Union, TypeVar, Protocol, cast
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
 
+from functools import cached_property
+
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_calling_async_iterator import CallChunkCallingAsyncIterator
 from ...iterators.call_chunk_chaining_async_iterator import CallChunkChainingAsyncIterator
 from ...iterators.async_call_chunk import AsyncCallChunk
 from ...models.modmail_ASYNC import (
     ConversationInfo,
@@ -20,24 +22,26 @@
     load_conversation_info,
     load_message,
     load_conversation_aggregate,
     load_user_dossier_conversation_aggregate,
     load_optional_user_dossier_conversation_aggregate,
 )
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class ConversationProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    async def fetch(self, idn: int, *, mark_read: bool = False) -> OptionalUserDossierConversationAggregate:
+    async def fetch(self, idy: Union[int, str], *, mark_read: bool = False) -> OptionalUserDossierConversationAggregate:
         """Get a conversation.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Conversation ID.
         :param `bool` mark_read:
             Mark retrieved conversations as read.
 
             Default: false.
 
         .. .RETURNS
@@ -50,16 +54,16 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `SUBREDDIT_NO_ACCESS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('GET', f'/api/mod/conversations/{convo_id36}')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('GET', f'/api/mod/conversations/{id36}')
         return load_optional_user_dossier_conversation_aggregate(
             root['conversation'],
             root['messages'],
             root['modActions'],
             root['user'] or None,
             client=self._client,
         )
@@ -114,20 +118,20 @@
         root = await self._client.request('POST', '/api/mod/conversations', data=data)
         conversation_data = root['conversation']
         conversation = load_conversation_info(conversation_data, self._client)
         message_id36 = conversation_data['objIds'][0]['id']
         message = load_message(root['messages'][message_id36], self._client)
         return (conversation, message)
 
-    async def reply(self, idn: int, body: str, *, hidden: bool = False, internal: bool = False) -> ConversationAggregate:
+    async def reply(self, idy: Union[int, str], body: str, *, hidden: bool = False, internal: bool = False) -> ConversationAggregate:
         """Create a new message on an existing conversation.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Conversation ID.
         :param `str` body:
             Markdown text.
         :param `bool` hidden:
             Expose your user name to the recipient.
 
             Default: false.
@@ -152,100 +156,149 @@
             + `NO_TEXT`:
                 The `body` was empty.
             + `TOO_LONG`:
                 The value specified for `body` must be 10000 characters or fewer
                 (despite error message saying under 10000).
         """
         data = {'body': body, 'isAuthorHidden': '01'[hidden], 'isInternal': '01'[internal]}
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}', data=data)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}', data=data)
         conversation_data = root['conversation']
         messages_mapping_data = root['messages']
         mod_actions_mapping_data = conversation_data['modActions']
         return load_conversation_aggregate(
             conversation_data,
             messages_mapping_data,
             mod_actions_mapping_data,
             client=self._client,
         )
 
-    async def mark_read(self, idn: int) -> None:
+    async def mark_read(self, idy: Union[int, str]) -> None:
         """Mark a conversation as read.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'conversationIds': to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'conversationIds': id36}
         await self._client.request('POST', '/api/mod/conversations/read', data=data)
 
-    def bulk_mark_read(self, ids: Iterable[int]) -> CallChunkCallingAsyncIterator[None]:
+    def bulk_mark_read(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingAsyncIterator[None]:
         """Mark conversations as read.
 
         Any specified conversation that does not exist will be ignored.
         If any of the IDs refer to a conversation you do not have permission over,
         an `INVALID_CONVERSATION_ID` API error will occur and none of the conversations
         will be processed.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_calling_async_iterator.CallChunkCallingAsyncIterator`\\[`None`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `INVALID_CONVERSATION_ID`:
                 You do not have permission to mark as read one of the specified conversations.
                 The operation is aborted and none of the items will be processed.
         """
-        async def mass_mark_read(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        # https://github.com/python/mypy/issues/13408
+        async def mass_mark_read(ids: Sequence[_YIntOrStr]) -> None:  # type: ignore[return]
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             ids_str = ','.join(id36s)
             await self._client.request('POST', '/api/mod/conversations/read', data={'conversationIds': ids_str})
 
-        return CallChunkCallingAsyncIterator(AsyncCallChunk(mass_mark_read, chunk) for chunk in chunked(ids, 100))
+        return CallChunkCallingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], None](mass_mark_read, chunk) for chunk in chunked(ids, 100))
 
-    async def mark_unread(self, idn: int) -> None:
+    async def mark_unread(self, idy: Union[int, str]) -> None:
         """Mark a conversation as unread.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        data = {'conversationIds': to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'conversationIds': id36}
         await self._client.request('POST', '/api/mod/conversations/unread', data=data)
 
-    def bulk_mark_unread(self, ids: Iterable[int]) -> CallChunkCallingAsyncIterator[None]:
+    def bulk_mark_unread(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingAsyncIterator[None]:
         """Mark conversations as unread.
 
         Behaves similarly to :meth:`.bulk_mark_read`.
         """
-        async def mass_mark_unread(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        # https://github.com/python/mypy/issues/13408
+        async def mass_mark_unread(ids: Sequence[_YIntOrStr]) -> None:  # type: ignore[return]
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             ids_str = ','.join(id36s)
             await self._client.request('POST', '/api/mod/conversations/unread', data={'conversationIds': ids_str})
 
-        return CallChunkCallingAsyncIterator(AsyncCallChunk(mass_mark_unread, chunk) for chunk in chunked(ids, 100))
+        return CallChunkCallingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], None](mass_mark_unread, chunk) for chunk in chunked(ids, 100))
+
+    class BulkMarkAllRead:
+        class GenericOverload(Protocol[_YIntOrStr]):
+            def __call__(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingAsyncIterator[_YIntOrStr]: ...
+
+        def __init__(self, outer: ConversationProcedures) -> None:
+            self._outer: ConversationProcedures = outer
+            self._client: Client = outer._client
+
+        def __call__(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingAsyncIterator[int]:
+            return self[int](mailbox, subrs)
+
+        def __getitem__(self, key: type[_YIntOrStr]) -> GenericOverload[_YIntOrStr]:
+            d = {
+                int: self.y_int,
+                str: self.y_str,
+            }
+            try:
+                v = d[key]
+            except KeyError as e:
+                raise TypeError from e
+            # https://github.com/python/mypy/issues/4177
+            return cast("__class__.GenericOverload[_YIntOrStr]", cast(object, v))  # type: ignore[name-defined]
+
+        async def __helper(self, mailbox: str, subrs: Sequence[str]) -> Sequence[str]:
+            subrs_str = ','.join(subrs)
+            data = {'state': mailbox, 'entity': subrs_str}
+            root = await self._client.request('POST', '/api/mod/conversations/bulk/read', data=data)
+            return root['conversation_ids']
+
+        def y_int(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingAsyncIterator[int]:
+            async def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[int]:
+                l = await self.__helper(mailbox, subrs)
+                return [int(id36, 36) for id36 in l]
 
-    def bulk_mark_all_read(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingAsyncIterator[int]:
-        """Mark all conversations across select mailboxes and subreddits as read.
+            return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[str], Sequence[int]](mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+
+        def y_str(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingAsyncIterator[str]:
+            async def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[str]:
+                return list(await self.__helper(mailbox, subrs))
+
+            return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[str], Sequence[str]](mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+
+    bulk_mark_all_read: cached_property[BulkMarkAllRead] = cached_property(BulkMarkAllRead)
+    ("""
+        Mark all conversations across select mailboxes and subreddits as read.
 
         Specified subreddit names that do not exist will be ignored, but if none of
         the subreddits exist then a 500 HTTP error will occur. If any of the subreddits
         are not moderated by you then a `BAD_SR_NAME` API error will occur, and none of
         the conversations will be processed.
 
         .. .PARAMETERS
@@ -257,39 +310,37 @@
             Defaults to `all` if empty string.
         :param `Iterable[str]` subrs:
             Subreddit names.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[`int`]
+        :returns:
+            For `_YIntOrStr` = `int`:
+                :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[`int`]
+            For `_YIntOrStr` = `str`:
+                :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[`str`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `INVALID_OPTION`
                 The specified `mailbox` was invalid.
             + `BAD_SR_NAME`:
                 One of the specified subreddits is not a subreddit you have access to.
-        """
-        async def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[int]:
-            subrs_str = ','.join(subrs)
-            data = {'state': mailbox, 'entity': subrs_str}
-            root = await self._client.request('POST', '/api/mod/conversations/bulk/read', data=data)
-            return [int(id36, 36) for id36 in root['conversation_ids']]
-
-        return CallChunkChainingAsyncIterator(AsyncCallChunk(mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+        """)
 
-    async def highlight(self, idn: int) -> ConversationAggregate:
+    async def highlight(self, idy: Union[int, str]) -> ConversationAggregate:
         """Mark a conversation as highlighted.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_ASYNC.ConversationAggregate`
 
         .. .RAISES
 
@@ -297,46 +348,46 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `SUBREDDIT_NO_ACCESS`:
                 The subreddit associated with the conversation is not moderated by you.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/highlight')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/highlight')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    async def unhighlight(self, idn: int) -> ConversationAggregate:
+    async def unhighlight(self, idy: Union[int, str]) -> ConversationAggregate:
         """Unmark a conversation as highlighted.
 
         Behaves similarly to :meth:`.highlight`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('DELETE', f'/api/mod/conversations/{convo_id36}/highlight')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('DELETE', f'/api/mod/conversations/{id36}/highlight')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    async def archive(self, idn: int) -> ConversationAggregate:
+    async def archive(self, idy: Union[int, str]) -> ConversationAggregate:
         """Archive a conversation.
 
         .. hint::
             Archiving a conversation moves it to the `archived` mailbox folder.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_ASYNC.ConversationAggregate`
 
         .. .RAISES
 
@@ -344,43 +395,43 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/archive')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/archive')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    async def unarchive(self, idn: int) -> ConversationAggregate:
+    async def unarchive(self, idy: Union[int, str]) -> ConversationAggregate:
         """Unmark a conversation as highlighted.
 
         Behaves similarly to :meth:`.highlight`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unarchive')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/unarchive')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    async def approve_user(self, idn: int) -> UserDossierConversationAggregate:
+    async def approve_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Approve the user associated with a conversation.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_ASYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -390,45 +441,45 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/approve')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/approve')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def unapprove_user(self, idn: int) -> UserDossierConversationAggregate:
+    async def unapprove_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unapprove the user associated with a conversation.
 
         Behaves similarly to :meth:`.approve_user`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/disapprove')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/disapprove')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def mute_user_3d(self, idn: int) -> UserDossierConversationAggregate:
+    async def mute_user_3d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 3 days.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_ASYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -438,77 +489,77 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '72'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '72'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def mute_user_7d(self, idn: int) -> UserDossierConversationAggregate:
+    async def mute_user_7d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 7 days.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '168'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '168'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def mute_user_28d(self, idn: int) -> UserDossierConversationAggregate:
+    async def mute_user_28d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 28 days.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '672'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '672'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def unmute_user(self, idn: int) -> UserDossierConversationAggregate:
+    async def unmute_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unmute the user associated with a conversation.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unmute')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/unmute')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def shorten_user_ban(self, idn: int, duration: int) -> UserDossierConversationAggregate:
+    async def shorten_user_ban(self, idy: Union[int, str], duration: int) -> UserDossierConversationAggregate:
         """Switch a permanent ban to a temporary one of the user associated with a conversation.
 
         If the user is not permanently banned, an API error will be raised.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` duration:
             The number of days the temporary ban should last.
 
             Specify an integer from 1 to 999.
 
             The UI has the options: 1, 3, 7, or 28 days.
 
@@ -530,31 +581,31 @@
             + `Participant must be banned.`:
                 The user associated with the conversation is not banned from the subreddit.
             + `Participant must be banned permanently.`:
                 The user associated with the conversation is not permanently banned from the subreddit.
             + `BAD_NUMBER`:
                 The number specified by the `duration` parameter was not in range.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/temp_ban',
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/temp_ban',
                 data={'duration': str(duration)})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    async def unban_user(self, idn: int) -> UserDossierConversationAggregate:
+    async def unban_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unban the user associated with a conversation from the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_ASYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -564,16 +615,16 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = await self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unban')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = await self._client.request('POST', f'/api/mod/conversations/{id36}/unban')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/conversation_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/conversation_SYNC.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence, Iterable
+from typing import TYPE_CHECKING, Sequence, Iterable, Union, TypeVar, Protocol, cast
 if TYPE_CHECKING:
     from ...client_SYNC import Client
 
+from functools import cached_property
+
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_calling_iterator import CallChunkCallingIterator
 from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
 from ...iterators.call_chunk import CallChunk
 from ...models.modmail_SYNC import (
     ConversationInfo,
@@ -20,24 +22,26 @@
     load_conversation_info,
     load_message,
     load_conversation_aggregate,
     load_user_dossier_conversation_aggregate,
     load_optional_user_dossier_conversation_aggregate,
 )
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class ConversationProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    def fetch(self, idn: int, *, mark_read: bool = False) -> OptionalUserDossierConversationAggregate:
+    def fetch(self, idy: Union[int, str], *, mark_read: bool = False) -> OptionalUserDossierConversationAggregate:
         """Get a conversation.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Conversation ID.
         :param `bool` mark_read:
             Mark retrieved conversations as read.
 
             Default: false.
 
         .. .RETURNS
@@ -50,16 +54,16 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `SUBREDDIT_NO_ACCESS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('GET', f'/api/mod/conversations/{convo_id36}')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('GET', f'/api/mod/conversations/{id36}')
         return load_optional_user_dossier_conversation_aggregate(
             root['conversation'],
             root['messages'],
             root['modActions'],
             root['user'] or None,
             client=self._client,
         )
@@ -114,20 +118,20 @@
         root = self._client.request('POST', '/api/mod/conversations', data=data)
         conversation_data = root['conversation']
         conversation = load_conversation_info(conversation_data, self._client)
         message_id36 = conversation_data['objIds'][0]['id']
         message = load_message(root['messages'][message_id36], self._client)
         return (conversation, message)
 
-    def reply(self, idn: int, body: str, *, hidden: bool = False, internal: bool = False) -> ConversationAggregate:
+    def reply(self, idy: Union[int, str], body: str, *, hidden: bool = False, internal: bool = False) -> ConversationAggregate:
         """Create a new message on an existing conversation.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Conversation ID.
         :param `str` body:
             Markdown text.
         :param `bool` hidden:
             Expose your user name to the recipient.
 
             Default: false.
@@ -152,100 +156,147 @@
             + `NO_TEXT`:
                 The `body` was empty.
             + `TOO_LONG`:
                 The value specified for `body` must be 10000 characters or fewer
                 (despite error message saying under 10000).
         """
         data = {'body': body, 'isAuthorHidden': '01'[hidden], 'isInternal': '01'[internal]}
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}', data=data)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}', data=data)
         conversation_data = root['conversation']
         messages_mapping_data = root['messages']
         mod_actions_mapping_data = conversation_data['modActions']
         return load_conversation_aggregate(
             conversation_data,
             messages_mapping_data,
             mod_actions_mapping_data,
             client=self._client,
         )
 
-    def mark_read(self, idn: int) -> None:
+    def mark_read(self, idy: Union[int, str]) -> None:
         """Mark a conversation as read.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'conversationIds': to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'conversationIds': id36}
         self._client.request('POST', '/api/mod/conversations/read', data=data)
 
-    def bulk_mark_read(self, ids: Iterable[int]) -> CallChunkCallingIterator[None]:
+    def bulk_mark_read(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingIterator[None]:
         """Mark conversations as read.
 
         Any specified conversation that does not exist will be ignored.
         If any of the IDs refer to a conversation you do not have permission over,
         an `INVALID_CONVERSATION_ID` API error will occur and none of the conversations
         will be processed.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_calling_iterator.CallChunkCallingIterator`\\[`None`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `INVALID_CONVERSATION_ID`:
                 You do not have permission to mark as read one of the specified conversations.
                 The operation is aborted and none of the items will be processed.
         """
-        def mass_mark_read(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        def mass_mark_read(ids: Sequence[_YIntOrStr]) -> None:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             ids_str = ','.join(id36s)
             self._client.request('POST', '/api/mod/conversations/read', data={'conversationIds': ids_str})
 
-        return CallChunkCallingIterator(CallChunk(mass_mark_read, chunk) for chunk in chunked(ids, 100))
+        return CallChunkCallingIterator(CallChunk[Sequence[_YIntOrStr], None](mass_mark_read, chunk) for chunk in chunked(ids, 100))
 
-    def mark_unread(self, idn: int) -> None:
+    def mark_unread(self, idy: Union[int, str]) -> None:
         """Mark a conversation as unread.
 
         Behaves similarly to :meth:`.mark_read`.
         """
-        data = {'conversationIds': to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'conversationIds': id36}
         self._client.request('POST', '/api/mod/conversations/unread', data=data)
 
-    def bulk_mark_unread(self, ids: Iterable[int]) -> CallChunkCallingIterator[None]:
+    def bulk_mark_unread(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingIterator[None]:
         """Mark conversations as unread.
 
         Behaves similarly to :meth:`.bulk_mark_read`.
         """
-        def mass_mark_unread(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        def mass_mark_unread(ids: Sequence[_YIntOrStr]) -> None:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             ids_str = ','.join(id36s)
             self._client.request('POST', '/api/mod/conversations/unread', data={'conversationIds': ids_str})
 
-        return CallChunkCallingIterator(CallChunk(mass_mark_unread, chunk) for chunk in chunked(ids, 100))
+        return CallChunkCallingIterator(CallChunk[Sequence[_YIntOrStr], None](mass_mark_unread, chunk) for chunk in chunked(ids, 100))
+
+    class BulkMarkAllRead:
+        class GenericOverload(Protocol[_YIntOrStr]):
+            def __call__(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingIterator[_YIntOrStr]: ...
+
+        def __init__(self, outer: ConversationProcedures) -> None:
+            self._outer: ConversationProcedures = outer
+            self._client: Client = outer._client
+
+        def __call__(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingIterator[int]:
+            return self[int](mailbox, subrs)
+
+        def __getitem__(self, key: type[_YIntOrStr]) -> GenericOverload[_YIntOrStr]:
+            d = {
+                int: self.y_int,
+                str: self.y_str,
+            }
+            try:
+                v = d[key]
+            except KeyError as e:
+                raise TypeError from e
+            # https://github.com/python/mypy/issues/4177
+            return cast("__class__.GenericOverload[_YIntOrStr]", cast(object, v))  # type: ignore[name-defined]
+
+        def __helper(self, mailbox: str, subrs: Sequence[str]) -> Sequence[str]:
+            subrs_str = ','.join(subrs)
+            data = {'state': mailbox, 'entity': subrs_str}
+            root = self._client.request('POST', '/api/mod/conversations/bulk/read', data=data)
+            return root['conversation_ids']
+
+        def y_int(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingIterator[int]:
+            def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[int]:
+                l = self.__helper(mailbox, subrs)
+                return [int(id36, 36) for id36 in l]
 
-    def bulk_mark_all_read(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingIterator[int]:
-        """Mark all conversations across select mailboxes and subreddits as read.
+            return CallChunkChainingIterator(CallChunk[Sequence[str], Sequence[int]](mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+
+        def y_str(self, mailbox: str, subrs: Iterable[str]) -> CallChunkChainingIterator[str]:
+            def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[str]:
+                return list(self.__helper(mailbox, subrs))
+
+            return CallChunkChainingIterator(CallChunk[Sequence[str], Sequence[str]](mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+
+    bulk_mark_all_read: cached_property[BulkMarkAllRead] = cached_property(BulkMarkAllRead)
+    ("""
+        Mark all conversations across select mailboxes and subreddits as read.
 
         Specified subreddit names that do not exist will be ignored, but if none of
         the subreddits exist then a 500 HTTP error will occur. If any of the subreddits
         are not moderated by you then a `BAD_SR_NAME` API error will occur, and none of
         the conversations will be processed.
 
         .. .PARAMETERS
@@ -257,39 +308,37 @@
             Defaults to `all` if empty string.
         :param `Iterable[str]` subrs:
             Subreddit names.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`int`]
+        :returns:
+            For `_YIntOrStr` = `int`:
+                :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`int`]
+            For `_YIntOrStr` = `str`:
+                :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`str`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
             + `INVALID_OPTION`
                 The specified `mailbox` was invalid.
             + `BAD_SR_NAME`:
                 One of the specified subreddits is not a subreddit you have access to.
-        """
-        def mass_mark_all_read(subrs: Sequence[str]) -> Sequence[int]:
-            subrs_str = ','.join(subrs)
-            data = {'state': mailbox, 'entity': subrs_str}
-            root = self._client.request('POST', '/api/mod/conversations/bulk/read', data=data)
-            return [int(id36, 36) for id36 in root['conversation_ids']]
-
-        return CallChunkChainingIterator(CallChunk(mass_mark_all_read, chunk) for chunk in chunked(subrs, 100))
+        """)
 
-    def highlight(self, idn: int) -> ConversationAggregate:
+    def highlight(self, idy: Union[int, str]) -> ConversationAggregate:
         """Mark a conversation as highlighted.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_SYNC.ConversationAggregate`
 
         .. .RAISES
 
@@ -297,46 +346,46 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `SUBREDDIT_NO_ACCESS`:
                 The subreddit associated with the conversation is not moderated by you.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/highlight')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/highlight')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    def unhighlight(self, idn: int) -> ConversationAggregate:
+    def unhighlight(self, idy: Union[int, str]) -> ConversationAggregate:
         """Unmark a conversation as highlighted.
 
         Behaves similarly to :meth:`.highlight`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('DELETE', f'/api/mod/conversations/{convo_id36}/highlight')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('DELETE', f'/api/mod/conversations/{id36}/highlight')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    def archive(self, idn: int) -> ConversationAggregate:
+    def archive(self, idy: Union[int, str]) -> ConversationAggregate:
         """Archive a conversation.
 
         .. hint::
             Archiving a conversation moves it to the `archived` mailbox folder.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_SYNC.ConversationAggregate`
 
         .. .RAISES
 
@@ -344,43 +393,43 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/archive')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/archive')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    def unarchive(self, idn: int) -> ConversationAggregate:
+    def unarchive(self, idy: Union[int, str]) -> ConversationAggregate:
         """Unmark a conversation as highlighted.
 
         Behaves similarly to :meth:`.highlight`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unarchive')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/unarchive')
         return load_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             client=self._client,
         )
 
-    def approve_user(self, idn: int) -> UserDossierConversationAggregate:
+    def approve_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Approve the user associated with a conversation.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_SYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -390,45 +439,45 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/approve')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/approve')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def unapprove_user(self, idn: int) -> UserDossierConversationAggregate:
+    def unapprove_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unapprove the user associated with a conversation.
 
         Behaves similarly to :meth:`.approve_user`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/disapprove')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/disapprove')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def mute_user_3d(self, idn: int) -> UserDossierConversationAggregate:
+    def mute_user_3d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 3 days.
 
         .. .PARAMETERS
 
-        :params `int` idn:
+        :params `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_SYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -438,77 +487,77 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '72'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '72'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def mute_user_7d(self, idn: int) -> UserDossierConversationAggregate:
+    def mute_user_7d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 7 days.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '168'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '168'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def mute_user_28d(self, idn: int) -> UserDossierConversationAggregate:
+    def mute_user_28d(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Mute the user associated with a conversation for 28 days.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/mute', data={'num_hours': '672'})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/mute', data={'num_hours': '672'})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def unmute_user(self, idn: int) -> UserDossierConversationAggregate:
+    def unmute_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unmute the user associated with a conversation.
 
         Behaves similarly to :meth:`.mute_user_3d`.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unmute')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/unmute')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def shorten_user_ban(self, idn: int, duration: int) -> UserDossierConversationAggregate:
+    def shorten_user_ban(self, idy: Union[int, str], duration: int) -> UserDossierConversationAggregate:
         """Switch a permanent ban to a temporary one of the user associated with a conversation.
 
         If the user is not permanently banned, an API error will be raised.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` duration:
             The number of days the temporary ban should last.
 
             Specify an integer from 1 to 999.
 
             The UI has the options: 1, 3, 7, or 28 days.
 
@@ -530,31 +579,31 @@
             + `Participant must be banned.`:
                 The user associated with the conversation is not banned from the subreddit.
             + `Participant must be banned permanently.`:
                 The user associated with the conversation is not permanently banned from the subreddit.
             + `BAD_NUMBER`:
                 The number specified by the `duration` parameter was not in range.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/temp_ban',
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/temp_ban',
                 data={'duration': str(duration)})
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
 
-    def unban_user(self, idn: int) -> UserDossierConversationAggregate:
+    def unban_user(self, idy: Union[int, str]) -> UserDossierConversationAggregate:
         """Unban the user associated with a conversation from the subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.modmail_SYNC.UserDossierConversationAggregate`
 
         .. .RAISES
 
@@ -564,16 +613,16 @@
             + `CONVERSATION_NOT_FOUND`:
                 The specified conversation does not exist.
             + `INVALID_MOD_PERMISSIONS`:
                 The subreddit associated with the conversation is not moderated by you.
             + `CANT_RESTRICT_MODERATOR`:
                 There is no user associated with the conversation.
         """
-        convo_id36 = to_base36(idn)
-        root = self._client.request('POST', f'/api/mod/conversations/{convo_id36}/unban')
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        root = self._client.request('POST', f'/api/mod/conversations/{id36}/unban')
         return load_user_dossier_conversation_aggregate(
             root['conversations'],
             root['messages'],
             root['modActions'],
             root['user'],
             client=self._client,
         )
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/pull_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/pull_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/modmail/pull_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/modmail/pull_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/ASYNC.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, IO, Mapping, Union
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, IO, Mapping, Union, TypeVar
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.submission_ASYNC import Submission, TextPost
     from ...models.comment_ASYNC import Comment
     from ...dtos.submission import GalleryItem
     from ...types import JSON_ro
 
 import os.path as op
 from functools import cached_property
 import json
 
 from ...model_loaders.submission_ASYNC import load_submission, load_text_post
-from ...models.media_upload_lease import MediaUploadLease
-from ...model_loaders.media_upload_lease import load_media_upload_lease
+from ...models.submission_media_upload_lease import SubmissionMediaUploadLease
+from ...model_loaders.submission_media_upload_lease import load_submission_media_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_calling_async_iterator import CallChunkCallingAsyncIterator
 from ...iterators.call_chunk_chaining_async_iterator import CallChunkChainingAsyncIterator
 from ...iterators.async_call_chunk import AsyncCallChunk
 from ...pagination.paginator_chaining_async_iterator import ImpartedPaginatorChainingAsyncIterator
 from ...pagination.paginators.submission_async1 import SubmissionSearchAsyncPaginator, SubmissionDuplicatesAsyncPaginator
 from ...model_loaders.comment_ASYNC import load_comment
 from .fetch_ASYNC import Fetch
 from .get_ASYNC import Get
+from .create.ASYNC import Create
+
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 
 class SubmissionProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.fetch: Fetch = Fetch(self, client)
         ("""
             Fetch a submission.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `Union[int, str]` idy:
                 Submission ID.
 
             .. .RETURNS
 
             :rtype: :class:`~.models.submission_ASYNC.Submission`
 
             .. .RAISES
@@ -50,51 +54,57 @@
             """)
         self.get: Get = Get(client)
         ("""
             Get a submission.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `Union[int, str]` idy:
                 Submission ID.
 
             .. .RETURNS
 
             :rtype: `Optional`\\[:class:`~.models.submission_ASYNC.Submission`]
             """)
+        self.create: Create = Create(client)
+        ("""
+            Create a submission.
+            """)
 
-    def bulk_fetch(self, ids: Iterable[int]) -> CallChunkChainingAsyncIterator[Submission]:
+    def bulk_fetch(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingAsyncIterator[Submission]:
         """Bulk fetch submissions.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
             Submission IDs.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[:class:`~.models.submission_ASYNC.Submission`]
         """
-        async def mass_fetch(ids: Sequence[int]) -> Sequence[Submission]:
-            id36s = map(to_base36, ids)
+        async def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[Submission]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = await self._client.request('GET', '/api/info', params={'id': ids_str})
-            return [load_submission(i['data'], self._client) for i in root['data']['children']]
+            # https://github.com/python/mypy/issues/13408
+            return [load_submission(i['data'], self._client) for i in root['data']['children']]  # type: ignore[return-value]
 
-        return CallChunkChainingAsyncIterator(AsyncCallChunk(mass_fetch, chunk) for chunk in chunked(ids, 100))
+        return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], Sequence[Submission]](mass_fetch, chunk) for chunk in chunked(ids, 100))
 
-    async def reply(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    async def reply(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Comment on a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_ASYNC.Comment`
@@ -102,15 +112,16 @@
         .. .RAISES
 
         :(raises):
             Same as comment :meth:`~.siteprocs.comment.SYNC.CommentProcedures.reply`
             but for submissions.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't3_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = await self._client.request('POST', '/api/comment', files=dict(g()))
@@ -121,44 +132,44 @@
             self._client = outer._client
 
         async def __call__(self,
             file: IO[bytes],
             *,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             return await self.upload(file, filepath=filepath, timeout=timeout)
 
         async def obtain_upload_lease(self,
             *,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = await self._client.request('POST', '/api/media/asset',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_media_upload_lease(result)
+            return load_submission_media_upload_lease(result)
 
         async def deposit_file(self,
             file: IO[bytes],
-            upload_lease: MediaUploadLease,
+            upload_lease: SubmissionMediaUploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = await self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         async def upload(self,
             file: IO[bytes],
             *,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = await self.obtain_upload_lease(filepath=filepath)
             await self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
@@ -179,106 +190,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a text post.
 
-        .. .PARAMETERS
-
-        :param `str` sr:
-            Name of the subreddit to submit the post to.
-        :param `str` title:
-            Title of the post.
-        :param body:
-            The body text of the post.
-
-            Specify either markdown text or a richtext document.
-        :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
-        :param `bool` reply_notifications:
-            Receive inbox notifications for replies.
-        :param `bool` spoiler:
-            Mark as spoiler.
-        :param `bool` nsfw:
-            Mark as NSFW.
-        :param `bool` oc:
-            Mark as original content.
-        :param `Optional[str]` collection_uuid:
-            The UUID of a collection to add this post to a collection.
-        :param `Optional[str]` flair_uuid:
-            The UUID of a flair template to use.
-        :param `Optional[str]` flair_text:
-            Custom flair text.
-        :param `Optional[str]` event_start:
-            A datetime ISO 8601 string. E.g. `2018-09-11T12:00:00`.
-        :param `Optional[str]` event_end:
-            A datetime ISO 8601 string.
-        :param `Optional[str]` event_tz:
-            A timezone. E.g., `America/Los_Angeles`.
-
-        .. .RETURNS
-
-        :returns: The ID of the newly created post.
-        :rtype: `int`
-
-        .. .RAISES
-
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `BAD_SR_NAME`:
-                An empty string was specified for `sr`.
-            + `SUBREDDIT_NOEXIST`:
-               - The specified subreddit does not exist.
-               - The specified subreddit is invalid.
-
-            + `SUBREDDIT_NOTALLOWED`:
-               - The subreddit is restricted and you are not an approved user.
-               - You are banned from the subreddit.
-               - You are trying to submit an image or video post to a NSFW subreddit.
-
-               Note, quarantined subreddits can be posted to even if you haven't
-               yet opt-ed in to viewing its content.
-            + `NO_TEXT`:
-                The `title` parameter was not specified, was blank, or contained only whitespace.
-            + `JSON_PARSE_ERROR`:
-                Richtext was passed and it was not in the correct format.
-            + `TOO_LONG`:
-               - The `title` parameter must be under 300 characters.
-               - The `body` parameter must be under 40000 characters.
-
-            + `NO_SELFS`:
-                The subreddit doesn't accept text posts.
-            + `USER_REQUIRED`:
-                There is no user context.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `404`:
-                The target subreddit is private or banned.
+        Alias of `self.create.text[int]()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'self')
-            yield ('sr', sr)
-            yield ('title', title)
-            if isinstance(body, str):
-                yield ('text', body)
-            else:
-                yield ('richtext_json', json.dumps(body))
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = await self._client.request('POST', '/api/submit', files=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return await self.create.text[int](
+            sr=sr,
+            title=title,
+            body=body,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     async def create_link_post(self,
         sr: str,
         title: str,
         link: str,
         *,
         reply_notifications: bool = True,
@@ -291,61 +227,32 @@
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
         resubmit: bool = True,
     ) -> int:
         """Create a link post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` url:
-            A URL.
-        :param `bool` resubmit:
-            When the "Restrict how often the same link can be posted" content control
-            setting is enabled, if a link with the same URL has already been submitted
-            then an `ALREADY_SUB` API error would be returned unless this field is true.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
-
-        :raises redditwarp.exceptions.RedditError:
-            + `NO_URL`:
-                The `link` parameter was not specified, or the URL is invalid.
-            + `ALREADY_SUB`:
-                The given link has already been submitted to the subreddit.
-                See parameter `resubmit`.
+        Alias of `self.create.link[int]()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'link')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            if resubmit: yield ('resubmit', '1')
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = await self._client.request('POST', '/api/submit', data=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return await self.create.link[int](
+            sr=sr,
+            title=title,
+            link=link,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+            resubmit=resubmit,
+        )
 
     async def create_image_post(self,
         sr: str,
         title: str,
         link: str,
         *,
         reply_notifications: bool = True,
@@ -357,48 +264,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> None:
         """Create an image post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` link:
-            A URL to an image.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.image()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'image')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        await self._client.request('POST', '/api/submit', data=dict(g()))
+        return await self.create.image(
+            sr=sr,
+            title=title,
+            link=link,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     async def create_video_post(self,
         sr: str,
         title: str,
         link: str,
         thumbnail: str,
         *,
@@ -412,59 +302,33 @@
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
         vgif: bool = False,
     ) -> None:
         """Create a video post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` link:
-            A URL to a video.
-        :param `str` thumbnail:
-            A URL to an image to be used as a thumbnail for the video.
-        :param `bool` vgif:
-            Pass `True` to create a video GIF.
-
-        .. .RETURNS
-
-        :rtype: `None`
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
-
-        :raises redditwarp.exceptions.RedditError:
-            + `MISSING_VIDEO_URLS`:
-                The `thumbnail` parameter was empty.
-            + `NO_VIDEOS`:
-                The subreddit does not accept video posts.
+        Alias of `self.create.video()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'video' + ('gif' if vgif else ''))
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            yield ('video_poster_url', thumbnail)
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        await self._client.request('POST', '/api/submit', data=dict(g()))
+        return await self.create.video(
+            sr=sr,
+            title=title,
+            link=link,
+            thumbnail=thumbnail,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+            vgif=vgif,
+        )
 
     async def create_gallery_post(self,
         sr: str,
         title: str,
         items: Sequence[GalleryItem],
         *,
         reply_notifications: bool = True,
@@ -476,58 +340,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a gallery post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param items:
-            A list of gallery items.
-        :type items: `Sequence`\\[:class:`~.dtos.submission.GalleryItem`]
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.gallery[int]()`.
         """
-        gallery_items: list[dict[str, str]] = [
-            {
-                'media_id': m.media_id,
-                'caption': m.caption,
-                'outbound_url': m.outbound_link,
-            }
-            for m in items
-        ]
-
-        def g() -> Iterable[tuple[str, JSON_ro]]:
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('items', gallery_items)
-            yield ('sendreplies', reply_notifications)
-            if spoiler: yield ('spoiler', True)
-            if nsfw: yield ('nsfw', True)
-            if oc: yield ('original_content', True)
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = await self._client.request('POST', '/api/submit_gallery_post', json=dict(g()))
-        return int(root['json']['data']['id'][3:], 36)
+        return await self.create.gallery[int](
+            sr=sr,
+            title=title,
+            items=items,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     async def create_poll_post(self,
         sr: str,
         title: str,
         body: str,
         options: Sequence[str],
         duration: int,
@@ -540,117 +377,111 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a poll post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` body:
-        :param `Sequence[str]` options:
-        :param `int` duration:
-            The number of days the poll runs for.
-
-            Valid values are 1 to 7. If a number is specified outside
-            this range it is clamped within range.
-
-            The UI default is 3 days.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.poll[int]()`.
         """
-        def g() -> Iterable[tuple[str, JSON_ro]]:
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('text', body)
-            yield ('options', options)
-            yield ('duration', duration)
-            yield ('sendreplies', reply_notifications)
-            if spoiler: yield ('spoiler', True)
-            if nsfw: yield ('nsfw', True)
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = await self._client.request('POST', '/api/submit_poll_post', json=dict(g()))
-        return int(root['json']['data']['id'][3:], 36)
+        return await self.create.poll[int](
+            sr=sr,
+            title=title,
+            body=body,
+            options=options,
+            duration=duration,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     async def create_crosspost(self,
         sr: str,
         title: str,
-        idn: int,
+        target: Union[int, str],
         *,
         reply_notifications: bool = True,
         spoiler: bool = False,
         nsfw: bool = False,
         oc: bool = False,
         collection_uuid: Optional[str] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a crosspost.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `int` idn:
-            The ID of a submission.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.cross[int]()`.
+        """
+        return await self.create.cross[int](
+            sr=sr,
+            title=title,
+            target=target,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
-        .. .RAISES
+    async def create_cross_post(self,
+        sr: str,
+        title: str,
+        target: Union[int, str],
+        *,
+        reply_notifications: bool = True,
+        spoiler: bool = False,
+        nsfw: bool = False,
+        oc: bool = False,
+        collection_uuid: Optional[str] = None,
+        flair_uuid: Optional[str] = None,
+        flair_text: Optional[str] = None,
+        event_start: Optional[str] = None,
+        event_end: Optional[str] = None,
+        event_tz: Optional[str] = None,
+    ) -> int:
+        """Alias of :meth:`.create_crosspost`.
 
-        :(raises): Similar to :meth:`.create_text_post`.
+        .. versionadded:: 1.1.0
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'self')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('crosspost_parent', 't3_' + to_base36(idn))
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = await self._client.request('POST', '/api/submit', data=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return await self.create_crosspost(
+            sr,
+            title,
+            target,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
-    async def edit_text_post_body(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> TextPost:
+    async def edit_text_post_body(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> TextPost:
         """Edit the body text of a text post.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.submission_ASYNC.TextPost`
@@ -658,109 +489,113 @@
         .. .RAISES
 
         :raises:
             Same as comment :meth:`~.siteprocs.comment.SYNC.CommentProcedures.edit_body`
             but for submissions.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't3_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = await self._client.request('POST', '/api/editusertext', files=dict(g()))
         return load_text_post(result, self._client)
 
-    async def delete(self, idn: int) -> None:
+    async def delete(self, idy: Union[int, str]) -> None:
         """Delete a submission.
 
         If the target doesn't exist or isn't valid, nothing happens.
 
         When a submission is deleted it's text content (if a text post)
         will be set to "`[deleted]`" and the submission will be unlisted
         from its subreddit. Users can still otherwise view and reply to
         deleted to submissions if they have a direct link to it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/del', data=data)
 
-    async def lock(self, idn: int) -> None:
+    async def lock(self, idy: Union[int, str]) -> None:
         """Lock a submission.
 
         Nothing happens if the target is already locked.
 
         .. hint::
            Locking prevents a submission/comment from receiving new comments.
            A locked submission is unable to receive any new comments.
            Locking a comment only stops direct comments, but
            existing child comments can still receive replies.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target doesn't exist or you don't have permission to lock it.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/lock', data=data)
 
-    async def unlock(self, idn: int) -> None:
+    async def unlock(self, idy: Union[int, str]) -> None:
         """Unlock a submission.
 
         Behaves similarly to :meth:`.lock`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises:
             Similar to :meth:`.lock`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/unlock', data=data)
 
-    async def vote(self, idn: int, direction: int) -> None:
+    async def vote(self, idy: Union[int, str], direction: int) -> None:
         """Cast a vote on a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` direction:
             Either: `1` (upvote), `0` unvote, `-1` downvote.
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -769,26 +604,27 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'dir': str(direction),
         }
         await self._client.request('POST', '/api/vote', data=data)
 
-    async def save(self, idn: int, category: Optional[str] = None) -> None:
+    async def save(self, idy: Union[int, str], category: Optional[str] = None) -> None:
         """Save a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` category:
             A category/label.
 
             Requires Reddit Premium. Ignored if no Reddit Premium.
 
         .. .RETURNS
 
@@ -799,191 +635,201 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The category name specified was invalid.
         """
-        data = {
-            'id': 't3_' + to_base36(idn),
-        }
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         if category is not None:
             data['category'] = category
         await self._client.request('POST', '/api/save', data=data)
 
-    async def unsave(self, idn: int) -> None:
+    async def unsave(self, idy: Union[int, str]) -> None:
         """Save a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/unsave', data=data)
 
-    async def hide(self, idn: int) -> None:
+    async def hide(self, idy: Union[int, str]) -> None:
         """Hide a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 The target was not found.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/hide', data=data)
 
-    async def unhide(self, idn: int) -> None:
+    async def unhide(self, idy: Union[int, str]) -> None:
         """Unhide a submission.
 
         See :meth:`.hide`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/unhide', data=data)
 
-    def bulk_hide(self, ids: Iterable[int]) -> CallChunkCallingAsyncIterator[None]:
+    def bulk_hide(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingAsyncIterator[None]:
         """Bulk hide submissions.
 
         If *any* of the list of submission IDs don't exist then the endpoint will
         return a HTTP 400 status error and none of the submissions will be hidden.
         This can be annoying since if the list is long it can be hard to tell which
         ID is the culprit.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_calling_async_iterator.CallChunkCallingAsyncIterator`\\[`None`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 If any of the IDs were not found.
         """
-        async def mass_hide(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        # https://github.com/python/mypy/issues/13408
+        async def mass_hide(ids: Sequence[_YIntOrStr]) -> None:  # type: ignore[return]
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             await self._client.request('POST', '/api/hide', data={'id': ids_str})
 
-        return CallChunkCallingAsyncIterator(AsyncCallChunk(mass_hide, chunk) for chunk in chunked(ids, 300))
+        return CallChunkCallingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], None](mass_hide, chunk) for chunk in chunked(ids, 300))
 
-    def bulk_unhide(self, ids: Iterable[int]) -> CallChunkCallingAsyncIterator[None]:
+    def bulk_unhide(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingAsyncIterator[None]:
         """Bulk hide submissions.
 
         See :meth:`.bulk_hide`.
         """
-        async def mass_unhide(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        # https://github.com/python/mypy/issues/13408
+        async def mass_unhide(ids: Sequence[_YIntOrStr]) -> None:  # type: ignore[return]
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             await self._client.request('POST', '/api/unhide', data={'id': ids_str})
 
-        return CallChunkCallingAsyncIterator(AsyncCallChunk(mass_unhide, chunk) for chunk in chunked(ids, 300))
+        return CallChunkCallingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], None](mass_unhide, chunk) for chunk in chunked(ids, 300))
 
-    async def mark_nsfw(self, idn: int) -> None:
+    async def mark_nsfw(self, idy: Union[int, str]) -> None:
         """Mark a submission as NSFW.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to mark the target.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/marknsfw', data=data)
 
-    async def unmark_nsfw(self, idn: int) -> None:
+    async def unmark_nsfw(self, idy: Union[int, str]) -> None:
         """Unmark a submission as NSFW.
 
         See :meth:`.mark_nsfw`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/unmarknsfw', data=data)
 
-    async def mark_spoiler(self, idn: int) -> None:
+    async def mark_spoiler(self, idy: Union[int, str]) -> None:
         """Mark a submission as spoiler.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to mark the target.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/spoiler', data=data)
 
-    async def unmark_spoiler(self, idn: int) -> None:
+    async def unmark_spoiler(self, idy: Union[int, str]) -> None:
         """Unmark a submission as spoiler.
 
         See :meth:`.mark_spoiler`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/unspoiler', data=data)
 
-    async def distinguish(self, idn: int) -> Submission:
+    async def distinguish(self, idy: Union[int, str]) -> Submission:
         """Distinguish a submission.
 
         .. hint::
 
            Distinguishing decoratates the author's name by
            giving it a different color and putting a sigil beside it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target submission.
         :rtype: :class:`~.models.submission_ASYNC.Submission`
 
         .. .RAISES
@@ -993,27 +839,28 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'how': 'yes',
         }
         root = await self._client.request('POST', '/api/distinguish', data=data)
         return load_submission(root['json']['data']['things'][0]['data'], self._client)
 
-    async def undistinguish(self, idn: int) -> Submission:
+    async def undistinguish(self, idy: Union[int, str]) -> Submission:
         """Undistinguish a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target submission.
         :rtype: :class:`~.models.submission_ASYNC.Submission`
 
         .. .RAISES
@@ -1023,22 +870,23 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'how': 'no',
         }
         root = await self._client.request('POST', '/api/distinguish', data=data)
         return load_submission(root['json']['data']['things'][0]['data'], self._client)
 
-    async def sticky(self, idn: int, slot: Optional[int] = None) -> None:
+    async def sticky(self, idy: Union[int, str], slot: Optional[int] = None) -> None:
         """Set a submission as sticky in its subreddit.
 
         .. hint::
            Stickied posts are shown at the top of the subreddit in the default 'Hot' listing.
 
         In a subreddit, there can be at most 2 sticked posts at a time.
 
@@ -1051,15 +899,15 @@
         Unstickying a post that isn't stickied does nothing.
 
         .. note::
            You cannot reorder sticky posts directly. You must unsticky and re-sticky them.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` slot:
             Which sticky slot to use.
 
             If not specified, the bottom-most slot will be used if available.
             If the sticky list is at maximum length, the bottom-most slot will
             be replaced with the new post.
 
@@ -1074,36 +922,38 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to sticky that post.
             + `409`:
                 The post is already stickied.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '1',
         }
         if slot is not None:
             data['num'] = str(slot)
         await self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    async def unsticky(self, idn: int) -> None:
+    async def unsticky(self, idy: Union[int, str]) -> None:
         """Unsticky a submission.
 
         See :meth:`.sticky`.
 
         Unstickying a post that isn't stickied does nothing.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '0',
         }
         await self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    async def pin_to_profile(self, idn: int, slot: Optional[int] = None) -> None:
+    async def pin_to_profile(self, idy: Union[int, str], slot: Optional[int] = None) -> None:
         """Pin a post you created to your user profile.
 
         .. hint::
            Pinned posts show up at the start of the
            'Overview', or 'Submitted' (old UI) / 'POSTS' (redesign UI)
            user profile listings.
 
@@ -1128,15 +978,15 @@
         Unpinning a post that isn't pinned does nothing.
 
         .. note::
            You cannot reorder pinned posts directly. You must unpin and re-pin them.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` slot:
             Which pin slot to use.
 
             If `slot` is not specified, the new post is inserted at the top of the list.
             If the list is at maximum length, the least recently pinned post will be evicted.
             It acts like a queue.
 
@@ -1151,48 +1001,50 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to pin that post.
             + `409`:
                 The post is already pinned.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'to_profile': '1',
             'state': '1',
         }
         if slot is not None:
             data['num'] = str(slot)
         await self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    async def unpin_from_profile(self, idn: int) -> None:
+    async def unpin_from_profile(self, idy: Union[int, str]) -> None:
         """Unpin a submission from your user profile.
 
         See :meth:`.pin_to_profile`.
 
         Unpinning a post that isn't pinned does nothing.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'to_profile': '1',
             'state': '0',
         }
         await self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    async def set_contest_mode(self, idn: int, state: bool) -> None:
+    async def set_contest_mode(self, idy: Union[int, str], state: bool) -> None:
         """Set or unset 'contest mode' for a submission's comments.
 
         .. hint::
 
             In contest mode, vote counts are hidden and comments are displayed
             in a random order.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `bool` state:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1201,31 +1053,32 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The specified ID was not found.
                - You do not have permission to modify the target.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '01'[state],
         }
         await self._client.request('POST', '/api/set_contest_mode', data=data)
 
-    async def set_suggested_sort(self, idn: int, sort: str) -> None:
+    async def set_suggested_sort(self, idy: Union[int, str], sort: str) -> None:
         """Set or unset the suggested sort for a submission's comments.
 
         .. hint::
 
            When set, users will see comments in the suggested sort order by default.
            They can still manually change back to their preferred sort if they choose.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `str` sort:
             Either: `confidence`, `top`, `new`, `controversial`,
             `old`, `random`, `qa`, `live`, `blank`.
 
             If not specified or an unknown value, the suggested sort will be unset.
 
         .. .RETURNS
@@ -1238,67 +1091,70 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The specified ID was not found.
                - You do not have permission to modify the target.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'sort': sort,
         }
         await self._client.request('POST', '/api/set_suggested_sort', data=data)
 
-    async def enable_reply_notifications(self, idn: int) -> None:
+    async def enable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Enable inbox reply notifications for a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '1'
         }
         await self._client.request('POST', '/api/sendreplies', data=data)
 
-    async def disable_reply_notifications(self, idn: int) -> None:
+    async def disable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Disable inbox reply notifications for a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '0'
         }
         await self._client.request('POST', '/api/sendreplies', data=data)
 
-    async def set_event_time(self, idn: int,
+    async def set_event_time(self, idy: Union[int, str],
             event_start: Optional[str] = None,
             event_end: Optional[str] = None,
             event_tz: Optional[str] = None) -> None:
         """Add or modify event times on a submission.
 
         Specify only `event_start` to change only the starting date.
         The same cannot be done for `event_end`, a 500 HTTP error will occur.
@@ -1307,15 +1163,15 @@
         `event_end` in time, otherwise a `MIN_EVENT_TIME` API error is returned.
         It is possible however to make a second request specifying only `event_start` to modify
         the start date so that `event_start` is after `event_end`. If this happens then the time
         difference can be longer than 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` event_start:
             A datetime ISO 8601 string. E.g. `2018-09-11T12:00:00`.
         :param `Optional[str]` event_end:
             A datetime ISO 8601 string.
         :param `Optional[str]` event_tz:
             A timezone. E.g., `America/Los_Angeles`.
 
@@ -1343,30 +1199,31 @@
             + `INVALID_TIMEZONE`:
                 The value specified for `event_tz` is invalid.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `500`:
                 The `event_start` parameter was not specified.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('id', 't3_' + id36)
             if event_start: yield ('event_start', event_start)
             if event_end: yield ('event_end', event_end)
             if event_tz: yield ('event_tz', event_tz)
 
         await self._client.request('POST', '/api/event_post_time', data=dict(g()))
 
-    async def follow_event(self, idn: int) -> None:
+    async def follow_event(self, idy: Union[int, str]) -> None:
         """Follow a post event.
 
         .. hint::
            Followers receive a push notification when the event starts.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1375,37 +1232,39 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target submission is not an event.
             + `404`:
                 The target submission does not exist.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'fullname': 't3_' + to_base36(idn),
+            'fullname': 't3_' + id36,
             'follow': '1',
         }
         await self._client.request('POST', '/api/follow_post', data=data)
 
-    async def unfollow_event(self, idn: int) -> None:
+    async def unfollow_event(self, idy: Union[int, str]) -> None:
         """Unfollow a post event.
 
         See :meth:`.follow_event`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'fullname': 't3_' + to_base36(idn),
+            'fullname': 't3_' + id36,
             'follow': '0',
         }
         await self._client.request('POST', '/api/follow_post', data=data)
 
-    async def approve(self, idn: int) -> None:
+    async def approve(self, idy: Union[int, str]) -> None:
         """Approve a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1415,25 +1274,26 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         await self._client.request('POST', '/api/approve', data=data)
 
-    async def remove(self, idn: int) -> None:
+    async def remove(self, idy: Union[int, str]) -> None:
         """Remove a submission.
 
         This is a moderator action.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1443,43 +1303,45 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'spam': '0',
         }
         await self._client.request('POST', '/api/remove', data=data)
 
-    async def remove_spam(self, idn: int) -> None:
+    async def remove_spam(self, idy: Union[int, str]) -> None:
         """Remove as spam.
 
         See :meth:`.remove`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'spam': '1',
         }
         await self._client.request('POST', '/api/remove', data=data)
 
-    async def ignore_reports(self, idn: int) -> None:
+    async def ignore_reports(self, idy: Union[int, str]) -> None:
         """Ignore reports on a submission.
 
         .. hint::
            If you ignore reports, you won't receive notifications and the
            ignored thing will be absent from moderation listings.
 
         Nothing happens if the target is already ignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1488,24 +1350,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        await self._client.request('POST', '/api/ignore_reports', data={'id': 't3_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        await self._client.request('POST', '/api/ignore_reports', data={'id': 't3_' + id36})
 
-    async def unignore_reports(self, idn: int) -> None:
+    async def unignore_reports(self, idy: Union[int, str]) -> None:
         """Unignore reports on a submission.
 
         Nothing happens if the target is already unignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1514,22 +1377,23 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        await self._client.request('POST', '/api/unignore_reports', data={'id': 't3_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        await self._client.request('POST', '/api/unignore_reports', data={'id': 't3_' + id36})
 
-    async def snooze_reports(self, idn: int, reason: str) -> None:
+    async def snooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Ignore a custom report reason in a subreddit for 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
         :param `str` reason:
             The custom report reason to snooze.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -1540,36 +1404,38 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't3_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36, 'reason': reason}
         await self._client.request('POST', '/api/snooze_reports', data=data)
 
-    async def unsnooze_reports(self, idn: int, reason: str) -> None:
+    async def unsnooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Unsnooze a custom report.
 
         See :meth:`.snooze_reports`.
         """
-        data = {'id': 't3_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36, 'reason': reason}
         await self._client.request('POST', '/api/unsnooze_reports', data=data)
 
     async def apply_removal_reason(self,
-            idn: int,
+            idy: Union[int, str],
             reason_id: Optional[str] = None,
             note: Optional[str] = None) -> None:
         """Set a removal reason on a removed submission.
 
         If the target is not a removed submission, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
         :param `Optional[int]` reason_id:
             A removal reason ID.
         :param `Optional[str]` note:
             A note.
 
         .. .RETURNS
@@ -1590,20 +1456,20 @@
                 The reason ID is invalid.
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't3_' + to_base36(idn)
-        json_data = {'item_ids': [target], 'reason_id': reason_id, 'mod_note': note}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        json_data = {'item_ids': ['t3_' + id36], 'reason_id': reason_id, 'mod_note': note}
         await self._client.request('POST', '/api/v1/modactions/removal_reasons', json=json_data)
 
     async def send_removal_comment(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False,
             locked: bool = False) -> Comment:
         """Send a removal comment.
 
@@ -1613,15 +1479,15 @@
         (The UI does not normally let you do this.)
 
         Unlike :meth:`.apply_removal_reason`, the target you specify must be a
         removed item otherwise an `INVALID_ID` API error is produced.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed submission.
         :param `str` title:
             A title.
 
             This is ultimately unused for removal comments, but a non-empty
             string must be specified or you'll get a `NO_TEXT` API error.
 
@@ -1657,38 +1523,38 @@
 
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't3_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'public' + ('' if exposed else '_as_subreddit'),
-            'item_id': [target],
+            'item_id': ['t3_' + id36],
             'title': title,
             'message': message,
             'lock_comment': '01'[locked],
         }
         root = await self._client.request('POST', '/api/v1/modactions/removal_link_message', json=json_data)
         return load_comment(root, self._client)
 
     async def send_removal_message(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False) -> None:
         """Send a removal message.
 
         Behaves similarly to :meth:`.send_removal_comment`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             A non-empty string must be specified or you'll get a `NO_TEXT` API error.
 
             The UI sends the title of the selected removal reason.
@@ -1705,18 +1571,18 @@
 
         :returns: `None`
 
         .. .RAISES
 
         :(raises): See :meth:`.send_removal_comment`.
         """
-        target = 't3_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'private' + ('_exposed' if exposed else ''),
-            'item_id': [target],
+            'item_id': ['t3_' + id36],
             'title': title,
             'message': message,
         }
         await self._client.request('POST', '/api/v1/modactions/removal_link_message', json=json_data)
 
     def search(self, sr: str, query: str, amount: Optional[int] = None, *,
         sort: str = 'relevance', time: str = 'all',
@@ -1751,22 +1617,22 @@
             url = f'/r/{sr}/search'
         p = SubmissionSearchAsyncPaginator(
                 self._client, url,
                 params={'q': query, 'restrict_sr': '1'},
                     sort=sort, time=time)
         return ImpartedPaginatorChainingAsyncIterator(p, amount)
 
-    def duplicates(self, target: int, amount: Optional[int] = None, *,
+    def duplicates(self, target: Union[int, str], amount: Optional[int] = None, *,
         sort: str = 'num_comments',
     ) -> ImpartedPaginatorChainingAsyncIterator[SubmissionDuplicatesAsyncPaginator, Submission]:
         """Get crossposts for a submission.
 
         .. .PARAMETERS
 
-        :param `int` target:
+        :param `Union[int, str]` target:
             Submission ID.
         :param `Optional[int]` amount:
             The number of items to retrieve.
         :param `str` sort:
             Either `num_comments` or `new`.
 
             Default: `num_comments`.
@@ -1779,10 +1645,10 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 Fetching some submissions resulted in a 403.
             + `404`:
                 The target submission could not be found.
         """
-        subm_id = to_base36(target)
-        p = SubmissionDuplicatesAsyncPaginator(self._client, f'/duplicates/{subm_id}', sort=sort)
+        id36 = x if isinstance((x := target), str) else to_base36(x)
+        p = SubmissionDuplicatesAsyncPaginator(self._client, f'/duplicates/{id36}', sort=sort)
         return ImpartedPaginatorChainingAsyncIterator(p, amount)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/SYNC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence, Iterable, IO, Mapping, Union
+from typing import TYPE_CHECKING, Optional, Sequence, Iterable, IO, Mapping, Union, TypeVar
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.submission_SYNC import Submission, TextPost
     from ...models.comment_SYNC import Comment
     from ...dtos.submission import GalleryItem
     from ...types import JSON_ro
 
 import os.path as op
 from functools import cached_property
 import json
 
 from ...model_loaders.submission_SYNC import load_submission, load_text_post
-from ...models.media_upload_lease import MediaUploadLease
-from ...model_loaders.media_upload_lease import load_media_upload_lease
+from ...models.submission_media_upload_lease import SubmissionMediaUploadLease
+from ...model_loaders.submission_media_upload_lease import load_submission_media_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 from ...util.base_conversion import to_base36
 from ...iterators.chunking import chunked
 from ...iterators.call_chunk_calling_iterator import CallChunkCallingIterator
 from ...iterators.call_chunk_chaining_iterator import CallChunkChainingIterator
 from ...iterators.call_chunk import CallChunk
 from ...pagination.paginator_chaining_iterator import ImpartedPaginatorChainingIterator
 from ...pagination.paginators.submission_sync1 import SubmissionSearchPaginator, SubmissionDuplicatesPaginator
 from ...model_loaders.comment_SYNC import load_comment
 from .fetch_SYNC import Fetch
 from .get_SYNC import Get
+from .create.SYNC import Create
+
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 
 class SubmissionProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.fetch: Fetch = Fetch(self, client)
         ("""
             Fetch a submission.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `Union[int, str]` idy:
                 Submission ID.
 
             .. .RETURNS
 
             :rtype: :class:`~.models.submission_SYNC.Submission`
 
             .. .RAISES
@@ -50,51 +54,56 @@
             """)
         self.get: Get = Get(client)
         ("""
             Get a submission.
 
             .. .PARAMETERS
 
-            :param `int` idn:
+            :param `Union[int, str]` idy:
                 Submission ID.
 
             .. .RETURNS
 
             :rtype: `Optional`\\[:class:`~.models.submission_SYNC.Submission`]
             """)
+        self.create: Create = Create(client)
+        ("""
+            Create a submission.
+            """)
 
-    def bulk_fetch(self, ids: Iterable[int]) -> CallChunkChainingIterator[Submission]:
+    def bulk_fetch(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingIterator[Submission]:
         """Bulk fetch submissions.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
             Submission IDs.
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[:class:`~.models.submission_SYNC.Submission`]
         """
-        def mass_fetch(ids: Sequence[int]) -> Sequence[Submission]:
-            id36s = map(to_base36, ids)
+        def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[Submission]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = self._client.request('GET', '/api/info', params={'id': ids_str})
             return [load_submission(i['data'], self._client) for i in root['data']['children']]
 
-        return CallChunkChainingIterator(CallChunk(mass_fetch, chunk) for chunk in chunked(ids, 100))
+        return CallChunkChainingIterator(CallChunk[Sequence[_YIntOrStr], Sequence[Submission]](mass_fetch, chunk) for chunk in chunked(ids, 100))
 
-    def reply(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
+    def reply(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> Comment:
         """Comment on a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.comment_SYNC.Comment`
@@ -102,15 +111,16 @@
         .. .RAISES
 
         :(raises):
             Same as comment :meth:`~.siteprocs.comment.SYNC.CommentProcedures.reply`
             but for submissions.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't3_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = self._client.request('POST', '/api/comment', files=dict(g()))
@@ -121,44 +131,44 @@
             self._client = outer._client
 
         def __call__(self,
             file: IO[bytes],
             *,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             return self.upload(file, filepath=filepath, timeout=timeout)
 
         def obtain_upload_lease(self,
             *,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = self._client.request('POST', '/api/media/asset',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_media_upload_lease(result)
+            return load_submission_media_upload_lease(result)
 
         def deposit_file(self,
             file: IO[bytes],
-            upload_lease: MediaUploadLease,
+            upload_lease: SubmissionMediaUploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         def upload(self,
             file: IO[bytes],
             *,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> MediaUploadLease:
+        ) -> SubmissionMediaUploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = self.obtain_upload_lease(filepath=filepath)
             self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
@@ -179,106 +189,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a text post.
 
-        .. .PARAMETERS
-
-        :param `str` sr:
-            Name of the subreddit to submit the post to.
-        :param `str` title:
-            Title of the post.
-        :param body:
-            The body text of the post.
-
-            Specify either markdown text or a richtext document.
-        :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
-        :param `bool` reply_notifications:
-            Receive inbox notifications for replies.
-        :param `bool` spoiler:
-            Mark as spoiler.
-        :param `bool` nsfw:
-            Mark as NSFW.
-        :param `bool` oc:
-            Mark as original content.
-        :param `Optional[str]` collection_uuid:
-            The UUID of a collection to add this post to a collection.
-        :param `Optional[str]` flair_uuid:
-            The UUID of a flair template to use.
-        :param `Optional[str]` flair_text:
-            Custom flair text.
-        :param `Optional[str]` event_start:
-            A datetime ISO 8601 string. E.g. `2018-09-11T12:00:00`.
-        :param `Optional[str]` event_end:
-            A datetime ISO 8601 string.
-        :param `Optional[str]` event_tz:
-            A timezone. E.g., `America/Los_Angeles`.
-
-        .. .RETURNS
-
-        :returns: The ID of the newly created post.
-        :rtype: `int`
-
-        .. .RAISES
-
-        :raises redditwarp.exceptions.RedditError:
-            + `USER_REQUIRED`:
-                There is no user context.
-            + `BAD_SR_NAME`:
-                An empty string was specified for `sr`.
-            + `SUBREDDIT_NOEXIST`:
-               - The specified subreddit does not exist.
-               - The specified subreddit is invalid.
-
-            + `SUBREDDIT_NOTALLOWED`:
-               - The subreddit is restricted and you are not an approved user.
-               - You are banned from the subreddit.
-               - You are trying to submit an image or video post to a NSFW subreddit.
-
-               Note, quarantined subreddits can be posted to even if you haven't
-               yet opt-ed in to viewing its content.
-            + `NO_TEXT`:
-                The `title` parameter was not specified, was blank, or contained only whitespace.
-            + `JSON_PARSE_ERROR`:
-                Richtext was passed and it was not in the correct format.
-            + `TOO_LONG`:
-               - The `title` parameter must be under 300 characters.
-               - The `body` parameter must be under 40000 characters.
-
-            + `NO_SELFS`:
-                The subreddit doesn't accept text posts.
-            + `USER_REQUIRED`:
-                There is no user context.
-        :raises redditwarp.http.exceptions.StatusCodeException:
-            + `404`:
-                The target subreddit is private or banned.
+        Alias of `self.create.text[int]()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'self')
-            yield ('sr', sr)
-            yield ('title', title)
-            if isinstance(body, str):
-                yield ('text', body)
-            else:
-                yield ('richtext_json', json.dumps(body))
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = self._client.request('POST', '/api/submit', files=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return self.create.text[int](
+            sr=sr,
+            title=title,
+            body=body,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     def create_link_post(self,
         sr: str,
         title: str,
         link: str,
         *,
         reply_notifications: bool = True,
@@ -291,61 +226,32 @@
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
         resubmit: bool = True,
     ) -> int:
         """Create a link post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` url:
-            A URL.
-        :param `bool` resubmit:
-            When the "Restrict how often the same link can be posted" content control
-            setting is enabled, if a link with the same URL has already been submitted
-            then an `ALREADY_SUB` API error would be returned unless this field is true.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
-
-        :raises redditwarp.exceptions.RedditError:
-            + `NO_URL`:
-                The `link` parameter was not specified, or the URL is invalid.
-            + `ALREADY_SUB`:
-                The given link has already been submitted to the subreddit.
-                See parameter `resubmit`.
+        Alias of `self.create.link[int]()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'link')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            if resubmit: yield ('resubmit', '1')
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = self._client.request('POST', '/api/submit', data=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return self.create.link[int](
+            sr=sr,
+            title=title,
+            link=link,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+            resubmit=resubmit,
+        )
 
     def create_image_post(self,
         sr: str,
         title: str,
         link: str,
         *,
         reply_notifications: bool = True,
@@ -357,48 +263,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> None:
         """Create an image post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` link:
-            A URL to an image.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.image()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'image')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        self._client.request('POST', '/api/submit', data=dict(g()))
+        return self.create.image(
+            sr=sr,
+            title=title,
+            link=link,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     def create_video_post(self,
         sr: str,
         title: str,
         link: str,
         thumbnail: str,
         *,
@@ -412,59 +301,33 @@
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
         vgif: bool = False,
     ) -> None:
         """Create a video post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` link:
-            A URL to a video.
-        :param `str` thumbnail:
-            A URL to an image to be used as a thumbnail for the video.
-        :param `bool` vgif:
-            Pass `True` to create a video GIF.
-
-        .. .RETURNS
-
-        :rtype: `None`
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
-
-        :raises redditwarp.exceptions.RedditError:
-            + `MISSING_VIDEO_URLS`:
-                The `thumbnail` parameter was empty.
-            + `NO_VIDEOS`:
-                The subreddit does not accept video posts.
+        Alias of `self.create.video()`.
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'video' + ('gif' if vgif else ''))
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('url', link)
-            yield ('video_poster_url', thumbnail)
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        self._client.request('POST', '/api/submit', data=dict(g()))
+        return self.create.video(
+            sr=sr,
+            title=title,
+            link=link,
+            thumbnail=thumbnail,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+            vgif=vgif,
+        )
 
     def create_gallery_post(self,
         sr: str,
         title: str,
         items: Sequence[GalleryItem],
         *,
         reply_notifications: bool = True,
@@ -476,58 +339,31 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a gallery post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param items:
-            A list of gallery items.
-        :type items: `Sequence`\\[:class:`~.dtos.submission.GalleryItem`]
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.gallery[int]()`.
         """
-        gallery_items: list[dict[str, str]] = [
-            {
-                'media_id': m.media_id,
-                'caption': m.caption,
-                'outbound_url': m.outbound_link,
-            }
-            for m in items
-        ]
-
-        def g() -> Iterable[tuple[str, JSON_ro]]:
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('items', gallery_items)
-            yield ('sendreplies', reply_notifications)
-            if spoiler: yield ('spoiler', True)
-            if nsfw: yield ('nsfw', True)
-            if oc: yield ('original_content', True)
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = self._client.request('POST', '/api/submit_gallery_post', json=dict(g()))
-        return int(root['json']['data']['id'][3:], 36)
+        return self.create.gallery[int](
+            sr=sr,
+            title=title,
+            items=items,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     def create_poll_post(self,
         sr: str,
         title: str,
         body: str,
         options: Sequence[str],
         duration: int,
@@ -540,117 +376,111 @@
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a poll post.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `str` body:
-        :param `Sequence[str]` options:
-        :param `int` duration:
-            The number of days the poll runs for.
-
-            Valid values are 1 to 7. If a number is specified outside
-            this range it is clamped within range.
-
-            The UI default is 3 days.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
-
-        .. .RAISES
-
-        :(raises): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.poll[int]()`.
         """
-        def g() -> Iterable[tuple[str, JSON_ro]]:
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('text', body)
-            yield ('options', options)
-            yield ('duration', duration)
-            yield ('sendreplies', reply_notifications)
-            if spoiler: yield ('spoiler', True)
-            if nsfw: yield ('nsfw', True)
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = self._client.request('POST', '/api/submit_poll_post', json=dict(g()))
-        return int(root['json']['data']['id'][3:], 36)
+        return self.create.poll[int](
+            sr=sr,
+            title=title,
+            body=body,
+            options=options,
+            duration=duration,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
     def create_crosspost(self,
         sr: str,
         title: str,
-        idn: int,
+        target: Union[int, str],
         *,
         reply_notifications: bool = True,
         spoiler: bool = False,
         nsfw: bool = False,
         oc: bool = False,
         collection_uuid: Optional[str] = None,
         flair_uuid: Optional[str] = None,
         flair_text: Optional[str] = None,
         event_start: Optional[str] = None,
         event_end: Optional[str] = None,
         event_tz: Optional[str] = None,
     ) -> int:
         """Create a crosspost.
 
-        Behaves similarly to :meth:`.create_text_post`.
-
-        .. .PARAMETERS
-
-        :(parameters): Similar to :meth:`.create_text_post`.
-
-        :param `int` idn:
-            The ID of a submission.
-
-        .. .RETURNS
-
-        :(returns): Similar to :meth:`.create_text_post`.
+        Alias of `self.create.cross[int]()`.
+        """
+        return self.create.cross[int](
+            sr=sr,
+            title=title,
+            target=target,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
-        .. .RAISES
+    def create_cross_post(self,
+        sr: str,
+        title: str,
+        target: Union[int, str],
+        *,
+        reply_notifications: bool = True,
+        spoiler: bool = False,
+        nsfw: bool = False,
+        oc: bool = False,
+        collection_uuid: Optional[str] = None,
+        flair_uuid: Optional[str] = None,
+        flair_text: Optional[str] = None,
+        event_start: Optional[str] = None,
+        event_end: Optional[str] = None,
+        event_tz: Optional[str] = None,
+    ) -> int:
+        """Alias of :meth:`.create_crosspost`.
 
-        :(raises): Similar to :meth:`.create_text_post`.
+        .. versionadded:: 1.1.0
         """
-        def g() -> Iterable[tuple[str, str]]:
-            yield ('kind', 'self')
-            yield ('sr', sr)
-            yield ('title', title)
-            yield ('crosspost_parent', 't3_' + to_base36(idn))
-            yield ('sendreplies', '01'[reply_notifications])
-            if spoiler: yield ('spoiler', '1')
-            if nsfw: yield ('nsfw', '1')
-            if oc: yield ('original_content', '1')
-            if collection_uuid: yield ('collection_id', collection_uuid)
-            if flair_uuid: yield ('flair_id', flair_uuid)
-            if flair_text: yield ('flair_text', flair_text)
-            if event_start: yield ('event_start', event_start)
-            if event_end: yield ('event_end', event_end)
-            if event_tz: yield ('event_tz', event_tz)
-
-        root = self._client.request('POST', '/api/submit', data=dict(g()))
-        return int(root['json']['data']['id'], 36)
+        return self.create_crosspost(
+            sr,
+            title,
+            target,
+            reply_notifications=reply_notifications,
+            spoiler=spoiler,
+            nsfw=nsfw,
+            oc=oc,
+            collection_uuid=collection_uuid,
+            flair_uuid=flair_uuid,
+            flair_text=flair_text,
+            event_start=event_start,
+            event_end=event_end,
+            event_tz=event_tz,
+        )
 
-    def edit_text_post_body(self, idn: int, body: Union[str, Mapping[str, JSON_ro]]) -> TextPost:
+    def edit_text_post_body(self, idy: Union[int, str], body: Union[str, Mapping[str, JSON_ro]]) -> TextPost:
         """Edit the body text of a text post.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param body:
             Either markdown or richtext.
         :type body: `Union`\\[`str`, `Mapping`\\[`str`, :class:`~.types.JSON_ro`]]
 
         .. .RETURNS
 
         :rtype: :class:`~.models.submission_SYNC.TextPost`
@@ -658,109 +488,113 @@
         .. .RAISES
 
         :raises:
             Same as comment :meth:`~.siteprocs.comment.SYNC.CommentProcedures.edit_body`
             but for submissions.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('thing_id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('thing_id', 't3_' + id36)
             yield ('return_rtjson', '1')
             if isinstance(body, str):
                 yield ('text', body)
             else:
                 yield ('richtext_json', json.dumps(body))
 
         result = self._client.request('POST', '/api/editusertext', files=dict(g()))
         return load_text_post(result, self._client)
 
-    def delete(self, idn: int) -> None:
+    def delete(self, idy: Union[int, str]) -> None:
         """Delete a submission.
 
         If the target doesn't exist or isn't valid, nothing happens.
 
         When a submission is deleted it's text content (if a text post)
         will be set to "`[deleted]`" and the submission will be unlisted
         from its subreddit. Users can still otherwise view and reply to
         deleted to submissions if they have a direct link to it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/del', data=data)
 
-    def lock(self, idn: int) -> None:
+    def lock(self, idy: Union[int, str]) -> None:
         """Lock a submission.
 
         Nothing happens if the target is already locked.
 
         .. hint::
            Locking prevents a submission/comment from receiving new comments.
            A locked submission is unable to receive any new comments.
            Locking a comment only stops direct comments, but
            existing child comments can still receive replies.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target doesn't exist or you don't have permission to lock it.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/lock', data=data)
 
-    def unlock(self, idn: int) -> None:
+    def unlock(self, idy: Union[int, str]) -> None:
         """Unlock a submission.
 
         Behaves similarly to :meth:`.lock`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises:
             Similar to :meth:`.lock`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/unlock', data=data)
 
-    def vote(self, idn: int, direction: int) -> None:
+    def vote(self, idy: Union[int, str], direction: int) -> None:
         """Cast a vote on a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `int` direction:
             Either: `1` (upvote), `0` unvote, `-1` downvote.
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -769,26 +603,27 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'dir': str(direction),
         }
         self._client.request('POST', '/api/vote', data=data)
 
-    def save(self, idn: int, category: Optional[str] = None) -> None:
+    def save(self, idy: Union[int, str], category: Optional[str] = None) -> None:
         """Save a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` category:
             A category/label.
 
             Requires Reddit Premium. Ignored if no Reddit Premium.
 
         .. .RETURNS
 
@@ -799,191 +634,199 @@
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The category name specified was invalid.
         """
-        data = {
-            'id': 't3_' + to_base36(idn),
-        }
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         if category is not None:
             data['category'] = category
         self._client.request('POST', '/api/save', data=data)
 
-    def unsave(self, idn: int) -> None:
+    def unsave(self, idy: Union[int, str]) -> None:
         """Save a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/unsave', data=data)
 
-    def hide(self, idn: int) -> None:
+    def hide(self, idy: Union[int, str]) -> None:
         """Hide a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 The target was not found.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/hide', data=data)
 
-    def unhide(self, idn: int) -> None:
+    def unhide(self, idy: Union[int, str]) -> None:
         """Unhide a submission.
 
         See :meth:`.hide`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/unhide', data=data)
 
-    def bulk_hide(self, ids: Iterable[int]) -> CallChunkCallingIterator[None]:
+    def bulk_hide(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingIterator[None]:
         """Bulk hide submissions.
 
         If *any* of the list of submission IDs don't exist then the endpoint will
         return a HTTP 400 status error and none of the submissions will be hidden.
         This can be annoying since if the list is long it can be hard to tell which
         ID is the culprit.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :rtype: :class:`~.iterators.call_chunk_calling_iterator.CallChunkCallingIterator`\\[`None`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `400`:
                 If any of the IDs were not found.
         """
-        def mass_hide(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        def mass_hide(ids: Sequence[_YIntOrStr]) -> None:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             self._client.request('POST', '/api/hide', data={'id': ids_str})
 
-        return CallChunkCallingIterator(CallChunk(mass_hide, chunk) for chunk in chunked(ids, 300))
+        return CallChunkCallingIterator(CallChunk[Sequence[_YIntOrStr], None](mass_hide, chunk) for chunk in chunked(ids, 300))
 
-    def bulk_unhide(self, ids: Iterable[int]) -> CallChunkCallingIterator[None]:
+    def bulk_unhide(self, ids: Iterable[_YIntOrStr]) -> CallChunkCallingIterator[None]:
         """Bulk hide submissions.
 
         See :meth:`.bulk_hide`.
         """
-        def mass_unhide(ids: Sequence[int]) -> None:
-            id36s = map(to_base36, ids)
+        def mass_unhide(ids: Sequence[_YIntOrStr]) -> None:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t3_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             self._client.request('POST', '/api/unhide', data={'id': ids_str})
 
-        return CallChunkCallingIterator(CallChunk(mass_unhide, chunk) for chunk in chunked(ids, 300))
+        return CallChunkCallingIterator(CallChunk[Sequence[_YIntOrStr], None](mass_unhide, chunk) for chunk in chunked(ids, 300))
 
-    def mark_nsfw(self, idn: int) -> None:
+    def mark_nsfw(self, idy: Union[int, str]) -> None:
         """Mark a submission as NSFW.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to mark the target.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/marknsfw', data=data)
 
-    def unmark_nsfw(self, idn: int) -> None:
+    def unmark_nsfw(self, idy: Union[int, str]) -> None:
         """Unmark a submission as NSFW.
 
         See :meth:`.mark_nsfw`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/unmarknsfw', data=data)
 
-    def mark_spoiler(self, idn: int) -> None:
+    def mark_spoiler(self, idy: Union[int, str]) -> None:
         """Mark a submission as spoiler.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to mark the target.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/spoiler', data=data)
 
-    def unmark_spoiler(self, idn: int) -> None:
+    def unmark_spoiler(self, idy: Union[int, str]) -> None:
         """Unmark a submission as spoiler.
 
         See :meth:`.mark_spoiler`.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/unspoiler', data=data)
 
-    def distinguish(self, idn: int) -> Submission:
+    def distinguish(self, idy: Union[int, str]) -> Submission:
         """Distinguish a submission.
 
         .. hint::
 
            Distinguishing decoratates the author's name by
            giving it a different color and putting a sigil beside it.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target submission.
         :rtype: :class:`~.models.submission_SYNC.Submission`
 
         .. .RAISES
@@ -993,27 +836,28 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to distinguish the target.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'how': 'yes',
         }
         root = self._client.request('POST', '/api/distinguish', data=data)
         return load_submission(root['json']['data']['things'][0]['data'], self._client)
 
-    def undistinguish(self, idn: int) -> Submission:
+    def undistinguish(self, idy: Union[int, str]) -> Submission:
         """Undistinguish a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns: The target submission.
         :rtype: :class:`~.models.submission_SYNC.Submission`
 
         .. .RAISES
@@ -1023,22 +867,23 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission.
             + `404`:
                 The target could not be found.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'how': 'no',
         }
         root = self._client.request('POST', '/api/distinguish', data=data)
         return load_submission(root['json']['data']['things'][0]['data'], self._client)
 
-    def sticky(self, idn: int, slot: Optional[int] = None) -> None:
+    def sticky(self, idy: Union[int, str], slot: Optional[int] = None) -> None:
         """Set a submission as sticky in its subreddit.
 
         .. hint::
            Stickied posts are shown at the top of the subreddit in the default 'Hot' listing.
 
         In a subreddit, there can be at most 2 sticked posts at a time.
 
@@ -1051,15 +896,15 @@
         Unstickying a post that isn't stickied does nothing.
 
         .. note::
            You cannot reorder sticky posts directly. You must unsticky and re-sticky them.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` slot:
             Which sticky slot to use.
 
             If not specified, the bottom-most slot will be used if available.
             If the sticky list is at maximum length, the bottom-most slot will
             be replaced with the new post.
 
@@ -1074,36 +919,38 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to sticky that post.
             + `409`:
                 The post is already stickied.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '1',
         }
         if slot is not None:
             data['num'] = str(slot)
         self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    def unsticky(self, idn: int) -> None:
+    def unsticky(self, idy: Union[int, str]) -> None:
         """Unsticky a submission.
 
         See :meth:`.sticky`.
 
         Unstickying a post that isn't stickied does nothing.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '0',
         }
         self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    def pin_to_profile(self, idn: int, slot: Optional[int] = None) -> None:
+    def pin_to_profile(self, idy: Union[int, str], slot: Optional[int] = None) -> None:
         """Pin a post you created to your user profile.
 
         .. hint::
            Pinned posts show up at the start of the
            'Overview', or 'Submitted' (old UI) / 'POSTS' (redesign UI)
            user profile listings.
 
@@ -1128,15 +975,15 @@
         Unpinning a post that isn't pinned does nothing.
 
         .. note::
            You cannot reorder pinned posts directly. You must unpin and re-pin them.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` slot:
             Which pin slot to use.
 
             If `slot` is not specified, the new post is inserted at the top of the list.
             If the list is at maximum length, the least recently pinned post will be evicted.
             It acts like a queue.
 
@@ -1151,48 +998,50 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 You do not have permission to pin that post.
             + `409`:
                 The post is already pinned.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'to_profile': '1',
             'state': '1',
         }
         if slot is not None:
             data['num'] = str(slot)
         self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    def unpin_from_profile(self, idn: int) -> None:
+    def unpin_from_profile(self, idy: Union[int, str]) -> None:
         """Unpin a submission from your user profile.
 
         See :meth:`.pin_to_profile`.
 
         Unpinning a post that isn't pinned does nothing.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'to_profile': '1',
             'state': '0',
         }
         self._client.request('POST', '/api/set_subreddit_sticky', data=data)
 
-    def set_contest_mode(self, idn: int, state: bool) -> None:
+    def set_contest_mode(self, idy: Union[int, str], state: bool) -> None:
         """Set or unset 'contest mode' for a submission's comments.
 
         .. hint::
 
             In contest mode, vote counts are hidden and comments are displayed
             in a random order.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `bool` state:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1201,31 +1050,32 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The specified ID was not found.
                - You do not have permission to modify the target.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '01'[state],
         }
         self._client.request('POST', '/api/set_contest_mode', data=data)
 
-    def set_suggested_sort(self, idn: int, sort: str) -> None:
+    def set_suggested_sort(self, idy: Union[int, str], sort: str) -> None:
         """Set or unset the suggested sort for a submission's comments.
 
         .. hint::
 
            When set, users will see comments in the suggested sort order by default.
            They can still manually change back to their preferred sort if they choose.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `str` sort:
             Either: `confidence`, `top`, `new`, `controversial`,
             `old`, `random`, `qa`, `live`, `blank`.
 
             If not specified or an unknown value, the suggested sort will be unset.
 
         .. .RETURNS
@@ -1238,67 +1088,70 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The specified ID was not found.
                - You do not have permission to modify the target.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'sort': sort,
         }
         self._client.request('POST', '/api/set_suggested_sort', data=data)
 
-    def enable_reply_notifications(self, idn: int) -> None:
+    def enable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Enable inbox reply notifications for a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '1'
         }
         self._client.request('POST', '/api/sendreplies', data=data)
 
-    def disable_reply_notifications(self, idn: int) -> None:
+    def disable_reply_notifications(self, idy: Union[int, str]) -> None:
         """Disable inbox reply notifications for a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.RedditError:
             + `USER_REQUIRED`:
                 There is no user context.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'state': '0'
         }
         self._client.request('POST', '/api/sendreplies', data=data)
 
-    def set_event_time(self, idn: int,
+    def set_event_time(self, idy: Union[int, str],
             event_start: Optional[str] = None,
             event_end: Optional[str] = None,
             event_tz: Optional[str] = None) -> None:
         """Add or modify event times on a submission.
 
         Specify only `event_start` to change only the starting date.
         The same cannot be done for `event_end`, a 500 HTTP error will occur.
@@ -1307,15 +1160,15 @@
         `event_end` in time, otherwise a `MIN_EVENT_TIME` API error is returned.
         It is possible however to make a second request specifying only `event_start` to modify
         the start date so that `event_start` is after `event_end`. If this happens then the time
         difference can be longer than 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[str]` event_start:
             A datetime ISO 8601 string. E.g. `2018-09-11T12:00:00`.
         :param `Optional[str]` event_end:
             A datetime ISO 8601 string.
         :param `Optional[str]` event_tz:
             A timezone. E.g., `America/Los_Angeles`.
 
@@ -1343,30 +1196,31 @@
             + `INVALID_TIMEZONE`:
                 The value specified for `event_tz` is invalid.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `500`:
                 The `event_start` parameter was not specified.
         """
         def g() -> Iterable[tuple[str, str]]:
-            yield ('id', 't3_' + to_base36(idn))
+            id36 = x if isinstance((x := idy), str) else to_base36(x)
+            yield ('id', 't3_' + id36)
             if event_start: yield ('event_start', event_start)
             if event_end: yield ('event_end', event_end)
             if event_tz: yield ('event_tz', event_tz)
 
         self._client.request('POST', '/api/event_post_time', data=dict(g()))
 
-    def follow_event(self, idn: int) -> None:
+    def follow_event(self, idy: Union[int, str]) -> None:
         """Follow a post event.
 
         .. hint::
            Followers receive a push notification when the event starts.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1375,37 +1229,39 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The target submission is not an event.
             + `404`:
                 The target submission does not exist.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'fullname': 't3_' + to_base36(idn),
+            'fullname': 't3_' + id36,
             'follow': '1',
         }
         self._client.request('POST', '/api/follow_post', data=data)
 
-    def unfollow_event(self, idn: int) -> None:
+    def unfollow_event(self, idy: Union[int, str]) -> None:
         """Unfollow a post event.
 
         See :meth:`.follow_event`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'fullname': 't3_' + to_base36(idn),
+            'fullname': 't3_' + id36,
             'follow': '0',
         }
         self._client.request('POST', '/api/follow_post', data=data)
 
-    def approve(self, idn: int) -> None:
+    def approve(self, idy: Union[int, str]) -> None:
         """Approve a submission.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1415,25 +1271,26 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't3_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36}
         self._client.request('POST', '/api/approve', data=data)
 
-    def remove(self, idn: int) -> None:
+    def remove(self, idy: Union[int, str]) -> None:
         """Remove a submission.
 
         This is a moderator action.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -1443,43 +1300,45 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                You do not have permission.
 
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'spam': '0',
         }
         self._client.request('POST', '/api/remove', data=data)
 
-    def remove_spam(self, idn: int) -> None:
+    def remove_spam(self, idy: Union[int, str]) -> None:
         """Remove as spam.
 
         See :meth:`.remove`.
         """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         data = {
-            'id': 't3_' + to_base36(idn),
+            'id': 't3_' + id36,
             'spam': '1',
         }
         self._client.request('POST', '/api/remove', data=data)
 
-    def ignore_reports(self, idn: int) -> None:
+    def ignore_reports(self, idy: Union[int, str]) -> None:
         """Ignore reports on a submission.
 
         .. hint::
            If you ignore reports, you won't receive notifications and the
            ignored thing will be absent from moderation listings.
 
         Nothing happens if the target is already ignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1488,24 +1347,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        self._client.request('POST', '/api/ignore_reports', data={'id': 't3_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/ignore_reports', data={'id': 't3_' + id36})
 
-    def unignore_reports(self, idn: int) -> None:
+    def unignore_reports(self, idy: Union[int, str]) -> None:
         """Unignore reports on a submission.
 
         Nothing happens if the target is already unignored.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
@@ -1514,22 +1374,23 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        self._client.request('POST', '/api/unignore_reports', data={'id': 't3_' + to_base36(idn)})
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        self._client.request('POST', '/api/unignore_reports', data={'id': 't3_' + id36})
 
-    def snooze_reports(self, idn: int, reason: str) -> None:
+    def snooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Ignore a custom report reason in a subreddit for 7 days.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
         :param `str` reason:
             The custom report reason to snooze.
 
         .. .RETURNS
 
         :rtype: `None`
@@ -1540,36 +1401,38 @@
             + `USER_REQUIRED`:
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not exist.
                - The target belongs to a subreddit you do not have permission over.
         """
-        data = {'id': 't3_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36, 'reason': reason}
         self._client.request('POST', '/api/snooze_reports', data=data)
 
-    def unsnooze_reports(self, idn: int, reason: str) -> None:
+    def unsnooze_reports(self, idy: Union[int, str], reason: str) -> None:
         """Unsnooze a custom report.
 
         See :meth:`.snooze_reports`.
         """
-        data = {'id': 't3_' + to_base36(idn), 'reason': reason}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        data = {'id': 't3_' + id36, 'reason': reason}
         self._client.request('POST', '/api/unsnooze_reports', data=data)
 
     def apply_removal_reason(self,
-            idn: int,
+            idy: Union[int, str],
             reason_id: Optional[str] = None,
             note: Optional[str] = None) -> None:
         """Set a removal reason on a removed submission.
 
         If the target is not a removed submission, nothing happens.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             Submission ID.
         :param `Optional[int]` reason_id:
             A removal reason ID.
         :param `Optional[str]` note:
             A note.
 
         .. .RETURNS
@@ -1590,20 +1453,20 @@
                 The reason ID is invalid.
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't3_' + to_base36(idn)
-        json_data = {'item_ids': [target], 'reason_id': reason_id, 'mod_note': note}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        json_data = {'item_ids': ['t3_' + id36], 'reason_id': reason_id, 'mod_note': note}
         self._client.request('POST', '/api/v1/modactions/removal_reasons', json=json_data)
 
     def send_removal_comment(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False,
             locked: bool = False) -> Comment:
         """Send a removal comment.
 
@@ -1613,15 +1476,15 @@
         (The UI does not normally let you do this.)
 
         Unlike :meth:`.apply_removal_reason`, the target you specify must be a
         removed item otherwise an `INVALID_ID` API error is produced.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed submission.
         :param `str` title:
             A title.
 
             This is ultimately unused for removal comments, but a non-empty
             string must be specified or you'll get a `NO_TEXT` API error.
 
@@ -1657,38 +1520,38 @@
 
             + `MUST_BE_PRESENT`:
                 The subreddit specified does not exist.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                - The target specified does not belong to a subreddit you moderate.
         """
-        target = 't3_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'public' + ('' if exposed else '_as_subreddit'),
-            'item_id': [target],
+            'item_id': ['t3_' + id36],
             'title': title,
             'message': message,
             'lock_comment': '01'[locked],
         }
         root = self._client.request('POST', '/api/v1/modactions/removal_link_message', json=json_data)
         return load_comment(root, self._client)
 
     def send_removal_message(self,
-            idn: int,
+            idy: Union[int, str],
             title: str,
             message: str,
             *,
             exposed: bool = False) -> None:
         """Send a removal message.
 
         Behaves similarly to :meth:`.send_removal_comment`.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
             ID of a removed comment.
         :param `str` title:
             A title.
 
             A non-empty string must be specified or you'll get a `NO_TEXT` API error.
 
             The UI sends the title of the selected removal reason.
@@ -1705,18 +1568,18 @@
 
         :returns: `None`
 
         .. .RAISES
 
         :(raises): See :meth:`.send_removal_comment`.
         """
-        target = 't3_' + to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         json_data = {
             'type': 'private' + ('_exposed' if exposed else ''),
-            'item_id': [target],
+            'item_id': ['t3_' + id36],
             'title': title,
             'message': message,
         }
         self._client.request('POST', '/api/v1/modactions/removal_link_message', json=json_data)
 
     def search(self, sr: str, query: str, amount: Optional[int] = None, *,
         sort: str = 'relevance', time: str = 'all',
@@ -1751,22 +1614,22 @@
             url = f'/r/{sr}/search'
         p = SubmissionSearchPaginator(
                 self._client, url,
                 params={'q': query, 'restrict_sr': '1'},
                     sort=sort, time=time)
         return ImpartedPaginatorChainingIterator(p, amount)
 
-    def duplicates(self, target: int, amount: Optional[int] = None, *,
+    def duplicates(self, target: Union[int, str], amount: Optional[int] = None, *,
         sort: str = 'num_comments',
     ) -> ImpartedPaginatorChainingIterator[SubmissionDuplicatesPaginator, Submission]:
         """Get crossposts for a submission.
 
         .. .PARAMETERS
 
-        :param `int` target:
+        :param `Union[int, str]` target:
             Submission ID.
         :param `Optional[int]` amount:
             The number of items to retrieve.
         :param `str` sort:
             Either `num_comments` or `new`.
 
             Default: `num_comments`.
@@ -1779,10 +1642,10 @@
 
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 Fetching some submissions resulted in a 403.
             + `404`:
                 The target submission could not be found.
         """
-        subm_id = to_base36(target)
-        p = SubmissionDuplicatesPaginator(self._client, f'/duplicates/{subm_id}', sort=sort)
+        id36 = x if isinstance((x := target), str) else to_base36(x)
+        p = SubmissionDuplicatesPaginator(self._client, f'/duplicates/{id36}', sort=sort)
         return ImpartedPaginatorChainingIterator(p, amount)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/fetch_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/fetch_ASYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Mapping, TypeVar, Generic
+from typing import TYPE_CHECKING, Any, Mapping, TypeVar, Generic, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from .ASYNC import SubmissionProcedures
 
 from ...model_loaders.submission_ASYNC import load_submission
 from ...models.submission_ASYNC import Submission, LinkPost, TextPost
 from ...util.base_conversion import to_base36
@@ -13,16 +13,16 @@
 
 T = TypeVar('T')
 
 class Common(Generic[T]):
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    async def __call__(self, idn: int) -> T:
-        id36 = to_base36(idn)
+    async def __call__(self, idy: Union[int, str]) -> T:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return await self.by_id36(id36)
 
     def _load_object(self, m: Mapping[str, Any]) -> T:
         raise NotImplementedError
 
     async def by_id36(self, id36: str) -> T:
         full_id36 = 't3_' + id36
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/fetch_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/fetch_SYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Mapping, TypeVar, Generic
+from typing import TYPE_CHECKING, Any, Mapping, TypeVar, Generic, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from .SYNC import SubmissionProcedures
 
 from ...model_loaders.submission_SYNC import load_submission
 from ...models.submission_SYNC import Submission, LinkPost, TextPost
 from ...util.base_conversion import to_base36
@@ -13,16 +13,16 @@
 
 T = TypeVar('T')
 
 class Common(Generic[T]):
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    def __call__(self, idn: int) -> T:
-        id36 = to_base36(idn)
+    def __call__(self, idy: Union[int, str]) -> T:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return self.by_id36(id36)
 
     def _load_object(self, m: Mapping[str, Any]) -> T:
         raise NotImplementedError
 
     def by_id36(self, id36: str) -> T:
         full_id36 = 't3_' + id36
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/get_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/get_ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Mapping, Optional, TypeVar, Generic
+from typing import TYPE_CHECKING, Any, Mapping, Optional, TypeVar, Generic, Union
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
 
 from ...model_loaders.submission_ASYNC import load_submission
 from ...models.submission_ASYNC import Submission, LinkPost, TextPost
 from ...util.base_conversion import to_base36
 from ...util.extract_id_from_url import extract_submission_id_from_url
 
 T = TypeVar('T')
 
 class Common(Generic[T]):
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    async def __call__(self, idn: int) -> Optional[T]:
-        id36 = to_base36(idn)
+    async def __call__(self, idy: Union[int, str]) -> Optional[T]:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return await self.by_id36(id36)
 
     def _load_object(self, m: Mapping[str, Any]) -> Optional[T]:
         raise NotImplementedError
 
     async def by_id36(self, id36: str) -> Optional[T]:
         full_id36 = 't3_' + id36
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/submission/get_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/submission/get_SYNC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Mapping, Optional, TypeVar, Generic
+from typing import TYPE_CHECKING, Any, Mapping, Optional, TypeVar, Generic, Union
 if TYPE_CHECKING:
     from ...client_SYNC import Client
 
 from ...model_loaders.submission_SYNC import load_submission
 from ...models.submission_SYNC import Submission, LinkPost, TextPost
 from ...util.base_conversion import to_base36
 from ...util.extract_id_from_url import extract_submission_id_from_url
 
 T = TypeVar('T')
 
 class Common(Generic[T]):
     def __init__(self, client: Client) -> None:
         self._client = client
 
-    def __call__(self, idn: int) -> Optional[T]:
-        id36 = to_base36(idn)
+    def __call__(self, idy: Union[int, str]) -> Optional[T]:
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         return self.by_id36(id36)
 
     def _load_object(self, m: Mapping[str, Any]) -> Optional[T]:
         raise NotImplementedError
 
     def by_id36(self, id36: str) -> Optional[T]:
         full_id36 = 't3_' + id36
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/ASYNC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Any, Mapping
+from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Any, Mapping, Union, TypeVar
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.comment_ASYNC import LooseComment
     from ...models.subreddit_rules import SubredditRules
     from ...types import JSON_ro
 
 from ...models.subreddit_ASYNC import Subreddit, InaccessibleSubreddit
@@ -18,63 +18,67 @@
 from ...pagination.paginators.listing.comment_listing_async_paginator import LooseCommentListingAsyncPaginator
 from ...pagination.paginators.subreddit_async1 import SubredditSearchAsyncPaginator
 from ... import exceptions
 from ... import http
 from .pull_ASYNC import Pull
 from .pulls_ASYNC import Pulls
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class SubredditProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.pull: Pull = Pull(client)
         ("""
             Pull subreddit submissions.
             """)
         self.pulls: Pulls = Pulls(client)
         ("""
             Pull subreddits.
             """)
 
-    async def get(self, idn: int) -> Optional[Subreddit]:
+    async def get(self, idy: Union[int, str]) -> Optional[Subreddit]:
         """Get information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * `None` if the subreddit does not exist, or the subreddit is private or banned.
             * :class:`~.models.subreddit_ASYNC.Subreddit`
         :rtype: `Optional`\\[:class:`~.models.subreddit_ASYNC.Subreddit`]
         """
-        v = await self.get_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = await self.get_potentially_inaccessible(id36)
         if isinstance(v, Subreddit):
             return v
         return None
 
-    async def fetch(self, idn: int) -> Subreddit:
+    async def fetch(self, idy: Union[int, str]) -> Subreddit:
         """Fetch information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.subreddit_ASYNC.Subreddit`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.OperationException:
            - The target subreddit is was not found.
            - The target subreddit is private or banned.
         """
-        v = await self.fetch_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = await self.fetch_potentially_inaccessible(id36)
         if isinstance(v, Subreddit):
             return v
         if isinstance(v, InaccessibleSubreddit):
             raise exceptions.RejectedResultException
         raise Exception
 
     async def get_by_name(self, name: str) -> Optional[Subreddit]:
@@ -138,57 +142,58 @@
                - The specified subreddit name was too long or contained invalid characters.
         """
         root = await self._client.request('GET', f'/r/{name}/about')
         if root['kind'] == 'Listing':
             raise exceptions.NoResultException('target not found')
         return load_subreddit(root['data'], self._client)
 
-    async def get_potentially_inaccessible(self, idn: int) -> Optional[object]:
+    async def get_potentially_inaccessible(self, idy: Union[int, str]) -> Optional[object]:
         """Get information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * :class:`~.models.subreddit_ASYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_ASYNC.Subreddit`
         :rtype: `Optional`\\[`object`]
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         root = await self._client.request('GET', '/api/info', params={'id': full_id36})
         if children := root['data']['children']:
             return load_potentially_inaccessible_subreddit(children[0]['data'], self._client)
         return None
 
-    async def fetch_potentially_inaccessible(self, idn: int) -> object:
+    async def fetch_potentially_inaccessible(self, idy: Union[int, str]) -> object:
         """Fetch information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * :class:`~.models.subreddit_ASYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_ASYNC.Subreddit`
         :rtype: `Optional`\\[`object`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.NoResultException:
             The target subreddit is was not found.
         """
-        v = await self.get_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = await self.get_potentially_inaccessible(id36)
         if v is None:
             raise exceptions.NoResultException('target not found')
         return v
 
     async def get_potentially_inaccessible_by_name(self, name: str) -> Optional[object]:
         """Get information about a potentially inacessible subreddit.
 
@@ -230,41 +235,43 @@
             The target subreddit is was not found.
         """
         v = await self.get_potentially_inaccessible_by_name(name)
         if v is None:
             raise exceptions.NoResultException('target not found')
         return v
 
-    def bulk_fetch_potentially_inaccessible(self, ids: Iterable[int]) -> CallChunkChainingAsyncIterator[object]:
+    def bulk_fetch_potentially_inaccessible(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingAsyncIterator[object]:
         """Bulk fetch information about a potentially inacessible subreddits, by ID.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :returns:
             Iterator of:
 
             * :class:`~.models.subreddit_ASYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_ASYNC.Subreddit`
         :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[`object`]
         """
-        async def mass_fetch(ids: Sequence[int]) -> Sequence[object]:
-            id36s = map(to_base36, ids)
+        async def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[object]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t5_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = await self._client.request('GET', '/api/info', params={'id': ids_str})
-            return [load_potentially_inaccessible_subreddit(i['data'], self._client) for i in root['data']['children']]
+            # https://github.com/python/mypy/issues/13408
+            return [load_potentially_inaccessible_subreddit(i['data'], self._client) for i in root['data']['children']]  # type: ignore[return-value]
 
-        return CallChunkChainingAsyncIterator(AsyncCallChunk(mass_fetch, chunk) for chunk in chunked(ids, 100))
+        return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], Sequence[object]](mass_fetch, chunk) for chunk in chunked(ids, 100))
 
     def bulk_fetch_potentially_inaccessible_by_name(self, names: Iterable[str]) -> CallChunkChainingAsyncIterator[object]:
         """Bulk fetch information about a potentially inacessible subreddits, by name.
 
         Any name not found will be ignored.
 
         .. .PARAMETERS
@@ -323,20 +330,20 @@
                - You don't have permission to view this subreddit's settings.
         """
         root = await self._client.request('GET', f'/r/{sr}/about/edit')
         if root['kind'] != 'subreddit_settings':
             raise exceptions.NoResultException('target not found')
         return root['data']
 
-    async def update_settings(self, idn: int, settings: Mapping[str, JSON_ro]) -> None:
+    async def update_settings(self, idy: Union[int, str], settings: Mapping[str, JSON_ro]) -> None:
         """Update a subreddit's settings.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param settings:
         :type settings: `Mapping`\\[`str`, :class:`~.types.JSON_ro`]
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -346,25 +353,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `SUBREDDIT_REQUIRED`:
                 The specified subreddit does not exist.
             + `MOD_REQUIRED`:
                 The current user is not a moderator of the subreddit.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         json: Mapping[str, JSON_ro] = {**settings, 'sr': full_id36}
         await self._client.request('PATCH', '/api/v1/subreddit/update_settings', json=json)
 
-    async def subscribe_by_id(self, idn: int) -> None:
+    async def subscribe_by_id(self, idy: Union[int, str]) -> None:
         """Subscribe to a subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -373,15 +380,15 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The specified subreddit could not be accessed.
             + `404`:
                 The specified subreddit does not exist.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         await self._client.request('POST', '/api/subscribe', data={'action': 'sub', 'sr': full_id36})
 
     async def subscribe_by_name(self, name: str) -> None:
         """Subscribe to a subreddit.
 
         .. .PARAMETERS
@@ -403,32 +410,38 @@
                - The specified subreddit was a special name such as `popular`, `all`, or `random`.
 
             + `404`:
                 The specified subreddit does not exist.
         """
         await self._client.request('POST', '/api/subscribe', data={'action': 'sub', 'sr_name': name})
 
-    async def unsubscribe_by_id(self, idn: int) -> None:
+    async def unsubscribe_by_id(self, idy: Union[int, str]) -> None:
         """Unsubscribe from a subreddit.
 
         Behaves similarly to :meth:`.subscribe_by_id`.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         await self._client.request('POST', '/api/subscribe', data={'action': 'unsub', 'sr': full_id36})
 
     async def unsubscribe_by_name(self, name: str) -> None:
         """Unsubscribe from a subreddit.
 
         Behaves similarly to :meth:`.subscribe_by_name`.
         """
         await self._client.request('POST', '/api/subscribe', data={'action': 'unsub', 'sr_name': name})
 
     async def get_rules(self, sr: str) -> SubredditRules:
-        """Get a subreddit's rules.
+        r"""Get a subreddit's rules.
+
+        Example::
+
+           rules = await client.p.subreddit.get_rules(SR)
+           for i, rule in enumerate(rules, 1):
+               print(f"{i}. {rule.short_name}\n{rule.description}\n")
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
 
@@ -517,27 +530,28 @@
             await self._client.request('GET', '/api/search_reddit_names', params={'query': name, 'exact': '1'})
         except http.exceptions.StatusCodeException as e:
             if e.status_code == 404:
                 return False
             raise
         return True
 
-    async def get_similar_subreddits(self, idn: int, n: Optional[int] = None) -> Sequence[Subreddit]:
+    async def get_similar_subreddits(self, idy: Union[int, str], n: Optional[int] = None) -> Sequence[Subreddit]:
         """Get a list of similar subreddits.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` n:
             The maximum number of entries to return.
 
             Effective default: 10.
 
         .. .RETURNS
 
         :rtype: `Sequence`\\[:class:`~.models.subreddit_ASYNC.Subreddit`]
         """
-        params = {'sr_fullnames': 't5_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        params = {'sr_fullnames': 't5_' + id36}
         if n is not None:
             params['max_recs'] = str(n)
         root = await self._client.request('GET', '/api/similar_subreddits', params=params)
         return [load_subreddit(d['data'], client=self._client) for d in root['data']['children']]
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/SYNC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Any, Mapping
+from typing import TYPE_CHECKING, Optional, Iterable, Sequence, Any, Mapping, Union, TypeVar
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.comment_SYNC import LooseComment
     from ...models.subreddit_rules import SubredditRules
     from ...types import JSON_ro
 
 from ...models.subreddit_SYNC import Subreddit, InaccessibleSubreddit
@@ -18,63 +18,67 @@
 from ...pagination.paginators.listing.comment_listing_paginator import LooseCommentListingPaginator
 from ...pagination.paginators.subreddit_sync1 import SubredditSearchPaginator
 from ... import exceptions
 from ... import http
 from .pull_SYNC import Pull
 from .pulls_SYNC import Pulls
 
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
+
 class SubredditProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
         self.pull: Pull = Pull(client)
         ("""
             Pull subreddit submissions.
             """)
         self.pulls: Pulls = Pulls(client)
         ("""
             Pull subreddits.
             """)
 
-    def get(self, idn: int) -> Optional[Subreddit]:
+    def get(self, idy: Union[int, str]) -> Optional[Subreddit]:
         """Get information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * `None` if the subreddit does not exist, or the subreddit is private or banned.
             * :class:`~.models.subreddit_SYNC.Subreddit`
         :rtype: `Optional`\\[:class:`~.models.subreddit_SYNC.Subreddit`]
         """
-        v = self.get_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = self.get_potentially_inaccessible(id36)
         if isinstance(v, Subreddit):
             return v
         return None
 
-    def fetch(self, idn: int) -> Subreddit:
+    def fetch(self, idy: Union[int, str]) -> Subreddit:
         """Fetch information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: :class:`~.models.subreddit_SYNC.Subreddit`
 
         .. .RAISES
 
         :raises redditwarp.exceptions.OperationException:
            - The target subreddit is was not found.
            - The target subreddit is private or banned.
         """
-        v = self.fetch_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = self.fetch_potentially_inaccessible(id36)
         if isinstance(v, Subreddit):
             return v
         if isinstance(v, InaccessibleSubreddit):
             raise exceptions.RejectedResultException
         raise Exception
 
     def get_by_name(self, name: str) -> Optional[Subreddit]:
@@ -138,57 +142,58 @@
                - The specified subreddit name was too long or contained invalid characters.
         """
         root = self._client.request('GET', f'/r/{name}/about')
         if root['kind'] == 'Listing':
             raise exceptions.NoResultException('target not found')
         return load_subreddit(root['data'], self._client)
 
-    def get_potentially_inaccessible(self, idn: int) -> Optional[object]:
+    def get_potentially_inaccessible(self, idy: Union[int, str]) -> Optional[object]:
         """Get information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * :class:`~.models.subreddit_SYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_SYNC.Subreddit`
         :rtype: `Optional`\\[`object`]
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         root = self._client.request('GET', '/api/info', params={'id': full_id36})
         if children := root['data']['children']:
             return load_potentially_inaccessible_subreddit(children[0]['data'], self._client)
         return None
 
-    def fetch_potentially_inaccessible(self, idn: int) -> object:
+    def fetch_potentially_inaccessible(self, idy: Union[int, str]) -> object:
         """Fetch information about a potentially inaccessible subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :returns:
             * :class:`~.models.subreddit_SYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_SYNC.Subreddit`
         :rtype: `Optional`\\[`object`]
 
         .. .RAISES
 
         :raises redditwarp.exceptions.NoResultException:
             The target subreddit is was not found.
         """
-        v = self.get_potentially_inaccessible(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        v = self.get_potentially_inaccessible(id36)
         if v is None:
             raise exceptions.NoResultException('target not found')
         return v
 
     def get_potentially_inaccessible_by_name(self, name: str) -> Optional[object]:
         """Get information about a potentially inacessible subreddit.
 
@@ -230,41 +235,42 @@
             The target subreddit is was not found.
         """
         v = self.get_potentially_inaccessible_by_name(name)
         if v is None:
             raise exceptions.NoResultException('target not found')
         return v
 
-    def bulk_fetch_potentially_inaccessible(self, ids: Iterable[int]) -> CallChunkChainingIterator[object]:
+    def bulk_fetch_potentially_inaccessible(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingIterator[object]:
         """Bulk fetch information about a potentially inacessible subreddits, by ID.
 
         Any ID not found will be ignored.
 
         .. .PARAMETERS
 
-        :param `Iterable[int]` ids:
+        :param `Iterable[_YIntOrStr]` ids:
 
         .. .RETURNS
 
         :returns:
             Iterator of:
 
             * :class:`~.models.subreddit_SYNC.InaccessibleSubreddit` if the subreddit is private or banned.
             * `None` if the subreddit does not exist.
             * :class:`~.models.subreddit_SYNC.Subreddit`
         :rtype: :class:`~.iterators.call_chunk_chaining_iterator.CallChunkChainingIterator`\\[`object`]
         """
-        def mass_fetch(ids: Sequence[int]) -> Sequence[object]:
-            id36s = map(to_base36, ids)
+        def mass_fetch(ids: Sequence[_YIntOrStr]) -> Sequence[object]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
             full_id36s = map('t5_'.__add__, id36s)
             ids_str = ','.join(full_id36s)
             root = self._client.request('GET', '/api/info', params={'id': ids_str})
             return [load_potentially_inaccessible_subreddit(i['data'], self._client) for i in root['data']['children']]
 
-        return CallChunkChainingIterator(CallChunk(mass_fetch, chunk) for chunk in chunked(ids, 100))
+        return CallChunkChainingIterator(CallChunk[Sequence[_YIntOrStr], Sequence[object]](mass_fetch, chunk) for chunk in chunked(ids, 100))
 
     def bulk_fetch_potentially_inaccessible_by_name(self, names: Iterable[str]) -> CallChunkChainingIterator[object]:
         """Bulk fetch information about a potentially inacessible subreddits, by name.
 
         Any name not found will be ignored.
 
         .. .PARAMETERS
@@ -323,20 +329,20 @@
                - You don't have permission to view this subreddit's settings.
         """
         root = self._client.request('GET', f'/r/{sr}/about/edit')
         if root['kind'] != 'subreddit_settings':
             raise exceptions.NoResultException('target not found')
         return root['data']
 
-    def update_settings(self, idn: int, settings: Mapping[str, JSON_ro]) -> None:
+    def update_settings(self, idy: Union[int, str], settings: Mapping[str, JSON_ro]) -> None:
         """Update a subreddit's settings.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param settings:
         :type settings: `Mapping`\\[`str`, :class:`~.types.JSON_ro`]
 
         .. .RETURNS
 
         :rtype: `None`
 
@@ -346,25 +352,25 @@
             + `USER_REQUIRED`:
                 There is no user context.
             + `SUBREDDIT_REQUIRED`:
                 The specified subreddit does not exist.
             + `MOD_REQUIRED`:
                 The current user is not a moderator of the subreddit.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         json: Mapping[str, JSON_ro] = {**settings, 'sr': full_id36}
         self._client.request('PATCH', '/api/v1/subreddit/update_settings', json=json)
 
-    def subscribe_by_id(self, idn: int) -> None:
+    def subscribe_by_id(self, idy: Union[int, str]) -> None:
         """Subscribe to a subreddit.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
 
         .. .RETURNS
 
         :rtype: `None`
 
         .. .RAISES
 
@@ -373,15 +379,15 @@
                 There is no user context.
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `403`:
                 The specified subreddit could not be accessed.
             + `404`:
                 The specified subreddit does not exist.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         self._client.request('POST', '/api/subscribe', data={'action': 'sub', 'sr': full_id36})
 
     def subscribe_by_name(self, name: str) -> None:
         """Subscribe to a subreddit.
 
         .. .PARAMETERS
@@ -403,32 +409,38 @@
                - The specified subreddit was a special name such as `popular`, `all`, or `random`.
 
             + `404`:
                 The specified subreddit does not exist.
         """
         self._client.request('POST', '/api/subscribe', data={'action': 'sub', 'sr_name': name})
 
-    def unsubscribe_by_id(self, idn: int) -> None:
+    def unsubscribe_by_id(self, idy: Union[int, str]) -> None:
         """Unsubscribe from a subreddit.
 
         Behaves similarly to :meth:`.subscribe_by_id`.
         """
-        id36 = to_base36(idn)
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
         full_id36 = 't5_' + id36
         self._client.request('POST', '/api/subscribe', data={'action': 'unsub', 'sr': full_id36})
 
     def unsubscribe_by_name(self, name: str) -> None:
         """Unsubscribe from a subreddit.
 
         Behaves similarly to :meth:`.subscribe_by_name`.
         """
         self._client.request('POST', '/api/subscribe', data={'action': 'unsub', 'sr_name': name})
 
     def get_rules(self, sr: str) -> SubredditRules:
-        """Get a subreddit's rules.
+        r"""Get a subreddit's rules.
+
+        Example::
+
+           rules = client.p.subreddit.get_rules(SR)
+           for i, rule in enumerate(rules, 1):
+               print(f"{i}. {rule.short_name}\n{rule.description}\n")
 
         .. .PARAMETERS
 
         :param `str` sr:
 
         .. .RETURNS
 
@@ -517,27 +529,28 @@
             self._client.request('GET', '/api/search_reddit_names', params={'query': name, 'exact': '1'})
         except http.exceptions.StatusCodeException as e:
             if e.status_code == 404:
                 return False
             raise
         return True
 
-    def get_similar_subreddits(self, idn: int, n: Optional[int] = None) -> Sequence[Subreddit]:
+    def get_similar_subreddits(self, idy: Union[int, str], n: Optional[int] = None) -> Sequence[Subreddit]:
         """Get a list of similar subreddits.
 
         .. .PARAMETERS
 
-        :param `int` idn:
+        :param `Union[int, str]` idy:
         :param `Optional[int]` n:
             The maximum number of entries to return.
 
             Effective default: 10.
 
         .. .RETURNS
 
         :rtype: `Sequence`\\[:class:`~.models.subreddit_SYNC.Subreddit`]
         """
-        params = {'sr_fullnames': 't5_' + to_base36(idn)}
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        params = {'sr_fullnames': 't5_' + id36}
         if n is not None:
             params['max_recs'] = str(n)
         root = self._client.request('GET', '/api/similar_subreddits', params=params)
         return [load_subreddit(d['data'], client=self._client) for d in root['data']['children']]
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pull_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pull_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pull_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pull_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pulls_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pulls_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit/pulls_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit/pulls_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_new/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_new/ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, IO, Optional, Iterable, Protocol
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
-    from ...models.subreddit_style_asset_upload_lease import SubredditStyleAssetUploadLease
+    from ...models.upload_lease import UploadLease
 
 import os.path as op
 from functools import cached_property
 
-from ...model_loaders.subreddit_style_asset_upload_lease import load_subreddit_style_asset_upload_lease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 
 class SubredditStyleNewProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     class BannerUploading:
@@ -21,121 +21,121 @@
 
         async def _obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
             imagetype: str,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = await self._client.request('POST', f'/api/v1/style_asset_upload_s3/{sr}',
                     data={'filepath': filepath, 'mimetype': mimetype, 'imagetype': imagetype})
-            return load_subreddit_style_asset_upload_lease(result)
+            return load_upload_lease(result)
 
         async def obtain_banner_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='bannerBackgroundImage')
 
         async def obtain_banner_overlay_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='bannerPositionedImage')
 
         async def obtain_banner_overlay_hover_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='secondaryBannerPositionedImage')
 
         async def obtain_mobile_banner_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='mobileBannerImage')
 
         async def deposit_file(self,
             file: IO[bytes],
-            upload_lease: SubredditStyleAssetUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = await self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         class ObtainUploadLeaseFunction(Protocol):
             async def __call__(self,
                 *,
                 sr: str,
                 filepath: str,
                 mimetype: Optional[str] = None,
-            ) -> SubredditStyleAssetUploadLease: ...
+            ) -> UploadLease: ...
 
         async def _upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
             obtain_upload_lease: ObtainUploadLeaseFunction,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = await obtain_upload_lease(sr=sr, filepath=filepath)
             await self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
 
         async def upload_banner(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_upload_lease)
 
         async def upload_banner_overlay(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_overlay_upload_lease)
 
         async def upload_banner_overlay_hover(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_overlay_hover_upload_lease)
 
         async def upload_mobile_banner(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return await self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_mobile_banner_upload_lease)
 
     banner_uploading: cached_property[BannerUploading] = cached_property(BannerUploading)
 
     async def modify_banner_settings(self,
         sr: str,
         *,
@@ -161,35 +161,35 @@
 
             Empty string or any other value defaults to `small`.
         :param `Optional[str]` banner_background_color:
             A hex color.
 
             Empty string or any other value defaults to `#33a8ff`.
         :param `Optional[str]` banner_image_url:
-            Location of the a banner image.
+            The URL location of a banner image.
 
             Use empty string to remove the image.
         :param `Optional[str]` banner_image_display:
             Either: `cover`, `tiled`.
 
             Empty string or any other value defaults to `cover`.
         :param `Optional[str]` banner_overlay_image_url:
-            Location of the a banner overlay image.
+            The URL location of a banner overlay image.
 
             Use empty string to remove the image.
         :param `Optional[str]` banner_overlay_image_position:
-            Either: `left`, `centered`, `right`.
+            Either: `left`, `center`, `right`.
 
             Empty string or any other value defaults to `left`.
         :param `Optional[str]` banner_overlay_hover_image_url:
-            The location of the a banner overlay hover image.
+            The URL location of a banner overlay hover image.
 
             Use empty string to remove the image.
         :param `Optional[str]` mobile_banner_image_url:
-            The location of the a mobile banner image.
+            The URL location of a mobile banner image.
 
             Use empty string to remove the image.
 
         .. .RETURNS
 
         :rtype: `None`
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_new/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_new/SYNC.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, IO, Optional, Iterable, Protocol
 if TYPE_CHECKING:
     from ...client_SYNC import Client
-    from ...models.subreddit_style_asset_upload_lease import SubredditStyleAssetUploadLease
+    from ...models.upload_lease import UploadLease
 
 import os.path as op
 from functools import cached_property
 
-from ...model_loaders.subreddit_style_asset_upload_lease import load_subreddit_style_asset_upload_lease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
 
 class SubredditStyleNewProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
 
     class BannerUploading:
@@ -21,121 +21,121 @@
 
         def _obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
             imagetype: str,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = self._client.request('POST', f'/api/v1/style_asset_upload_s3/{sr}',
                     data={'filepath': filepath, 'mimetype': mimetype, 'imagetype': imagetype})
-            return load_subreddit_style_asset_upload_lease(result)
+            return load_upload_lease(result)
 
         def obtain_banner_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='bannerBackgroundImage')
 
         def obtain_banner_overlay_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='bannerPositionedImage')
 
         def obtain_banner_overlay_hover_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='secondaryBannerPositionedImage')
 
         def obtain_mobile_banner_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._obtain_upload_lease(sr=sr, filepath=filepath, mimetype=mimetype, imagetype='mobileBannerImage')
 
         def deposit_file(self,
             file: IO[bytes],
-            upload_lease: SubredditStyleAssetUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         class ObtainUploadLeaseFunction(Protocol):
             def __call__(self,
                 *,
                 sr: str,
                 filepath: str,
                 mimetype: Optional[str] = None,
-            ) -> SubredditStyleAssetUploadLease: ...
+            ) -> UploadLease: ...
 
         def _upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
             obtain_upload_lease: ObtainUploadLeaseFunction,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = obtain_upload_lease(sr=sr, filepath=filepath)
             self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
 
         def upload_banner(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_upload_lease)
 
         def upload_banner_overlay(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_overlay_upload_lease)
 
         def upload_banner_overlay_hover(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_banner_overlay_hover_upload_lease)
 
         def upload_mobile_banner(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> SubredditStyleAssetUploadLease:
+        ) -> UploadLease:
             return self._upload(file=file, sr=sr, filepath=filepath, timeout=timeout, obtain_upload_lease=self.obtain_mobile_banner_upload_lease)
 
     banner_uploading: cached_property[BannerUploading] = cached_property(BannerUploading)
 
     def modify_banner_settings(self,
         sr: str,
         *,
@@ -161,35 +161,35 @@
 
             Empty string or any other value defaults to `small`.
         :param `Optional[str]` banner_background_color:
             A hex color.
 
             Empty string or any other value defaults to `#33a8ff`.
         :param `Optional[str]` banner_image_url:
-            Location of the a banner image.
+            The URL location of a banner image.
 
             Use empty string to remove the image.
         :param `Optional[str]` banner_image_display:
             Either: `cover`, `tiled`.
 
             Empty string or any other value defaults to `cover`.
         :param `Optional[str]` banner_overlay_image_url:
-            Location of the a banner overlay image.
+            The URL location of a banner overlay image.
 
             Use empty string to remove the image.
         :param `Optional[str]` banner_overlay_image_position:
-            Either: `left`, `centered`, `right`.
+            Either: `left`, `center`, `right`.
 
             Empty string or any other value defaults to `left`.
         :param `Optional[str]` banner_overlay_hover_image_url:
-            The location of the a banner overlay hover image.
+            The URL location of a banner overlay hover image.
 
             Use empty string to remove the image.
         :param `Optional[str]` mobile_banner_image_url:
-            The location of the a mobile banner image.
+            The URL location of a mobile banner image.
 
             Use empty string to remove the image.
 
         .. .RETURNS
 
         :rtype: `None`
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_old/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_old/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/subreddit_style_old/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/subreddit_style_old/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/user/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/ASYNC.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,35 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Union, TypeVar, Iterable
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.user_ASYNC import User
     from ...models.moderated_subreddit import ModeratedSubreddit
 
-from .get_user_summary_ASYNC import GetUserSummary
-from .bulk_fetch_user_summary_ASYNC import BulkFetchUserSummary
 from .pull_ASYNC import Pull
 from .pull_subreddits_ASYNC import PullSubreddits
 from ...model_loaders.user_ASYNC import load_user, load_potentially_suspended_user
 from ...model_loaders.moderated_subreddit import load_moderated_subreddit
 from ... import http
 from ...pagination.paginator_chaining_async_iterator import ImpartedPaginatorChainingAsyncIterator
 from ...pagination.paginators.user.async1 import UserSearchAsyncPaginator
 from ...exceptions import RejectedResultException
+from ...models.user_summary import UserSummary
+from ...model_loaders.user_summary import load_user_summary
+from ...util.base_conversion import to_base36
+from ...iterators.chunking import chunked
+from ...iterators.call_chunk_chaining_async_iterator import CallChunkChainingAsyncIterator
+from ...iterators.async_call_chunk import AsyncCallChunk
+
+_YIntOrStr = TypeVar('_YIntOrStr', int, str)
 
 class UserProcedures:
     def __init__(self, client: Client) -> None:
         self._client = client
-        self.get_user_summary: GetUserSummary = GetUserSummary(client)
-        ("""
-            Get a partial user object by ID.
-
-            .. .PARAMETERS
-
-            :param `int` idn:
-
-            .. .RETURNS
-
-            :returns:
-                * :class:`~.models.user_summary.UserSummary`
-                * `None` if the user was not found.
-            :rtype: `Optional`\\[:class:`~.models.user_summary.UserSummary`]
-            """)
-        self.bulk_fetch_user_summary: BulkFetchUserSummary = BulkFetchUserSummary(client)
-        ("""
-            Bulk fetch partial user objects, by ID.
-
-            Any ID that can't be resolved will be ignored.
-            Duplicate IDs in a batch will be ignored.
-
-            .. .PARAMETERS
-
-            :param `Iterable[int]` ids:
-
-            .. .RETURNS
-
-            :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[:class:`~.models.user_summary.UserSummary`]
-            """)
         self.pull: Pull = Pull(client)
         ("""
             Pull submissions and comments associated with a user.
             """)
         self.pull_subreddits: PullSubreddits = PullSubreddits(client)
         ("""
             Get user subreddits.
@@ -155,14 +131,73 @@
         :raises redditwarp.http.exceptions.StatusCodeException:
             + `404`:
                 The specified user was not found.
         """
         root = await self._client.request('GET', f'/user/{name}/about')
         return load_potentially_suspended_user(root['data'], self._client)
 
+    async def get_user_summary(self, idy: Union[int, str]) -> Optional[UserSummary]:
+        """Get a partial user object by ID.
+
+        .. .PARAMETERS
+
+        :param `Union[int, str]` idn:
+
+        .. .RETURNS
+
+        :returns:
+            * :class:`~.models.user_summary.UserSummary`
+            * `None` if the user was not found.
+        :rtype: `Optional`\\[:class:`~.models.user_summary.UserSummary`]
+        """
+        id36 = x if isinstance((x := idy), str) else to_base36(x)
+        full_id36 = 't2_' + id36
+        try:
+            root = await self._client.request('GET', '/api/user_data_by_account_ids',
+                    params={'ids': full_id36})
+        except http.exceptions.StatusCodeException as e:
+            if e.status_code == 404:
+                return None
+            raise
+        obj_data = root[full_id36]
+        return load_user_summary(obj_data, id36)
+
+    def bulk_fetch_user_summary(self, ids: Iterable[_YIntOrStr]) -> CallChunkChainingAsyncIterator[UserSummary]:
+        """
+        Bulk fetch partial user objects, by ID.
+
+        Any ID that can't be resolved will be ignored.
+        Duplicate IDs in a batch will be ignored.
+
+        .. .PARAMETERS
+
+        :param `Iterable[_YIntOrStr]` ids:
+
+        .. .RETURNS
+
+        :rtype: :class:`~.iterators.call_chunk_chaining_async_iterator.CallChunkChainingAsyncIterator`\\[:class:`~.models.user_summary.UserSummary`]
+        """
+        async def mass_fetch_by_id(ids: Sequence[_YIntOrStr]) -> Sequence[UserSummary]:
+            # https://github.com/python/mypy/issues/4134
+            id36s = ((x if isinstance((x := i), str) else to_base36(x)) for i in ids)  # type: ignore[arg-type]
+            full_id36s = map('t2_'.__add__, id36s)
+            ids_str = ','.join(full_id36s)
+
+            try:
+                root = await self._client.request('GET', '/api/user_data_by_account_ids', params={'ids': ids_str})
+            except http.exceptions.StatusCodeException as e:
+                if e.status_code == 404:
+                    # https://github.com/python/mypy/issues/13408
+                    return []  # type: ignore[return-value]
+                raise
+            # https://github.com/python/mypy/issues/13408
+            return [load_user_summary(v, k) for k, v in root.items()]  # type: ignore[return-value]
+
+        return CallChunkChainingAsyncIterator(AsyncCallChunk[Sequence[_YIntOrStr], Sequence[UserSummary]](mass_fetch_by_id, idfs) for idfs in chunked(ids, 100))
+
     async def moderating(self, name: str) -> Sequence[ModeratedSubreddit]:
         """Get a list of partial subreddit objects the target user is a moderator of.
 
         This endpoint isn't very reliable on users with big lists.
 
         The specified user's own user subreddit won't be returned, but any other user
         subreddit they moderate will be.
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/pull_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/pull_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_subreddits_ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/pull_subreddits_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/user/pull_subreddits_SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/user/pull_subreddits_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/widget/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/widget/ASYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     )
     from ...types import JSON_ro
 
 import os.path as op
 from functools import cached_property
 
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
-from ...models.widget.widget_image_upload_lease import WidgetImageUploadLease
+from ...models.upload_lease import UploadLease
 from ...models.widget.ASYNC import WidgetList
-from ...model_loaders.widget import load_widget_image_upload_lease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...model_loaders.widget_ASYNC import (
     load_widget,
     load_text_area_widget,
     load_button_widget,
     load_image_widget,
     load_community_list_widget,
     load_calendar_widget,
@@ -288,46 +288,46 @@
 
         async def __call__(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             return await self.upload(file, sr=sr, filepath=filepath, timeout=timeout)
 
         async def obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = await self._client.request('POST', f'/api/v1/{sr}/emoji_asset_upload_s3',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_widget_image_upload_lease(result)
+            return load_upload_lease(result)
 
         async def deposit_file(self,
             file: IO[bytes],
-            upload_lease: WidgetImageUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = await self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         async def upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = await self.obtain_upload_lease(sr=sr, filepath=filepath)
             await self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/widget/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/widget/SYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     )
     from ...types import JSON_ro
 
 import os.path as op
 from functools import cached_property
 
 from ...http.util.guess_filename_mimetype import guess_filename_mimetype
-from ...models.widget.widget_image_upload_lease import WidgetImageUploadLease
+from ...models.upload_lease import UploadLease
 from ...models.widget.SYNC import WidgetList
-from ...model_loaders.widget import load_widget_image_upload_lease
+from ...model_loaders.upload_lease import load_upload_lease
 from ...model_loaders.widget_SYNC import (
     load_widget,
     load_text_area_widget,
     load_button_widget,
     load_image_widget,
     load_community_list_widget,
     load_calendar_widget,
@@ -288,46 +288,46 @@
 
         def __call__(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             return self.upload(file, sr=sr, filepath=filepath, timeout=timeout)
 
         def obtain_upload_lease(self,
             *,
             sr: str,
             filepath: str,
             mimetype: Optional[str] = None,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             if mimetype is None:
                 mimetype = guess_filename_mimetype(filepath)
             result = self._client.request('POST', f'/api/v1/{sr}/emoji_asset_upload_s3',
                     data={'filepath': filepath, 'mimetype': mimetype})
-            return load_widget_image_upload_lease(result)
+            return load_upload_lease(result)
 
         def deposit_file(self,
             file: IO[bytes],
-            upload_lease: WidgetImageUploadLease,
+            upload_lease: UploadLease,
             *,
             timeout: float = 1000,
         ) -> None:
             resp = self._client.http.request('POST', upload_lease.endpoint,
                     data=upload_lease.fields, files={'file': file}, timeout=timeout)
             resp.ensure_successful_status()
 
         def upload(self,
             file: IO[bytes],
             *,
             sr: str,
             filepath: Optional[str] = None,
             timeout: float = 1000,
-        ) -> WidgetImageUploadLease:
+        ) -> UploadLease:
             if filepath is None:
                 filepath = op.basename(getattr(file, 'name', ''))
                 if not filepath:
                     raise ValueError("the `filepath` parameter must be explicitly specified if the file object has no `name` attribute.")
             upload_lease = self.obtain_upload_lease(sr=sr, filepath=filepath)
             self.deposit_file(file, upload_lease, timeout=timeout)
             return upload_lease
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/wiki/ASYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/wiki/ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/siteprocs/wiki/SYNC.py` & `redditwarp-1.1.0/redditwarp/siteprocs/wiki/SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/message_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/message_ASYNC.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.message_ASYNC import MailboxMessage
-    from ..stream_ASYNC import IStandardStreamEventSubject
+    from ..impls.stream_ASYNC import IStandardStreamEventSubject
     from ...pagination.async_paginator import CursorAsyncPaginator
 
 from ...models.message_ASYNC import ComposedMessage, CommentMessage
-from ..stream_ASYNC import Stream
+from ..impls.stream_ASYNC import SimpleImprintExtractorStream
 
 
-def inbox_message_extractor(x: MailboxMessage) -> object:
-    if isinstance(x, ComposedMessage):
-        return (0, x.id)
-    elif isinstance(x, CommentMessage):
-        return (1, x.comment.id)
-    raise Exception
-
 def get_inbox_message_stream_paginator(client: Client) -> CursorAsyncPaginator[MailboxMessage]:
     return client.p.message.pulls.inbox().get_paginator()
 
-def make_inbox_message_stream(paginator: CursorAsyncPaginator[MailboxMessage], past: Optional[Iterable[MailboxMessage]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[MailboxMessage]:
-    return Stream(paginator, inbox_message_extractor, past=past, seen=seen)
+def make_inbox_message_stream(paginator: CursorAsyncPaginator[MailboxMessage], past: Optional[Iterable[MailboxMessage]] = None) -> IStandardStreamEventSubject[MailboxMessage]:
+    def inbox_message_extractor(x: MailboxMessage) -> object:
+        if isinstance(x, ComposedMessage):
+            return (0, x.id)
+        elif isinstance(x, CommentMessage):
+            return (1, x.comment.id)
+        raise Exception
+    return SimpleImprintExtractorStream(paginator, inbox_message_extractor, past=past)
 
 def create_inbox_message_stream(client: Client) -> IStandardStreamEventSubject[MailboxMessage]:
     return make_inbox_message_stream(get_inbox_message_stream_paginator(client))
 
 
-def mentions_message_extractor(x: CommentMessage) -> object:
-    return x.comment.id
-
 def get_mentions_message_stream_paginator(client: Client) -> CursorAsyncPaginator[CommentMessage]:
     return client.p.message.pulls.mentions().get_paginator()
 
-def make_mentions_message_stream(paginator: CursorAsyncPaginator[CommentMessage], past: Optional[Iterable[CommentMessage]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[CommentMessage]:
-    return Stream(paginator, mentions_message_extractor, past=past, seen=seen)
+def make_mentions_message_stream(paginator: CursorAsyncPaginator[CommentMessage], past: Optional[Iterable[CommentMessage]] = None) -> IStandardStreamEventSubject[CommentMessage]:
+    def mentions_message_extractor(x: CommentMessage) -> object:
+        return x.comment.id
+    return SimpleImprintExtractorStream(paginator, mentions_message_extractor, past=past)
 
 def create_mentions_message_stream(client: Client) -> IStandardStreamEventSubject[CommentMessage]:
     return make_mentions_message_stream(get_mentions_message_stream_paginator(client))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/moderation_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/moderation_ASYNC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.moderation_action_log_entry import ModerationActionLogEntry
-    from ..stream_ASYNC import IStandardStreamEventSubject
+    from ..impls.stream_ASYNC import IStandardStreamEventSubject
     from ...pagination.async_paginator import CursorAsyncPaginator
 
-from ..stream_ASYNC import Stream
+from ..impls.stream_ASYNC import SimpleImprintExtractorStream
 
 
-def action_log_extractor(x: ModerationActionLogEntry) -> object:
-    return x.uuid
-
 def get_action_log_stream_paginator(client: Client, sr: str) -> CursorAsyncPaginator[ModerationActionLogEntry]:
     return client.p.moderation.pull_actions(sr).get_paginator()
 
-def make_action_log_stream(paginator: CursorAsyncPaginator[ModerationActionLogEntry], past: Optional[Iterable[ModerationActionLogEntry]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
-    return Stream(paginator, action_log_extractor, past=past, seen=seen)
+def make_action_log_stream(paginator: CursorAsyncPaginator[ModerationActionLogEntry], past: Optional[Iterable[ModerationActionLogEntry]] = None) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
+    def action_log_extractor(x: ModerationActionLogEntry) -> object:
+        return x.uuid
+    return SimpleImprintExtractorStream(paginator, action_log_extractor, past=past)
 
 def create_action_log_stream(client: Client, sr: str) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
     return make_action_log_stream(get_action_log_stream_paginator(client, sr))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/moderation_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/moderation_SYNC.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.moderation_action_log_entry import ModerationActionLogEntry
-    from ..stream_SYNC import IStandardStreamEventSubject
+    from ..impls.stream_SYNC import IStandardStreamEventSubject
     from ...pagination.paginator import CursorPaginator
 
-from ..stream_SYNC import Stream
+from ..impls.stream_SYNC import SimpleImprintExtractorStream
 
 
-def action_log_extractor(x: ModerationActionLogEntry) -> object:
-    return x.uuid
-
 def get_action_log_stream_paginator(client: Client, sr: str) -> CursorPaginator[ModerationActionLogEntry]:
     return client.p.moderation.pull_actions(sr).get_paginator()
 
-def make_action_log_stream(paginator: CursorPaginator[ModerationActionLogEntry], past: Optional[Iterable[ModerationActionLogEntry]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
-    return Stream(paginator, action_log_extractor, past=past, seen=seen)
+def make_action_log_stream(paginator: CursorPaginator[ModerationActionLogEntry], past: Optional[Iterable[ModerationActionLogEntry]] = None) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
+    def action_log_extractor(x: ModerationActionLogEntry) -> object:
+        return x.uuid
+    return SimpleImprintExtractorStream(paginator, action_log_extractor, past=past)
 
 def create_action_log_stream(client: Client, sr: str) -> IStandardStreamEventSubject[ModerationActionLogEntry]:
     return make_action_log_stream(get_action_log_stream_paginator(client, sr))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/modmail_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/impls/modmail_stream_ASYNC.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, Optional
+from typing import TYPE_CHECKING, Callable, Iterable, Optional, Tuple
 if TYPE_CHECKING:
-    from ...client_SYNC import Client
-    from ...models.modmail_SYNC import ConversationInfo, Message
-    from ..stream_SYNC import IStandardStreamEventSubject
-    from ...pagination.paginator import CursorPaginator
+    from ...pagination.async_paginator import CursorAsyncPaginator
 
-from ..stream_SYNC import Stream
+from ...models.modmail_ASYNC import ConversationInfo, Message
 
+from .stream_ASYNC import CommonStreamBase
 
-def conversation_message_new_extractor(x: tuple[ConversationInfo, Message]) -> object:
-    return (x[0].id, x[1].id)
+class ModmailStream(CommonStreamBase[Tuple[ConversationInfo, Message]]):
+    def __init__(self,
+        paginator: CursorAsyncPaginator[tuple[ConversationInfo, Message]],
+        *,
+        max_limit: int = 100,
+        past: Optional[Iterable[tuple[ConversationInfo, Message]]] = None,
+        memory: int = 2000,
+    ) -> None:
+        super().__init__(
+            paginator,
+            max_limit=max_limit,
+            past=past,
+        )
+
+        def checkin_func_fn(*,
+            memory: int,
+        ) -> Callable[[tuple[ConversationInfo, Message]], bool]:
+            def extractor(x: tuple[ConversationInfo, Message]) -> tuple[object, object]:
+                return (x[0].id, x[1].id)
+
+            seen: dict[object, object] = {}
+
+            def fn(obj: tuple[ConversationInfo, Message]) -> bool:
+                k, v = extractor(obj)
+                if seen.get(k) == v:
+                    return False
+                if len(seen) >= memory:
+                    del seen[next(iter(seen))]
+                seen.pop(k, None)
+                seen[k] = v
+                return True
 
-def get_conversation_message_new_stream_paginator(client: Client) -> CursorPaginator[tuple[ConversationInfo, Message]]:
-    return client.p.modmail.pull.new().get_paginator()
+            return fn
 
-def make_conversation_message_new_stream(paginator: CursorPaginator[tuple[ConversationInfo, Message]], past: Optional[Iterable[tuple[ConversationInfo, Message]]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[tuple[ConversationInfo, Message]]:
-    return Stream(paginator, conversation_message_new_extractor, past=past, seen=seen)
+        self._checkin_func = checkin_func_fn(memory=memory)
 
-def create_conversation_message_new_stream(client: Client) -> IStandardStreamEventSubject[tuple[ConversationInfo, Message]]:
-    return make_conversation_message_new_stream(get_conversation_message_new_stream_paginator(client))
-
-
-def conversation_message_join_request_extractor(x: tuple[ConversationInfo, Message]) -> object:
-    return (x[0].id, x[1].id)
-
-def get_conversation_message_join_request_stream_paginator(client: Client) -> CursorPaginator[tuple[ConversationInfo, Message]]:
-    return client.p.modmail.pull.join_requests().get_paginator()
-
-def make_conversation_message_join_request_stream(paginator: CursorPaginator[tuple[ConversationInfo, Message]], past: Optional[Iterable[tuple[ConversationInfo, Message]]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[tuple[ConversationInfo, Message]]:
-    return Stream(paginator, conversation_message_join_request_extractor, past=past, seen=seen)
-
-def create_conversation_message_join_request_stream(client: Client) -> IStandardStreamEventSubject[tuple[ConversationInfo, Message]]:
-    return make_conversation_message_join_request_stream(get_conversation_message_join_request_stream_paginator(client))
+    def _checkin(self, obj: tuple[ConversationInfo, Message]) -> bool:
+        return self._checkin_func(obj)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/subreddit_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/subreddit_ASYNC.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,50 +2,47 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
     from ...client_ASYNC import Client
     from ...models.submission_ASYNC import Submission
     from ...models.comment_ASYNC import LooseComment
     from ...models.subreddit_ASYNC import Subreddit
-    from ..stream_ASYNC import IStandardStreamEventSubject
+    from ..impls.stream_ASYNC import IStandardStreamEventSubject
     from ...pagination.async_paginator import CursorAsyncPaginator
 
-from ..stream_ASYNC import Stream
+from ..impls.stream_ASYNC import SimpleImprintExtractorStream
 
 
-def submission_stream_extractor(x: Submission) -> object:
-    return x.id
-
 def get_submission_stream_paginator(client: Client, sr: str) -> CursorAsyncPaginator[Submission]:
     return client.p.subreddit.pull.new(sr).get_paginator()
 
-def make_submission_stream(paginator: CursorAsyncPaginator[Submission], past: Optional[Iterable[Submission]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Submission]:
-    return Stream(paginator, submission_stream_extractor, past=past, seen=seen)
+def make_submission_stream(paginator: CursorAsyncPaginator[Submission], past: Optional[Iterable[Submission]] = None) -> IStandardStreamEventSubject[Submission]:
+    def submission_stream_extractor(x: Submission) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, submission_stream_extractor, past=past)
 
 def create_submission_stream(client: Client, sr: str) -> IStandardStreamEventSubject[Submission]:
     return make_submission_stream(get_submission_stream_paginator(client, sr))
 
 
-def comment_stream_extractor(x: LooseComment) -> object:
-    return x.id
-
 def get_comment_stream_paginator(client: Client, sr: str) -> CursorAsyncPaginator[LooseComment]:
     return client.p.subreddit.pull_new_comments(sr).get_paginator()
 
-def make_comment_stream(paginator: CursorAsyncPaginator[LooseComment], past: Optional[Iterable[LooseComment]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[LooseComment]:
-    return Stream(paginator, comment_stream_extractor, past=past, seen=seen)
+def make_comment_stream(paginator: CursorAsyncPaginator[LooseComment], past: Optional[Iterable[LooseComment]] = None) -> IStandardStreamEventSubject[LooseComment]:
+    def comment_stream_extractor(x: LooseComment) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, comment_stream_extractor, past=past)
 
 def create_comment_stream(client: Client, sr: str) -> IStandardStreamEventSubject[LooseComment]:
     return make_comment_stream(get_comment_stream_paginator(client, sr))
 
 
-def subreddit_stream_extractor(x: Subreddit) -> object:
-    return x.id
-
 def get_subreddit_stream_paginator(client: Client) -> CursorAsyncPaginator[Subreddit]:
     return client.p.subreddit.pulls.new().get_paginator()
 
-def make_subreddit_stream(paginator: CursorAsyncPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Subreddit]:
-    return Stream(paginator, subreddit_stream_extractor, past=past, seen=seen)
+def make_subreddit_stream(paginator: CursorAsyncPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None) -> IStandardStreamEventSubject[Subreddit]:
+    def subreddit_stream_extractor(x: Subreddit) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, subreddit_stream_extractor, past=past)
 
 def create_subreddit_stream(client: Client) -> IStandardStreamEventSubject[Subreddit]:
     return make_subreddit_stream(get_subreddit_stream_paginator(client))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/subreddit_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/subreddit_SYNC.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,50 +2,47 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
     from ...client_SYNC import Client
     from ...models.submission_SYNC import Submission
     from ...models.comment_SYNC import LooseComment
     from ...models.subreddit_SYNC import Subreddit
-    from ..stream_SYNC import IStandardStreamEventSubject
+    from ..impls.stream_SYNC import IStandardStreamEventSubject
     from ...pagination.paginator import CursorPaginator
 
-from ..stream_SYNC import Stream
+from ..impls.stream_SYNC import SimpleImprintExtractorStream
 
 
-def submission_stream_extractor(x: Submission) -> object:
-    return x.id
-
 def get_submission_stream_paginator(client: Client, sr: str) -> CursorPaginator[Submission]:
     return client.p.subreddit.pull.new(sr).get_paginator()
 
-def make_submission_stream(paginator: CursorPaginator[Submission], past: Optional[Iterable[Submission]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Submission]:
-    return Stream(paginator, submission_stream_extractor, past=past, seen=seen)
+def make_submission_stream(paginator: CursorPaginator[Submission], past: Optional[Iterable[Submission]] = None) -> IStandardStreamEventSubject[Submission]:
+    def submission_stream_extractor(x: Submission) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, submission_stream_extractor, past=past)
 
 def create_submission_stream(client: Client, sr: str) -> IStandardStreamEventSubject[Submission]:
     return make_submission_stream(get_submission_stream_paginator(client, sr))
 
 
-def comment_stream_extractor(x: LooseComment) -> object:
-    return x.id
-
 def get_comment_stream_paginator(client: Client, sr: str) -> CursorPaginator[LooseComment]:
     return client.p.subreddit.pull_new_comments(sr).get_paginator()
 
-def make_comment_stream(paginator: CursorPaginator[LooseComment], past: Optional[Iterable[LooseComment]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[LooseComment]:
-    return Stream(paginator, comment_stream_extractor, past=past, seen=seen)
+def make_comment_stream(paginator: CursorPaginator[LooseComment], past: Optional[Iterable[LooseComment]] = None) -> IStandardStreamEventSubject[LooseComment]:
+    def comment_stream_extractor(x: LooseComment) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, comment_stream_extractor, past=past)
 
 def create_comment_stream(client: Client, sr: str) -> IStandardStreamEventSubject[LooseComment]:
     return make_comment_stream(get_comment_stream_paginator(client, sr))
 
 
-def subreddit_stream_extractor(x: Subreddit) -> object:
-    return x.id
-
 def get_subreddit_stream_paginator(client: Client) -> CursorPaginator[Subreddit]:
     return client.p.subreddit.pulls.new().get_paginator()
 
-def make_subreddit_stream(paginator: CursorPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Subreddit]:
-    return Stream(paginator, subreddit_stream_extractor, past=past, seen=seen)
+def make_subreddit_stream(paginator: CursorPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None) -> IStandardStreamEventSubject[Subreddit]:
+    def subreddit_stream_extractor(x: Subreddit) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, subreddit_stream_extractor, past=past)
 
 def create_subreddit_stream(client: Client) -> IStandardStreamEventSubject[Subreddit]:
     return make_subreddit_stream(get_subreddit_stream_paginator(client))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/user_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/user_SYNC.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
-    from ...client_ASYNC import Client
-    from ...models.subreddit_ASYNC import Subreddit
-    from ..stream_ASYNC import IStandardStreamEventSubject
-    from ...pagination.async_paginator import CursorAsyncPaginator
+    from ...client_SYNC import Client
+    from ...models.subreddit_SYNC import Subreddit
+    from ..impls.stream_SYNC import IStandardStreamEventSubject
+    from ...pagination.paginator import CursorPaginator
 
-from ..stream_ASYNC import Stream
+from ..impls.stream_SYNC import SimpleImprintExtractorStream
 
 
-def user_subreddit_stream_extractor(x: Subreddit) -> object:
-    return x.id
-
-def get_user_subreddit_stream_paginator(client: Client) -> CursorAsyncPaginator[Subreddit]:
+def get_user_subreddit_stream_paginator(client: Client) -> CursorPaginator[Subreddit]:
     return client.p.user.pull_subreddits.new().get_paginator()
 
-def make_user_subreddit_stream(paginator: CursorAsyncPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Subreddit]:
-    return Stream(paginator, user_subreddit_stream_extractor, past=past, seen=seen)
+def make_user_subreddit_stream(paginator: CursorPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None) -> IStandardStreamEventSubject[Subreddit]:
+    def user_subreddit_stream_extractor(x: Subreddit) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, user_subreddit_stream_extractor, past=past)
 
 def create_user_subreddit_stream(client: Client) -> IStandardStreamEventSubject[Subreddit]:
     return make_user_subreddit_stream(get_user_subreddit_stream_paginator(client))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/makers/user_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/makers/user_ASYNC.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
 if TYPE_CHECKING:
-    from ...client_SYNC import Client
-    from ...models.subreddit_SYNC import Subreddit
-    from ..stream_SYNC import IStandardStreamEventSubject
-    from ...pagination.paginator import CursorPaginator
+    from ...client_ASYNC import Client
+    from ...models.subreddit_ASYNC import Subreddit
+    from ..impls.stream_ASYNC import IStandardStreamEventSubject
+    from ...pagination.async_paginator import CursorAsyncPaginator
 
-from ..stream_SYNC import Stream
+from ..impls.stream_ASYNC import SimpleImprintExtractorStream
 
 
-def user_subreddit_stream_extractor(x: Subreddit) -> object:
-    return x.id
-
-def get_user_subreddit_stream_paginator(client: Client) -> CursorPaginator[Subreddit]:
+def get_user_subreddit_stream_paginator(client: Client) -> CursorAsyncPaginator[Subreddit]:
     return client.p.user.pull_subreddits.new().get_paginator()
 
-def make_user_subreddit_stream(paginator: CursorPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None, seen: Optional[Iterable[object]] = None) -> IStandardStreamEventSubject[Subreddit]:
-    return Stream(paginator, user_subreddit_stream_extractor, past=past, seen=seen)
+def make_user_subreddit_stream(paginator: CursorAsyncPaginator[Subreddit], past: Optional[Iterable[Subreddit]] = None) -> IStandardStreamEventSubject[Subreddit]:
+    def user_subreddit_stream_extractor(x: Subreddit) -> object:
+        return x.id
+    return SimpleImprintExtractorStream(paginator, user_subreddit_stream_extractor, past=past)
 
 def create_user_subreddit_stream(client: Client) -> IStandardStreamEventSubject[Subreddit]:
     return make_user_subreddit_stream(get_user_subreddit_stream_paginator(client))
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/runners_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/runners_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/runners_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/runners_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/stream_ASYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/impls/stream_ASYNC.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Sequence, MutableSequence, Callable, Generic, TypeVar, Protocol, Awaitable, Generator, Optional, Iterator, AsyncIterator, Iterable
 if TYPE_CHECKING:
     from asyncio import Future
-    from ..pagination.async_paginator import CursorAsyncPaginator
+    from ...pagination.async_paginator import CursorAsyncPaginator
 
 import asyncio
 import random
 import time
 
-from ..pagination.async_paginator import Resettable
-from ..util.ordered_set import BoundedSet
-from ..util.event_dispatcher import EventDispatcher
+from ...pagination.async_paginator import Resettable
+from ...util.ordered_set import OrderedSet
+from ...util.event_dispatcher import EventDispatcher
 
 
 TEvent_contra = TypeVar('TEvent_contra', contravariant=True)
 TEvent = TypeVar('TEvent')
 
 class StreamEventHandlerProtocol(Protocol[TEvent_contra]):
     async def __call__(self, event: TEvent_contra, /) -> None:
@@ -43,49 +43,40 @@
         async def coro_fn() -> None:
             async for s in self:
                 await asyncio.sleep(s)
         return coro_fn().__await__()
 
 
 
-class Stream(IStandardStreamEventSubject[TOutput]):
+class CommonStreamBase(IStandardStreamEventSubject[TOutput]):
     _BASE_POLL_INTERVAL: float = 5.0
     _MAX_POLL_INTERVAL: float = 50.0
     _BACKOFF_FACTOR: float =  2.0
     _JITTER_FACTOR: float = 0.4
 
-    _MEMORY: int = 2000
     _TARGET_LIMIT_MULTIPLIER: float = 1.2
 
     _BACKTRACK_DEPTH: int = 300
 
     def __init__(self,
         paginator: CursorAsyncPaginator[TOutput],
-        extractor: Callable[[TOutput], object],
         *,
         max_limit: int = 100,
         past: Optional[Iterable[TOutput]] = None,
-        seen: Optional[Iterable[object]] = None,
     ) -> None:
-        if None not in (past, seen):
-            raise TypeError("mutually exclusive parameters: `past`, `seen`")
         if not isinstance(paginator, Resettable):
             raise ValueError('paginator must be Resettable')
 
         self._paginator: CursorAsyncPaginator[TOutput] = paginator
         self._paginator__resettable: Resettable = paginator
-        self._extractor: Callable[[TOutput], object] = extractor
         self._max_limit: int = max_limit
 
-        init_seen: Iterable[object] = ()
-        if seen is not None:
-            init_seen = seen
-        elif past is not None:
-            init_seen = map(extractor, past)
-        self._init_seen: Iterable[object] = init_seen
+        if past is not None:
+            for obj in past:
+                self._checkin(obj)
 
         self._agen: AsyncIterator[float] = self.__routine()
 
         self.output: StreamEventDispatcher[TOutput] = StreamEventDispatcher()
         ("")
         self.error: StreamEventDispatcher[Exception] = StreamEventDispatcher()
         ("")
@@ -96,50 +87,50 @@
     @staticmethod
     def _intermit(duration: float) -> Iterator[float]:
         point = time.monotonic() + duration
         yield duration
         while (n := point - time.monotonic()) > 0:
             yield n
 
+    def _checkin(self, obj: TOutput) -> bool:
+        raise NotImplementedError
+
     async def __routine(self) -> AsyncIterator[float]:
         paginator = self._paginator
         paginator__resettable = self._paginator__resettable
-        extractor = self._extractor
         max_limit = self._max_limit
 
-        seen: BoundedSet[object] = BoundedSet(self._init_seen, self._MEMORY)
         delay: float = self._BASE_POLL_INTERVAL
 
         paginator.limit = max_limit
 
         retrieved: Sequence[TOutput] = ()
 
-        if not paginator.get_cursor():
-            while True:
-                try:
-                    retrieved = await paginator.fetch()
-                except Exception as error:
-                    await self.emit_error(error)
-                    if delay < self._MAX_POLL_INTERVAL:
-                        delay = min(self._BACKOFF_FACTOR * delay, self._MAX_POLL_INTERVAL)
-                    for v in self._intermit(random.uniform(
-                            delay * (1 - self._JITTER_FACTOR),
-                            delay * (1 + self._JITTER_FACTOR))):
-                        yield v
-                    continue
-                break
+        while True:
+            try:
+                retrieved = await paginator.fetch()
+            except Exception as error:
+                await self.emit_error(error)
+                if delay < self._MAX_POLL_INTERVAL:
+                    delay = min(self._BACKOFF_FACTOR * delay, self._MAX_POLL_INTERVAL)
+                for v in self._intermit(random.uniform(
+                        delay * (1 - self._JITTER_FACTOR),
+                        delay * (1 + self._JITTER_FACTOR))):
+                    yield v
+                continue
+            break
 
-            delay = self._BASE_POLL_INTERVAL
+        delay = self._BASE_POLL_INTERVAL
 
-            paginator__resettable.reset()
+        paginator__resettable.reset()
 
-            for obj in retrieved:
-                seen.add(extractor(obj))
+        for obj in retrieved:
+            self._checkin(obj)
 
-            yield 0
+        yield 0
 
         tuna_limit: float = max_limit
         backtrack_count: int = 0
 
         while True:
             effective_limit = round(tuna_limit)
             paginator.limit = effective_limit
@@ -150,17 +141,15 @@
                 retrieved = await paginator.fetch()
             except Exception as error:
                 fetch_successful = False
                 await self.emit_error(error)
 
             selection: MutableSequence[TOutput] = []
             for obj in retrieved:
-                imprint = self._extractor(obj)
-                if imprint not in seen:
-                    seen.add(imprint)
+                if self._checkin(obj):
                     selection.append(obj)
 
             for obj in selection:
                 await self.emit_output(obj)
 
             backtrack_count += len(selection)
 
@@ -193,7 +182,45 @@
                 yield v
 
     async def emit_output(self, output: TOutput) -> None:
         await self.output(output)
 
     async def emit_error(self, error: Exception) -> None:
         await self.error(error)
+
+
+class SimpleImprintExtractorStream(CommonStreamBase[TOutput]):
+    def __init__(self,
+        paginator: CursorAsyncPaginator[TOutput],
+        extractor: Callable[[TOutput], object],
+        *,
+        max_limit: int = 100,
+        past: Optional[Iterable[TOutput]] = None,
+        memory: int = 2000,
+    ) -> None:
+        super().__init__(
+            paginator,
+            max_limit=max_limit,
+            past=past,
+        )
+
+        def checkin_func_fn(*,
+            extractor: Callable[[TOutput], object],
+            memory: int,
+        ) -> Callable[[TOutput], bool]:
+            seen: OrderedSet[object] = OrderedSet()
+
+            def fn(obj: TOutput) -> bool:
+                imprint = extractor(obj)
+                if imprint in seen:
+                    return False
+                if len(seen) >= memory:
+                    seen.remove(next(iter(seen)))
+                seen.add(imprint)
+                return True
+
+            return fn
+
+        self._checkin_func = checkin_func_fn(extractor=extractor, memory=memory)
+
+    def _checkin(self, obj: TOutput) -> bool:
+        return self._checkin_func(obj)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/streaming/stream_SYNC.py` & `redditwarp-1.1.0/redditwarp/streaming/impls/stream_SYNC.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Sequence, MutableSequence, Callable, Generic, TypeVar, Iterator, Protocol, Iterable, Optional
 if TYPE_CHECKING:
-    from ..pagination.paginator import CursorPaginator
+    from ...pagination.paginator import CursorPaginator
 
 import random
 import time
 
-from ..pagination.paginator import Resettable
-from ..util.ordered_set import BoundedSet
-from ..util.event_dispatcher import EventDispatcher
+from ...pagination.paginator import Resettable
+from ...util.ordered_set import OrderedSet
+from ...util.event_dispatcher import EventDispatcher
 
 
 TEvent_contra = TypeVar('TEvent_contra', contravariant=True)
 TEvent = TypeVar('TEvent')
 
 class StreamEventHandlerProtocol(Protocol[TEvent_contra]):
     def __call__(self, event: TEvent_contra, /) -> None:
@@ -35,49 +35,40 @@
         return self
 
     def __next__(self) -> float:
         raise NotImplementedError
 
 
 
-class Stream(IStandardStreamEventSubject[TOutput]):
+class CommonStreamBase(IStandardStreamEventSubject[TOutput]):
     _BASE_POLL_INTERVAL: float = 5.0
     _MAX_POLL_INTERVAL: float = 50.0
     _BACKOFF_FACTOR: float =  2.0
     _JITTER_FACTOR: float = 0.4
 
-    _MEMORY: int = 2000
     _TARGET_LIMIT_MULTIPLIER: float = 1.2
 
     _BACKTRACK_DEPTH: int = 300
 
     def __init__(self,
         paginator: CursorPaginator[TOutput],
-        extractor: Callable[[TOutput], object],
         *,
         max_limit: int = 100,
         past: Optional[Iterable[TOutput]] = None,
-        seen: Optional[Iterable[object]] = None,
     ) -> None:
-        if None not in (past, seen):
-            raise TypeError("mutually exclusive parameters: `past`, `seen`")
         if not isinstance(paginator, Resettable):
             raise ValueError('paginator must be Resettable')
 
         self._paginator: CursorPaginator[TOutput] = paginator
         self._paginator__resettable: Resettable = paginator
-        self._extractor: Callable[[TOutput], object] = extractor
         self._max_limit: int = max_limit
 
-        init_seen: Iterable[object] = ()
-        if seen is not None:
-            init_seen = seen
-        elif past is not None:
-            init_seen = map(extractor, past)
-        self._init_seen: Iterable[object] = init_seen
+        if past is not None:
+            for obj in past:
+                self._checkin(obj)
 
         self._gen: Iterator[float] = self._routine()
 
         self.output: StreamEventDispatcher[TOutput] = StreamEventDispatcher()
         ("")
         self.error: StreamEventDispatcher[Exception] = StreamEventDispatcher()
         ("")
@@ -88,49 +79,49 @@
     @staticmethod
     def _intermit(duration: float) -> Iterator[float]:
         point = time.monotonic() + duration
         yield duration
         while (n := point - time.monotonic()) > 0:
             yield n
 
+    def _checkin(self, obj: TOutput) -> bool:
+        raise NotImplementedError
+
     def _routine(self) -> Iterator[float]:
         paginator = self._paginator
         paginator__resettable = self._paginator__resettable
-        extractor = self._extractor
         max_limit = self._max_limit
 
-        seen: BoundedSet[object] = BoundedSet(self._init_seen, self._MEMORY)
         delay: float = self._BASE_POLL_INTERVAL
 
         paginator.limit = max_limit
 
         retrieved: Sequence[TOutput] = ()
 
-        if not paginator.get_cursor():
-            while True:
-                try:
-                    retrieved = paginator.fetch()
-                except Exception as error:
-                    self.emit_error(error)
-                    if delay < self._MAX_POLL_INTERVAL:
-                        delay = min(self._BACKOFF_FACTOR * delay, self._MAX_POLL_INTERVAL)
-                    yield from self._intermit(random.uniform(
-                        delay * (1 - self._JITTER_FACTOR),
-                        delay * (1 + self._JITTER_FACTOR)))
-                    continue
-                break
+        while True:
+            try:
+                retrieved = paginator.fetch()
+            except Exception as error:
+                self.emit_error(error)
+                if delay < self._MAX_POLL_INTERVAL:
+                    delay = min(self._BACKOFF_FACTOR * delay, self._MAX_POLL_INTERVAL)
+                yield from self._intermit(random.uniform(
+                    delay * (1 - self._JITTER_FACTOR),
+                    delay * (1 + self._JITTER_FACTOR)))
+                continue
+            break
 
-            delay = self._BASE_POLL_INTERVAL
+        delay = self._BASE_POLL_INTERVAL
 
-            paginator__resettable.reset()
+        paginator__resettable.reset()
 
-            for obj in retrieved:
-                seen.add(extractor(obj))
+        for obj in retrieved:
+            self._checkin(obj)
 
-            yield 0
+        yield 0
 
         tuna_limit: float = max_limit
         backtrack_count: int = 0
 
         while True:
             effective_limit = round(tuna_limit)
             paginator.limit = effective_limit
@@ -141,17 +132,15 @@
                 retrieved = paginator.fetch()
             except Exception as error:
                 fetch_successful = False
                 self.emit_error(error)
 
             selection: MutableSequence[TOutput] = []
             for obj in retrieved:
-                imprint = self._extractor(obj)
-                if imprint not in seen:
-                    seen.add(imprint)
+                if self._checkin(obj):
                     selection.append(obj)
 
             for obj in selection:
                 self.emit_output(obj)
 
             backtrack_count += len(selection)
 
@@ -183,7 +172,45 @@
             yield from self._intermit(t)
 
     def emit_output(self, output: TOutput) -> None:
         self.output(output)
 
     def emit_error(self, error: Exception) -> None:
         self.error(error)
+
+
+class SimpleImprintExtractorStream(CommonStreamBase[TOutput]):
+    def __init__(self,
+        paginator: CursorPaginator[TOutput],
+        extractor: Callable[[TOutput], object],
+        *,
+        max_limit: int = 100,
+        past: Optional[Iterable[TOutput]] = None,
+        memory: int = 2000,
+    ) -> None:
+        super().__init__(
+            paginator,
+            max_limit=max_limit,
+            past=past,
+        )
+
+        def checkin_func_fn(*,
+            extractor: Callable[[TOutput], object],
+            memory: int,
+        ) -> Callable[[TOutput], bool]:
+            seen: OrderedSet[object] = OrderedSet()
+
+            def fn(obj: TOutput) -> bool:
+                imprint = extractor(obj)
+                if imprint in seen:
+                    return False
+                if len(seen) >= memory:
+                    seen.remove(next(iter(seen)))
+                seen.add(imprint)
+                return True
+
+            return fn
+
+        self._checkin_func = checkin_func_fn(extractor=extractor, memory=memory)
+
+    def _checkin(self, obj: TOutput) -> bool:
+        return self._checkin_func(obj)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/attribute_mapping_proxy.py` & `redditwarp-1.1.0/redditwarp/util/attribute_mapping_proxy.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/base_conversion.py` & `redditwarp-1.1.0/redditwarp/util/base_conversion.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/booleanify.py` & `redditwarp-1.1.0/redditwarp/util/booleanify.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/data_members_namespace.py` & `redditwarp-1.1.0/redditwarp/util/data_members_namespace.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/event_dispatcher.py` & `redditwarp-1.1.0/redditwarp/util/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/except_without_context.py` & `redditwarp-1.1.0/redditwarp/util/except_without_context.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/extract_id_from_url.py` & `redditwarp-1.1.0/redditwarp/util/extract_id_from_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Extract the ID from a Reddit submission or comment URL."""
 
 import urllib.parse
 from pathlib import Path
 from collections import deque
 
-def extract_submission_id_from_url(url: str) -> int:
+def extract_submission_id36_from_url(url: str) -> str:
     urlparts = urllib.parse.urlsplit(url)
     if urlparts.scheme not in {'https', 'http'}:
         raise ValueError
     if urlparts.netloc not in {'www.reddit.com', 'reddit.com', 'redd.it', 'ssl.reddit.com'}:
         raise ValueError
 
     parts = deque(Path(urlparts.path).parts)
@@ -39,17 +39,25 @@
             if parts:
                 raise ValueError
     else:
         val = t
         if parts:
             raise ValueError
 
-    return int(val, 36)
+    return val
 
-def extract_comment_id_from_url(url: str) -> int:
+def extract_submission_idn_from_url(url: str) -> int:
+    return int(extract_submission_id36_from_url(url), 36)
+
+def extract_submission_id_from_url(url: str) -> int:
+    """Alias of :func:`extract_submission_idn_from_url`."""
+    return extract_submission_idn_from_url(url)
+
+
+def extract_comment_id36_from_url(url: str) -> str:
     urlparts = urllib.parse.urlsplit(url)
     if urlparts.scheme not in {'https', 'http'}:
         raise ValueError
     if urlparts.netloc not in {'www.reddit.com', 'reddit.com', 'redd.it', 'ssl.reddit.com'}:
         raise ValueError
 
     parts = deque(Path(urlparts.path).parts)
@@ -73,8 +81,15 @@
         comments = popq()
         if comments != 'comments':
             raise ValueError
         popq()  # submission ID36
         popq()  # slug
         val = popq()
 
-    return int(val, 36)
+    return val
+
+def extract_comment_idn_from_url(url: str) -> int:
+    return int(extract_comment_id36_from_url(url), 36)
+
+def extract_comment_id_from_url(url: str) -> int:
+    """Alias of :func:`extract_comment_idn_from_url`."""
+    return extract_comment_idn_from_url(url)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/imports.py` & `redditwarp-1.1.0/redditwarp/util/imports.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/ordered_set.py` & `redditwarp-1.1.0/redditwarp/util/ordered_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """An ordered set implementation."""
 
 from __future__ import annotations
-from typing import TypeVar, Iterator, Iterable, MutableSet
+from typing import TypeVar, Iterator, Iterable, MutableSet, Reversible
 
 from itertools import islice
 
 T = TypeVar('T')
 
-class OrderedSet(MutableSet[T]):
+class OrderedSet(Reversible[T], MutableSet[T]):
     """An ordered set.
 
     An ordered set is a set that remembers insertion order.
     """
 
-    def __init__(self, it: Iterable[T]) -> None:
+    def __init__(self, it: Iterable[T] = ()) -> None:
         store: dict[T, None] = {}
         self._store = store
         for i in it:
             store[i] = None
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({list(self)})'
@@ -27,14 +27,17 @@
 
     def __contains__(self, item: object) -> bool:
         return item in self._store
 
     def __iter__(self) -> Iterator[T]:
         return iter(self._store)
 
+    def __reversed__(self) -> Iterator[T]:
+        return reversed(self._store)
+
     def add(self, value: T) -> None:
         self._store[value] = None
 
     def discard(self, value: T) -> None:
         self._store.pop(value, None)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/passthru.py` & `redditwarp-1.1.0/redditwarp/util/passthru.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/praw_config.py` & `redditwarp-1.1.0/redditwarp/util/praw_config.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/praw_config_ASYNC.py` & `redditwarp-1.1.0/redditwarp/util/praw_config_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/praw_config_SYNC.py` & `redditwarp-1.1.0/redditwarp/util/praw_config_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/shdlr.py` & `redditwarp-1.1.0/redditwarp/util/shdlr.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/shdlr_ctx.py` & `redditwarp-1.1.0/redditwarp/util/shdlr_ctx.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/util/token_bucket.py` & `redditwarp-1.1.0/redditwarp/util/token_bucket.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/const.py` & `redditwarp-1.1.0/redditwarp/websocket/const.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/events.py` & `redditwarp-1.1.0/redditwarp/websocket/events.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/aiohttp.py` & `redditwarp-1.1.0/redditwarp/websocket/transport/carriers/aiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             self.state = ConnectionState.CLOSED
             yield events.ConnectionClosed()
         elif wsm.type == aiohttp.WSMsgType.ERROR:
             raise exceptions.TransportError from wsm.data
 
     async def close(self, code: Optional[int] = 1000, reason: str = '', *, waitfor: float = -2) -> None:
         if code is None:
-            raise RuntimeError('must specify a close code with aiohttp library websockets')
+            raise RuntimeError('must specify a close code with aiohttp library')
 
         t: Optional[float] = waitfor
         if waitfor == -2:
             t = self.default_waittime
         elif waitfor == -1:
             t = None
         elif waitfor < 0:
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/websocket.py` & `redditwarp-1.1.0/redditwarp/websocket/transport/carriers/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         self.close_code: int
         self.close_reason: str
         self.close_code, self.close_reason = parse_close(m.data)
         self.state = ConnectionState.CLOSED
         yield events.ConnectionClosed()
 
     def _send_close_frame_impl(self, code: Optional[int] = 1000, reason: str = '') -> None:
+        if code is None:
+            raise RuntimeError('must specify a close code with websocket-client library')
+
         try:
             self.ws.send_close(code, reason.encode())
         except Exception as cause:
             raise exceptions.TransportError from cause
 
     def close(self, code: Optional[int] = 1000, reason: str = '', *, waitfor: float = -2) -> None:
         super().close(code, reason, waitfor=waitfor)
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/transport/carriers/websockets.py` & `redditwarp-1.1.0/redditwarp/websocket/transport/carriers/websockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             if isinstance(data, str):
                 yield TextMessage(data)
             else:
                 yield BytesMessage(data)
 
     async def close(self, code: Optional[int] = 1000, reason: str = '', *, waitfor: float = -2) -> None:
         if code is None:
-            raise RuntimeError('must specify a close code with websockets library websockets')
+            raise RuntimeError('must specify a close code with websockets library')
 
         t: Optional[float] = waitfor
         if waitfor == -2:
             t = self.default_waittime
         elif waitfor == -1:
             t = None
         elif waitfor < 0:
```

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/transport/reg_ASYNC.py` & `redditwarp-1.1.0/redditwarp/websocket/transport/reg_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/transport/reg_SYNC.py` & `redditwarp-1.1.0/redditwarp/websocket/transport/reg_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/utils.py` & `redditwarp-1.1.0/redditwarp/websocket/utils.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/websocket_ASYNC.py` & `redditwarp-1.1.0/redditwarp/websocket/websocket_ASYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/redditwarp/websocket/websocket_SYNC.py` & `redditwarp-1.1.0/redditwarp/websocket/websocket_SYNC.py`

 * *Files identical despite different names*

### Comparing `redditwarp-1.0.0rc0/setup.py` & `redditwarp-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,35 +46,37 @@
  'redditwarp.siteprocs.front',
  'redditwarp.siteprocs.live_thread',
  'redditwarp.siteprocs.message',
  'redditwarp.siteprocs.misc',
  'redditwarp.siteprocs.moderation',
  'redditwarp.siteprocs.modmail',
  'redditwarp.siteprocs.submission',
+ 'redditwarp.siteprocs.submission.create',
  'redditwarp.siteprocs.subreddit',
  'redditwarp.siteprocs.subreddit_style_new',
  'redditwarp.siteprocs.subreddit_style_old',
  'redditwarp.siteprocs.user',
  'redditwarp.siteprocs.widget',
  'redditwarp.siteprocs.wiki',
  'redditwarp.streaming',
+ 'redditwarp.streaming.impls',
  'redditwarp.streaming.makers',
  'redditwarp.util',
  'redditwarp.websocket',
  'redditwarp.websocket.transport',
  'redditwarp.websocket.transport.carriers']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'redditwarp',
-    'version': '1.0.0rc0',
+    'version': '1.1.0',
     'description': 'A library for interacting with the Reddit API.',
-    'long_description': '\n# RedditWarp\n\n[![Latest version](https://img.shields.io/pypi/v/redditwarp)](https://pypi.org/p/redditwarp/)\n![Supported Python versions](https://img.shields.io/pypi/pyversions/redditwarp)\n[![Discord guild](https://img.shields.io/discord/1084793643673600062?logo=discord&logoColor=white&logoWidth=20&label=&labelColor=5865F2&color=7289DA)](http://pyprohly.github.io/redditwarp/discord-invite)\n\nA comprehensive, type-complete, easy-to-learn Python Reddit API wrapper.\n\nRedditWarp is a Python library that simplifies working with the Reddit API.\nIt handles the complexities of the Reddit API in a way that is comprehensive,\nhighly discoverable, and static-type conscious. It includes a variety of useful\ntools to facilitate a wide range of use cases, and even provides tools for\naccessing the API in ways previously not possible.\n\nLook how easy it is to use:\n\n```python\nimport redditwarp.SYNC\n\nclient = redditwarp.SYNC.Client()\n\nit = client.p.front.pull.hot(5)\nl = list(it)\nfor subm in l:\n    print("r/{0.subreddit.name} | {0.id36}+ ^{0.score} | {0.title!r:.80}".format(subm))\n```\n\n## Features\n\n* A consistent and easy-to-use programming interface.\n* Modern type-complete codebase.\n* Sync and asynchronous IO support.\n* Automatic rate limit handling.\n* A comprehensive and discoverable index of API procedures.\n* Model classes that sensibly wrap API structures.\n* Formal data structures to facilitate comment tree traversals and pagination.\n* HTTP transport library agnosticism.\n* OAuth2 tooling and CLI utilities to help manage auth tokens.\n* A simple event-based listing endpoint streaming framework.\n\n## Installation\n\n**Requires Python 3.8+.**\nType annotations may use 3.9 features.\nCode examples will assume 3.10.\n\nInstall/update:\n\n    pip install -U redditwarp\n\n## Demonstration\n\n<details open>\n  <summary>Examples</summary>\n\n```python\nimport redditwarp.SYNC\n\nclient = redditwarp.SYNC.Client()\n\n# Display the first 5 submissions on the Reddit frontpage.\nit = client.p.front.pull.hot(5)\nl = list(it)\nfor subm in l:\n    print("r/{0.subreddit.name} | {0.id36}+ ^{0.score} | {0.title!r:.80}".format(subm))\n\n# How many subscribers does r/Python have?\nsubr = client.p.subreddit.fetch_by_name(\'Python\')\nprint(subr.subscriber_count)\n\n# Display the top submission of the week in the r/YouShouldKnow subreddit.\nm = next(client.p.subreddit.pull.top(\'YouShouldKnow\', amount=1, time=\'week\'))\nprint(f\'\'\'\\\n{m.permalink}\n{m.id36}+ ^{m.score} | {m.title}\nSubmitted {m.created_at.astimezone().ctime()}{\' *\' if m.is_edited else \'\'} \\\nby u/{m.author_display_name} to r/{m.subreddit.name}\n\'\'\')\n\n# Get the first comment of a submission.\ntree_node = client.p.comment_tree.fetch(int(\'uc8i1g\', 36), sort=\'top\', limit=1)\nc = tree_node.children[0].value\nprint(f\'\'\'\\\n{c.submission.id36}+{c.id36} ^{c.score}\nu/{c.author_display_name} says:\n{c.body}\n\'\'\')\n\n# List the moderators of r/redditdev.\nit1 = client.p.moderation.pull_users.moderators(\'redditdev\')\nfor mod in it1:\n    print(mod.name)\n```\n\n</details>\n\n<details>\n  <summary>More examples</summary>\n\n```python\n# ...\n\n# Need credentials for these next few API calls.\nCLIENT_ID = \'...\'\nCLIENT_SECRET = \'...\'\nREFRESH_TOKEN = \'...\'\nclient1 = redditwarp.SYNC.Client(CLIENT_ID, CLIENT_SECRET, REFRESH_TOKEN)\n\n# Who am I?\nme = client1.p.account.fetch()\nprint(f"Hello u/{me.name}!")\n\n# Show my last 5 comments.\nit2 = client.p.user.pull.comments(me.name, 5)\nfor comm in it2:\n    print(\'###\')\n    print(comm.body)\n\n# Show my last 10 saved items.\nfrom redditwarp.models.submission_SYNC import Submission\nfrom redditwarp.models.comment_SYNC import Comment\nit3 = client1.p.user.pull.saved(me.name, 10)\nl = list(it3)\nfor obj in l:\n    print(\'###\')\n    match obj:\n        case Submission() as m:\n            print(f\'\'\'\\\n{m.permalink}\n{m.id36}+ ^{m.score} | {m.title}\nSubmitted {m.created_at.astimezone().ctime()}{\' *\' if m.is_edited else \'\'} \\\nby u/{m.author_display_name} to r/{m.subreddit.name}\n\'\'\')\n        case Comment() as c:\n            print(f\'\'\'\\\n{c.permalink}\n{c.submission.id36}+{c.id36} ^{c.score}\nu/{c.author_display_name} says:\n{c.body}\n\'\'\')\n\n# Submit a link post to r/test.\nsubm_id = client1.p.submission.create_link_post(\'test\',\n        "Check out this cool website", "https://www.reddit.com")\n\n# Reply to a submission.\nfrom redditwarp.util.extract_id_from_url import extract_submission_id_from_url\nidn = extract_submission_id_from_url("https://www.reddit.com/comments/5e1az9")\ncomm1 = client1.p.submission.reply(idn, "Pretty cool stuff!")\n\n# Delete the post and the comment reply.\nclient1.p.submission.delete(subm_id)\nclient1.p.comment.delete(comm1.id)\n```\n\n</details>\n\n<details>\n  <summary>Streaming example</summary>\n\n```python\n#!/usr/bin/env python\nfrom __future__ import annotations\nfrom typing import TYPE_CHECKING\nif TYPE_CHECKING:\n    from redditwarp.models.submission_ASYNC import Submission\n\nimport asyncio\n\nimport redditwarp.ASYNC\nfrom redditwarp.streaming.makers.subreddit_ASYNC import create_submission_stream\nfrom redditwarp.streaming.ASYNC import flow\n\nasync def main() -> None:\n    client = redditwarp.ASYNC.Client()\n    async with client:\n        submission_stream = create_submission_stream(client, \'AskReddit\')\n\n        @submission_stream.output.attach\n        async def _(subm: Submission) -> None:\n            print(subm.id36, \'~\', subm.title)\n\n        @submission_stream.error.attach\n        async def _(exc: Exception) -> None:\n            print(\'ERROR:\', repr(exc))\n\n        await flow(submission_stream)\n\nasyncio.run(main())\n```\n\n</details>\n\n## Support\n\nPost any questions you have to [r/redditdev].\n\n[r/redditdev]: https://www.reddit.com/r/redditdev/\n\nJoin the conversation in the RedditWarp [Discord guild].\n\n[Discord guild]: http://pyprohly.github.io/redditwarp/discord-invite\n\n## Links\n\n* [Repository](https://github.com/Pyprohly/redditwarp)\n* [PyPI](https://pypi.org/p/redditwarp/)\n* [Documentation](https://redditwarp.readthedocs.io/)\n* [r/redditdev]\n* [Discord guild]\n',
+    'long_description': '\n# RedditWarp\n\n[![Latest version](https://img.shields.io/pypi/v/redditwarp)](https://pypi.org/p/redditwarp/)\n![Supported Python versions](https://img.shields.io/pypi/pyversions/redditwarp)\n[![Discord guild](https://img.shields.io/discord/1084793643673600062?logo=discord&logoColor=white&logoWidth=20&label=&labelColor=5865F2&color=7289DA)](http://pyprohly.github.io/redditwarp/discord-invite)\n\nA comprehensive, type-complete, easy-to-learn Python Reddit API wrapper.\n\nRedditWarp is a Python library that simplifies working with the Reddit API.\nIt handles the complexities of the Reddit API in a way that is comprehensive,\nhighly discoverable, and static-type conscious. It includes a variety of useful\ntools to facilitate a wide range of use cases, and even provides tools for\naccessing the API in ways previously not possible.\n\nLook how easy it is to use:\n\n```python\nimport redditwarp.SYNC\n\nclient = redditwarp.SYNC.Client()\n\nit = client.p.front.pull.hot(5)\nl = list(it)\nfor subm in l:\n    print("r/{0.subreddit.name} | {0.id36}+ ^{0.score} | {0.title!r:.80}".format(subm))\n```\n\n## Features\n\n* A consistent and easy-to-use programming interface.\n* Modern type-complete codebase.\n* Sync and asynchronous IO support.\n* Automatic rate limit handling.\n* A comprehensive and discoverable index of API procedures.\n* Model classes that are fully typed and sensibly wrap API structures.\n* Formal data structures to facilitate comment tree traversals and pagination.\n* HTTP transport library agnosticism.\n* OAuth2 tooling and CLI utilities to help manage auth tokens.\n* A simple event-based listing endpoint streaming framework.\n\n## Installation\n\n**Requires Python 3.8+.**\nType annotations may use 3.9 features.\nCode examples will assume 3.10.\n\nInstall/update:\n\n    pip install -U redditwarp\n\n## Demonstration\n\n<details open>\n  <summary>Examples</summary>\n\n```python\nimport redditwarp.SYNC\n\nclient = redditwarp.SYNC.Client()\n\n# Display the first 5 submissions on the Reddit frontpage.\nit = client.p.front.pull.hot(5)\nl = list(it)\nfor subm in l:\n    print("r/{0.subreddit.name} | {0.id36}+ ^{0.score} | {0.title!r:.80}".format(subm))\n\n# How many subscribers does r/Python have?\nsubr = client.p.subreddit.fetch_by_name(\'Python\')\nprint(subr.subscriber_count)\n\n# Display the top submission of the week in the r/YouShouldKnow subreddit.\nm = next(client.p.subreddit.pull.top(\'YouShouldKnow\', amount=1, time=\'week\'))\nprint(f\'\'\'\\\n{m.permalink}\n{m.id36}+ ^{m.score} | {m.title}\nSubmitted {m.created_at.astimezone().ctime()}{\' *\' if m.is_edited else \'\'} \\\nby u/{m.author_display_name} to r/{m.subreddit.name}\n\'\'\')\n\n# Get the first comment of a submission.\ntree_node = client.p.comment_tree.fetch(int(\'uc8i1g\', 36), sort=\'top\', limit=1)\nc = tree_node.children[0].value\nprint(f\'\'\'\\\n{c.submission.id36}+{c.id36} ^{c.score}\nu/{c.author_display_name} says:\n{c.body}\n\'\'\')\n\n# List the moderators of r/redditdev.\nit1 = client.p.moderation.pull_users.moderators(\'redditdev\')\nfor mod in it1:\n    print(mod.name)\n```\n\n</details>\n\n<details>\n  <summary>More examples</summary>\n\n```python\n# ...\n\n# Need credentials for these next few API calls.\nCLIENT_ID = \'...\'\nCLIENT_SECRET = \'...\'\nREFRESH_TOKEN = \'...\'\nclient1 = redditwarp.SYNC.Client(CLIENT_ID, CLIENT_SECRET, REFRESH_TOKEN)\n\n# Who am I?\nme = client1.p.account.fetch()\nprint(f"Hello u/{me.name}!")\n\n# Show my last 5 comments.\nit2 = client.p.user.pull.comments(me.name, 5)\nfor comm in it2:\n    print(\'###\')\n    print(comm.body)\n\n# Show my last 10 saved items.\nfrom redditwarp.models.submission_SYNC import Submission\nfrom redditwarp.models.comment_SYNC import Comment\nit3 = client1.p.user.pull.saved(me.name, 10)\nl = list(it3)\nfor obj in l:\n    print(\'###\')\n    match obj:\n        case Submission() as m:\n            print(f\'\'\'\\\n{m.permalink}\n{m.id36}+ ^{m.score} | {m.title}\nSubmitted {m.created_at.astimezone().ctime()}{\' *\' if m.is_edited else \'\'} \\\nby u/{m.author_display_name} to r/{m.subreddit.name}\n\'\'\')\n        case Comment() as c:\n            print(f\'\'\'\\\n{c.permalink}\n{c.submission.id36}+{c.id36} ^{c.score}\nu/{c.author_display_name} says:\n{c.body}\n\'\'\')\n\n# Submit a link post to r/test.\nsubm_id = client1.p.submission.create_link_post(\'test\',\n        "Check out this cool website", "https://www.reddit.com")\n\n# Reply to a submission.\nfrom redditwarp.util.extract_id_from_url import extract_submission_id_from_url\nidn = extract_submission_id_from_url("https://www.reddit.com/comments/5e1az9")\ncomm1 = client1.p.submission.reply(idn, "Pretty cool stuff!")\n\n# Delete the post and the comment reply.\nclient1.p.submission.delete(subm_id)\nclient1.p.comment.delete(comm1.id)\n```\n\n</details>\n\n<details>\n  <summary>Streaming example</summary>\n\n```python\n#!/usr/bin/env python\nfrom __future__ import annotations\nfrom typing import TYPE_CHECKING\nif TYPE_CHECKING:\n    from redditwarp.models.submission_ASYNC import Submission\n\nimport asyncio\n\nimport redditwarp.ASYNC\nfrom redditwarp.streaming.makers.subreddit_ASYNC import create_submission_stream\nfrom redditwarp.streaming.ASYNC import flow\n\nasync def main() -> None:\n    client = redditwarp.ASYNC.Client()\n    async with client:\n        submission_stream = create_submission_stream(client, \'AskReddit\')\n\n        @submission_stream.output.attach\n        async def _(subm: Submission) -> None:\n            print(subm.id36, \'~\', subm.title)\n\n        @submission_stream.error.attach\n        async def _(exc: Exception) -> None:\n            print(\'ERROR:\', repr(exc))\n\n        await flow(submission_stream)\n\nasyncio.run(main())\n```\n\n</details>\n\n## Support\n\nPost any questions you have to [r/redditdev].\n\n[r/redditdev]: https://www.reddit.com/r/redditdev/\n\nJoin the conversation in the RedditWarp [Discord guild].\n\n[Discord guild]: http://pyprohly.github.io/redditwarp/discord-invite\n\n## Links\n\n* [Repository](https://github.com/Pyprohly/redditwarp)\n* [PyPI](https://pypi.org/p/redditwarp/)\n* [Documentation](https://redditwarp.readthedocs.io/)\n* [r/redditdev]\n* [Discord guild]\n',
     'author': 'Pyprohly',
     'author_email': 'pyprohly@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `redditwarp-1.0.0rc0/PKG-INFO` & `redditwarp-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redditwarp
-Version: 1.0.0rc0
+Version: 1.1.0
 Summary: A library for interacting with the Reddit API.
 License: MIT
 Keywords: reddit,api,wrapper
 Author: Pyprohly
 Author-email: pyprohly@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,15 @@
 ## Features
 
 * A consistent and easy-to-use programming interface.
 * Modern type-complete codebase.
 * Sync and asynchronous IO support.
 * Automatic rate limit handling.
 * A comprehensive and discoverable index of API procedures.
-* Model classes that sensibly wrap API structures.
+* Model classes that are fully typed and sensibly wrap API structures.
 * Formal data structures to facilitate comment tree traversals and pagination.
 * HTTP transport library agnosticism.
 * OAuth2 tooling and CLI utilities to help manage auth tokens.
 * A simple event-based listing endpoint streaming framework.
 
 ## Installation
```

