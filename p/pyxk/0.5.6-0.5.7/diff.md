# Comparing `tmp/pyxk-0.5.6.tar.gz` & `tmp/pyxk-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.6.tar", last modified: Sat May 13 09:36:54 2023, max compression
+gzip compressed data, was "pyxk-0.5.7.tar", last modified: Sun May 14 14:03:29 2023, max compression
```

## Comparing `pyxk-0.5.6.tar` & `pyxk-0.5.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.6/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-13 09:36:54.033999 pyxk-0.5.6/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.6/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       53 2023-05-08 09:38:07.000000 pyxk-0.5.6/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-13 08:37:44.000000 pyxk-0.5.6/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    17711 2023-05-13 08:47:34.000000 pyxk-0.5.6/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-13 05:40:17.000000 pyxk-0.5.6/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.6/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.6/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.6/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk/m3u8downloader/
--rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.6/pyxk/m3u8downloader/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3462 2023-05-13 09:36:19.000000 pyxk-0.5.6/pyxk/m3u8downloader/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4884 2023-05-13 09:28:48.000000 pyxk-0.5.6/pyxk/m3u8downloader/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.6/pyxk/m3u8downloader/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    11732 2023-05-13 09:23:24.000000 pyxk-0.5.6/pyxk/m3u8downloader/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.6/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.6/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.6/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.6/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19219 2023-05-13 07:41:11.000000 pyxk-0.5.6/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-13 09:36:54.033999 pyxk-0.5.6/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-13 09:36:53.000000 pyxk-0.5.6/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-13 09:36:54.033999 pyxk-0.5.6/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-13 09:36:32.000000 pyxk-0.5.6/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.7/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-14 14:03:29.231998 pyxk-0.5.7/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.7/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-14 14:00:13.000000 pyxk-0.5.7/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-13 08:37:44.000000 pyxk-0.5.7/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    18023 2023-05-14 13:50:42.000000 pyxk-0.5.7/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-13 05:40:17.000000 pyxk-0.5.7/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.7/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.7/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.7/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/pyxk/m3u8downloader/
+-rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.7/pyxk/m3u8downloader/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3448 2023-05-13 14:37:26.000000 pyxk-0.5.7/pyxk/m3u8downloader/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-14 14:00:57.000000 pyxk-0.5.7/pyxk/m3u8downloader/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.7/pyxk/m3u8downloader/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    11732 2023-05-13 09:23:24.000000 pyxk-0.5.7/pyxk/m3u8downloader/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.231998 pyxk-0.5.7/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.7/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.7/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.7/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.7/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-14 13:59:58.000000 pyxk-0.5.7/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-14 14:03:29.221998 pyxk-0.5.7/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-14 14:03:29.000000 pyxk-0.5.7/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-14 14:03:29.231998 pyxk-0.5.7/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-14 14:03:10.000000 pyxk-0.5.7/setup.py
```

### Comparing `pyxk-0.5.6/LICENSE` & `pyxk-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/aclient/client.py` & `pyxk-0.5.7/pyxk/aclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
         # aiohttp session
         self._session: Session = None
         # base_url
         self._base_url: StrOrURL = self.set_base_url(base_url)
 
     @classmethod
     def run(cls, **kwargs):
+        """程序运行入口 - 应该调用该方法运行
+
+        :params: **kwargs: 类实例化关键字参数
+        """
         self = cls(**kwargs)
         # 创建新的 event loop
         self._loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self._loop)
         # 运行
         self._loop.run_until_complete(self.async_start())
         # 关闭 event loop
@@ -169,15 +173,15 @@
         """关闭异步下载器"""
         await self.close()
         # 关闭 aiohttp client session
         if isinstance(self._session, aiohttp.ClientSession) and self._session.closed is False:
             await self._session.close()
 
     async def start_request(self) -> list:
-        """发送 start_urls 链接"""
+        """start_urls 默认运行方法"""
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
             raise NotImplementedError(f"{self.__class__.__name__}.start_urls is not available!")
         tasks = []
         for item in self.start_urls:
             url, cb_kwargs = item, None
             if isinstance(item, (list, tuple)) and len(item) >= 2:
                 url, cb_kwargs = item[0], dict(item[1])
