# Comparing `tmp/litestar-2.0.0a6.tar.gz` & `tmp/litestar-2.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0a6.tar", max compression
+gzip compressed data, was "litestar-2.0.0a7.tar", max compression
```

## Comparing `litestar-2.0.0a6.tar` & `litestar-2.0.0a7.tar`

### file list

```diff
@@ -1,305 +1,307 @@
--rw-r--r--   0        0        0     1092 2023-05-09 15:45:08.809052 litestar-2.0.0a6/LICENSE
--rw-r--r--   0        0        0    50573 2023-05-09 15:45:08.809052 litestar-2.0.0a6/README.md
--rw-r--r--   0        0        0      744 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/__init__.py
--rw-r--r--   0        0        0      103 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     8651 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4239 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14907 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20450 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5935 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10117 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5525 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1476 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10196 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7074 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2104 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    31705 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5240 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1464 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2338 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     5995 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/field.py
--rw-r--r--   0        0        0       64 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    13197 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3736 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     6680 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     6510 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/utils.py
--rw-r--r--   0        0        0    35419 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2768 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9208 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15678 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/cli/__init__.py
--rw-r--r--   0        0        0    11640 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     4571 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2365 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2224 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     1210 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12358 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10821 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/request.py
--rw-r--r--   0        0        0    11256 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1098 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     8324 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     3978 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3916 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      180 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2206 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0      290 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0     9259 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/abc.py
--rw-r--r--   0        0        0      328 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     1785 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    13409 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4324 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0     3431 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      742 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     3602 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11308 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11500 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     2849 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1600 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1447 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0    21855 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/repository.py
--rw-r--r--   0        0        0     1856 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9559 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/controller.py
--rw-r--r--   0        0        0    16460 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9302 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3360 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/url.py
--rw-r--r--   0        0        0     2386 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/di.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/__init__.py
--rw-r--r--   0        0        0      337 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/exceptions.py
--rw-r--r--   0        0        0      188 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      245 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/__init__.py
--rw-r--r--   0        0        0    14863 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/abc.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/__init__.py
--rw-r--r--   0        0        0     1282 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/backend.py
--rw-r--r--   0        0        0     1836 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/utils.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/__init__.py
--rw-r--r--   0        0        0     1242 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/backend.py
--rw-r--r--   0        0        0     1681 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/utils.py
--rw-r--r--   0        0        0     3161 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/types.py
--rw-r--r--   0        0        0    10354 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/utils.py
--rw-r--r--   0        0        0     7508 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/abc.py
--rw-r--r--   0        0        0     1193 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/config.py
--rw-r--r--   0        0        0      313 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/exc.py
--rw-r--r--   0        0        0     1269 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/field.py
--rw-r--r--   0        0        0       65 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/stdlib/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0     1088 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/types.py
--rw-r--r--   0        0        0     1594 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/utils.py
--rw-r--r--   0        0        0     4465 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/interface.py
--rw-r--r--   0        0        0      309 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/__init__.py
--rw-r--r--   0        0        0     4597 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/listener.py
--rw-r--r--   0        0        0     1142 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1621 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5330 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3877 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    20202 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     8104 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    25662 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    60867 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6415 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    15216 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3619 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     2967 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/base.py
--rw-r--r--   0        0        0     8359 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2565 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6466 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7191 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     8990 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13372 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10811 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7935 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10365 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8558 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      231 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/config.py
--rw-r--r--   0        0        0    16443 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    10984 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/pagination.py
--rw-r--r--   0        0        0    16805 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/params.py
--rw-r--r--   0        0        0     7100 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/partial.py
--rw-r--r--   0        0        0     3926 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/py.typed
--rw-r--r--   0        0        0      278 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/__init__.py
--rw-r--r--   0        0        0    12173 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/base.py
--rw-r--r--   0        0        0     9225 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/file.py
--rw-r--r--   0        0        0     2952 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/redirect.py
--rw-r--r--   0        0        0     4883 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/streaming.py
--rw-r--r--   0        0        0     2994 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/template.py
--rw-r--r--   0        0        0    14975 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response_containers.py
--rw-r--r--   0        0        0    15028 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/router.py
--rw-r--r--   0        0        0      191 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1757 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6437 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/base.py
--rw-r--r--   0        0        0    13254 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/http.py
--rw-r--r--   0        0        0     3052 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4933 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     7355 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5019 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4377 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/__init__.py
--rw-r--r--   0        0        0     4113 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17445 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19555 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    31473 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2532 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21905 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8086 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/transport.py
--rw-r--r--   0        0        0     8527 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4105 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/__init__.py
--rw-r--r--   0        0        0     8697 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2291 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1645 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/empty.py
--rw-r--r--   0        0        0     2662 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1720 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2607 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/serialization.py
--rw-r--r--   0        0        0     1906 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/compat.py
--rw-r--r--   0        0        0     3578 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     1732 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/path.py
--rw-r--r--   0        0        0    10434 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2720 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/sequence.py
--rw-r--r--   0        0        0    13743 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/signature.py
--rw-r--r--   0        0        0     5337 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/sync.py
--rw-r--r--   0        0        0     6405 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/version.py
--rw-r--r--   0        0        0     9810 2023-05-09 15:45:08.849052 litestar-2.0.0a6/pyproject.toml
--rw-r--r--   0        0        0    54208 1970-01-01 00:00:00.000000 litestar-2.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-14 12:46:25.414940 litestar-2.0.0a7/LICENSE
+-rw-r--r--   0        0        0    50912 2023-05-14 12:46:25.414940 litestar-2.0.0a7/README.md
+-rw-r--r--   0        0        0      744 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6380 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4239 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14907 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20450 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5935 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0    10147 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5525 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1476 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    10196 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     7074 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2104 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    31771 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5240 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1464 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2338 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     8190 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/field.py
+-rw-r--r--   0        0        0       64 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    13459 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     3736 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     6680 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     6510 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    35626 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2768 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9208 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15649 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    11640 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4571 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2365 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2224 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     1210 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11509 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10821 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/request.py
+-rw-r--r--   0        0        0    11256 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1098 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     8324 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     3978 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3916 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/mako.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/msgspec/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4206 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2206 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0     9259 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/abc.py
+-rw-r--r--   0        0        0      328 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     1759 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    13453 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5258 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0     3414 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      742 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11339 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11500 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     2867 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1644 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1447 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0    21972 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/repository.py
+-rw-r--r--   0        0        0     2759 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9559 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/controller.py
+-rw-r--r--   0        0        0    16460 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17316 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9302 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3360 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     2783 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/exceptions.py
+-rw-r--r--   0        0        0      240 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/__init__.py
+-rw-r--r--   0        0        0    16643 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/abc.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/backend.py
+-rw-r--r--   0        0        0     1836 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/backend.py
+-rw-r--r--   0        0        0     1681 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/utils.py
+-rw-r--r--   0        0        0     3334 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/types.py
+-rw-r--r--   0        0        0    10628 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/utils.py
+-rw-r--r--   0        0        0     7691 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/abc.py
+-rw-r--r--   0        0        0     1261 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/config.py
+-rw-r--r--   0        0        0     1449 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/data_structures.py
+-rw-r--r--   0        0        0      313 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/exc.py
+-rw-r--r--   0        0        0     1269 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/field.py
+-rw-r--r--   0        0        0       65 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/stdlib/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0     1088 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/types.py
+-rw-r--r--   0        0        0     1594 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/utils.py
+-rw-r--r--   0        0        0     4455 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/interface.py
+-rw-r--r--   0        0        0      309 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/listener.py
+-rw-r--r--   0        0        0     1165 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1702 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5330 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3877 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    20395 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     8104 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26009 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    60853 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     7151 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18553 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3619 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     2967 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8359 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2565 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6466 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7210 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     8990 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13372 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10811 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7935 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10365 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8558 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      231 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/config.py
+-rw-r--r--   0        0        0    16544 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    10984 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/pagination.py
+-rw-r--r--   0        0        0    16805 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/params.py
+-rw-r--r--   0        0        0     7100 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/partial.py
+-rw-r--r--   0        0        0     3926 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/py.typed
+-rw-r--r--   0        0        0      278 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/__init__.py
+-rw-r--r--   0        0        0    12404 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/base.py
+-rw-r--r--   0        0        0     9225 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/file.py
+-rw-r--r--   0        0        0     2952 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/redirect.py
+-rw-r--r--   0        0        0     4883 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/streaming.py
+-rw-r--r--   0        0        0     2994 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/template.py
+-rw-r--r--   0        0        0    14975 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/response_containers.py
+-rw-r--r--   0        0        0    14997 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1757 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6437 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/base.py
+-rw-r--r--   0        0        0    13307 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/http.py
+-rw-r--r--   0        0        0     3052 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4952 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     7355 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5019 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4113 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17445 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5132 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19555 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    29563 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2532 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21927 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8086 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8527 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4047 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8697 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      453 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2235 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1678 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/empty.py
+-rw-r--r--   0        0        0     2662 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1720 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2607 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/protocols.py
+-rw-r--r--   0        0        0     1820 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/serialization.py
+-rw-r--r--   0        0        0     1906 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3578 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     1732 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/path.py
+-rw-r--r--   0        0        0    10434 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2720 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/sequence.py
+-rw-r--r--   0        0        0    14118 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/signature.py
+-rw-r--r--   0        0        0     5337 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/sync.py
+-rw-r--r--   0        0        0     6405 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/version.py
+-rw-r--r--   0        0        0     1331 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    10041 2023-05-14 12:46:25.462940 litestar-2.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0    54547 1970-01-01 00:00:00.000000 litestar-2.0.0a7/PKG-INFO
```

### Comparing `litestar-2.0.0a6/LICENSE` & `litestar-2.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/README.md` & `litestar-2.0.0a7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-100-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-101-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -49,15 +49,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha3
+pip install litestar==2.0.0alpha6
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -409,14 +409,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://hexcode.tech"><img src="https://avatars.githubusercontent.com/u/419606?v=4?s=100" width="100px;" alt="Phyo Arkar Lwin"/><br /><sub><b>Phyo Arkar Lwin</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=v3ss0n" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.0.0a6/litestar/__init__.py` & `litestar-2.0.0a7/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0a7/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0a7/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0a7/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0a7/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_asgi/utils.py` & `litestar-2.0.0a7/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_kwargs/cleanup.py` & `litestar-2.0.0a7/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_kwargs/dependencies.py` & `litestar-2.0.0a7/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_kwargs/extractors.py` & `litestar-2.0.0a7/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0a7/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0a7/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_layers/utils.py` & `litestar-2.0.0a7/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_multipart.py` & `litestar-2.0.0a7/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/parameters.py` & `litestar-2.0.0a7/litestar/_openapi/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     "create_path_parameter_schema",
     "get_layered_parameter",
     "get_recursive_handler_parameters",
 )
 
 
 if TYPE_CHECKING:
+    from litestar.di import Provide
     from litestar.handlers.base import BaseRouteHandler
     from litestar.openapi.spec import Reference
-    from litestar.types import Dependencies
     from litestar.types.internal_types import PathParameterDefinition
 
 
 def create_path_parameter_schema(
     path_parameter: PathParameterDefinition,
     field: SignatureField,
     generate_examples: bool,
@@ -140,37 +140,37 @@
         schema=result,
     )
 
 
 def get_recursive_handler_parameters(
     field_name: str,
     signature_field: SignatureField,
-    dependencies: Dependencies,
+    dependency_providers: dict[str, Provide],
     route_handler: BaseRouteHandler,
     path_parameters: tuple[PathParameterDefinition, ...],
     generate_examples: bool,
     schemas: dict[str, Schema],
 ) -> list[Parameter]:
     """Create and return parameters for a handler.
 
     If the provided field is not a dependency, a normal parameter is created and returned as a list, otherwise
     `create_parameter_for_handler()` is called to generate parameters for the dependency.
     """
 
-    if field_name not in dependencies:
+    if field_name not in dependency_providers:
         return [
             create_parameter(
                 generate_examples=generate_examples,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
                 schemas=schemas,
                 signature_field=signature_field,
             )
         ]
