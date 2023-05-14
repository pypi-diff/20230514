# Comparing `tmp/tomcru-0.2.4.tar.gz` & `tmp/tomcru-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru-0.2.4.tar", max compression
+gzip compressed data, was "tomcru-0.2.5.tar", max compression
```

## Comparing `tomcru-0.2.4.tar` & `tomcru-0.2.5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.4/LICENSE
--rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.4/README.md
--rw-r--r--   0        0        0      632 2023-05-09 23:36:55.518391 tomcru-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.4/tomcru/__init__.py
--rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.4/tomcru/appbuilders/envmapping.py
--rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.4/tomcru/appbuilders/faas/InjectableAppBase.py
--rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.4/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/appbuilders/faas/sam_app/__init__.py
--rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.4/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
--rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/appbuilders/faas/static_app/__init__.py
--rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.4/tomcru/cfgparsers/BaseCfgParser.py
--rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.4/tomcru/cfgparsers/EnvParser.py
--rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.4/tomcru/cfgparsers/MergeCfgParser.py
--rw-r--r--   0        0        0     5090 2023-04-29 12:02:36.779844 tomcru-0.2.4/tomcru/cfgparsers/SwaggerCfgParser.py
--rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.4/tomcru/cfgparsers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.4/tomcru/core/__init__.py
--rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.4/tomcru/core/cfg/api.py
--rw-r--r--   0        0        0     1244 2023-04-29 11:52:34.470450 tomcru-0.2.4/tomcru/core/cfg/authorizers.py
--rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.4/tomcru/core/cfg/integrations.py
--rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.4/tomcru/core/cfg/proj.py
--rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.4/tomcru/core/modloader.py
--rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.4/tomcru/core/obj_store.py
--rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.4/tomcru/core/project.py
--rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.4/tomcru/core/servmgr.py
--rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.4/tomcru/core/utils/MyMetaLoader.py
--rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.4/tomcru/core/utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.4/tomcru/core/utils/toml_custom.py
--rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.4/tomcru/core/utils/yaml_custom.py
--rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/index.js
--rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/package.json
--rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/proxylib.js
--rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/serv/ddb.js
--rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.4/tomcru/etc/proxies/t_proxy.js
--rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.4/tomcru/services/ServiceBase.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/__init__.py
--rw-r--r--   0        0        0     6799 2023-04-29 12:52:25.243899 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
--rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     3877 2023-05-07 02:35:21.861467 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
--rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
--rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
--rw-r--r--   0        0        0     4871 2023-05-01 09:27:22.908562 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
--rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
--rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
--rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
--rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
--rw-r--r--   0        0        0     3897 2023-04-29 11:55:18.949636 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
--rw-r--r--   0        0        0     1808 2023-04-29 11:52:43.966414 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
--rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
--rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
--rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
--rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
--rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
--rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
--rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
--rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
--rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.4/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
--rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.4/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
--rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.4/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/boto3_b/__init__.py
--rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.4/tomcru/services/aws/hosted/boto3_b/boto3.py
--rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.4/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
--rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.4/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/__init__.py
--rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/proxy.py
--rw-r--r--   0        0        0     8743 2023-05-09 21:48:13.121335 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
--rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
--rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
--rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
--rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
--rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
--rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/__init__.py
--rw-r--r--   0        0        0     5103 2023-05-06 18:34:46.898263 tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
--rw-r--r--   0        0        0     2555 2023-04-27 21:53:01.387107 tomcru-0.2.4/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
--rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.4/tomcru/services/aws/hosted/s3_b/S3Service.py
--rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.4/tomcru/services/aws/hosted/s3_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/onpremise/__init__.py
--rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.4/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
--rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/onpremise/model_checker/__init__.py
--rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.4/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
--rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/onpremise/s3_static/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/SamTplBuilder.py
--rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/core.yaml
--rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/httpapi.yaml
--rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/integ_normal.yaml
--rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/integ_ws.yaml
--rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/lambda.yaml
--rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/layer.yaml
--rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/template.yaml
--rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/_junk/wsapi.yaml
--rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.4/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/lambda_b/__init__.py
--rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.4/tomcru/services/aws/sam/params_b/ParametersBuilder.py
--rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/params_b/__init__.py
--rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
--rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
--rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
--rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.4/tomcru/services/general/eme2swagger/Eme2Swagger.py
--rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.4/tomcru/services/general/eme2swagger/__init__.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.5/LICENSE
+-rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.5/README.md
+-rw-r--r--   0        0        0      632 2023-05-14 01:35:31.110041 tomcru-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.5/tomcru/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.5/tomcru/appbuilders/envmapping.py
+-rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.5/tomcru/appbuilders/faas/InjectableAppBase.py
+-rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.5/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
+-rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/appbuilders/faas/static_app/__init__.py
+-rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.5/tomcru/cfgparsers/BaseCfgParser.py
+-rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.5/tomcru/cfgparsers/EnvParser.py
+-rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.5/tomcru/cfgparsers/MergeCfgParser.py
+-rw-r--r--   0        0        0     5090 2023-04-29 12:02:36.779844 tomcru-0.2.5/tomcru/cfgparsers/SwaggerCfgParser.py
+-rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.5/tomcru/cfgparsers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.5/tomcru/core/__init__.py
+-rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.5/tomcru/core/cfg/api.py
+-rw-r--r--   0        0        0     1244 2023-04-29 11:52:34.470450 tomcru-0.2.5/tomcru/core/cfg/authorizers.py
+-rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.5/tomcru/core/cfg/integrations.py
+-rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.5/tomcru/core/cfg/proj.py
+-rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.5/tomcru/core/modloader.py
+-rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.5/tomcru/core/obj_store.py
+-rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.5/tomcru/core/project.py
+-rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.5/tomcru/core/servmgr.py
+-rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.5/tomcru/core/utils/MyMetaLoader.py
+-rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.5/tomcru/core/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.5/tomcru/core/utils/toml_custom.py
+-rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.5/tomcru/core/utils/yaml_custom.py
+-rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/index.js
+-rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/package.json
+-rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/proxylib.js
+-rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/serv/ddb.js
+-rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.5/tomcru/etc/proxies/t_proxy.js
+-rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.5/tomcru/services/ServiceBase.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/__init__.py
+-rw-r--r--   0        0        0     6799 2023-04-29 12:52:25.243899 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
+-rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     3318 2023-05-13 22:33:23.948162 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
+-rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
+-rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
+-rw-r--r--   0        0        0     4871 2023-05-01 09:27:22.908562 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
+-rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
+-rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
+-rw-r--r--   0        0        0     4019 2023-05-13 22:36:02.291646 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0     1808 2023-05-13 22:27:41.433281 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
+-rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
+-rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
+-rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
+-rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
+-rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
+-rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
+-rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/boto3.py
+-rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
+-rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/proxy.py
+-rw-r--r--   0        0        0     8695 2023-05-13 22:09:34.428940 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
+-rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
+-rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
+-rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
+-rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/__init__.py
+-rw-r--r--   0        0        0     5074 2023-05-13 17:44:03.162000 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
+-rw-r--r--   0        0        0     2585 2023-05-12 20:18:40.139204 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
+-rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3Service.py
+-rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/__init__.py
+-rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
+-rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
+-rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/SamTplBuilder.py
+-rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/core.yaml
+-rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/httpapi.yaml
+-rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_normal.yaml
+-rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_ws.yaml
+-rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/lambda.yaml
+-rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/layer.yaml
+-rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/template.yaml
+-rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/wsapi.yaml
+-rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/__init__.py
+-rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.5/tomcru/services/aws/sam/params_b/ParametersBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/params_b/__init__.py
+-rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
+-rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
+-rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
+-rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.5/tomcru/services/general/eme2swagger/Eme2Swagger.py
+-rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.5/tomcru/services/general/eme2swagger/__init__.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.5/PKG-INFO
```

### Comparing `tomcru-0.2.4/LICENSE` & `tomcru-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/pyproject.toml` & `tomcru-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomcru"
-version = "0.2.4"
+version = "0.2.5"
 description = "Serverless app framework"
 authors = ["Rajmund Csombordi <rajmund.csombordi@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "tomcru"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tomcru-0.2.4/tomcru/appbuilders/envmapping.py` & `tomcru-0.2.5/tomcru/appbuilders/envmapping.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/appbuilders/faas/InjectableAppBase.py` & `tomcru-0.2.5/tomcru/appbuilders/faas/InjectableAppBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py` & `tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py` & `tomcru-0.2.5/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/cfgparsers/BaseCfgParser.py` & `tomcru-0.2.5/tomcru/cfgparsers/BaseCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/cfgparsers/EnvParser.py` & `tomcru-0.2.5/tomcru/cfgparsers/EnvParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/cfgparsers/MergeCfgParser.py` & `tomcru-0.2.5/tomcru/cfgparsers/MergeCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/cfgparsers/SwaggerCfgParser.py` & `tomcru-0.2.5/tomcru/cfgparsers/SwaggerCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/cfg/api.py` & `tomcru-0.2.5/tomcru/core/cfg/api.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/cfg/authorizers.py` & `tomcru-0.2.5/tomcru/core/cfg/authorizers.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/cfg/integrations.py` & `tomcru-0.2.5/tomcru/core/cfg/integrations.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/cfg/proj.py` & `tomcru-0.2.5/tomcru/core/cfg/proj.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/modloader.py` & `tomcru-0.2.5/tomcru/core/modloader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/obj_store.py` & `tomcru-0.2.5/tomcru/core/obj_store.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/project.py` & `tomcru-0.2.5/tomcru/core/project.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/servmgr.py` & `tomcru-0.2.5/tomcru/core/servmgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/utils/MyMetaLoader.py` & `tomcru-0.2.5/tomcru/core/utils/MyMetaLoader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/utils/toml_custom.py` & `tomcru-0.2.5/tomcru/core/utils/toml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/core/utils/yaml_custom.py` & `tomcru-0.2.5/tomcru/core/utils/yaml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/proxylib.js` & `tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/proxylib.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/etc/proxies/aws-sdk/serv/ddb.js` & `tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/serv/ddb.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/etc/proxies/t_proxy.js` & `tomcru-0.2.5/tomcru/etc/proxies/t_proxy.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/ServiceBase.py` & `tomcru-0.2.5/tomcru/services/ServiceBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,33 +17,28 @@
         self.audience = cfg.audience
         self.scopes = cfg.scopes # this is redundant (scopes_supported is fetched from OIDC ep); but AWS requires to be checked
 
         # OIDC endpoint:
         self.initialized = False
         self.scopes_supported: list = None
         self.issuer = None
-        self.jwks_client: jwt.PyJWKClient | None = None
+        self.jwks_client = None
 
     def authorize(self, event: dict):
         jwt = self._initialize_oidc()
 
         if 'authorization' not in event['headers']:
             return None
-        token_jwt: str = event['headers']['authorization'].removeprefix('Bearer ')
-
         try:
+            prefix, token_jwt = event['headers']['authorization'].split(" ")
+            assert prefix.lower() in ('bearer', 'jwt')
+
             # base64 decode JWT & get JWK for it
             signing_key = self.jwks_client.get_signing_key_from_jwt(token_jwt)
 
-            # jwk = {'alg': 'RS256', 'e': 'AQAB',
-            #        'kid': 'hnLucpd8Fq24b_5m16AuLmRHx0nTcw4K6Fq8XW8WQXU', 'kty': 'RSA',
-            #        'n': 'rZZot-D9G5g1Qk7UdfBH1PypwPK0jzQ2xZ34hQ4C7JBogRJSS1KRSwRQZxO5cWcoWvp7UUk4FpzBmAw_EidpgcJM7JfmkyX-OG2tY8_TtiNh57DZ4Jyugtc0xlcneVuKxhcGSwC5jWi4Lzz0O83AW-LNqfJ0wkxNJHdnA9ebipQuctZHYoTErKxX25yjmr8Y9oJAgiGqC1m8_BFhhJW2FX63K_u1TYME-WP4BCjctq5LSqVTGOP4TqQp_PJhdQKVwNy-ecK1G6u8ZJ9iTvnSdY4C5XB-bLMUgxTIneJOgJeTPMCgk1S91Wg2YjjRSyrjLeH7Kgi-N3s9noJOCV3MsQ',
-            #        'use': 'sig'}
-            # pyjwk = jwt.PyJWK(jwk)
-
             # verify JWT
             data = jwt.decode(token_jwt, signing_key.key, algorithms=["RS256"], audience=self.audience, issuer=self.issuer)
             #headers = jwt.get_unverified_header(token_jwt)
             # jwk = next(filter(lambda x: x['kid'] == kid, jwks))
 
             scopes = self.verify_claims(data)
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from flask import request, Response, jsonify
 
 from tomcru.services.aws.hosted.apigw.api_shared.integration import TomcruApiGWHttpIntegration, \
     LambdaAuthorizerIntegration
 from tomcru import TomcruApiEP, TomcruLambdaIntegrationEP, TomcruEndpoint
 
-
 base_headers = {
-    "content-type": "application/json"
+    "Access-Control-Expose-Headers": "*",
+    "Content-Type": "application/json",
+    "Access-Control-Allow-Origin": "*",
+    "Access-Control-Allow-Headers": "*"
 }
 
 
 class LambdaIntegration(TomcruApiGWHttpIntegration):
 
     def __init__(self, endpoint: TomcruLambdaIntegrationEP, auth: LambdaAuthorizerIntegration, lambda_builder, env=None):
         self.endpoint = endpoint
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tomcru.services.aws.hosted.apigw.api_shared.integration.TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
 
 
 from tomcru_jerry.mockapi import transform_response
 
 
 base_headers = {
-    "content-type": "application/json"
+    "Content-Type": "application/json"
 }
 
 
 class MockedIntegration(LambdaIntegration):
 
     def __init__(self, endpoint: TomcruMockedIntegrationEP, auth: TomcruApiGWAuthorizerIntegration, response: dict, env=None):
         self.endpoint = endpoint
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/boto3_b/boto3.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/boto3.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/ddb/proxy.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/proxy.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from sqlalchemy.orm import Session, Query, DeclarativeBase
+from sqlalchemy.orm import Session, Query
 from sqlalchemy.orm.attributes import flag_modified
 
 from botocore.exceptions import ClientError
 from sqlalchemy import text
 
 
 class DDBSqlAlchemyTable:
@@ -54,16 +54,14 @@
                 setattr(ent, self.sort_key, key[self.sort_key])
 
             setattr(ent, 'ddb_content', Item.copy())
             #         for k,v in kwargs.items():
             #             setattr(self, k, v)
             #
             #         self.ddb_content = kwargs.copy()
-
-            print(1)
             #ent = self.T(**Item)
         else:
             ent.ddb_content = Item
 
         self.session.add(ent)
 
         if self._autocommit:
@@ -249,9 +247,9 @@
 
         return _key
 
     def _truncate(self):
         self.session.execute(f'''TRUNCATE TABLE "{self.table_name}"''')
         self.session.commit()
 
-    def sql(self) -> tuple[Query, DeclarativeBase]:
+    def sql(self) -> tuple[Query, object]:
         return self.session.query(self.T), self.T
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,23 +64,22 @@
 
         # todo: @later: pass serialzied json as binary instead of base64 between processes
         resp = None
         with subprocess.Popen(cmd, bufsize=1, universal_newlines=True, shell=self.is_shell,
                               cwd=self.lambda_path, env=env_dict,
                               stdin=subprocess.PIPE, stdout=subprocess.PIPE) as p:
             for line in p.stdout:
-                print("Received", line.rstrip('\n'))
                 if line.startswith('FOO'):
                     p.stdin.write('BAR\n')
                     continue
 
                 t_in = deser(line)
 
                 if 'serv_id' in t_in:
-                    print("    REQUEST service:", t_in)
+                    print("  [LUAEXEC]: requesting service", t_in)
                     if 'boto3' in t_in:
                         import boto3
                         #boto3 = self.srvmgr.service(self.env, 'boto3').boto3
 
                         if t_in['boto3'] == 'resource':
                             srv = boto3.resource(t_in['serv_id'])
 
@@ -89,25 +88,25 @@
                             srv = boto3.client(t_in['serv_id'])
 
                         serv_resp = getattr(srv, t_in['method'])(**t_in['args'])
                         p.stdin.write(ser(serv_resp)+'\n')
                     else:
                         raise NotImplementedError(t_in)
                 elif 'log' in t_in:
-                    print("    LOG received:", t_in['log'])
+                    print("  [LUAEXEC.LOG]:", t_in['log'])
                 elif 'err' in t_in:
-                    print("    ERROR received:", t_in['err'])
+                    print("  [LUAEXEC.ERROR]:", t_in['err'])
                 elif 'resp' in t_in:
                     resp = t_in['resp'].copy()
                 elif 'bye' in t_in:
-                    print("    said GOODBYE")
+                    print("  [LUAEXEC] said GOODBYE")
                     p.send_signal(signal.SIGINT)
                     break
                 else:
-                    print("unknown message from child:", t_in)
+                    print("  [LUAEXEC] received:", line.rstrip('\n'))
 
             p.terminate()
 
         if resp:
             return resp
         else:
             raise Exception("no resp from lambda!")
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,12 +68,12 @@
 
         to_dir = os.path.dirname(from_path)
         if not os.path.exists(to_dir):
             os.makedirs(to_dir)
 
         if not os.path.exists(from_path):
             # todo: throw proper boto3 exception
-            raise Exception("not exists")
+            raise Exception("S3 adapter: path not found: " + from_path)
 
         shutil.copy(from_path, Filename)
 
         # todo: apply meta tags & callback
```

### Comparing `tomcru-0.2.4/tomcru/services/aws/hosted/s3_b/S3Service.py` & `tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3Service.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py` & `tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/SamTplBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/SamTplBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/core.yaml` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/core.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/httpapi.yaml` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/httpapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/integ_ws.yaml` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_ws.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/template.yaml` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/template.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/_junk/wsapi.yaml` & `tomcru-0.2.5/tomcru/services/aws/sam/_junk/wsapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/params_b/ParametersBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/params_b/ParametersBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py` & `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py` & `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/tomcru/services/general/eme2swagger/Eme2Swagger.py` & `tomcru-0.2.5/tomcru/services/general/eme2swagger/Eme2Swagger.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.4/PKG-INFO` & `tomcru-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru
-Version: 0.2.4
+Version: 0.2.5
 Summary: Serverless app framework
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