@@ -203,99 +207,87 @@
         :params: url: URL
         :params: callback: 响应response 回调函数(函数是异步的)
         :params: *
         :params: method: 请求方法(default: GET)
         :params: cb_kwargs: 回调函数 关键字参数
         :params: **req_kwargs: 异步请求 request参数
         """
-        async with self.semaphore:
-            url = self.build_url(url)
-            response = await self.send(method=method, url=url, **req_kwargs)
-            # 添加自定义方法
-            add_method_to_response(response)
-            # 开启回调函数
-            if callable(callback):
-                cb_kwargs = dict(cb_kwargs or {})
-                result = await callback(response, **cb_kwargs)
-                response.close()
-                return result
-            return response
-
-    async def send(
-        self, method: str, url: StrOrURL, **req_kwargs
-    ) -> Response:
-        """异步请求发送
-
-        :params: method: 请求方法
-        :params: url: URL
-        :params: **req_kwargs: 异步请求 request参数
-        """
-        retry, exc_count = 0, 0
+        retry, exc_count, ret, response = 0, 0, None, None
         maximum_retry = self.maximum_retry \
             if isinstance(self.maximum_retry, int) and self.maximum_retry > 0 else dict(self.attr)["maximum_retry"]
-        while True:
-            try:
-                response = await self._session.request(method=method, url=url, **req_kwargs)
-                # 抛出 error status_code
-                if isinstance(self.error_status_code, (list, tuple)) and response.status in self.error_status_code:
-                    raise aiohttp.InvalidURL(f"<Response[{response.status}] {url}>")
-                # 重试 retry status_code
-                if isinstance(self.retry_status_code, (list, tuple)) and response.status in self.retry_status_code:
-                    response.close()
-                    retry += 1
-                    if retry % 10 == 0:
-                        warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
+        async with self.semaphore:
+            url = self.build_url(url)
+            while True:
+                try:
+                    response = await self._session.request(method=method, url=url, **req_kwargs)
+                    # 抛出 error status_code
+                    if isinstance(self.error_status_code, (list, tuple)) and response.status in self.error_status_code:
+                        raise aiohttp.InvalidURL(f"<Response[{response.status}] {url}>")
+                    # 重试 retry status_code
+                    if isinstance(self.retry_status_code, (list, tuple)) and response.status in self.retry_status_code:
+                        response.close()
+                        retry += 1
+                        if retry % 10 == 0:
+                            warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
+                        await self.sleep()
+                        continue
+                    # 直到请求状态码200才返回 until_request_succeed
+                    as_succeed = self.until_request_succeed \
+                        if self.until_request_succeed is not None else dict(self.attr)["until_request_succeed"]
+                    if not isinstance(as_succeed, (list, tuple)):
+                        as_succeed = [200] if as_succeed else []
+                    if as_succeed and response.status not in as_succeed:
+                        response.close()
+                        retry += 1
+                        if retry % 10 == 0:
+                            warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
+                        await self.sleep()
+                        continue
+                    # 添加自定义方法
+                    add_method_to_response(response)
+                    # 开启回调函数
+                    if callable(callback):
+                        cb_kwargs = dict(cb_kwargs or {})
+                        ret = await callback(response, **cb_kwargs)
+                        response.close()
+                    else:
+                        ret = response
+                    break
+                # 请求超时 重试
+                except asyncio.exceptions.TimeoutError:
+                    if response:
+                        response.close()
+                    exc_count += 1
+                    if exc_count >= maximum_retry:
+                        raise
+                    # warnings.warn(f"<{url}> Timeout", stacklevel=4)
                     await self.sleep()
-                    continue
-                # 直到请求状态码200才返回 until_request_succeed
-                as_succeed = self.until_request_succeed \
-                    if self.until_request_succeed is not None else dict(self.attr)["until_request_succeed"]
-                if not isinstance(as_succeed, (list, tuple)):
-                    as_succeed = [200] if as_succeed else []
-                if as_succeed and response.status not in as_succeed:
-                    response.close()
-                    retry += 1
-                    if retry % 10 == 0:
-                        warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
+                # 连接错误 重试
+                except (
+                    aiohttp_client_exceptions.ClientOSError,
+                    aiohttp_client_exceptions.ClientPayloadError,
+                    aiohttp_client_exceptions.ClientConnectorError,
+                ):
+                    if response:
+                        response.close()
+                    exc_count += 1
+                    if exc_count >= maximum_retry:
+                        raise
+                    # warnings.warn(f"<{url}> ConnectorError", stacklevel=4)
                     await self.sleep()
-                    continue
-                break
-            # 请求超时 重试
-            except asyncio.exceptions.TimeoutError:
-                exc_count += 1
-                if exc_count >= maximum_retry:
-                    raise
-                # warnings.warn(f"<{url}> Timeout", stacklevel=4)
-                await self.sleep()
-            # 连接错误 重试
-            except (
-                aiohttp_client_exceptions.ClientOSError,
-                aiohttp_client_exceptions.ClientPayloadError,
-                aiohttp_client_exceptions.ClientConnectorError,
-            ):
-                exc_count += 1
-                if exc_count >= maximum_retry:
-                    raise
-                # warnings.warn(f"<{url}> ConnectorError", stacklevel=4)
-                await self.sleep()
-            # 服务器拒绝连接
-            except aiohttp_client_exceptions.ServerDisconnectedError:
-                exc_count += 1
-                if exc_count >= maximum_retry:
-                    raise
-                # warnings.warn(f"<{url}> ServerDisconnectedError", stacklevel=4)
-                await self.sleep()
-        return response
-
-    async def sleep(self, delay: Optional[Union[int, float]]=None, result: Any=None):
-        """异步休眠"""
-        if not isinstance(delay, int) or delay <= 0:
-            delay = self.async_sleep \
-                if isinstance(self.async_sleep, int) and self.async_sleep > 0 else dict(self.attr)["async_sleep"]
-        return await asyncio.sleep(delay, result=result)
+                # 服务器拒绝连接
+                except aiohttp_client_exceptions.ServerDisconnectedError:
+                    if response:
+                        response.close()
+                    exc_count += 1
+                    if exc_count >= maximum_retry:
+                        raise
+                    # warnings.warn(f"<{url}> ServerDisconnectedError", stacklevel=4)
+                    await self.sleep()
+            return ret
 
     async def gather(
         self,
         urls: List[StrOrURL],
         callback: RequestCallback = None,
         *,
         method: str = "GET",
@@ -342,14 +334,21 @@
                 cb_kwargs=cb_kwargs,
                 **req_kwargs
             )
             tasks.append(task)
         result = await asyncio.gather(*tasks, return_exceptions=return_exceptions)
         return result
 
+    async def sleep(self, delay: Optional[Union[int, float]]=None, result: Any=None):
+        """异步休眠"""
+        if not isinstance(delay, int) or delay <= 0:
+            delay = self.async_sleep \
+                if isinstance(self.async_sleep, int) and self.async_sleep > 0 else dict(self.attr)["async_sleep"]
+        return await asyncio.sleep(delay, result=result)
+
     def build_url(self, _url) -> StrOrURL:
         """构造完整url地址"""
         if not isinstance(_url, (str, _yarl.URL)):
             return _url
         _url = _yarl.URL(_url)
         if _url.is_absolute():
             return _url
```

### Comparing `pyxk-0.5.6/pyxk/aclient/typedef.py` & `pyxk-0.5.7/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/aes/_fmtdata.py` & `pyxk-0.5.7/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/aes/cryptor.py` & `pyxk-0.5.7/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/m3u8downloader/enter_point.py` & `pyxk-0.5.7/pyxk/m3u8downloader/enter_point.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def file(obj, content, url, output, reload, reserve, headers, verify, limit, user_agent):
     """下载m3u8资源 - m3u8 content"""
     m3u8downloader.load_content(
         content=content,
-        url=url or obj["url"],
+        url=url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
         limit=limit or obj["limit"],
         user_agent=get_user_agent(user_agent or obj["user_agent"])
```

### Comparing `pyxk-0.5.6/pyxk/m3u8downloader/m3u8download.py` & `pyxk-0.5.7/pyxk/m3u8downloader/m3u8download.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from concurrent.futures import ThreadPoolExecutor
 
 from pyxk.aes import Cryptor
 from pyxk.utils import make_open
 from pyxk.aclient import Client, Response
 
 
-
 class Downloader(Client):
     """m3u8 - segments 下载器
 
     :params: m3u8keys: m3u8资源加密密钥
     :params: segments: m3u8 segments
     :params: progress: rich.progress.Progress
     :params: download: rich.progress.Progress
     """
     timeout = 30
+    maximum_retry = 999
     error_status_code = list(range(403, 411))
     until_request_succeed = True
 
     def __init__(
         self,
         *,
         m3obj,
```

### Comparing `pyxk-0.5.6/pyxk/m3u8downloader/m3u8parse.py` & `pyxk-0.5.7/pyxk/m3u8downloader/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/m3u8downloader/main.py` & `pyxk-0.5.7/pyxk/m3u8downloader/main.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/requests/api.py` & `pyxk-0.5.7/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/requests/entry_point.py` & `pyxk-0.5.7/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/requests/sessions.py` & `pyxk-0.5.7/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/pyxk/utils.py` & `pyxk-0.5.7/pyxk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import (
     Any,
     Dict,
     Union,
     Tuple,
+    Literal,
     Optional,
     Callable,
     Coroutine,
 )
 from types import ModuleType
 from importlib import import_module
 
+
 __all__ = [
     "LazyLoader",
     "runtime",
     "coro_runtime",
     "make_open",
     "get_user_agent",
     "default_headers",
@@ -29,16 +31,14 @@
     "pyfile_conversion_lazyloader",
     "units_conversion_from_byte",
     "download_column",
     "progress_column",
     "chardet"
 ]
 
-
-
 class LazyLoader(ModuleType):
     """
     模块 延迟加载
     :params: local_name: 模块引用名称
     :params: module_life_cycle: 模块生命周期( 建议使用全局变量 globals() )
     :params: import_name: 导入模块名称
     """
@@ -74,18 +74,15 @@
 itertools = LazyLoader("itertools", globals(), "itertools")
 collections = LazyLoader("collections", globals(),"collections")
 rich_console = LazyLoader("rich_console", globals(), "rich.console")
 
 
 # 计算函数运行时间
 def runtime(func: Callable):
-    """计算函数运行时间
-
-    :params: func: 需要计算运行时间的函数
-    """
+    """装饰器: 计算函数运行时间"""
     @functools.wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         console = rich_console.Console()
         try:
             start_time = time.perf_counter()
             result = func(*args, **kwargs)
         finally:
@@ -93,37 +90,31 @@
             console.print(f"{func.__name__!r} [magenta]running time[/]: {end_time - start_time}")
         return result
     return wrapper
 
 
 # 计算异步函数运行时间
 def coro_runtime(func: Coroutine):
-    """计算异步函数运行时间
-
-    :params: func: 需要计算运行时间的协程函数
-    """
+    """装饰器: 计算异步函数运行时间"""
     @functools.wraps(func)
     async def wrapper(*args, **kwargs) -> Any:
         console = rich_console.Console()
         try:
             start_time = time.perf_counter()
             result = await func(*args, **kwargs)
         finally:
             end_time = time.perf_counter()
             console.print(f"{func.__name__!r} [magenta]coroutine running time[/]: {end_time - start_time}")
         return result
     return wrapper
 
 
 # 内置方法 `open` 装饰器
-def _open_wrapper(func) -> open:
-    """内置方法 `open` 装饰器
-
-    文件模式 w/a 下，创建不存在的目录
-    """
+def _open_wrapper(func):
+    """内置方法 `open` 装饰器 - 文件模式 w/a 下，创建不存在的目录"""
     @functools.wraps(func)
     def wrapper(
         file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None
     ):
         if not isinstance(mode, str):
             raise TypeError(f"{func.__name__}() argument 'mode' must be str, not {type(mode).__name__!r}")
         # file mode `w` or `a`
@@ -148,16 +139,14 @@
 # User Agent
 def get_user_agent(ua: Optional[str]=None, overwrite: bool=False) -> str:
     """获取 UserAgent，默认 Android
 
     :params: ua: 模糊查找内置字典UserAgent
         (android, windows, mac, iphone, ipad, symbian, apad)
     :params: overwrite: 若为True, 直接返回UserAgent