-    dependency_fields = dependencies[field_name].signature_model.fields
+    dependency_fields = dependency_providers[field_name].signature_model.fields
     return create_parameter_for_handler(
         route_handler, dependency_fields, path_parameters, generate_examples, schemas=schemas
     )
 
 
 def get_layered_parameter(
     field_name: str,
@@ -235,15 +235,15 @@
 
     for field_name, signature_field in unique_handler_fields:
         if isinstance(signature_field.kwarg_model, DependencyKwarg) and field_name not in dependencies:
             # never document explicit dependencies
             continue
 
         for parameter in get_recursive_handler_parameters(
-            dependencies=dependencies,
+            dependency_providers=dependencies,
             field_name=field_name,
             generate_examples=generate_examples,
             path_parameters=path_parameters,
             route_handler=route_handler,
             schemas=schemas,
             signature_field=signature_field,
         ):
```

### Comparing `litestar-2.0.0a6/litestar/_openapi/path_item.py` & `litestar-2.0.0a7/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/request_body.py` & `litestar-2.0.0a7/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/responses.py` & `litestar-2.0.0a7/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0a7/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0a7/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0a7/litestar/_openapi/schema_generation/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,17 @@
     """
 
     field_type_hints = get_type_hints(field_type)
     return Schema(
         required=sorted([field.alias or field.name for field in field_type.__fields__.values() if field.required]),
         properties={
             (f.alias or f.name): create_schema(
-                field=SignatureField.create(field_type=field_type_hints[f.name], name=f.alias or f.name),
+                field=SignatureField.create(
+                    field_type=field_type_hints[f.name], name=f.alias or f.name, default_value=f.field_info
+                ),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
             )
             for f in field_type.__fields__.values()
         },
         type=OpenAPIType.OBJECT,
```

### Comparing `litestar-2.0.0a6/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0a7/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0a7/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0a7/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0a7/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_openapi/utils.py` & `litestar-2.0.0a7/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_parsers.py` & `litestar-2.0.0a7/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0a7/litestar/_signature/models/attrs_signature_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,20 @@
 
         # this is a hack to create a catch-all hook, see: https://github.com/python-attrs/cattrs/issues/311
         self._structure_func._function_dispatch._handler_pairs[-1] = (
             *_create_default_structuring_hooks(self),
             False,
         )
 
+        # ensure attrs instances are not unstructured into dict
+        self.register_unstructure_hook_factory(
+            lambda value: attrs.has(value) and AttrsSignatureModel not in list(value.__mro__),
+            _pass_through_unstructure_hook,
+        )
+
         for cls, structure_hook in hooks:
             self.register_structure_hook(cls, structure_hook)
             self.register_unstructure_hook(cls, _pass_through_unstructure_hook)
 
 
 _converter: Converter = Converter()
```

### Comparing `litestar-2.0.0a6/litestar/_signature/models/base.py` & `litestar-2.0.0a7/litestar/_signature/models/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0a7/litestar/_signature/models/pydantic_signature_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/_signature/utils.py` & `litestar-2.0.0a7/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/app.py` & `litestar-2.0.0a7/litestar/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
+import inspect
 import logging
+from contextlib import AbstractAsyncContextManager, AsyncExitStack, asynccontextmanager
 from datetime import date, datetime, time, timedelta
+from functools import partial
 from itertools import chain
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Literal, Mapping, Sequence, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Literal, Mapping, Sequence, cast
 
 from typing_extensions import Self, TypedDict
 
 from litestar._asgi import ASGIRouter
 from litestar._asgi.utils import get_route_handlers, wrap_in_exception_handler
 from litestar._openapi.path_item import create_path_item
 from litestar.config.allowed_hosts import AllowedHostsConfig
@@ -35,14 +38,15 @@
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
 from litestar.types import Empty
 from litestar.types.internal_types import PathParameterDefinition
 from litestar.utils import (
     as_async_callable_list,
+    is_async_callable,
     join_paths,
     unique,
 )
 from litestar.utils.dataclass import extract_dataclass_items
 
 if TYPE_CHECKING:
     from litestar.config.compression import CompressionConfig
@@ -68,16 +72,14 @@
         BeforeRequestHookHandler,
         ControllerRouterHandler,
         Dependencies,
         EmptyType,
         ExceptionHandlersMap,
         GetLogger,
         Guard,
-        LifeSpanHandler,
-        LifeSpanHookHandler,
         LifeSpanReceive,
         LifeSpanScope,
         LifeSpanSend,
         Logger,
         Message,
         Middleware,
         OnAppInitHandler,
@@ -87,14 +89,15 @@
         ResponseCookies,
         ResponseType,
         RouteHandlerType,
         Scope,
         Send,
         TypeEncodersMap,
     )
+    from litestar.types.callable_types import LifespanHook
 
 __all__ = ("HandlerIndex", "Litestar", "DEFAULT_OPENAPI_CONFIG")
 
 DEFAULT_OPENAPI_CONFIG = OpenAPIConfig(title="Litestar API", version="1.0.0")
 """The default OpenAPI config used if not configuration is explicitly passed to the
 :class:`Litestar <.app.Litestar>` instance constructor.
 """
@@ -121,25 +124,22 @@
     """The Litestar application.
 
     ``Litestar`` is the root level of the app - it has the base path of ``/`` and all root level Controllers, Routers
     and Route Handlers should be registered on it.
     """
 
     __slots__ = (
+        "_lifespan_managers",
         "_debug",
         "_openapi_schema",
         "after_exception",
-        "after_shutdown",
-        "after_startup",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
-        "before_shutdown",
-        "before_startup",
         "compression_config",
         "cors_config",
         "csrf_config",
         "event_emitter",
         "get_logger",
         "logger",
         "logging_config",
@@ -164,21 +164,17 @@
     def __init__(
         self,
         route_handlers: OptionalSequence[ControllerRouterHandler] = None,
         *,
         after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
-        after_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-        after_startup: OptionalSequence[LifeSpanHookHandler] = None,
         allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
-        before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-        before_startup: OptionalSequence[LifeSpanHookHandler] = None,
         cache_control: CacheControlHeader | None = None,
         compression_config: CompressionConfig | None = None,
         cors_config: CORSConfig | None = None,
         csrf_config: CSRFConfig | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         debug: bool = False,
         dependencies: Dependencies | None = None,
@@ -187,16 +183,16 @@
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: OptionalSequence[Guard] = None,
         listeners: OptionalSequence[EventListener] = None,
         logging_config: BaseLoggingConfig | EmptyType | None = Empty,
         middleware: OptionalSequence[Middleware] = None,
         multipart_form_part_limit: int = 1000,
         on_app_init: OptionalSequence[OnAppInitHandler] = None,
-        on_shutdown: OptionalSequence[LifeSpanHandler] = None,
-        on_startup: OptionalSequence[LifeSpanHandler] = None,
+        on_shutdown: OptionalSequence[LifespanHook] = None,
+        on_startup: OptionalSequence[LifespanHook] = None,
         openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
         plugins: OptionalSequence[PluginProtocol] = None,
         preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
         request_class: type[Request] | None = None,
         response_cache_config: ResponseCacheConfig | None = None,
@@ -209,41 +205,34 @@
         state: State | None = None,
         static_files_config: OptionalSequence[StaticFilesConfig] = None,
         stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
         type_encoders: TypeEncodersMap | None = None,
         websocket_class: type[WebSocket] | None = None,
+        lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     ) -> None:
         """Initialize a ``Litestar`` application.
 
         Args:
             after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
                 hook is called after an exception occurs. In difference to exception handlers, it is not meant to
                 return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
             after_request: A sync or async function executed after the route handler function returned and the response
                 object has been resolved. Receives the response object.
             after_response: A sync or async function called after the response has been awaited. It receives the
                 :class:`Request <.connection.Request>` object and should not return any values.
-            after_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-                the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
-            after_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-                the ASGI startup, after all callables in the 'on_startup' list have been called.
             allowed_hosts: A sequence of allowed hosts, or an
                 :class:`AllowedHostsConfig <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin
                 allowed hosts middleware.
             before_request: A sync or async function called immediately before calling the route handler. Receives the
                 :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
                 response, bypassing the route handler.
             before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
                 when the ASGI send function is called.
-            before_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-                the ASGI shutdown, before any 'on_shutdown' hooks are called.
-            before_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-                the ASGI startup, before any 'on_startup' hooks are called.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
                 this app. Can be overridden by route handlers.
             compression_config: Configures compression behaviour of the application, this enabled a builtin or user
                 defined Compression middleware.
             cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
             csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
@@ -253,26 +242,27 @@
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
                 Can be overridden by route handlers.
             event_emitter_backend: A subclass of
                 :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            lifespan: A list of callables returning async context managers, wrapping the lifespan of the ASGI application
             listeners: A sequence of :class:`EventListener <.events.listener.EventListener>`.
             logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
             middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request. This limit
                 is intended to protect from DoS attacks.
             on_app_init: A sequence of :class:`OnAppInitHandler <.types.OnAppInitHandler>` instances. Handlers receive
                 an instance of :class:`AppConfig <.config.app.AppConfig>` that will have been initially populated with
                 the parameters passed to :class:`Litestar <litestar.app.Litestar>`, and must return an instance of same.
                 If more than one handler is registered they are called in the order they are provided.
-            on_shutdown: A sequence of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application
+            on_shutdown: A sequence of :class:`LifespanHook <.types.LifespanHook>` called during application
                 shutdown.
-            on_startup: A sequence of :class:`LifeSpanHandler <litestar.types.LifeSpanHandler>` called during
+            on_startup: A sequence of :class:`LifespanHook <litestar.types.LifespanHook>` called during
                 application startup.
             openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
             opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <litestar.connection.request.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
             parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
                 paths.
@@ -309,32 +299,29 @@
         if logging_config is Empty:
             logging_config = LoggingConfig()
 
         config = AppConfig(
             after_exception=list(after_exception or []),
             after_request=after_request,
             after_response=after_response,
-            after_shutdown=list(after_shutdown or []),
-            after_startup=list(after_startup or []),
             allowed_hosts=allowed_hosts if isinstance(allowed_hosts, AllowedHostsConfig) else list(allowed_hosts or []),
             before_request=before_request,
             before_send=list(before_send or []),
-            before_shutdown=list(before_shutdown or []),
-            before_startup=list(before_startup or []),
             cache_control=cache_control,
             compression_config=compression_config,
             cors_config=cors_config,
             csrf_config=csrf_config,
             debug=debug,
             dependencies=dict(dependencies or {}),
             dto=dto,
             etag=etag,
             event_emitter_backend=event_emitter_backend,
             exception_handlers=exception_handlers or {},
             guards=list(guards or []),
+            lifespan=lifespan or [],
             listeners=list(listeners or []),
             logging_config=cast("BaseLoggingConfig | None", logging_config),
             middleware=list(middleware or []),
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
@@ -359,31 +346,29 @@
             type_encoders=type_encoders,
             websocket_class=websocket_class,
         )
         for handler in chain(
             on_app_init or [],
             (p.on_app_init for p in config.plugins if isinstance(p, InitPluginProtocol)),
         ):
-            config = handler(config)
+            config = handler(config)  # pyright: ignore
 
         self._openapi_schema: OpenAPI | None = None
         self._debug: bool = True
+        self._lifespan_managers = config.lifespan
+
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.asgi_router = ASGIRouter(app=self)
 
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.after_exception = as_async_callable_list(config.after_exception)
-        self.after_shutdown = as_async_callable_list(config.after_shutdown)
-        self.after_startup = as_async_callable_list(config.after_startup)
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.before_send = as_async_callable_list(config.before_send)
-        self.before_shutdown = as_async_callable_list(config.before_shutdown)
-        self.before_startup = as_async_callable_list(config.before_startup)
         self.compression_config = config.compression_config
         self.cors_config = config.cors_config
         self.csrf_config = config.csrf_config
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.logging_config = config.logging_config
         self.multipart_form_part_limit = config.multipart_form_part_limit
         self.on_shutdown = config.on_shutdown
@@ -478,14 +463,46 @@
         scope["app"] = self
         if scope["type"] == "lifespan":
             await self.asgi_router.lifespan(receive=receive, send=send)  # type: ignore[arg-type]
             return
         scope["state"] = {}
         await self.asgi_handler(scope, receive, self._wrap_send(send=send, scope=scope))  # type: ignore[arg-type]
 
+    async def _call_lifespan_hook(self, hook: LifespanHook) -> None:
+        ret = hook(self) if inspect.signature(hook).parameters else hook()  # type: ignore
+
+        if is_async_callable(hook):  # type: ignore
+            await ret
+
+    @asynccontextmanager
+    async def lifespan(self) -> AsyncGenerator[None, None]:
+        """Context manager handling the ASGI lifespan.
+
+        It will be entered when the ``lifespan`` message has been received from the
+        server, and exit after the ``asgi.shutdown`` message. During this period, it is
+        responsible for calling the ``before_startup``, ``after_startup``,
+        `on_startup``, ``before_shutdown``, ``on_shutdown`` and ``after_shutdown``
+        hooks, as well as custom lifespan managers.
+        """
+        async with AsyncExitStack() as exit_stack:
+            for hook in self.on_shutdown[::-1]:
+                exit_stack.push_async_callback(partial(self._call_lifespan_hook, hook))
+
+            await exit_stack.enter_async_context(self.event_emitter)
+
+            for manager in self._lifespan_managers:
+                if not isinstance(manager, AbstractAsyncContextManager):
+                    manager = manager(self)
+                await exit_stack.enter_async_context(manager)
+
+            for hook in self.on_startup:
+                await self._call_lifespan_hook(hook)
+
+            yield
+
     @property
     def openapi_schema(self) -> OpenAPI:
         """Access  the OpenAPI schema of the application.
 
         Returns:
             The :class:`OpenAPI`
             <pydantic_openapi_schema.open_api.OpenAPI> instance of the
@@ -703,15 +720,15 @@
         If CORS or TrustedHost configs are provided to the constructor, they will wrap the router as well.
         """
         asgi_handler: ASGIApp = self.asgi_router
         if self.cors_config:
             asgi_handler = CORSMiddleware(app=asgi_handler, config=self.cors_config)
 
         return wrap_in_exception_handler(
-            debug=self.debug, app=asgi_handler, exception_handlers=self.exception_handlers or {}
+            debug=self.debug, app=asgi_handler, exception_handlers=self.exception_handlers or {}  # pyright: ignore
         )
 
     def _wrap_send(self, send: Send, scope: Scope) -> Send:
         """Wrap the ASGI send and handles any 'before send' hooks.
 
         Args:
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a6/litestar/background_tasks.py` & `litestar-2.0.0a7/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/channels/backends/base.py` & `litestar-2.0.0a7/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/channels/backends/memory.py` & `litestar-2.0.0a7/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/channels/backends/redis.py` & `litestar-2.0.0a7/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/channels/plugin.py` & `litestar-2.0.0a7/litestar/channels/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from asyncio import CancelledError, Queue, Task, create_task
-from contextlib import asynccontextmanager, suppress
+from contextlib import AbstractAsyncContextManager, asynccontextmanager, suppress
 from functools import partial
 from os.path import join as join_path
 from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Iterable
 
 import msgspec.json
 
 from litestar.di import Provide
@@ -14,28 +14,28 @@
 from litestar.handlers import WebsocketRouteHandler
 from litestar.plugins import InitPluginProtocol
 from litestar.serialization import default_serializer
 
 from .subscriber import BacklogStrategy, EventCallback, Subscriber
 
 if TYPE_CHECKING:
-    from inspect import Traceback
+    from types import TracebackType
 
     from litestar.channels.backends.base import ChannelsBackend
     from litestar.config.app import AppConfig
     from litestar.connection import WebSocket
     from litestar.types import LitestarEncodableType, TypeEncodersMap
     from litestar.types.asgi_types import WebSocketMode
 
 
 class ChannelsException(LitestarException):
     pass
 
 
-class ChannelsPlugin(InitPluginProtocol):
+class ChannelsPlugin(InitPluginProtocol, AbstractAsyncContextManager):
     def __init__(
         self,
         backend: ChannelsBackend,
         *,
         channels: Iterable[str] | None = None,
         arbitrary_channels_allowed: bool = False,
         create_ws_route_handlers: bool = False,
@@ -105,17 +105,16 @@
         if isinstance(data, str):
             return data.encode()
 
         return self._encode_json(data)
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         """Plugin hook. Set up a ``channels`` dependency, add route handlers and register application hooks"""
-        app_config.dependencies["channels"] = Provide(lambda: self, use_cache=True)
-        app_config.on_startup.append(self._on_startup)
-        app_config.on_shutdown.append(self._on_shutdown)
+        app_config.dependencies["channels"] = Provide(lambda: self, use_cache=True, sync_to_thread=False)
+        app_config.lifespan.append(self)
 
         if self._create_route_handlers:
             if self._arbitrary_channels_allowed:
                 path = join_path(self._handler_root_path, "{channel_name:str}")  # noqa: PTH118
                 route_handlers = [WebsocketRouteHandler(path)(self._ws_handler_func)]
             else:
                 route_handlers = [
@@ -226,15 +225,14 @@
 
             try:
                 channel_subscribers.remove(subscriber)
             except KeyError:  # subscriber was not subscribed to this channel. This may happen if channels is None
                 continue
 
             if not channel_subscribers:
-                del self._channels[channel]
                 channels_to_unsubscribe.add(channel)
 
         if not any(subscriber in queues for queues in self._channels.values()):
             await subscriber.put(None)  # this will stop any running task or generator by breaking the inner loop
             if subscriber.is_running:
                 await subscriber.stop()
 
@@ -350,10 +348,10 @@
         await self._on_startup()
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
-        exc_tb: Traceback | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         await self._on_shutdown()
```

### Comparing `litestar-2.0.0a6/litestar/channels/subscriber.py` & `litestar-2.0.0a7/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/cli/_utils.py` & `litestar-2.0.0a7/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/cli/commands/core.py` & `litestar-2.0.0a7/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/cli/commands/schema.py` & `litestar-2.0.0a7/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/cli/commands/sessions.py` & `litestar-2.0.0a7/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/cli/main.py` & `litestar-2.0.0a7/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/config/allowed_hosts.py` & `litestar-2.0.0a7/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/config/app.py` & `litestar-2.0.0a7/litestar/config/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Literal, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Literal, Sequence
 
 from litestar.config.allowed_hosts import AllowedHostsConfig
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.datastructures import State
 from litestar.events.emitter import SimpleEventEmitter
 from litestar.types.empty import Empty
 
 if TYPE_CHECKING:
+    from contextlib import AbstractAsyncContextManager
+
+    from litestar import Litestar
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.connection import Request, WebSocket
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
     from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
@@ -27,29 +30,30 @@
     from litestar.stores.base import Store
     from litestar.stores.registry import StoreRegistry
     from litestar.template.config import TemplateConfig
     from litestar.types import (
         AfterExceptionHookHandler,
         AfterRequestHookHandler,
         AfterResponseHookHandler,
+        AnyCallable,
         BeforeMessageSendHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
         ExceptionHandlersMap,
         Guard,
-        LifeSpanHandler,
-        LifeSpanHookHandler,
         Middleware,
         ParametersMap,
         ResponseCookies,
         ResponseType,
         TypeEncodersMap,
     )
+    from litestar.types.callable_types import LifespanHook
     from litestar.types.empty import EmptyType
 
+
 __all__ = ("AppConfig",)
 
 
 @dataclass
 class AppConfig:
     """The parameters provided to the ``Litestar`` app are used to instantiate an instance, and then the instance is
     passed to any callbacks registered to ``on_app_init`` in the order they are provided.
@@ -69,46 +73,26 @@
 
     Receives the response object which may be any subclass of :class:`Response <.response.Response>`.
     """
     after_response: AfterResponseHookHandler | None = field(default=None)
     """A sync or async function called after the response has been awaited. It receives the
     :class:`Request <.connection.Request>` object and should not return any values.
     """
-    after_shutdown: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
-
-    This hook is called during the ASGI shutdown, after all callables in the ``on_shutdown`` list have been called.
-    """
-    after_startup: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
-
-    This hook is called during the ASGI startup, after all callables in the ``on_startup`` list have been called.
-    """
     allowed_hosts: list[str] | AllowedHostsConfig | None = field(default=None)
     """If set enables the builtin allowed hosts middleware."""
     before_request: BeforeRequestHookHandler | None = field(default=None)
     """A sync or async function called immediately before calling the route handler. Receives the
     :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the response,
     bypassing the route handler.
     """
     before_send: list[BeforeMessageSendHookHandler] = field(default_factory=list)
     """An application level :class:`before send hook handler <.types.BeforeMessageSendHookHandler>` or list thereof.
 
     This hook is called when the ASGI send function is called.
     """
-    before_shutdown: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
-
-    This hook is called during the ASGI shutdown, before any callables in the ``on_shutdown`` list have been called.
-    """
-    before_startup: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
-
-    This hook is called during the ASGI startup, before any callables in the ``on_startup`` list have been called.
-    """
     cache_control: CacheControlHeader | None = field(default=None)
     """A ``cache-control`` header of type :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to
     route handlers of this app.
 
     Can be overridden by route handlers.
     """
     compression_config: CompressionConfig | None = field(default=None)
@@ -117,39 +101,43 @@
     """
     cors_config: CORSConfig | None = field(default=None)
     """If set this enables the builtin CORS middleware."""
     csrf_config: CSRFConfig | None = field(default=None)
     """If set this enables the builtin CSRF middleware."""
     debug: bool = field(default=False)
     """If ``True``, app errors rendered as HTML with a stack trace."""
-    dependencies: dict[str, Provide] = field(default_factory=dict)
+    dependencies: dict[str, Provide | AnyCallable] = field(default_factory=dict)
     """A string keyed dictionary of dependency :class:`Provider <.di.Provide>` instances."""
     dto: type[DTOInterface] | None | EmptyType = field(default=Empty)
     """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data."""
     etag: ETag | None = field(default=None)
     """An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
 
     Can be overridden by route handlers.
     """
     event_emitter_backend: type[BaseEventEmitterBackend] = field(default=SimpleEventEmitter)
     """A subclass of :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`."""
     exception_handlers: ExceptionHandlersMap = field(default_factory=dict)
     """A dictionary that maps handler functions to status codes and/or exception types."""
     guards: list[Guard] = field(default_factory=list)
     """A list of :class:`Guard <.types.Guard>` callables."""
+    lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] = field(
+        default_factory=list
+    )
+    """A list of callables returning async context managers, wrapping the lifespan of the ASGI application"""
     listeners: list[EventListener] = field(default_factory=list)
     """A list of :class:`EventListener <.events.listener.EventListener>`."""
     logging_config: BaseLoggingConfig | None = field(default=None)
     """An instance of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>` subclass."""
     middleware: list[Middleware] = field(default_factory=list)
     """A list of :class:`Middleware <.types.Middleware>`."""
-    on_shutdown: list[LifeSpanHandler] = field(default_factory=list)
-    """A list of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application shutdown."""
-    on_startup: list[LifeSpanHandler] = field(default_factory=list)
-    """A list of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application startup."""
+    on_shutdown: list[LifespanHook] = field(default_factory=list)
+    """A list of :class:`LifespanHook <.types.LifespanHook>` called during application shutdown."""
+    on_startup: list[LifespanHook] = field(default_factory=list)
+    """A list of :class:`LifespanHook <.types.LifespanHook>` called during application startup."""
     openapi_config: OpenAPIConfig | None = field(default=None)
     """Defaults to :data:`DEFAULT_OPENAPI_CONFIG <litestar.app.DEFAULT_OPENAPI_CONFIG>`"""
     opt: dict[str, Any] = field(default_factory=dict)
     """A string keyed dictionary of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
     wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <litestar.types.Scope>`.
 
     Can be overridden by routers and router handlers.
```

### Comparing `litestar-2.0.0a6/litestar/config/compression.py` & `litestar-2.0.0a7/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/config/cors.py` & `litestar-2.0.0a7/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/config/csrf.py` & `litestar-2.0.0a7/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/config/response_cache.py` & `litestar-2.0.0a7/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/connection/__init__.py` & `litestar-2.0.0a7/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/connection/base.py` & `litestar-2.0.0a7/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/connection/request.py` & `litestar-2.0.0a7/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/connection/websocket.py` & `litestar-2.0.0a7/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/constants.py` & `litestar-2.0.0a7/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0a7/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/htmx/request.py` & `litestar-2.0.0a7/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/htmx/response.py` & `litestar-2.0.0a7/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/htmx/types.py` & `litestar-2.0.0a7/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/jinja.py` & `litestar-2.0.0a7/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0a7/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0a7/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0a7/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0a7/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/mako.py` & `litestar-2.0.0a7/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0a7/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0a7/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0a7/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/repository/abc.py` & `litestar-2.0.0a7/litestar/contrib/repository/abc.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/repository/filters.py` & `litestar-2.0.0a7/litestar/contrib/repository/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Collection filter datastructures."""
 from __future__ import annotations
 
+from collections import abc  # noqa: TCH003
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Generic, Literal, TypeVar
-
-if TYPE_CHECKING:
-    from collections import abc
-    from datetime import datetime
+from datetime import datetime  # noqa: TCH003
+from typing import Generic, Literal, TypeVar
 
 T = TypeVar("T")
 
 __all__ = ["BeforeAfter", "CollectionFilter", "LimitOffset", "OrderBy", "SearchFilter"]
 
 
 @dataclass
@@ -42,25 +40,25 @@
     limit: int
     """Value for ``LIMIT`` clause of query."""
     offset: int
     """Value for ``OFFSET`` clause of query."""
 
 
 @dataclass
-class OrderBy(Generic[T]):
+class OrderBy:
     """Data required to construct a ``ORDER BY ...`` clause."""
 
     field_name: str
     """Name of the model attribute to sort on."""
-    sort_order: Literal["asc", "desc"]
+    sort_order: Literal["asc", "desc"] = "asc"
     """Sort ascending or descending"""
 
 
 @dataclass
-class SearchFilter(Generic[T]):
+class SearchFilter:
     """Data required to construct a ``WHERE field_name LIKE '%' || :value || '%'`` clause."""
 
     field_name: str
     """Name of the model attribute to sort on."""
     value: str
     """Values for ``LIKE`` clause."""
     ignore_case: bool | None = False
```

### Comparing `litestar-2.0.0a6/litestar/contrib/repository/handlers.py` & `litestar-2.0.0a7/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0a7/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if existing:
             for field_name, new_field_value in kwargs.items():
                 field = getattr(existing, field_name, None)
                 if field and field != new_field_value:
                     setattr(existing, field_name, new_field_value)
 
             return existing, False
-        return await self.add(self.model_type(**kwargs)), True
+        return await self.add(self.model_type(**kwargs)), True  # pyright: ignore[reportGeneralTypeIssues]
 
     async def get_one(self, **kwargs: Any) -> ModelT:
         """Get instance identified by query filters.
 
         Args:
             **kwargs: Instance attribute value filters.
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/dto.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         for key, parsed_type in get_model_type_hints(model_type, namespace=namespace).items():
             elem: ElementType | None
             elem = columns.get(key, relationships.get(key))  # pyright:ignore
             if elem is None:
                 continue
 
             if parsed_type.origin is Mapped:
-                (parsed_type,) = parsed_type.inner_types  # noqa: PLW2901
+                (parsed_type,) = parsed_type.inner_types
 
             default, default_factory = _detect_defaults(elem)
 
             field_def = FieldDefinition(
                 name=key,
                 default=default,
                 parsed_type=parsed_type,
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, cast
 
 from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, AsyncSession, async_sessionmaker, create_async_engine
 
 from litestar.types import Empty
-from litestar.utils import (
-    delete_litestar_scope_state,
-    get_litestar_scope_state,
-)
+from litestar.utils import delete_litestar_scope_state, get_litestar_scope_state
 
 from .common import SESSION_SCOPE_KEY, SESSION_TERMINUS_ASGI_EVENTS, GenericSessionConfig, GenericSQLAlchemyConfig
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from sqlalchemy.orm import Session
 
+    from litestar import Litestar
     from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, EmptyType, Message, Scope
 
 __all__ = ("SQLAlchemyAsyncConfig", "AsyncSessionConfig")
 
 
 async def default_before_send_handler(message: Message, _: State, scope: Scope) -> None:
@@ -77,18 +75,18 @@
         """Return the plugin's signature namespace.
 
         Returns:
             A string keyed dict of names to be added to the namespace for signature forward reference resolution.
         """
         return {"AsyncEngine": AsyncEngine, "AsyncSession": AsyncSession}
 
-    async def on_shutdown(self, state: State) -> None:
+    async def on_shutdown(self, app: Litestar) -> None:
         """Disposes of the SQLAlchemy engine.
 
         Args:
-            state: The ``Litestar.state`` instance.
+            app: The ``Litestar`` instance.
 
         Returns:
             None
         """
-        engine = cast("AsyncEngine", state.pop(self.engine_app_state_key))
+        engine = cast("AsyncEngine", app.state.pop(self.engine_app_state_key))
         await engine.dispose()
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     from sqlalchemy import Connection, Engine
     from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, AsyncSession, async_sessionmaker
     from sqlalchemy.orm import Mapper, Query, Session, sessionmaker
     from sqlalchemy.orm.session import JoinTransactionMode
     from sqlalchemy.sql import TableClause
 
+    from litestar import Litestar
     from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, EmptyType, Scope
 
 __all__ = (
     "SESSION_SCOPE_KEY",
     "SESSION_TERMINUS_ASGI_EVENTS",
     "GenericSQLAlchemyConfig",
@@ -236,14 +237,14 @@
     def create_app_state_items(self) -> dict[str, Any]:
         """Key/value pairs to be stored in application state."""
         return {
             self.engine_app_state_key: self.create_engine(),
             self.session_maker_app_state_key: self.create_session_maker(),
         }
 
-    def update_app_state(self, state: State) -> None:
+    def update_app_state(self, app: Litestar) -> None:
         """Set the app state with engine and session.
 
         Args:
-            state: The ``Litestar.state`` instance.
+            app: The ``Litestar`` instance.
         """
-        state.update(self.create_app_state_items())
+        app.state.update(self.create_app_state_items())
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, cast
 
 from sqlalchemy import Connection, Engine, create_engine
 from sqlalchemy.orm import Session, sessionmaker
 
-from litestar.utils import (
-    delete_litestar_scope_state,
-    get_litestar_scope_state,
-)
+from litestar.utils import delete_litestar_scope_state, get_litestar_scope_state
 
 from .common import SESSION_SCOPE_KEY, SESSION_TERMINUS_ASGI_EVENTS, GenericSessionConfig, GenericSQLAlchemyConfig
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
+    from litestar import Litestar
     from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, Message, Scope
 
 __all__ = ("SQLAlchemySyncConfig", "SyncSessionConfig")
 
 
 async def default_before_send_handler(message: Message, _: State, scope: Scope) -> None:
@@ -67,18 +65,18 @@
         """Return the plugin's signature namespace.
 
         Returns:
             A string keyed dict of names to be added to the namespace for signature forward reference resolution.
         """
         return {"Engine": Engine, "Session": Session}
 
-    def on_shutdown(self, state: State) -> None:
+    def on_shutdown(self, app: Litestar) -> None:
         """Disposes of the SQLAlchemy engine.
 
         Args:
-            state: The ``Litestar.state`` instance.
+            app: The ``Litestar`` instance.
 
         Returns:
             None
         """
-        engine = cast("Engine", state.pop(self.engine_app_state_key))
+        engine = cast("Engine", app.state.pop(self.engine_app_state_key))
         engine.dispose()
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         """Configure application for use with SQLAlchemy.
 
         Args:
             app_config: The :class:`AppConfig <.config.app.AppConfig>` instance.
         """
         app_config.dependencies.update(
             {
-                self._config.engine_dependency_key: Provide(self._config.provide_engine),
-                self._config.session_dependency_key: Provide(self._config.provide_session),
+                self._config.engine_dependency_key: Provide(self._config.provide_engine, sync_to_thread=False),
+                self._config.session_dependency_key: Provide(self._config.provide_session, sync_to_thread=False),
             }
         )
         app_config.before_send.append(self._config.before_send_handler)
         app_config.on_startup.append(self._config.update_app_state)
         app_config.on_shutdown.append(self._config.on_shutdown)
         app_config.signature_namespace.update(self._config.signature_namespace)
         return app_config
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/repository.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     """
     try:
         yield
     except IntegrityError as exc:
         raise ConflictError from exc
     except SQLAlchemyError as exc:
         raise RepositoryError(f"An exception occurred: {exc}") from exc
+    except AttributeError as exc:
+        raise RepositoryError from exc
 
 
 class SQLAlchemyAsyncRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
     """SQLAlchemy based implementation of the repository interface."""
 
     match_fields: list[str] | str | None = None
 
@@ -262,15 +264,15 @@
                 for field_name in match_fields
                 if kwargs.get(field_name, None) is not None
             }
         else:
             match_filter = kwargs
         existing = await self.get_one_or_none(**match_filter)
         if not existing:
-            return await self.add(self.model_type(**kwargs)), True
+            return await self.add(self.model_type(**kwargs)), True  # pyright: ignore[reportGeneralTypeIssues]
         if upsert:
             for field_name, new_field_value in kwargs.items():
                 field = getattr(existing, field_name, None)
                 if field and field != new_field_value:
                     setattr(existing, field_name, new_field_value)
             if existing in self.session.dirty:
                 return (await self.update(existing)), False
```

### Comparing `litestar-2.0.0a6/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0a7/litestar/contrib/sqlalchemy/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,82 @@
 from __future__ import annotations
 
 import uuid
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, cast
 
 from sqlalchemy.dialects.postgresql import JSONB as PG_JSONB
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
-from sqlalchemy.types import CHAR, TypeDecorator
+from sqlalchemy.types import BINARY, CHAR, BigInteger, Integer, TypeDecorator
 from sqlalchemy.types import JSON as _JSON
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Dialect
 
+BigIntIdentity = BigInteger().with_variant(Integer, "sqlite")
+"""Platform-independent BigInteger Primary Key.
+
+User a Big Integer on engines that support it.
+
+Uses Integer for sqlite since there is no
+
+"""
+
 
 class GUID(TypeDecorator):
     """Platform-independent GUID type.
 
     Uses PostgreSQL's UUID type, otherwise uses
-    CHAR(32), storing as stringified hex values.
+    BINARY(16) or CHAR(32), storing as stringified hex values.
 
     Will accept stringified UUIDs as a hexstring or an actual UUID
 
     """
 
-    impl = CHAR
+    impl = BINARY(16)
     cache_ok = True
+    python_type = type(uuid.UUID)
+
+    def __init__(self, binary: bool = True) -> None:
+        self.binary = binary
 
     def load_dialect_impl(self, dialect: Dialect) -> Any:
         if dialect.name == "postgresql":
             return dialect.type_descriptor(PG_UUID())
+        if self.binary:
+            return dialect.type_descriptor(BINARY(16))
         return dialect.type_descriptor(CHAR(32))
 
-    def process_bind_param(self, value: str | uuid.UUID | None, dialect: Dialect) -> str | None:
+    def process_bind_param(self, value: bytes | str | uuid.UUID | None, dialect: Dialect) -> bytes | str | None:
         if value is None:
             return value
         if dialect.name == "postgresql":
             return str(value)
+        value = self.to_uuid(value)
+        if value is None:
+            return value
+        return value.bytes if self.binary else value.hex
 
-        if not isinstance(value, uuid.UUID):
-            return "%.32x" % uuid.UUID(value).int
-
-        # hexstring
-        return "%.32x" % value.int
-
-    def process_result_value(self, value: str | uuid.UUID | None, dialect: Dialect) -> uuid.UUID | None:
+    def process_result_value(self, value: bytes | str | uuid.UUID | None, dialect: Dialect) -> uuid.UUID | None:
         if value is None:
             return value
-        if not isinstance(value, uuid.UUID):
-            return uuid.UUID(value)
-        return value
+        if isinstance(value, uuid.UUID):
+            return value
+        if self.binary:
+            return uuid.UUID(bytes=cast("bytes", value))
+        return uuid.UUID(hex=cast("str", value))
+
+    @staticmethod
+    def to_uuid(value: Any) -> uuid.UUID | None:
+        if isinstance(value, uuid.UUID) or value is None:
+            return value
+        try:
+            value = uuid.UUID(hex=value)
+        except (TypeError, ValueError):
+            value = uuid.UUID(bytes=value)
+        return cast("uuid.UUID | None", value)
 
 
 class JSON(_JSON):
     """Platform-independent JSON type.
 
     Uses JSONB type for postgres, otherwise uses the generic JSON data type.
     """
```

### Comparing `litestar-2.0.0a6/litestar/controller.py` & `litestar-2.0.0a7/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/data_extractors.py` & `litestar-2.0.0a7/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/__init__.py` & `litestar-2.0.0a7/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/cookie.py` & `litestar-2.0.0a7/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/headers.py` & `litestar-2.0.0a7/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0a7/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/response_header.py` & `litestar-2.0.0a7/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/state.py` & `litestar-2.0.0a7/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/upload_file.py` & `litestar-2.0.0a7/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/datastructures/url.py` & `litestar-2.0.0a7/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/di.py` & `litestar-2.0.0a7/litestar/di.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from inspect import isclass
 from typing import TYPE_CHECKING, Any
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
 from litestar.utils import Ref, is_async_callable
+from litestar.utils.warnings import warn_implicit_sync_to_thread, warn_sync_to_thread_with_async_callable
 
 __all__ = ("Provide",)
 
 
 if TYPE_CHECKING:
     from litestar._signature import SignatureModel
     from litestar.types import AnyCallable
@@ -31,29 +32,35 @@
     signature_model: type[SignatureModel]
     dependency: Ref[AnyCallable]
 
     def __init__(
         self,
         dependency: AnyCallable | type,
         use_cache: bool = False,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
     ) -> None:
         """Initialize ``Provide``
 
         Args:
             dependency: Callable to call or class to instantiate. The result is then injected as a dependency.
             use_cache: Cache the dependency return value. Defaults to False.
             sync_to_thread: Run sync code in an async thread. Defaults to False.
         """
         if not callable(dependency):
             raise ImproperlyConfiguredException("Provider dependency must a callable value")
 
         self.dependency = Ref["AnyCallable"](dependency)
         self.has_sync_callable = isclass(dependency) or not is_async_callable(dependency)
-        self.sync_to_thread = sync_to_thread
+        if self.has_sync_callable and sync_to_thread is None:
+            warn_implicit_sync_to_thread(dependency, stacklevel=3)
+
+        if not self.has_sync_callable and sync_to_thread is not None:
+            warn_sync_to_thread_with_async_callable(dependency, stacklevel=3)
+
+        self.sync_to_thread = bool(sync_to_thread)
         self.use_cache = use_cache
         self.value: Any = Empty
 
     async def __call__(self, **kwargs: Any) -> Any:
         """Call the provider's dependency."""
 
         if self.use_cache and self.value is not Empty:
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/abc.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """DTO backends do the heavy lifting of decoding and validating raw bytes into domain models, and
 back again, to bytes.
 """
 from __future__ import annotations
 
+import secrets
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Final, Generic, TypeVar, Union
+
+from msgspec import UNSET, UnsetType
 
 from litestar._openapi.schema_generation import create_schema
 from litestar._signature.field import SignatureField
+from litestar.dto.factory import DTOData
 from litestar.utils.helpers import get_fully_qualified_class_name
+from litestar.utils.signature import ParsedType
 
 from .types import (
     CollectionType,
     CompositeType,
     MappingType,
     NestedFieldInfo,
     SimpleType,
@@ -24,23 +29,22 @@
     RenameStrategies,
     build_annotation_for_backend,
     should_exclude_field,
     transfer_data,
 )
 
 if TYPE_CHECKING:
-    from typing import AbstractSet, Any, Callable, Final, Generator
+    from typing import AbstractSet, Any, Callable, Generator
 
     from litestar.dto.factory import DTOConfig
     from litestar.dto.factory.types import FieldDefinition
     from litestar.dto.interface import ConnectionContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
-    from litestar.utils.signature import ParsedType
 
     from .types import FieldDefinitionsType
 
 __all__ = ("AbstractDTOBackend", "BackendContext")
 
 BackendT = TypeVar("BackendT")
 
@@ -95,14 +99,15 @@
     """
 
 
 class AbstractDTOBackend(ABC, Generic[BackendT]):
     __slots__ = (
         "annotation",
         "context",
+        "dto_data_type",
         "parsed_field_definitions",
         "reverse_name_map",
         "transfer_model_type",
     )
 
     def __init__(self, context: BackendContext) -> None:
         """Create dto backend instance.
@@ -111,15 +116,21 @@
             context: context of the type represented by this backend.
         """
         self.context = context
         self.parsed_field_definitions = self.parse_model(context.model_type, context.config.exclude)
         self.transfer_model_type = self.create_transfer_model_type(
             get_fully_qualified_class_name(context.model_type), self.parsed_field_definitions
         )
-        self.annotation = build_annotation_for_backend(context.parsed_type.annotation, self.transfer_model_type)
+        self.dto_data_type: type[DTOData] | None = None
+        if context.parsed_type.is_subclass_of(DTOData):
+            self.dto_data_type = context.parsed_type.annotation
+            annotation = self.dto_data_type.parsed_type.annotation
+        else:
+            annotation = context.parsed_type.annotation
+        self.annotation = build_annotation_for_backend(annotation, self.transfer_model_type)
 
     def parse_model(
         self,
         model_type: Any,
         exclude: AbstractSet[str],
         nested_depth: int = 0,
     ) -> FieldDefinitionsType:
@@ -148,14 +159,19 @@
             {"new_field": (str | None, None)}
         """
         defined_fields = []
         for field_definition in self.context.field_definition_generator(model_type):
             if should_exclude_field(field_definition, exclude, self.context.dto_for):
                 continue
 
+            if self.context.config.partial:
+                field_definition = field_definition.copy_with(
+                    parsed_type=ParsedType(Union[field_definition.parsed_type.annotation, UnsetType]), default=UNSET
+                )
+
             try:
                 transfer_type = self._create_transfer_type(
                     field_definition.parsed_type,
                     exclude,
                     field_definition.name,
                     field_definition.unique_name(),
                     nested_depth,
@@ -170,14 +186,15 @@
             else:
                 serialization_name = field_definition.name
 
             transfer_field_definition = TransferFieldDefinition.from_field_definition(
                 field_definition=field_definition,
                 serialization_name=serialization_name,
                 transfer_type=transfer_type,
+                is_partial=self.context.config.partial,
             )
             defined_fields.append(transfer_field_definition)
         return tuple(defined_fields)
 
     @abstractmethod
     def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BackendT]:
         """Create a model for data transfer.
@@ -220,31 +237,51 @@
         Args:
             builtins: Builtin type.
             connection_context: Information about the active connection.
 
         Returns:
             Instance or collection of ``model_type`` instances.
         """
-        return transfer_data(
-            self.context.model_type,
-            self.parse_builtins(builtins, connection_context),
-            self.parsed_field_definitions,
-            "data",
-        )
+        if self.dto_data_type:
+            return self.dto_data_type(
+                backend=self,
+                data_as_builtins=transfer_data(
+                    dict, self.parse_builtins(builtins, connection_context), self.parsed_field_definitions, "data"
+                ),
+            )
+        return self.transfer_data_from_builtins(self.parse_builtins(builtins, connection_context))
+
+    def transfer_data_from_builtins(self, builtins: Any) -> Any:
+        """Populate model instance from builtin types.
+
+        Args:
+            builtins: Builtin type.
+
+        Returns:
+            Instance or collection of ``model_type`` instances.
+        """
+        return transfer_data(self.context.model_type, builtins, self.parsed_field_definitions, "data")
 
     def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
         """Parse raw bytes into instance of `model_type`.
 
         Args:
             raw: bytes
             connection_context: Information about the active connection.
 
         Returns:
             Instance or collection of ``model_type`` instances.
         """
+        if self.dto_data_type:
+            return self.dto_data_type(
+                backend=self,
+                data_as_builtins=transfer_data(
+                    dict, self.parse_raw(raw, connection_context), self.parsed_field_definitions, "data"
+                ),
+            )
         return transfer_data(
             self.context.model_type, self.parse_raw(raw, connection_context), self.parsed_field_definitions, "data"
         )
 
     def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
         """Encode data into a ``LitestarEncodableType``.
 
@@ -368,14 +405,19 @@
         )
         return UnionType(
             parsed_type=parsed_type,
             inner_types=inner_types,
             has_nested=any(_determine_has_nested(t) for t in inner_types),
         )
 
+    def _gen_unique_name_id(self, unique_name: str, size: int = 12) -> str:
+        # Generate a unique ID
+        # Convert the ID to a short alphanumeric string
+        return f"{unique_name}-{secrets.token_hex(8)}"
+
 
 def _filter_exclude(exclude: AbstractSet[str], field_name: str) -> AbstractSet[str]:
     """Filter exclude set to only include exclusions for the given field name."""
     return {split[1] for s in exclude if (split := s.split(".", 1))[0] == field_name}
 
 
 def _enumerate_name(name: str, index: int) -> str:
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/backend.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 T = TypeVar("T")
 
 
 class MsgspecDTOBackend(AbstractDTOBackend[Struct]):
     __slots__ = ()
 
     def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[Struct]:
-        return _create_struct_for_field_definitions(unique_name, field_definitions)
+        fqn_uid: str = self._gen_unique_name_id(unique_name)
+        return _create_struct_for_field_definitions(fqn_uid, field_definitions)
 
     def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> Struct | Collection[Struct]:
         return decode_media_type(  # type:ignore[no-any-return]
             raw, connection_context.request_encoding_type, type_=self.annotation
         )
 
     def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/utils.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/backend.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 T = TypeVar("T")
 
 
 class PydanticDTOBackend(AbstractDTOBackend[BaseModel]):
     __slots__ = ()
 
     def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BaseModel]:
-        return _create_model_for_field_definitions(unique_name, field_definitions)
+        fqn_uid: str = self._gen_unique_name_id(unique_name)
+        return _create_model_for_field_definitions(fqn_uid, field_definitions)
 
     def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> BaseModel | Collection[BaseModel]:
         return decode_media_type(  # type:ignore[no-any-return]
             raw, connection_context.request_encoding_type, type_=self.annotation
         )
 
     def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/utils.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/types.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,32 +87,39 @@
 
     key_type: CompositeType | SimpleType
     value_type: CompositeType | SimpleType
 
 
 @dataclass(frozen=True)
 class TransferFieldDefinition(FieldDefinition):
-    __slots__ = ("transfer_type", "serialization_name")
+    __slots__ = (
+        "is_partial",
+        "serialization_name",
+        "transfer_type",
+    )
 
     transfer_type: TransferType
     """Type of the field for transfer."""
     serialization_name: str
     """Name of the field as it should feature on the transfer model."""
+    is_partial: bool
+    """Whether the field is optional for transfer."""
 
     @classmethod
     def from_field_definition(
-        cls, field_definition: FieldDefinition, transfer_type: TransferType, serialization_name: str
+        cls, field_definition: FieldDefinition, transfer_type: TransferType, serialization_name: str, is_partial: bool
     ) -> Self:
         return cls(
             name=field_definition.name,
             default=field_definition.default,
             parsed_type=field_definition.parsed_type,
             default_factory=field_definition.default_factory,
             serialization_name=serialization_name,
             unique_model_name=field_definition.unique_model_name,
             transfer_type=transfer_type,
             dto_field=field_definition.dto_field,
+            is_partial=is_partial,
         )
 
 
 FieldDefinitionsType: TypeAlias = "tuple[TransferFieldDefinition, ...]"
 """Generic representation of names and types."""
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/_backends/utils.py` & `litestar-2.0.0a7/litestar/dto/factory/_backends/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from collections.abc import Collection as CollectionsCollection
-from typing import TYPE_CHECKING, TypeVar, cast
+from typing import TYPE_CHECKING, Collection, Mapping, TypeVar, cast
 
+from msgspec import UNSET
 from typing_extensions import get_origin
 
 from litestar.dto.factory import Mark
 
 from .types import (
     CollectionType,
     CompositeType,
@@ -15,17 +15,15 @@
     SimpleType,
     TransferType,
     TupleType,
     UnionType,
 )
 
 if TYPE_CHECKING:
-    from typing import AbstractSet, Any, Collection, Iterable
-
-    from msgspec import Struct
+    from typing import AbstractSet, Any, Iterable
 
     from litestar.dto.factory.types import FieldDefinition, RenameStrategy
     from litestar.dto.types import ForType
 
     from .types import FieldDefinitionsType
 
 __all__ = (
@@ -134,42 +132,49 @@
         source_data: data that has been parsed and validated via the backend.
         field_definitions: model field definitions.
         dto_for: indicates whether the DTO is for the request body or response.
 
     Returns:
         Data parsed into ``destination_type``.
     """
-    if isinstance(source_data, CollectionsCollection):
+    if not isinstance(source_data, Mapping) and isinstance(source_data, Collection):
         return type(source_data)(
             transfer_data(destination_type, item, field_definitions, dto_for)  # type:ignore[call-arg]
             for item in source_data
         )
     return transfer_instance_data(destination_type, source_data, field_definitions, dto_for)
 
 
 def transfer_instance_data(
-    destination_type: type[T], source_instance: Struct, field_definitions: FieldDefinitionsType, dto_for: ForType
+    destination_type: type[T], source_instance: Any, field_definitions: FieldDefinitionsType, dto_for: ForType
 ) -> T:
     """Create instance of ``destination_type`` with data from ``source_instance``.
 
     Args:
         destination_type: the model type received by the DTO on type narrowing.
         source_instance: primitive data that has been parsed and validated via the backend.
         field_definitions: model field definitions.
         dto_for: indicates whether the DTO is for the request body or response.
 
     Returns:
         Data parsed into ``model_type``.
     """
     unstructured_data = {}
+    source_is_mapping = isinstance(source_instance, Mapping)
+
+    def filter_missing(value: Any) -> bool:
+        return value is UNSET
+
     for field_definition in field_definitions:
         transfer_type = field_definition.transfer_type
         source_name = field_definition.serialization_name if dto_for == "data" else field_definition.name
         destination_name = field_definition.name if dto_for == "data" else field_definition.serialization_name
-        source_value = getattr(source_instance, source_name)
+        source_value = source_instance[source_name] if source_is_mapping else getattr(source_instance, source_name)
+        if field_definition.is_partial and dto_for == "data" and filter_missing(source_value):
+            continue
         unstructured_data[destination_name] = transfer_type_data(source_value, transfer_type, dto_for)
     return destination_type(**unstructured_data)
 
 
 def transfer_type_data(source_value: Any, transfer_type: TransferType, dto_for: ForType) -> Any:
     if isinstance(transfer_type, SimpleType) and transfer_type.nested_field_info:
         dest_type = transfer_type.parsed_type.annotation if dto_for == "data" else transfer_type.nested_field_info.model
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/abc.py` & `litestar-2.0.0a7/litestar/dto/factory/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from litestar.dto.interface import ConnectionContext, DTOInterface
 from litestar.enums import RequestEncodingType
 from litestar.utils.signature import ParsedType
 
 from ._backends import MsgspecDTOBackend, PydanticDTOBackend
 from ._backends.abc import BackendContext
 from .config import DTOConfig
+from .data_structures import DTOData
 from .exc import InvalidAnnotation
 from .utils import parse_configs_from_annotation
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
     from typing_extensions import Self
@@ -126,20 +127,25 @@
     def on_registration(cls, handler_context: HandlerContext) -> None:
         """Called each time the DTO type is encountered during signature modelling.
 
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
         """
-        if handler_context.parsed_type.is_collection:
-            if len(handler_context.parsed_type.inner_types) != 1:
+        if handler_context.parsed_type.is_subclass_of(DTOData):
+            parsed_type = handler_context.parsed_type.annotation.parsed_type
+        else:
+            parsed_type = handler_context.parsed_type
+
+        if parsed_type.is_collection:
+            if len(parsed_type.inner_types) != 1:
                 raise InvalidAnnotation("AbstractDTOFactory only supports homogeneous collection types")
-            handler_type = handler_context.parsed_type.inner_types[0]
+            handler_type = parsed_type.inner_types[0]
         else:
-            handler_type = handler_context.parsed_type
+            handler_type = parsed_type
 
         if not handler_type.is_subclass_of(cls.model_type):
             raise InvalidAnnotation(
                 f"DTO narrowed with '{cls.model_type}', handler type is '{handler_context.parsed_type.annotation}'"
             )
 
         key = (handler_context.dto_for, handler_context.parsed_type, handler_context.request_encoding_type)
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/config.py` & `litestar-2.0.0a7/litestar/dto/factory/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 
     A custom strategy is any callable that accepts a string as an argument and
     return a string.
 
     Fields defined in ``rename_fields`` are ignored."""
     max_nested_depth: int = 1
     """The maximum depth of nested items allowed for data transfer."""
+    partial: bool = False
+    """Allow transfer of partial data."""
```

### Comparing `litestar-2.0.0a6/litestar/dto/factory/field.py` & `litestar-2.0.0a7/litestar/dto/factory/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0a7/litestar/dto/factory/stdlib/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/factory/types.py` & `litestar-2.0.0a7/litestar/dto/factory/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/factory/utils.py` & `litestar-2.0.0a7/litestar/dto/factory/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/dto/interface.py` & `litestar-2.0.0a7/litestar/dto/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,18 @@
         Returns:
             An optional :class:`RequestBody <.openapi.spec.request_body.RequestBody>` instance.
         """
         return Schema()
 
     @classmethod
     def on_registration(cls, handler_context: HandlerContext) -> None:
-        """Receive the ``parsed_type`` and ``route_handler`` that this DTO is configured to represent.
+        """Receive information about the handler and application of the DTO.
 
-        At this point, if the DTO type does not support the annotated type of ``parsed_type``, it should raise an
-        ``UnsupportedType`` exception.
+        At this point, if the DTO type does not support the annotated type of ``handler_context.parsed_type``, it should
+        raise an ``UnsupportedType`` exception.
 
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
 
         Raises:
             UnsupportedType: If the DTO type does not support the annotated type of ``parsed_type``.
```

### Comparing `litestar-2.0.0a6/litestar/enums.py` & `litestar-2.0.0a7/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/events/emitter.py` & `litestar-2.0.0a7/litestar/events/emitter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from __future__ import annotations
 
+import math
+import sys
 from abc import ABC, abstractmethod
-from asyncio import CancelledError, Queue, Task, create_task
 from collections import defaultdict
-from contextlib import suppress
+from contextlib import AsyncExitStack
 from typing import TYPE_CHECKING, Any, DefaultDict, Sequence
 
-import sniffio
+if sys.version_info < (3, 9):
+    from typing import AsyncContextManager
+else:
+    from contextlib import AbstractAsyncContextManager as AsyncContextManager
+
+import anyio
 
 from litestar.exceptions import ImproperlyConfiguredException
 
 __all__ = ("BaseEventEmitterBackend", "SimpleEventEmitter")
 
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
+    from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+
     from litestar.events.listener import EventListener
 
 
-class BaseEventEmitterBackend(ABC):
+class BaseEventEmitterBackend(AsyncContextManager["BaseEventEmitterBackend"], ABC):
     """Abstract class used to define event emitter backends."""
 
     __slots__ = ("listeners",)
 
     listeners: DefaultDict[str, set[EventListener]]
 
     def __init__(self, listeners: Sequence[EventListener]):
@@ -45,106 +55,79 @@
             **kwargs: kwargs to pass to the listener(s)
 
         Returns:
             None
         """
         raise NotImplementedError("not implemented")
 
-    @abstractmethod
-    async def on_startup(self) -> None:  # pragma: no cover
-        """Hook called on application startup, used to establish connection or perform other async operations.
-
-        Returns:
-            None
-        """
-        raise NotImplementedError("not implemented")
-
-    @abstractmethod
-    async def on_shutdown(self) -> None:  # pragma: no cover
-        """Hook called on application shutdown, used to perform cleanup.
-
-        Returns:
-            None
-        """
-        raise NotImplementedError("not implemented")
-
 
 class SimpleEventEmitter(BaseEventEmitterBackend):
     """Event emitter the works only in the current process"""
 
-    __slots__ = ("_queue", "_worker_task")
-
-    _worker_task: Task | None
+    __slots__ = ("_queue", "_exit_stack", "_receive_stream", "_send_stream")
 
     def __init__(self, listeners: Sequence[EventListener]):
         """Create an event emitter instance.
 
         Args:
             listeners: A list of listeners.
         """
         super().__init__(listeners=listeners)
-        self._queue: Queue | None = None
-        self._worker_task = None
+        self._receive_stream: MemoryObjectReceiveStream | None = None
+        self._send_stream: MemoryObjectSendStream | None = None
+        self._exit_stack: AsyncExitStack | None = None
 
-    async def _worker(self) -> None:
+    @staticmethod
+    async def _worker(receive_stream: MemoryObjectReceiveStream) -> None:
         """Worker that runs in a separate task and continuously pulls events from asyncio queue.
 
         Returns:
             None
         """
-        while self._queue:
-            fn, args, kwargs = await self._queue.get()
-            await fn(*args, **kwargs)
-            self._queue.task_done()
-
-    async def on_startup(self) -> None:
-        """Hook called on application startup, used to establish connection or perform other async operations.
-
-        Returns:
-            None
-        """
-        if sniffio.current_async_library() != "asyncio":
-            return
-
-        self._queue = Queue()
-        self._worker_task = create_task(self._worker())
-
-    async def on_shutdown(self) -> None:
-        """Hook called on application shutdown, used to perform cleanup.
-
-        Returns:
-            None
-        """
-
-        if self._queue:
-            await self._queue.join()
+        async with receive_stream:
+            async for item in receive_stream:
+                fn, args, kwargs = item
+                await fn(*args, **kwargs)
+
+    async def __aenter__(self) -> SimpleEventEmitter:
+        self._exit_stack = AsyncExitStack()
+        send_stream, receive_stream = anyio.create_memory_object_stream(math.inf)
+        self._send_stream = send_stream
+        task_group = anyio.create_task_group()
+
+        await self._exit_stack.enter_async_context(task_group)
+        await self._exit_stack.enter_async_context(send_stream)
+        task_group.start_soon(self._worker, receive_stream)
+
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        if self._exit_stack:
+            await self._exit_stack.__aexit__(exc_type, exc_val, exc_tb)
 
-        if self._worker_task:
-            self._worker_task.cancel()
-            with suppress(CancelledError):
-                await self._worker_task
-
-        self._worker_task = None
-        self._queue = None
+        self._exit_stack = None
+        self._send_stream = None
 
     def emit(self, event_id: str, *args: Any, **kwargs: Any) -> None:
         """Emit an event to all attached listeners.
 
         Args:
             event_id: The ID of the event to emit, e.g 'my_event'.
             *args: args to pass to the listener(s).
             **kwargs: kwargs to pass to the listener(s)
 
         Returns:
             None
         """
-        if not (self._worker_task and self._queue):
-            if sniffio.current_async_library() != "asyncio":
-                raise ImproperlyConfiguredException("{type(self).__name__} only supports 'asyncio' based event loops")
-
-            raise ImproperlyConfiguredException("Worker not running")
+        if not (self._send_stream and self._exit_stack):
+            raise RuntimeError("Emitter not initialized")
 
         if listeners := self.listeners.get(event_id):
             for listener in listeners:
-                self._queue.put_nowait((listener.fn, args, kwargs))
+                self._send_stream.send_nowait((listener.fn, args, kwargs))
             return
         raise ImproperlyConfiguredException(f"no event listeners are registered for event ID: {event_id}")
```

### Comparing `litestar-2.0.0a6/litestar/events/listener.py` & `litestar-2.0.0a7/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/exceptions/__init__.py` & `litestar-2.0.0a7/litestar/exceptions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from .base_exceptions import (
-    LitestarException,
-    MissingDependencyException,
-    SerializationException,
-)
+from .base_exceptions import LitestarException, LitestarWarning, MissingDependencyException, SerializationException
 from .http_exceptions import (
     ClientException,
     HTTPException,
     ImproperlyConfiguredException,
     InternalServerException,
     MethodNotAllowedException,
     NoRouteMatchFoundException,
@@ -21,22 +17,23 @@
 from .websocket_exceptions import WebSocketDisconnect, WebSocketException
 
 __all__ = (
     "ClientException",
     "HTTPException",
     "ImproperlyConfiguredException",
     "InternalServerException",
+    "LitestarException",
+    "LitestarWarning",
     "MethodNotAllowedException",
     "MissingDependencyException",
     "NoRouteMatchFoundException",
     "NotAuthorizedException",
     "NotFoundException",
     "PermissionDeniedException",
     "SerializationException",
     "ServiceUnavailableException",
-    "LitestarException",
     "TemplateNotFoundException",
     "TooManyRequestsException",
     "ValidationException",
     "WebSocketDisconnect",
     "WebSocketException",
 )
```

### Comparing `litestar-2.0.0a6/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0a7/litestar/exceptions/base_exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,7 +41,11 @@
             f"'pip install litestar[{install_package or package}]' to install litestar with the required extra "
             f"or 'pip install {install_package or package}' to install the package separately"
         )
 
 
 class SerializationException(LitestarException):
     """Encoding or decoding of an object failed."""
+
+
+class LitestarWarning(UserWarning):
+    """Base class for Litestar warnings"""
```

### Comparing `litestar-2.0.0a6/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0a7/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0a7/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/file_system.py` & `litestar-2.0.0a7/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/handlers/__init__.py` & `litestar-2.0.0a7/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0a7/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/handlers/base.py` & `litestar-2.0.0a7/litestar/handlers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from copy import copy
 from functools import partial
 from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar, cast
 
 from litestar._signature import create_signature_model
 from litestar._signature.field import SignatureField
+from litestar.di import Provide
 from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
 from litestar.utils import AsyncCallable, Ref, async_partial, get_name, is_async_callable, normalize_path
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_parameter
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar import Litestar
     from litestar._signature.models import SignatureModel
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
-    from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
     from litestar.params import ParameterKwarg
     from litestar.plugins import SerializationPluginProtocol
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.composite_types import MaybePartial
     from litestar.types.empty import EmptyType
@@ -178,15 +178,15 @@
         """
         return get_name(unwrap_partial(self.fn.value))
 
     @property
     def dependency_name_set(self) -> set[str]:
         """Set of all dependency names provided in the handler's ownership layers."""
         layered_dependencies = (layer.dependencies or {} for layer in self.ownership_layers)
-        return {name for layer in layered_dependencies for name in layer}
+        return {name for layer in layered_dependencies for name in layer}  # pyright: ignore
 
     @property
     def ownership_layers(self) -> list[T | Controller | Router]:
         """Return the handler layers from the app down to the route handler.
 
         ``app -> ... -> route handler``
         """
@@ -234,27 +234,29 @@
 
     def resolve_guards(self) -> list[Guard]:
         """Return all guards in the handlers scope, starting from highest to current layer."""
         if self._resolved_guards is Empty:
             self._resolved_guards = []
 
             for layer in self.ownership_layers:
-                self._resolved_guards.extend(layer.guards or [])
+                self._resolved_guards.extend(layer.guards or [])  # pyright: ignore
 
             self._resolved_guards = cast("list[Guard]", [AsyncCallable(guard) for guard in self._resolved_guards])
 
         return self._resolved_guards  # type:ignore
 
     def resolve_dependencies(self) -> dict[str, Provide]:
         """Return all dependencies correlating to handler function's kwargs that exist in the handler's scope."""
         if self._resolved_dependencies is Empty:
             self._resolved_dependencies = {}
 
             for layer in self.ownership_layers:
                 for key, value in (layer.dependencies or {}).items():
+                    if not isinstance(value, Provide):
+                        value = Provide(value)
                     self._validate_dependency_is_unique(
                         dependencies=self._resolved_dependencies, key=key, provider=value
                     )
                     self._resolved_dependencies[key] = value
 
         return cast("dict[str, Provide]", self._resolved_dependencies)
 
@@ -262,37 +264,37 @@
         """Build the middleware stack for the RouteHandler and return it.
 
         The middlewares are added from top to bottom (``app -> router -> controller -> route handler``) and then
         reversed.
         """
         resolved_middleware: list[Middleware] = []
         for layer in self.ownership_layers:
-            resolved_middleware.extend(layer.middleware or [])
+            resolved_middleware.extend(layer.middleware or [])  # pyright: ignore
         return list(reversed(resolved_middleware))
 
     def resolve_exception_handlers(self) -> ExceptionHandlersMap:
         """Resolve the exception_handlers by starting from the route handler and moving up.
 
         This method is memoized so the computation occurs only once.
         """
         resolved_exception_handlers: dict[int | type[Exception], ExceptionHandler] = {}
         for layer in self.ownership_layers:
-            resolved_exception_handlers.update(layer.exception_handlers or {})
+            resolved_exception_handlers.update(layer.exception_handlers or {})  # pyright: ignore
         return resolved_exception_handlers
 
     def resolve_opts(self) -> None:
         """Build the route handler opt dictionary by going from top to bottom.
 
         When merging keys from multiple layers, if the same key is defined by multiple layers, the value from the
         layer closest to the response handler will take precedence.
         """
 
         opt: dict[str, Any] = {}
         for layer in self.ownership_layers:
-            opt.update(layer.opt or {})
+            opt.update(layer.opt or {})  # pyright: ignore
 
         self.opt = opt
 
     def resolve_signature_namespace(self) -> dict[str, Any]:
         """Build the route handler signature namespace dictionary by going from top to bottom.
 
         When merging keys from multiple layers, if the same key is defined by multiple layers, the value from the
```

### Comparing `litestar-2.0.0a6/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0a7/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0a7/litestar/handlers/http_handlers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,38 +28,39 @@
 from litestar.types import (
     AfterRequestHookHandler,
     AfterResponseHookHandler,
     AnyCallable,
     ASGIApp,
     BeforeRequestHookHandler,
     CacheKeyBuilder,
+    Dependencies,
     Empty,
     EmptyType,
     ExceptionHandlersMap,
     Guard,
     Method,
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
     TypeEncodersMap,
 )
 from litestar.types.builtin_types import NoneType
 from litestar.utils import AsyncCallable, async_partial, is_async_callable
+from litestar.utils.warnings import warn_implicit_sync_to_thread, warn_sync_to_thread_with_async_callable
 
 if TYPE_CHECKING:
     from typing import Any, Awaitable, Callable, Sequence
 
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.connection import Request
     from litestar.datastructures import CacheControlHeader, ETag
     from litestar.datastructures.headers import Header
-    from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
     from litestar.types import MaybePartial  # noqa: F401
 
 
 __all__ = ("HTTPRouteHandler", "route")
@@ -120,30 +121,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: Mapping[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         http_method: HttpMethod | Method | Sequence[HttpMethod | Method],
         media_type: MediaType | str | None = None,
         middleware: Sequence[Middleware] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -276,14 +277,20 @@
         # memoized attributes, defaulted to Empty
         self._resolved_after_response: AsyncCallable | None | EmptyType = Empty
         self._resolved_before_request: AsyncCallable | None | EmptyType = Empty
         self._response_handler_mapping: ResponseHandlerMap = {"default_handler": Empty, "response_type_handler": Empty}
 
     def __call__(self, fn: AnyCallable) -> HTTPRouteHandler:
         """Replace a function with itself."""
+        if not is_async_callable(fn):
+            if self.sync_to_thread is None:
+                warn_implicit_sync_to_thread(fn, stacklevel=3)
+        elif self.sync_to_thread is not None:
+            warn_sync_to_thread_with_async_callable(fn, stacklevel=3)
+
         super().__call__(fn)
         return self
 
     def resolve_response_class(self) -> type[Response]:
         """Return the closest custom Response class in the owner graph or the default Response class.
 
         This method is memoized so the computation occurs only once.
```

### Comparing `litestar-2.0.0a6/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0a7/litestar/handlers/http_handlers/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 if TYPE_CHECKING:
     from typing import Any, Mapping
 
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
     from litestar.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
         CacheKeyBuilder,
+        Dependencies,
         EmptyType,
         ExceptionHandlersMap,
         Guard,
         Middleware,
         ResponseCookies,
         ResponseHeaders,
         ResponseType,
@@ -56,30 +56,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -217,30 +217,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -379,29 +379,29 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -558,30 +558,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -719,30 +719,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
@@ -880,30 +880,30 @@
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
-        dependencies: dict[str, Provide] | None = None,
+        dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
-        sync_to_thread: bool = False,
+        sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
```

### Comparing `litestar-2.0.0a6/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0a7/litestar/handlers/websocket_handlers/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, cast
+from functools import wraps
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Dict, cast
 
+from litestar.di import Provide
 from litestar.dto.interface import ConnectionContext
 from litestar.serialization import decode_json
 from litestar.utils import AsyncCallable
+from litestar.utils.helpers import unwrap_partial
 
 if TYPE_CHECKING:
     from contextlib import AbstractAsyncContextManager
 
     from msgspec.json import Encoder as JsonEncoder
 
     from litestar import WebSocket
@@ -108,29 +111,31 @@
             await socket.send_data(data_to_send, send_mode)  # pyright: ignore
 
     return handle_send
 
 
 def create_handler_function(
     listener_context: ListenerContext,
-    lifespan_manager: Callable[[WebSocket], AbstractAsyncContextManager],
+    lifespan_manager: Callable[..., AbstractAsyncContextManager],
 ) -> Callable[..., Coroutine[None, None, None]]:
     listener_callback = AsyncCallable(listener_context.listener_callback)
 
-    async def handler_fn(*args: Any, socket: WebSocket, **kwargs: Any) -> None:
+    async def handler_fn(
+        *args: Any, socket: WebSocket, connection_lifespan_dependencies: Dict[str, Any], **kwargs: Any  # noqa: UP006
+    ) -> None:
         ctx = ConnectionContext.from_connection(socket)
         data_dto = listener_context.resolved_data_dto(ctx) if listener_context.resolved_data_dto else None
         return_dto = listener_context.resolved_return_dto(ctx) if listener_context.resolved_return_dto else None
         handle_receive = listener_context.handle_receive
         handle_send = listener_context.handle_send if listener_context.can_send_data else None
 
         if listener_context.pass_socket:
             kwargs["socket"] = socket
 
-        async with lifespan_manager(socket):
+        async with lifespan_manager(**connection_lifespan_dependencies):
             while True:
                 received_data = await handle_receive(socket, data_dto)
                 data_to_send = await listener_callback(*args, data=received_data, **kwargs)
                 if handle_send:
                     await handle_send(socket, data_to_send, return_dto)
 
     return handler_fn
@@ -151,8 +156,28 @@
 
     Returns:
         The :class:`inspect.Signature` for the listener callback as required for signature modelling.
     """
     new_params = [p for p in callback_signature.parameters.values() if p.name not in {"data"}]
     if "socket" not in callback_signature.parameters:
         new_params.append(inspect.Parameter(name="socket", kind=inspect.Parameter.KEYWORD_ONLY, annotation="WebSocket"))
+
+    new_params.append(
+        inspect.Parameter(
+            name="connection_lifespan_dependencies", kind=inspect.Parameter.KEYWORD_ONLY, annotation="Dict[str, Any]"
+        )
+    )
+
     return callback_signature.replace(parameters=new_params)
+
+
+def create_stub_dependency(src: AnyCallable) -> Provide:
+    """Create a stub dependency, accepting any kwargs defined in ``src``, and
+    wrap it in ``Provide``
+    """
+    src = unwrap_partial(src)
+
+    @wraps(src)
+    async def stub(**kwargs: Any) -> Dict[str, Any]:  # noqa: UP006
+        return kwargs
+
+    return Provide(stub)
```

### Comparing `litestar-2.0.0a6/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0a7/litestar/router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,321 +1,312 @@
 from __future__ import annotations
 
-import inspect
-from abc import ABC, abstractmethod
-from contextlib import AbstractAsyncContextManager, asynccontextmanager
-from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    AsyncGenerator,
-    Callable,
-    Mapping,
-    cast,
-)
-
-from msgspec.json import Encoder as JsonEncoder
-
-from litestar._signature import create_signature_model
-from litestar.connection import WebSocket
-from litestar.dto.interface import HandlerContext
-from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
-from litestar.serialization import default_serializer
-from litestar.types import (
-    AnyCallable,
-    Dependencies,
-    Empty,
-    EmptyType,
-    ExceptionHandler,
-    Guard,
-    Middleware,
-    SyncOrAsyncUnion,
-    TypeEncodersMap,
-)
-from litestar.types.builtin_types import NoneType
-from litestar.utils import AsyncCallable
-from litestar.utils.signature import ParsedSignature
+from collections import defaultdict
+from copy import copy
+from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, Sequence, cast
+
+from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
+from litestar.controller import Controller
+from litestar.exceptions import ImproperlyConfiguredException
+from litestar.handlers.asgi_handlers import ASGIRouteHandler
+from litestar.handlers.http_handlers import HTTPRouteHandler
+from litestar.handlers.websocket_handlers import WebsocketListener, WebsocketRouteHandler
+from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
+from litestar.types.empty import Empty
+from litestar.utils import find_index, is_class_and_subclass, join_paths, normalize_path, unique
+from litestar.utils.sync import AsyncCallable
 
-from . import _utils
-from .route_handler import WebsocketRouteHandler
+__all__ = ("Router",)
 
-if TYPE_CHECKING:
-    from typing import Coroutine
 
-    from litestar import Litestar
+if TYPE_CHECKING:
+    from litestar.datastructures import CacheControlHeader, ETag
     from litestar.dto.interface import DTOInterface
-    from litestar.types.asgi_types import WebSocketMode
-
+    from litestar.openapi.spec import SecurityRequirement
+    from litestar.routes import BaseRoute
+    from litestar.types import (
+        AfterRequestHookHandler,
+        AfterResponseHookHandler,
+        BeforeRequestHookHandler,
+        ControllerRouterHandler,
+        ExceptionHandlersMap,
+        Guard,
+        Middleware,
+        ParametersMap,
+        ResponseCookies,
+        ResponseType,
+        RouteHandlerMapItem,
+        RouteHandlerType,
+        TypeEncodersMap,
+    )
+    from litestar.types.composite_types import Dependencies, ResponseHeaders
+    from litestar.types.empty import EmptyType
 
-__all__ = ("WebsocketListener", "websocket_listener")
 
+class Router:
+    """The Litestar Router class.
 
-class websocket_listener(WebsocketRouteHandler):
-    """A websocket listener that automatically accepts a connection, handles disconnects,
-    invokes a callback function every time new data is received and sends any data
-    returned
+    A Router instance is used to group controller, routers and route handler functions under a shared path fragment
     """
 
-    __slots__ = {
-        "connection_accept_handler": "Callback to accept a WebSocket connection. By default, calls WebSocket.accept",
-        "on_accept": "Callback invoked after a WebSocket connection has been accepted",
-        "on_disconnect": "Callback invoked after a WebSocket connection has been closed",
-        "_pass_socket": None,
-        "_receive_mode": None,
-        "_send_mode": None,
-        "_listener_context": None,
-        "_connection_lifespan": None,
-    }
+    __slots__ = (
+        "after_request",
+        "after_response",
+        "before_request",
+        "cache_control",
+        "dependencies",
+        "dto",
+        "etag",
+        "exception_handlers",
+        "guards",
+        "middleware",
+        "opt",
+        "owner",
+        "parameters",
+        "path",
+        "registered_route_handler_ids",
+        "response_class",
+        "response_cookies",
+        "response_headers",
+        "return_dto",
+        "routes",
+        "security",
+        "signature_namespace",
+        "tags",
+        "type_encoders",
+    )
 
     def __init__(
         self,
-        path: str | None | list[str] | None = None,
+        path: str,
         *,
-        connection_accept_handler: Callable[[WebSocket], Coroutine[Any, Any, None]] = WebSocket.accept,
-        connection_lifespan: Callable[[WebSocket], AbstractAsyncContextManager[Any]] | None = None,
+        after_request: AfterRequestHookHandler | None = None,
+        after_response: AfterResponseHookHandler | None = None,
+        before_request: BeforeRequestHookHandler | None = None,
+        cache_control: CacheControlHeader | None = None,
         dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
-        exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
-        guards: list[Guard] | None = None,
-        middleware: list[Middleware] | None = None,
-        receive_mode: WebSocketMode = "text",
-        send_mode: WebSocketMode = "text",
-        name: str | None = None,
-        on_accept: Callable[[WebSocket], SyncOrAsyncUnion[None]] | None = None,
-        on_disconnect: Callable[[WebSocket], SyncOrAsyncUnion[None]] | None = None,
-        opt: dict[str, Any] | None = None,
+        etag: ETag | None = None,
+        exception_handlers: ExceptionHandlersMap | None = None,
+        guards: Sequence[Guard] | None = None,
+        middleware: Sequence[Middleware] | None = None,
+        opt: Mapping[str, Any] | None = None,
+        parameters: ParametersMap | None = None,
+        response_class: ResponseType | None = None,
+        response_cookies: ResponseCookies | None = None,
+        response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        route_handlers: Sequence[ControllerRouterHandler],
+        security: Sequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
+        tags: Sequence[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
-        **kwargs: Any,
     ) -> None:
-        """Initialize ``WebsocketRouteHandler``
+        """Initialize a ``Router``.
 
         Args:
-            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
-                to ``/``
-            connection_accept_handler: A callable that accepts a :class:`WebSocket <.connection.WebSocket>` instance
-                and returns a coroutine that when awaited, will accept the connection. Defaults to ``WebSocket.accept``.
-            connection_lifespan: An asynchronous context manager, handling the lifespan of the connection. By default,
-                it calls the ``connection_accept_handler``, ``on_connect`` and ``on_disconnect``.
-            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
+                to any route handler. If this function returns a value, the request will not reach the route handler,
+                and instead this value will be used.
+            after_response: A sync or async function called after the response has been awaited. It receives the
+                :class:`Request <.connection.Request>` object and should not return any values.
+            before_request: A sync or async function called immediately before calling the route handler. Receives
+                the :class:`litestar.connection.Request` instance and any non-``None`` return value is used for the
+                response, bypassing the route handler.
+            cache_control: A ``cache-control`` header of type
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to route handlers of
+                this router. Can be overridden by route handlers.
+            dependencies: A string keyed mapping of dependency :class:`Provide <.di.Provide>` instances.
             dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
                 validation of request data.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
-            receive_mode: Websocket mode to receive data in, either `text` or `binary`.
-            send_mode: Websocket mode to receive data in, either `text` or `binary`.
-            name: A string identifying the route handler.
-            on_accept: Callback invoked after a connection has been accepted, receiving the
-                :class:`WebSocket <.connection.WebSocket>` instance as its only argument
-            on_disconnect: Callback invoked after a connection has been closed, receiving the
-                :class:`WebSocket <.connection.WebSocket>` instance as its only argument
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+            guards: A sequence of :data:`Guard <.types.Guard>` callables.
+            middleware: A sequence of :data:`Middleware <.types.Middleware>`.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :data:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <.connection.Request>` or
-                :class:`ASGI Scope <.types.Scope>`.
+                :data:`ASGI Scope <.types.Scope>`.
+            parameters: A mapping of :func:`Parameter <.params.Parameter>` definitions available to all application
+                paths.
+            path: A path fragment that is prefixed to all route handlers, controllers and other routers associated
+                with the router instance.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the default for
+                all route handlers, controllers and other routers associated with the router instance.
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
+                instances.
             return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
                 outbound response data.
-            signature_namespace: A mapping of names to types for use in forward reference resolution during signature
-                modelling.
+            route_handlers: A required sequence of route handlers, which can include instances of
+                :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
+                function decorated by the route handler decorators.
+            security: A sequence of dicts that will be added to the schema of all route handlers in the application.
+                See :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
+                for details.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+            tags: A sequence of string tags that will be appended to the schema of all route handlers under the
+                application.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-            **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
-        self._listener_context = _utils.ListenerContext()
-        self._receive_mode: WebSocketMode = receive_mode
-        self._send_mode: WebSocketMode = send_mode
-        self._connection_lifespan = connection_lifespan
-
-        self.connection_accept_handler = connection_accept_handler
-        self.on_accept = AsyncCallable(on_accept) if on_accept else None
-        self.on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
-        self.type_encoders = type_encoders
-
-        super().__init__(
-            path=path,
-            dependencies=dependencies,
-            exception_handlers=exception_handlers,
-            guards=guards,
-            middleware=middleware,
-            name=name,
-            opt=opt,
-            signature_namespace=signature_namespace,
-            **kwargs,
-        )
 
-        # need to be assigned after the super() call
+        self.after_request = AsyncCallable(after_request) if after_request else None  # type: ignore[arg-type]
+        self.after_response = AsyncCallable(after_response) if after_response else None
+        self.before_request = AsyncCallable(before_request) if before_request else None
+        self.cache_control = cache_control
         self.dto = dto
+        self.etag = etag
+        self.dependencies = dict(dependencies or {})
+        self.exception_handlers = dict(exception_handlers or {})
+        self.guards = list(guards or [])
+        self.middleware = list(middleware or [])
+        self.opt = dict(opt or {})
+        self.owner: Router | None = None
+        self.parameters = dict(parameters or {})
+        self.path = normalize_path(path)
+        self.response_class = response_class
+        self.response_cookies = narrow_response_cookies(response_cookies)
+        self.response_headers = narrow_response_headers(response_headers)
         self.return_dto = return_dto
+        self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
+        self.security = list(security or [])
+        self.signature_namespace = signature_namespace or {}
+        self.tags = list(tags or [])
+        self.registered_route_handler_ids: set[int] = set()
+        self.type_encoders = dict(type_encoders) if type_encoders is not None else None
 
-    @asynccontextmanager
-    async def default_connection_lifespan(self, socket: WebSocket) -> AsyncGenerator[None, None]:
-        """Handle the connection lifespan of a WebSocket.
-
-        By, default this will
-
-            - Call :attr:`connection_accept_handler` to accept a connection
-            - Call :attr:`on_accept` if defined after a connection has been accepted
-            - Call :attr:`on_disconnect` upon leaving the context
-        """
-        await self.connection_accept_handler(socket)
+        for route_handler in route_handlers or []:
+            self.register(value=route_handler)
 
-        if self.on_accept:
-            await self.on_accept(socket)
-        try:
-            yield
-        except WebSocketDisconnect:
-            pass
-        finally:
-            if self.on_disconnect:
-                await self.on_disconnect(socket)
-
-    def _validate_handler_function(self) -> None:
-        """Validate the route handler function once it's set by inspecting its return annotations."""
-        # since none of the validation rules of WebsocketRouteHandler apply here, this is let empty. Validation of the
-        # user supplied method happens at init time of this handler instead in __call__
-
-    def _init_handler_dtos(self) -> None:
-        """Initialize the data and return DTOs for the handler."""
-        if dto := self.resolve_dto():
-            data_parameter = self._listener_context.listener_callback_signature.parameters["data"]
-            dto.on_registration(HandlerContext("data", str(self), data_parameter.parsed_type))
-
-        if return_dto := self.resolve_return_dto():
-            return_type = self._listener_context.listener_callback_signature.return_type
-            return_dto.on_registration(HandlerContext("return", str(self), return_type))
-
-    def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
-        self._listener_context.listener_callback = listener_callback
-        self._listener_context.handler_function = handler_function = _utils.create_handler_function(
-            listener_context=self._listener_context,
-            lifespan_manager=self._connection_lifespan or self.default_connection_lifespan,
-        )
-        return super().__call__(handler_function)
+    def register(self, value: ControllerRouterHandler) -> list[BaseRoute]:
+        """Register a Controller, Route instance or RouteHandler on the router.
 
-    def on_registration(self, app: Litestar) -> None:
-        self._set_listener_context()
-        super().on_registration(app)
-
-    def _create_signature_model(self, app: Litestar) -> None:
-        """Create signature model for handler function."""
-        if not self.signature_model:
-            extra_signatures = []
-            if self.on_accept:
-                extra_signatures.append(inspect.signature(self.on_accept))
-            if self.on_disconnect:
-                extra_signatures.append(inspect.signature(self.on_disconnect))
-
-            new_signature = _utils.create_handler_signature(
-                self._listener_context.listener_callback_signature.original_signature
-            )
-            self.signature_model = create_signature_model(
-                dependency_name_set=self.dependency_name_set,
-                fn=cast("AnyCallable", self.fn.value),
-                preferred_validation_backend=app.preferred_validation_backend,
-                parsed_signature=ParsedSignature.from_signature(new_signature, self.resolve_signature_namespace()),
-            )
-
-    def _set_listener_context(self) -> None:
-        listener_context = self._listener_context
-        listener_context.listener_callback_signature = listener_callback_signature = ParsedSignature.from_fn(
-            listener_context.listener_callback, self.resolve_signature_namespace()
-        )
-
-        if "data" not in listener_callback_signature.parameters:
-            raise ImproperlyConfiguredException("Websocket listeners must accept a 'data' parameter")
-
-        for param in ("request", "body"):
-            if param in listener_callback_signature.parameters:
-                raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket listeners")
-
-        listener_context.can_send_data = not listener_callback_signature.return_type.is_subclass_of(NoneType)
-        listener_context.pass_socket = "socket" in listener_callback_signature.parameters
-        listener_context.resolved_data_dto = resolved_data_dto = self.resolve_dto()
-        listener_context.resolved_return_dto = resolved_return_dto = self.resolve_return_dto()
-        listener_context.handle_receive = _utils.create_handle_receive(
-            resolved_data_dto, self._receive_mode, listener_callback_signature.parameters["data"].annotation
-        )
-        should_encode_to_json = not (
-            listener_callback_signature.return_type.is_subclass_of((str, bytes))
-            or (
-                listener_callback_signature.return_type.is_optional
-                and listener_callback_signature.return_type.has_inner_subclass_of((str, bytes))
-            )
-        )
-        json_encoder = JsonEncoder(enc_hook=partial(default_serializer, type_encoders=self.resolve_type_encoders()))
-        listener_context.handle_send = _utils.create_handle_send(
-            resolved_return_dto, json_encoder, should_encode_to_json, self._send_mode
-        )
+        Args:
+            value: a subclass or instance of Controller, an instance of :class:`Router` or a function/method that has
+                been decorated by any of the routing decorators, e.g. :class:`get <.handlers.get>`,
+                :class:`post <.handlers.post>`.
 
+        Returns:
+            Collection of handlers added to the router.
+        """
+        validated_value = self._validate_registration_value(value)
 
-class WebsocketListener(ABC):
-    path: str | None | list[str] | None = None
-    """A path fragment for the route handler function or a sequence of path fragments. If not given defaults to ``/``"""
-    dependencies: Dependencies | None = None
-    """A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances."""
-    dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data"""
-    exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None
-    """A mapping of status codes and/or exception types to handler functions."""
-    guards: list[Guard] | None = None
-    """A sequence of :class:`Guard <.types.Guard>` callables."""
-    middleware: list[Middleware] | None = None
-    """A sequence of :class:`Middleware <.types.Middleware>`."""
-    receive_mode: WebSocketMode = "text"
-    """Websocket mode to receive data in, either `text` or `binary`."""
-    send_mode: WebSocketMode = "text"
-    """Websocket mode to send data in, either `text` or `binary`."""
-    name: str | None = None
-    """A string identifying the route handler."""
-    opt: dict[str, Any] | None = None
-    """
-    A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or wherever you
-    have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
-    """
-    return_dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing outbound response data."""
-    signature_namespace: Mapping[str, Any] | None = None
-    """
-    A mapping of names to types for use in forward reference resolution during signature modelling.
-    """
-    type_encoders: TypeEncodersMap | None = None
-    """
-    type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-    """
+        routes: list[BaseRoute] = []
 
-    def __init__(self) -> None:
-        self._handler = websocket_listener(
-            dependencies=self.dependencies,
-            dto=self.dto,
-            exception_handlers=self.exception_handlers,
-            guards=self.guards,
-            middleware=self.middleware,
-            send_mode=self.send_mode,
-            receive_mode=self.receive_mode,
-            name=self.name,
-            on_accept=self.on_accept,
-            on_disconnect=self.on_disconnect,
-            opt=self.opt,
-            path=self.path,
-            return_dto=self.return_dto,
-            signature_namespace=self.signature_namespace,
-            type_encoders=self.type_encoders,
-        )(self.on_receive)
-
-    def on_accept(self, socket: WebSocket) -> SyncOrAsyncUnion[None]:  # noqa: B027
-        """Called after a WebSocket connection has been accepted"""
-
-    @abstractmethod
-    def on_receive(self, *args: Any, **kwargs: Any) -> Any:
-        """Called after data has been received from the WebSocket.
-
-        This should take a ``data`` argument, receiving the processed WebSocket data,
-        and can additionally include handler dependencies such as ``state``, or other
-        regular dependencies.
+        for route_path, handlers_map in self.get_route_handler_map(value=validated_value).items():
+            path = join_paths([self.path, route_path])
+            if http_handlers := unique(
+                [handler for handler in handlers_map.values() if isinstance(handler, HTTPRouteHandler)]
+            ):
+                if existing_handlers := unique(
+                    [
+                        handler
+                        for handler in self.route_handler_method_map.get(path, {}).values()
+                        if isinstance(handler, HTTPRouteHandler)
+                    ]
+                ):
+                    http_handlers.extend(existing_handlers)
+                    existing_route_index = find_index(self.routes, lambda x: x.path == path)  # noqa: B023
+
+                    if existing_route_index == -1:  # pragma: no cover
+                        raise ImproperlyConfiguredException("unable to find_index existing route index")
+
+                    route: WebSocketRoute | ASGIRoute | HTTPRoute = HTTPRoute(
+                        path=path,
+                        route_handlers=http_handlers,
+                    )
+                    self.routes[existing_route_index] = route
+                else:
+                    route = HTTPRoute(path=path, route_handlers=http_handlers)
+                    self.routes.append(route)
+                routes.append(route)
+
+            if websocket_handler := handlers_map.get("websocket"):
+                route = WebSocketRoute(path=path, route_handler=cast("WebsocketRouteHandler", websocket_handler))
+                self.routes.append(route)
+                routes.append(route)
+
+            if asgi_handler := handlers_map.get("asgi"):
+                route = ASGIRoute(path=path, route_handler=cast("ASGIRouteHandler", asgi_handler))
+                self.routes.append(route)
+                routes.append(route)
+
+        return routes
+
+    @property
+    def route_handler_method_map(self) -> dict[str, RouteHandlerMapItem]:
+        """Map route paths to :class:`RouteHandlerMapItem <litestar.types.internal_typ es.RouteHandlerMapItem>`
 
-        Data returned from this function will be serialized and sent via the socket
-        according to handler configuration.
+        Returns:
+             A dictionary mapping paths to route handlers
         """
-        raise NotImplementedError
-
-    def on_disconnect(self, socket: WebSocket) -> SyncOrAsyncUnion[None]:  # noqa: B027
-        """Called after a WebSocket connection has been disconnected"""
+        route_map: dict[str, RouteHandlerMapItem] = defaultdict(dict)
+        for route in self.routes:
+            if isinstance(route, HTTPRoute):
+                for route_handler in route.route_handlers:
+                    for method in route_handler.http_methods:
+                        route_map[route.path][method] = route_handler
+            else:
+                route_map[route.path][
+                    "websocket" if isinstance(route, WebSocketRoute) else "asgi"
+                ] = route.route_handler
+        return route_map
+
+    @classmethod
+    def get_route_handler_map(
+        cls,
+        value: Controller | RouteHandlerType | Router,
+    ) -> dict[str, RouteHandlerMapItem]:
+        """Map route handlers to HTTP methods."""
+        if isinstance(value, Router):
+            return value.route_handler_method_map
+
+        if isinstance(value, (HTTPRouteHandler, ASGIRouteHandler, WebsocketRouteHandler)):
+            copied_value = copy(value)
+            if isinstance(value, HTTPRouteHandler):
+                return {path: {http_method: copied_value for http_method in value.http_methods} for path in value.paths}
+
+            return {
+                path: {"websocket" if isinstance(value, WebsocketRouteHandler) else "asgi": copied_value}
+                for path in value.paths
+            }
+
+        handlers_map: DefaultDict[str, RouteHandlerMapItem] = defaultdict(dict)
+        for route_handler in value.get_route_handlers():
+            for handler_path in route_handler.paths:
+                path = join_paths([value.path, handler_path]) if handler_path else value.path
+                if isinstance(route_handler, HTTPRouteHandler):
+                    for http_method in route_handler.http_methods:
+                        handlers_map[path][http_method] = route_handler
+                else:
+                    handlers_map[path][
+                        "websocket" if isinstance(route_handler, WebsocketRouteHandler) else "asgi"
+                    ] = cast("WebsocketRouteHandler | ASGIRouteHandler", route_handler)
+
+        return handlers_map
+
+    def _validate_registration_value(self, value: ControllerRouterHandler) -> Controller | RouteHandlerType | Router:
+        """Ensure values passed to the register method are supported."""
+        if is_class_and_subclass(value, Controller):
+            return value(owner=self)
+
+        # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
+        if is_class_and_subclass(value, WebsocketListener):  # type: ignore[type-abstract]
+            return value()._handler  # pyright: ignore
+
+        if isinstance(value, Router):
+            if value.owner:
+                raise ImproperlyConfiguredException(f"Router with path {value.path} has already been registered")
+            if value is self:
+                raise ImproperlyConfiguredException("Cannot register a router on itself")
+
+            value.owner = self
+            return value
+
+        if isinstance(value, (ASGIRouteHandler, HTTPRouteHandler, WebsocketRouteHandler)):
+            value.owner = self
+            return value
+
+        raise ImproperlyConfiguredException(
+            "Unsupported value passed to `Router.register`. "
+            "If you passed in a function or method, "
+            "make sure to decorate it first with one of the routing decorators"
+        )
```

### Comparing `litestar-2.0.0a6/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0a7/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/logging/_utils.py` & `litestar-2.0.0a7/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/logging/config.py` & `litestar-2.0.0a7/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/logging/picologging.py` & `litestar-2.0.0a7/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/logging/standard.py` & `litestar-2.0.0a7/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/_utils.py` & `litestar-2.0.0a7/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0a7/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/authentication.py` & `litestar-2.0.0a7/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/base.py` & `litestar-2.0.0a7/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/compression.py` & `litestar-2.0.0a7/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/cors.py` & `litestar-2.0.0a7/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/csrf.py` & `litestar-2.0.0a7/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0a7/litestar/middleware/exceptions/_debug_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     Returns:
         A string containing HTML representation of the execution frame.
     """
     frame_tpl = (tpl_dir / "frame.html").read_text()
 
     code_lines: list[str] = []
     for idx, line in enumerate(frame.code_context or []):
-        code_lines.append(create_line_html(line, frame.lineno, frame.index or 0, idx))
+        code_lines.append(create_line_html(line, frame.lineno, frame.index or 0, idx))  # pyright: ignore
 
     data = {
         "file": escape(frame.filename),
         "line": frame.lineno,
         "symbol_name": escape(get_symbol_name(frame)),
         "code": "".join(code_lines),
         "frame_class": "collapsed" if collapsed else "",
```

### Comparing `litestar-2.0.0a6/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0a7/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0a7/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0a7/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/logging.py` & `litestar-2.0.0a7/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/rate_limit.py` & `litestar-2.0.0a7/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/session/base.py` & `litestar-2.0.0a7/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/session/client_side.py` & `litestar-2.0.0a7/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/middleware/session/server_side.py` & `litestar-2.0.0a7/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/config.py` & `litestar-2.0.0a7/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/controller.py` & `litestar-2.0.0a7/litestar/openapi/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,19 +152,15 @@
         """
         return {
             "redoc": self.render_redoc,
             "swagger": self.render_swagger_ui,
             "elements": self.render_stoplight_elements,
         }
 
-    @get(
-        path="/openapi.yaml",
-        media_type=OpenAPIMediaType.OPENAPI_YAML,
-        include_in_schema=False,
-    )
+    @get(path="/openapi.yaml", media_type=OpenAPIMediaType.OPENAPI_YAML, include_in_schema=False, sync_to_thread=False)
     def retrieve_schema_yaml(self, request: Request) -> Response:
         """Return the OpenAPI schema as YAML with an ``application/vnd.oai.openapi`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
@@ -173,15 +169,15 @@
         """
         if self.should_serve_endpoint(request):
             return OpenAPISchemaResponse(
                 content=self.get_schema_from_request(request), media_type=OpenAPIMediaType.OPENAPI_YAML
             )
         return Response(content={}, status_code=HTTP_404_NOT_FOUND)
 
-    @get(path="/openapi.json", media_type=OpenAPIMediaType.OPENAPI_JSON, include_in_schema=False)
+    @get(path="/openapi.json", media_type=OpenAPIMediaType.OPENAPI_JSON, include_in_schema=False, sync_to_thread=False)
     def retrieve_schema_json(self, request: Request) -> Response:
         """Return the OpenAPI schema as JSON with an ``application/vnd.oai.openapi+json`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
@@ -190,15 +186,15 @@
         """
         if self.should_serve_endpoint(request):
             return OpenAPISchemaResponse(
                 content=self.get_schema_from_request(request), media_type=OpenAPIMediaType.OPENAPI_JSON
             )
         return Response(content={}, status_code=HTTP_404_NOT_FOUND)
 
-    @get(path="/", media_type=MediaType.HTML, include_in_schema=False)
+    @get(path="/", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
     def root(self, request: Request) -> Response:
         """Render a static documentation site.
 
          The site to be rendered is based on the ``root_schema_site`` value set in the application's
          :class:`OpenAPIConfig <.openapi.OpenAPIConfig>`. Defaults to ``redoc``.
 
         Args:
@@ -222,15 +218,15 @@
 
         return Response(
             content=self.render_404_page(),
             status_code=HTTP_404_NOT_FOUND,
             media_type=MediaType.HTML,
         )
 
-    @get(path="/swagger", media_type=MediaType.HTML, include_in_schema=False)
+    @get(path="/swagger", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
     def swagger_ui(self, request: Request) -> Response:
         """Route handler responsible for rendering Swagger-UI.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
@@ -241,30 +237,30 @@
             return Response(content=self.render_swagger_ui(request), media_type=MediaType.HTML)
         return Response(
             content=self.render_404_page(),
             status_code=HTTP_404_NOT_FOUND,
             media_type=MediaType.HTML,
         )
 
-    @get(path="/elements", media_type=MediaType.HTML, include_in_schema=False)
+    @get(path="/elements", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
     def stoplight_elements(self, request: Request) -> Response:
         """Route handler responsible for rendering StopLight Elements.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered stoplight elements documentation site
         """
         if self.should_serve_endpoint(request):
             return Response(content=self.render_stoplight_elements(request), media_type=MediaType.HTML)
         return Response(content=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
-    @get(path="/redoc", media_type=MediaType.HTML, include_in_schema=False)
+    @get(path="/redoc", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
     def redoc(self, request: Request) -> Response:  # pragma: no cover
         """Route handler responsible for rendering Redoc.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
```

### Comparing `litestar-2.0.0a6/litestar/openapi/datastructures.py` & `litestar-2.0.0a7/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/__init__.py` & `litestar-2.0.0a7/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/base.py` & `litestar-2.0.0a7/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/callback.py` & `litestar-2.0.0a7/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/components.py` & `litestar-2.0.0a7/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/contact.py` & `litestar-2.0.0a7/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0a7/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/encoding.py` & `litestar-2.0.0a7/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/enums.py` & `litestar-2.0.0a7/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/example.py` & `litestar-2.0.0a7/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0a7/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/header.py` & `litestar-2.0.0a7/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/info.py` & `litestar-2.0.0a7/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/license.py` & `litestar-2.0.0a7/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/link.py` & `litestar-2.0.0a7/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/media_type.py` & `litestar-2.0.0a7/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0a7/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0a7/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/open_api.py` & `litestar-2.0.0a7/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/operation.py` & `litestar-2.0.0a7/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/parameter.py` & `litestar-2.0.0a7/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/path_item.py` & `litestar-2.0.0a7/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/paths.py` & `litestar-2.0.0a7/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/reference.py` & `litestar-2.0.0a7/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/request_body.py` & `litestar-2.0.0a7/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/response.py` & `litestar-2.0.0a7/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/responses.py` & `litestar-2.0.0a7/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/schema.py` & `litestar-2.0.0a7/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0a7/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0a7/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/server.py` & `litestar-2.0.0a7/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0a7/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/tag.py` & `litestar-2.0.0a7/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/openapi/spec/xml.py` & `litestar-2.0.0a7/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/pagination.py` & `litestar-2.0.0a7/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/params.py` & `litestar-2.0.0a7/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/partial.py` & `litestar-2.0.0a7/litestar/partial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/plugins.py` & `litestar-2.0.0a7/litestar/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/response/base.py` & `litestar-2.0.0a7/litestar/response/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             else list(cookies or [])
         )
         self.encoding = encoding
         self.headers: dict[str, Any] = (
             dict(headers) if isinstance(headers, Mapping) else {h.name: h.value for h in headers or {}}
         )
         self.is_head_response = is_head_response
-        self.media_type = get_enum_string_value(media_type)
+        self.media_type = get_enum_string_value(media_type) or MediaType.JSON
         self.status_allows_body = not (
             status_code in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED} or status_code < HTTP_200_OK
         )
         self.status_code = status_code
         self._enc_hook = self.get_serializer(type_encoders)
 
         if not self.status_allows_body or is_head_response:
@@ -236,24 +236,27 @@
         Args:
             content: A value for the response body that will be rendered into bytes string.
 
         Returns:
             An encoded bytes string
         """
         try:
-            if self.media_type.startswith("text/"):
+            if self.media_type.startswith("text/") or isinstance(content, str):
                 if not content:
                     return b""
 
                 return content.encode(self.encoding)  # type: ignore
 
             if self.media_type == MediaType.MESSAGEPACK:
                 return encode_msgpack(content, self._enc_hook)
 
-            return encode_json(content, self._enc_hook)
+            if self.media_type.startswith("application/json"):
+                return encode_json(content, self._enc_hook)
+
+            raise ImproperlyConfiguredException(f"unsupported media_type {self.media_type} for content {content!r}")
         except (AttributeError, ValueError, TypeError) as e:
             raise ImproperlyConfiguredException("Unable to serialize response content") from e
 
     @property
     def content_length(self) -> int:
         """Content length of the response if applicable.
```

### Comparing `litestar-2.0.0a6/litestar/response/file.py` & `litestar-2.0.0a7/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/response/redirect.py` & `litestar-2.0.0a7/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/response/streaming.py` & `litestar-2.0.0a7/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/response/template.py` & `litestar-2.0.0a7/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/response_containers.py` & `litestar-2.0.0a7/litestar/response_containers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/routes/asgi.py` & `litestar-2.0.0a7/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/routes/base.py` & `litestar-2.0.0a7/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/routes/http.py` & `litestar-2.0.0a7/litestar/routes/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,22 +316,23 @@
                         headers=response_headers,
                     )
                 )
 
             return Response(
                 content=None,
                 status_code=HTTP_204_NO_CONTENT,
-                headers={"Allow": ", ".join(sorted(self.methods))},
+                headers={"Allow": ", ".join(sorted(self.methods))},  # pyright: ignore
                 media_type=MediaType.TEXT,
             )
 
         return HTTPRouteHandler(
             path=path,
             http_method=[HttpMethod.OPTIONS],
             include_in_schema=False,
+            sync_to_thread=False,
         )(options_handler)
 
     @staticmethod
     async def _cleanup_temporary_files(form_data: dict[str, Any]) -> None:
         for v in form_data.values():
             if isinstance(v, UploadFile) and not v.file.closed:
                 await v.close()
```

### Comparing `litestar-2.0.0a6/litestar/routes/websocket.py` & `litestar-2.0.0a7/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/security/base.py` & `litestar-2.0.0a7/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/security/session_auth/auth.py` & `litestar-2.0.0a7/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/security/session_auth/middleware.py` & `litestar-2.0.0a7/litestar/security/session_auth/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 exclude=self.config.exclude,
                 exclude_opt_key=self.config.exclude_opt_key,
                 scopes=self.config.scopes,
                 retrieve_user_handler=self.config.retrieve_user_handler,  # type: ignore
             )
             exception_middleware = ExceptionHandlerMiddleware(
                 app=auth_middleware,
-                exception_handlers=litestar_app.exception_handlers or {},
+                exception_handlers=litestar_app.exception_handlers or {},  # pyright: ignore
                 debug=litestar_app.debug,
             )
             self.app = SessionMiddleware(
                 app=exception_middleware,
                 backend=self.config.session_backend,
             )
             self.has_wrapped_middleware = True
```

### Comparing `litestar-2.0.0a6/litestar/serialization.py` & `litestar-2.0.0a7/litestar/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/static_files/base.py` & `litestar-2.0.0a7/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/static_files/config.py` & `litestar-2.0.0a7/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/status_codes.py` & `litestar-2.0.0a7/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/stores/base.py` & `litestar-2.0.0a7/litestar/stores/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     @property
     def expires_in(self) -> int:
         """Return the expiry time of this ``StorageObject`` in seconds. If no expiry time
         was set, return ``-1``.
         """
         if self.expires_at:
-            return (self.expires_at - datetime.now(tz=timezone.utc)).seconds
+            return int(self.expires_at.timestamp() - datetime.now(tz=timezone.utc).timestamp())
         return -1
 
     def to_bytes(self) -> bytes:
         """Encode the instance to bytes"""
         return msgpack_encode(self)
 
     @classmethod
```

### Comparing `litestar-2.0.0a6/litestar/stores/file.py` & `litestar-2.0.0a7/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/stores/memory.py` & `litestar-2.0.0a7/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/stores/redis.py` & `litestar-2.0.0a7/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/stores/registry.py` & `litestar-2.0.0a7/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/template/base.py` & `litestar-2.0.0a7/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/template/config.py` & `litestar-2.0.0a7/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/__init__.py` & `litestar-2.0.0a7/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/client/__init__.py` & `litestar-2.0.0a7/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/client/async_client.py` & `litestar-2.0.0a7/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/client/base.py` & `litestar-2.0.0a7/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/client/sync_client.py` & `litestar-2.0.0a7/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/helpers.py` & `litestar-2.0.0a7/litestar/testing/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Literal, Mapping, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Literal, Mapping, Sequence
 
 from litestar.app import DEFAULT_OPENAPI_CONFIG, Litestar
 from litestar.controller import Controller
 from litestar.events import SimpleEventEmitter
 from litestar.testing.client import AsyncTestClient, TestClient
 from litestar.types import Empty
 from litestar.utils.predicates import is_class_and_subclass
 
 if TYPE_CHECKING:
+    from contextlib import AbstractAsyncContextManager
+
     from litestar import Request, WebSocket
     from litestar.config.allowed_hosts import AllowedHostsConfig
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.config.response_cache import ResponseCacheConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader, State
@@ -35,16 +37,15 @@
         BeforeMessageSendHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
         Dependencies,
         EmptyType,
         ExceptionHandlersMap,
         Guard,
-        LifeSpanHandler,
-        LifeSpanHookHandler,
+        LifespanHook,
         Middleware,
         OnAppInitHandler,
         OptionalSequence,
         ParametersMap,
         ResponseCookies,
         ResponseType,
         TypeEncodersMap,
@@ -53,24 +54,20 @@
 
 def create_test_client(
     route_handlers: ControllerRouterHandler | Sequence[ControllerRouterHandler] | None = None,
     *,
     after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
     after_request: AfterRequestHookHandler | None = None,
     after_response: AfterResponseHookHandler | None = None,
-    after_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-    after_startup: OptionalSequence[LifeSpanHookHandler] = None,
     allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
-    before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-    before_startup: OptionalSequence[LifeSpanHookHandler] = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     debug: bool = False,
     dependencies: Dependencies | None = None,
     dto: type[DTOInterface] | None | EmptyType = Empty,
@@ -79,20 +76,21 @@
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] = None,
     listeners: OptionalSequence[EventListener] = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
     middleware: OptionalSequence[Middleware] = None,
     multipart_form_part_limit: int = 1000,
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
-    on_shutdown: OptionalSequence[LifeSpanHandler] = None,
-    on_startup: OptionalSequence[LifeSpanHandler] = None,
+    on_shutdown: OptionalSequence[LifespanHook] = None,
+    on_startup: OptionalSequence[LifespanHook] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
+    lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] = None,
@@ -148,30 +146,22 @@
         after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
             hook is called after an exception occurs. In difference to exception handlers, it is not meant to
             return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
         after_request: A sync or async function executed after the route handler function returned and the response
             object has been resolved. Receives the response object.
         after_response: A sync or async function called after the response has been awaited. It receives the
             :class:`Request <.connection.Request>` object and should not return any values.
-        after_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
-        after_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI startup, after all callables in the 'on_startup' list have been called.
         allowed_hosts: A sequence of allowed hosts, or an
             :class:`AllowedHostsConfig <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin
             allowed hosts middleware.
         before_request: A sync or async function called immediately before calling the route handler. Receives the
             :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
             response, bypassing the route handler.
         before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
             when the ASGI send function is called.
-        before_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI shutdown, before any 'on_shutdown' hooks are called.
-        before_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI startup, before any 'on_startup' hooks are called.
         cache_control: A ``cache-control`` header of type
             :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
@@ -181,26 +171,27 @@
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
         event_emitter_backend: A subclass of
             :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <.types.Guard>` callables.
+        lifespan: A list of callables returning async context managers, wrapping the lifespan of the ASGI application
         listeners: A sequence of :class:`EventListener <.events.listener.EventListener>`.
         logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
         middleware: A sequence of :class:`Middleware <.types.Middleware>`.
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request. This limit
             is intended to protect from DoS attacks.
         on_app_init: A sequence of :class:`OnAppInitHandler <.types.OnAppInitHandler>` instances. Handlers receive
             an instance of :class:`AppConfig <.config.app.AppConfig>` that will have been initially populated with
             the parameters passed to :class:`Litestar <litestar.app.Litestar>`, and must return an instance of same.
             If more than one handler is registered they are called in the order they are provided.
-        on_shutdown: A sequence of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application
+        on_shutdown: A sequence of :class:`LifespanHook <.types.LifespanHook>` called during application
             shutdown.
-        on_startup: A sequence of :class:`LifeSpanHandler <litestar.types.LifeSpanHandler>` called during
+        on_startup: A sequence of :class:`LifespanHook <litestar.types.LifespanHook>` called during
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
@@ -241,29 +232,26 @@
     if is_class_and_subclass(route_handlers, Controller) or not isinstance(route_handlers, Sequence):
         route_handlers = (route_handlers,)
 
     app = Litestar(
         after_exception=after_exception,
         after_request=after_request,
         after_response=after_response,
-        after_shutdown=after_shutdown,
-        after_startup=after_startup,
         allowed_hosts=allowed_hosts,
         before_request=before_request,
         before_send=before_send,
-        before_shutdown=before_shutdown,
-        before_startup=before_startup,
         cache_control=cache_control,
         compression_config=compression_config,
         cors_config=cors_config,
         csrf_config=csrf_config,
         debug=debug,
         dependencies=dependencies,
         dto=dto,
         etag=etag,
+        lifespan=lifespan,
         event_emitter_backend=event_emitter_backend,
         exception_handlers=exception_handlers,
         guards=guards,
         listeners=listeners,
         logging_config=logging_config,
         middleware=middleware,
         multipart_form_part_limit=multipart_form_part_limit,
@@ -306,42 +294,39 @@
 
 def create_async_test_client(
     route_handlers: ControllerRouterHandler | Sequence[ControllerRouterHandler] | None = None,
     *,
     after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
     after_request: AfterRequestHookHandler | None = None,
     after_response: AfterResponseHookHandler | None = None,
-    after_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-    after_startup: OptionalSequence[LifeSpanHookHandler] = None,
     allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
-    before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
-    before_startup: OptionalSequence[LifeSpanHookHandler] = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     debug: bool = False,
     dependencies: Dependencies | None = None,
     dto: type[DTOInterface] | None | EmptyType = Empty,
     etag: ETag | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] = None,
+    lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     listeners: OptionalSequence[EventListener] = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
     middleware: OptionalSequence[Middleware] = None,
     multipart_form_part_limit: int = 1000,
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
-    on_shutdown: OptionalSequence[LifeSpanHandler] = None,
-    on_startup: OptionalSequence[LifeSpanHandler] = None,
+    on_shutdown: OptionalSequence[LifespanHook] = None,
+    on_startup: OptionalSequence[LifespanHook] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
     preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
@@ -400,30 +385,22 @@
         after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
             hook is called after an exception occurs. In difference to exception handlers, it is not meant to
             return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
         after_request: A sync or async function executed after the route handler function returned and the response
             object has been resolved. Receives the response object.
         after_response: A sync or async function called after the response has been awaited. It receives the
             :class:`Request <.connection.Request>` object and should not return any values.
-        after_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
-        after_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI startup, after all callables in the 'on_startup' list have been called.
         allowed_hosts: A sequence of allowed hosts, or an
             :class:`AllowedHostsConfig <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin
             allowed hosts middleware.
         before_request: A sync or async function called immediately before calling the route handler. Receives the
             :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
             response, bypassing the route handler.
         before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
             when the ASGI send function is called.
-        before_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI shutdown, before any 'on_shutdown' hooks are called.
-        before_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
-            the ASGI startup, before any 'on_startup' hooks are called.
         cache_control: A ``cache-control`` header of type
             :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
@@ -433,26 +410,27 @@
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
         event_emitter_backend: A subclass of
             :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <.types.Guard>` callables.
+        lifespan: A list of callables returning async context managers, wrapping the lifespan of the ASGI application
         listeners: A sequence of :class:`EventListener <.events.listener.EventListener>`.
         logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
         middleware: A sequence of :class:`Middleware <.types.Middleware>`.
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request. This limit
             is intended to protect from DoS attacks.
         on_app_init: A sequence of :class:`OnAppInitHandler <.types.OnAppInitHandler>` instances. Handlers receive
             an instance of :class:`AppConfig <.config.app.AppConfig>` that will have been initially populated with
             the parameters passed to :class:`Litestar <litestar.app.Litestar>`, and must return an instance of same.
             If more than one handler is registered they are called in the order they are provided.
-        on_shutdown: A sequence of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application
+        on_shutdown: A sequence of :class:`LifespanHook <.types.LifespanHook>` called during application
             shutdown.
-        on_startup: A sequence of :class:`LifeSpanHandler <litestar.types.LifeSpanHandler>` called during
+        on_startup: A sequence of :class:`LifespanHook <litestar.types.LifespanHook>` called during
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
@@ -493,32 +471,29 @@
     if is_class_and_subclass(route_handlers, Controller) or not isinstance(route_handlers, Sequence):
         route_handlers = (route_handlers,)
 
     app = Litestar(
         after_exception=after_exception,
         after_request=after_request,
         after_response=after_response,
-        after_shutdown=after_shutdown,
-        after_startup=after_startup,
         allowed_hosts=allowed_hosts,
         before_request=before_request,
         before_send=before_send,
-        before_shutdown=before_shutdown,
-        before_startup=before_startup,
         cache_control=cache_control,
         compression_config=compression_config,
         cors_config=cors_config,
         csrf_config=csrf_config,
         debug=debug,
         dependencies=dependencies,
         dto=dto,
         etag=etag,
         event_emitter_backend=event_emitter_backend,
         exception_handlers=exception_handlers,
         guards=guards,
+        lifespan=lifespan,
         listeners=listeners,
         logging_config=logging_config,
         middleware=middleware,
         multipart_form_part_limit=multipart_form_part_limit,
         on_app_init=on_app_init,
         on_shutdown=on_shutdown,
         on_startup=on_startup,
```

### Comparing `litestar-2.0.0a6/litestar/testing/life_span_handler.py` & `litestar-2.0.0a7/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/request_factory.py` & `litestar-2.0.0a7/litestar/testing/request_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from httpx._types import FileTypes
 
     from litestar.datastructures.cookie import Cookie
     from litestar.handlers.http_handlers import HTTPRouteHandler
 
 
 def _create_default_route_handler() -> HTTPRouteHandler:
-    @get("/")
+    @get("/", sync_to_thread=False)
     def _default_route_handler() -> None:
         ...
 
     return _default_route_handler
 
 
 def _create_default_app() -> Litestar:
```

### Comparing `litestar-2.0.0a6/litestar/testing/transport.py` & `litestar-2.0.0a7/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/testing/websocket_test_session.py` & `litestar-2.0.0a7/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/types/__init__.py` & `litestar-2.0.0a7/litestar/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     AsyncAnyCallable,
     BeforeMessageSendHookHandler,
     BeforeRequestHookHandler,
     CacheKeyBuilder,
     ExceptionHandler,
     GetLogger,
     Guard,
-    LifeSpanHandler,
-    LifeSpanHookHandler,
+    LifespanHook,
     OnAppInitHandler,
     OperationIDCreator,
     Serializer,
 )
 from .composite_types import (
     Dependencies,
     ExceptionHandlersMap,
@@ -114,16 +113,15 @@
     "HTTPReceiveMessage",
     "HTTPRequestEvent",
     "HTTPResponseBodyEvent",
     "HTTPResponseStartEvent",
     "HTTPScope",
     "HTTPSendMessage",
     "HTTPServerPushEvent",
-    "LifeSpanHandler",
-    "LifeSpanHookHandler",
+    "LifespanHook",
     "LifeSpanReceive",
     "LifeSpanReceiveMessage",
     "LifeSpanScope",
     "LifeSpanSend",
     "LifeSpanSendMessage",
     "LifeSpanShutdownCompleteEvent",
     "LifeSpanShutdownEvent",
```

### Comparing `litestar-2.0.0a6/litestar/types/asgi_types.py` & `litestar-2.0.0a7/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/types/callable_types.py` & `litestar-2.0.0a7/litestar/types/callable_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,12 +45,14 @@
 BeforeMessageSendHookHandler = Callable[[Message, State, Scope], SyncOrAsyncUnion[None]]
 BeforeRequestHookHandler = Callable[[Request], Union[Any, Awaitable[Any]]]
 CacheKeyBuilder = Callable[[Request], str]
 ExceptionHandler = Callable[[Request, ExceptionT], Response]
 ExceptionLoggingHandler = Callable[[Logger, Scope, List[str]], None]
 GetLogger = Callable[..., Logger]
 Guard = Callable[[ASGIConnection, BaseRouteHandler], SyncOrAsyncUnion[None]]
-LifeSpanHandler = Union[Callable[[], SyncOrAsyncUnion[Any]], Callable[[State], SyncOrAsyncUnion[Any]]]
-LifeSpanHookHandler = Callable[[LitestarType], SyncOrAsyncUnion[None]]
+LifespanHook = Union[
+    Callable[[LitestarType], SyncOrAsyncUnion[Any]],
+    Callable[[], SyncOrAsyncUnion[Any]],
+]
 OnAppInitHandler = Callable[[AppConfig], AppConfig]
 OperationIDCreator = Callable[[HTTPRouteHandler, Method, List[Union[str, PathParameterDefinition]]], str]
 Serializer = Callable[[Any], Any]
```

### Comparing `litestar-2.0.0a6/litestar/types/composite_types.py` & `litestar-2.0.0a7/litestar/types/composite_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     TypeVar,
     Union,
 )
 
 from litestar.enums import ScopeType
 
 from .asgi_types import ASGIApp
-from .callable_types import ExceptionHandler
+from .callable_types import AnyCallable, ExceptionHandler
 
 if TYPE_CHECKING:
     from litestar.datastructures.cookie import Cookie
     from litestar.datastructures.response_header import ResponseHeader
     from litestar.di import Provide
     from litestar.middleware.base import DefineMiddleware, MiddlewareProtocol
     from litestar.params import ParameterKwarg
@@ -40,15 +40,15 @@
     ParameterKwarg = Any
     Provide = Any
     ResponseHeader = Any
 
 T = TypeVar("T")
 
 
-Dependencies = Mapping[str, Provide]
+Dependencies = Mapping[str, Union[Provide, AnyCallable]]
 ExceptionHandlersMap = Mapping[Union[int, Type[Exception]], ExceptionHandler]
 MaybePartial = Union[T, partial]
 Middleware = Union[
     Callable[..., ASGIApp], DefineMiddleware, Iterator[Tuple[ASGIApp, Dict[str, Any]]], Type[MiddlewareProtocol]
 ]
 ParametersMap = Mapping[str, ParameterKwarg]
 PathType = Union[Path, PathLike, str]
```

### Comparing `litestar-2.0.0a6/litestar/types/file_types.py` & `litestar-2.0.0a7/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/types/internal_types.py` & `litestar-2.0.0a7/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/types/protocols.py` & `litestar-2.0.0a7/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/types/serialization.py` & `litestar-2.0.0a7/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/__init__.py` & `litestar-2.0.0a7/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/compat.py` & `litestar-2.0.0a7/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/dataclass.py` & `litestar-2.0.0a7/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/deprecation.py` & `litestar-2.0.0a7/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/helpers.py` & `litestar-2.0.0a7/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/path.py` & `litestar-2.0.0a7/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/predicates.py` & `litestar-2.0.0a7/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/scope.py` & `litestar-2.0.0a7/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/sequence.py` & `litestar-2.0.0a7/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/signature.py` & `litestar-2.0.0a7/litestar/utils/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from litestar import connection, datastructures, types
 from litestar.datastructures import ImmutableState
 from litestar.enums import RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import AnyCallable, Empty
 from litestar.types.builtin_types import UNION_TYPES, NoneType
+from litestar.utils.dataclass import simple_asdict
 from litestar.utils.typing import get_safe_generic_origin, unwrap_annotation
 
 _GLOBAL_NAMES = {
     namespace: export
     for namespace, export in chain(
         tuple(getmembers(types)), tuple(getmembers(connection)), tuple(getmembers(datastructures))
     )
@@ -285,14 +286,26 @@
 
         return ParsedParameter(
             name=parameter.name,
             default=Empty if parameter.default is Signature.empty else parameter.default,
             parsed_type=ParsedType(annotation),
         )
 
+    def copy_with(self, **kwargs: Any) -> Self:
+        """Create a copy of the parameter with the given attributes updated.
+
+        Args:
+            kwargs: Attributes to update.
+
+        Returns:
+            ParsedParameter
+        """
+        data = {**simple_asdict(self), **kwargs}
+        return type(self)(**data)
+
 
 @dataclass(frozen=True)
 class ParsedSignature:
     """Parsed signature.
 
     This object is the primary source of handler/dependency signature information.
```

### Comparing `litestar-2.0.0a6/litestar/utils/sync.py` & `litestar-2.0.0a7/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/typing.py` & `litestar-2.0.0a7/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/litestar/utils/version.py` & `litestar-2.0.0a7/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a6/pyproject.toml` & `litestar-2.0.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0alpha6"
+version = "2.0.0alpha7"
 description = "Performant, light and flexible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
@@ -104,14 +104,15 @@
 mako = "*"
 mongomock-motor = { version = "*", markers = "sys_platform != 'win32'" }
 opentelemetry-instrumentation-asgi = "*"
 opentelemetry-sdk = "*"
 piccolo = "*"
 picologging = "*"
 pre-commit = "*"
+psycopg = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
 pytest_docker = "*"
 python-dateutil = "*"
@@ -210,15 +211,17 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:164",
     "ignore::DeprecationWarning:pkg_resources:2803",
 ]
 markers = [
     "sqlalchemy_asyncmy: SQLAlchemy MySQL (asyncmy) Tests",
-    "sqlalchemy_asyncpg: SQLAlchemy Postgres (asyncpg) Tests"
+    "sqlalchemy_asyncpg: SQLAlchemy Postgres (asyncpg) Tests",
+    "sqlalchemy_psycopg_async: SQLAlchemy Postgres (psycopg async) Tests",
+    "sqlalchemy_aiosqlite: SQLAlchemy SQLite (aiosqlite) Tests"
 ]
 
 [tool.pyright]
 include = ["litestar", "tests", "examples"]
 exclude = [
     "examples/plugins/sqlalchemy_plugin",
     "litestar/contrib/sqlalchemy_1",
@@ -282,14 +285,15 @@
     "D105",  # pydocstyle - missing docstring in magic method
     "D106",  # pydocstyle - missing docstring in public nested class
     "D107",  # pydocstyle - missing docstring in __init__
     "D202",  # pydocstyle - no blank lines allowed after function docstring
     "D205",  # pydocstyle - 1 blank line required between summary line and description
     "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
     "E501",  # pycodestyle line too long, handled by black
+    "PLW2901"  # pylint - for loop variable overwritten by assignment target
 ]
 line-length = 120
 src = ["litestar", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `litestar-2.0.0a6/PKG-INFO` & `litestar-2.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0a6
+Version: 2.0.0a7
 Summary: Performant, light and flexible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -95,15 +95,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-100-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-101-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -128,15 +128,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha3
+pip install litestar==2.0.0alpha6
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -488,14 +488,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://hexcode.tech"><img src="https://avatars.githubusercontent.com/u/419606?v=4?s=100" width="100px;" alt="Phyo Arkar Lwin"/><br /><sub><b>Phyo Arkar Lwin</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=v3ss0n" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