-
-    :return `str`
     """
     # 重写 UserAgent
     if overwrite:
         return ua
     # UserAgent 全部字典
     user_agent_dict = {
         "android" : "Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.91 Mobile Safari/537.36",
@@ -175,53 +164,49 @@
     ua = difflib.get_close_matches(ua.lower(), user_agent_dict.keys(), 1)
     if not ua:
         return user_agent_dict["android"]
     return user_agent_dict[ua[0]]
 
 
 # Headers
-def default_headers(ua: Optional[str]=None) -> Dict[str, str]:
+def default_headers(ua: Optional[str]=None) -> Dict[Literal["User-Agent"], str]:
     """默认 headers
 
     :params: ua: 模糊查找内置字典UserAgent
-
-    :return {"User-Agent": `str`}
     """
     return {"User-Agent": get_user_agent(ua)}
 
 
 # md5 加密
-def md5(plaintext: Union[str, bytes], encoding: Optional[str]=None) -> Dict[str, str]:
+def md5(plaintext: Union[str, bytes], encoding: Optional[str]=None):
     """MD5 加密
 
     :params: plaintext: 需加密明文
     :params: encoding: plaintext编码
-
-    :return {"plaintext": `str`, "ciphertext": `str`}
+    :return: {"plaintext": `str`, "ciphertext": `str`}
     """
     result = {"plaintext": None, "ciphertext": None}
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding or "utf-8")
     elif not isinstance(plaintext, bytes):
         result["plaintext"] = plaintext
         return result
     # md5加密
     ciphertext = hashlib.md5(plaintext).hexdigest()
     result["plaintext"], result["ciphertext"] = plaintext, ciphertext
     return result
 
 
 # hash256
-def hash256(plaintext: Union[str, bytes], encoding: Optional[str]=None) -> Dict[str, str]:
+def hash256(plaintext: Union[str, bytes], encoding: Optional[str]=None):
     """HASH_256
 
     :params: plaintext: 需加密明文
     :params: encoding: plaintext编码
-
-    :return {"plaintext": `str`, "ciphertext": `str`}
+    :return: {"plaintext": `str`, "ciphertext": `str`}
     """
     result = {"plaintext": None, "ciphertext": None}
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding or "utf-8")
     elif not isinstance(plaintext, bytes):
         result["plaintext"] = plaintext
         return result
@@ -232,16 +217,14 @@
 
 
 # 判断base64数据类型
 def is_base64(data: Union[str, bytes]) -> bool:
     """判断base64数据类型
 
     :params: data: 需要检测的数据
-
-    :return `bool`
     """
     if isinstance(data, bytes):
         # base64 数据类型 正则表达式判断
         B64_RE_PATTERN_B = re.compile(rb"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
         return bool(B64_RE_PATTERN_B.match(data))
 
     if isinstance(data, str):
@@ -254,35 +237,34 @@
 
 # base64数据类型 转化为bytes
 def base64_conversion_bytes(data: Union[str, bytes], encoding: str="utf-8") -> Tuple[bool, Union[str, bytes]]:
     """base64数据类型 转化为bytes
 
     :params: data: 需要 base64 解密的数据
     :params: encoding: type(data) is 'str' 通过 encoding 转换为 bytes
-
-    :return Tuple()
     """
     if (
         not isinstance(data, (str, bytes))
         or not is_base64(data)
     ):
         return False, data
     if isinstance(data, str):
         data = data.encode(encoding)
     return True, base64.b64decode(data)
 
 
 # 重命名本地存在的文件
-def rename_file(file: str, suffix: Optional[str]=None) -> Tuple[str, str, str]:
+def rename_file(
+    file: str, suffix: Optional[str]=None
+) -> Tuple[Literal["rename_file"], Literal["dirname"], Literal["basename"]]:
     """重命名本地存在的文件
 
     :params: file: 文件路径
     :params: suffix: 文件后缀名
-
-    :return Tuple(`rename_file`, `dirname`, `basename`)
+    :return: Tuple(`rename_file`, `dirname`, `basename`)
     """
     # 绝对路径
     file = os.path.abspath(file)
     # 后缀名解析
     if not isinstance(suffix, str) or not suffix:
         file_split, suffix = file.rsplit(".", 1), ""
         if len(file_split) == 2 and len(file_split[-1]) < 6:
@@ -299,40 +281,38 @@
         newfile = file.removesuffix(suffix) + f".{index}" + suffix
         if not os.path.isfile(newfile):
             break
     return newfile, *os.path.split(newfile)
 
 
 # 重命名本地存在的文件夹
-def rename_folder(folder: str) -> Tuple[str, str, str]:
+def rename_folder(folder: str) -> Tuple[Literal["rename_folder"], Literal["dirname"], Literal["basename"]]:
     """重命名本地存在的文件夹
 
     :params: folder: 文件夹路径
-
-    :return Tuple(`rename_folder`, `dirname`, `basename`)
+    :return: Tuple(`rename_folder`, `dirname`, `basename`)
     """
     folder = os.path.abspath(folder)
     if not os.path.isdir(folder):
         return folder, *os.path.split(folder)
 
     for index in itertools.count(1):
         new_folder = folder + f".{index}"
         if not os.path.isdir(new_folder):
             break
     return new_folder, *os.path.split(new_folder)
 
 
 # 字符串转换为数字
-def string_conversion_digits(target: Union[str, int, float], default: Any=None) -> Dict[str, Any]:
+def string_conversion_digits(target: Union[str, int, float], default: Any=None):
     """字符串转换为数字
 
     :params: target: 需要转换的目标
     :params: default: 不是数字返回默认值 `default=None`
-
-    :return {"is_digits": `bool`, "original": `Any`, "converted": `digits` or `default`}
+    :return: {"is_digits": `bool`, "original": `Any`, "converted": `digits`}
     """
     result = {"is_digits": False, "original": target, "converted": default}
     # target type = `int` or `float`
     if isinstance(target, (int, float)):
         result["is_digits"], result["converted"] = True, target
         return result
     # target type != `str`
@@ -354,16 +334,15 @@
 
 
 # 人类直观时间展示
 def human_playtime(playtime: Union[str, int, float]) -> Optional[str]:
     """人类直观时间展示
 
     :params: playtime: 传入一个时间(秒), 返回人类能理解的时间格式
-
-    :return `str` or None
+    :return: Optional[str]
     """
     digits = string_conversion_digits(playtime)
     if not digits["is_digits"]:
         return None
     playtime = digits["converted"]
     symbol, playtime = "-" if playtime < 0 else "", round(abs(playtime))
     hour, second = divmod(playtime, 3600)
@@ -372,16 +351,14 @@
 
 
 # python模块转换懒加载
 def pycode_conversion_lazyloader(string: str) -> str:
     """python模块转换懒加载
 
     :params: string: python代码
-
-    :return `str`
     """
     pattern = re.compile(
         r"^from\s+?(?P<from_name>\S+)\s+?import\s+?(?P<from_import_name>\S+)\s*?(as\s+?(?P<from_import_alias>\S+))?$|^import\s+?(?P<import_name>\S+)(\s+?as\s+(?P<import_alias>\S+?))?\s*?$",
         flags=re.M
     )
     def repl_string(match):
         match_dict = match.groupdict()
@@ -402,15 +379,15 @@
         return result.format(alias=alias, import_name=import_name)
     # 替换懒加载
     string = pattern.sub(repl=repl_string, string=string)
     return string
 
 
 # python模块转换懒加载 从文件
-def pyfile_conversion_lazyloader(read_file: str, write_file: str, encoding: Optional[str]=None) -> None:
+def pyfile_conversion_lazyloader(read_file: str, write_file: str, encoding: Optional[str]=None):
     """python模块转换懒加载 从文件
 
     :params: read_file: 读取python代码文件
     :params: write_file: 写入转换后的python代码文件
     """
     with open(read_file, "r", encoding=encoding) as fileobj:
         content = fileobj.read()
@@ -420,16 +397,14 @@
 
 
 # 字节单位自动换算
 def units_conversion_from_byte(target: Union[int, float]) -> Optional[str]:
     """字节单位自动换算
 
     :params: 换算目标(Bytes)
-
-    :return str or None
     """
     target = string_conversion_digits(target)
     if not target["is_digits"]:
         return None
     target, target_units = abs(target["converted"]), "Bytes"
     units_dict = {"Bytes": 1, "KB": 1024, "MB": 1024, "GB": 1024, "TB": 1024, "PB": 1024, "EB": 1024, "ZB": 1024, "YB": 1024, "BB": 1024}
     for units, rate in units_dict.items():
@@ -462,18 +437,18 @@
     :params: progress: rich.progress.Progress类 默认自动创建
     :params: completed: task 已完成步数 默认为0
     :params: transient: 转瞬即逝
     :params: description: 任务描述
     :params: show_transfer_speed: 显示任务速度
 
     `add_task` is `True`
-        return progress, task
+        :return: progress, task
 
     `add_task` is `False`
-        return progress
+        ;return: progress
     """
     import rich.progress as rich_progress
     if not isinstance(progress, rich_progress.Progress):
         column = [
             rich_progress.TextColumn("[progress.description]{task.description}"),
             rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
             rich_progress.BarColumn(),
@@ -517,18 +492,18 @@
     :params: progress: rich.progress.Progress类 默认自动创建
     :params: completed: task 已完成步数 默认为0
     :params: transient: 转瞬即逝
     :params: description: 任务描述
     :params: show_transfer_speed: 显示任务速度
 
     `add_task` is `True`
-        return progress, task
+        :return: progress, task
 
     `add_task` is `False`
-        return progress
+        :return: progress
     """
     import rich.progress as rich_progress
     if not isinstance(progress, rich_progress.Progress):
         column = [
             rich_progress.TextColumn("[progress.description]{task.description}"),
             rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
             rich_progress.BarColumn(),
```

### Comparing `pyxk-0.5.6/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.7/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.6/setup.py` & `pyxk-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.6",
+    version="0.5.7",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

