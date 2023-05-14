# Comparing `tmp/AnimeCrawler-0.2.0b0.tar.gz` & `tmp/AnimeCrawler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimeCrawler-0.2.0b0.tar", last modified: Wed May 10 12:27:12 2023, max compression
+gzip compressed data, was "AnimeCrawler-0.2.1.tar", last modified: Sun May 14 06:08:40 2023, max compression
```

## Comparing `AnimeCrawler-0.2.0b0.tar` & `AnimeCrawler-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.937047 AnimeCrawler-0.2.0b0/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.864089 AnimeCrawler-0.2.0b0/AnimeCrawler/
--rw-rw-rw-   0        0        0      389 2023-05-10 12:26:57.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-10 11:04:59.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/__main__.py
--rw-rw-rw-   0        0        0     2690 2023-05-10 12:08:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/base_spider.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.899071 AnimeCrawler-0.2.0b0/AnimeCrawler/command/
--rw-rw-rw-   0        0        0      117 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/command/__init__.py
--rw-rw-rw-   0        0        0     3250 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/command/run.py
--rw-rw-rw-   0        0        0      521 2023-05-10 11:07:22.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/log.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.917069 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/
--rw-rw-rw-   0        0        0      286 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/__init__.py
--rw-rw-rw-   0        0        0     2396 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/downloader.py
--rw-rw-rw-   0        0        0     2129 2023-05-10 12:07:35.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/searcher.py
--rw-rw-rw-   0        0        0     4138 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/spider.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.932050 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/
--rw-rw-rw-   0        0        0      128 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/decode.py
--rw-rw-rw-   0        0        0     3017 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/file.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.883078 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/
--rw-rw-rw-   0        0        0     3270 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.2.0b0/LICENSE
--rw-rw-rw-   0        0        0     3270 2023-05-10 12:27:12.936047 AnimeCrawler-0.2.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     2819 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 12:27:12.938046 AnimeCrawler-0.2.0b0/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-05-10 12:26:46.000000 AnimeCrawler-0.2.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.934049 AnimeCrawler-0.2.0b0/test/
--rw-rw-rw-   0        0        0      264 2023-05-03 13:36:29.000000 AnimeCrawler-0.2.0b0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.127356 AnimeCrawler-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.046402 AnimeCrawler-0.2.1/AnimeCrawler/
+-rw-rw-rw-   0        0        0      380 2023-05-14 05:55:12.000000 AnimeCrawler-0.2.1/AnimeCrawler/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-13 16:45:12.000000 AnimeCrawler-0.2.1/AnimeCrawler/__main__.py
+-rw-rw-rw-   0        0        0     2823 2023-05-14 05:26:33.000000 AnimeCrawler-0.2.1/AnimeCrawler/base_spider.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.094376 AnimeCrawler-0.2.1/AnimeCrawler/cli/
+-rw-rw-rw-   0        0        0      113 2023-05-14 05:07:33.000000 AnimeCrawler-0.2.1/AnimeCrawler/cli/__init__.py
+-rw-rw-rw-   0        0        0     3513 2023-05-14 05:13:54.000000 AnimeCrawler-0.2.1/AnimeCrawler/cli/run.py
+-rw-rw-rw-   0        0        0      795 2023-05-14 05:24:57.000000 AnimeCrawler-0.2.1/AnimeCrawler/log.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.109369 AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/
+-rw-rw-rw-   0        0        0      282 2023-05-14 05:07:31.000000 AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/__init__.py
+-rw-rw-rw-   0        0        0     2389 2023-05-14 05:25:04.000000 AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/downloader.py
+-rw-rw-rw-   0        0        0     3493 2023-05-14 05:56:31.000000 AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/searcher.py
+-rw-rw-rw-   0        0        0     4198 2023-05-14 05:50:28.000000 AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/spider.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.120360 AnimeCrawler-0.2.1/AnimeCrawler/utils/
+-rw-rw-rw-   0        0        0      128 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.1/AnimeCrawler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.2.1/AnimeCrawler/utils/decode.py
+-rw-rw-rw-   0        0        0     3017 2023-05-13 17:13:17.000000 AnimeCrawler-0.2.1/AnimeCrawler/utils/file.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.084380 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/
+-rw-rw-rw-   0        0        0     3268 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 06:08:39.000000 AnimeCrawler-0.2.1/AnimeCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3268 2023-05-14 06:08:40.124357 AnimeCrawler-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2819 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:08:40.127356 AnimeCrawler-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      882 2023-05-14 05:54:36.000000 AnimeCrawler-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:08:40.122358 AnimeCrawler-0.2.1/test/
+-rw-rw-rw-   0        0        0      264 2023-05-03 13:36:29.000000 AnimeCrawler-0.2.1/test/test.py
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/base_spider.py` & `AnimeCrawler-0.2.1/AnimeCrawler/base_spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import urllib.parse
 
 from ruia import Request, Spider
 
-from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import is_url
 
+from .log import Logger
+
 
 class BaseSpider(Spider):
     '''所有爬虫的基类，必须提供domain与downloader属性
 
     Args:
         Spider (ruia.Spider): 继承于ruia框架的爬虫
 
@@ -16,25 +17,33 @@
         ValueError: 未定义domain时报错
         ValueError: 未定义downloader时报错
 
     Returns:
         cls: 为了链式调用ruia.Spider.start()
     '''
 
-    logger = get_logger('Spider', 'INFO')
+    logger = Logger()
 
-    def __init__(self, *args, **spider_kwargs) -> None:
-        super().__init__(*args, **spider_kwargs)
+    def __init__(
+        self,
+        *spider_args,
+        is_debug=False,
+        **spider_kwargs,
+    ) -> None:
+        super().__init__(*spider_args, **spider_kwargs)
         if not hasattr(self, 'domain'):
             raise ValueError(f'{self.__class__.__name__} 未定义domain属性')
         elif not hasattr(self, 'downloader'):
             raise ValueError(f'{self.__class__.__name__} 未定义downloader下载器')
 
     @classmethod
-    def init(cls):
+    def init(cls, is_debug):
+        if is_debug:
+            cls.logger.level = 'DEBUG'
+        cls.logger.get_logger('Spider')
         cls.start_urls = [
             i if is_url(i) else urllib.parse.urljoin(cls.domain, i)
             for i in cls.start_urls
         ]  # 当url为相对路径时与域名拼接
         return cls
 
     def urljoin(self, base, url, avoid_collision: bool = False) -> str:
@@ -66,15 +75,14 @@
         Returns:
             ruia.Request: 可被yield
         '''
         return self.request(self.urljoin(self.domain, next_url), **kwargs)
 
     def get_domain(self, url: str) -> str:
         url_parts = urllib.parse.urlsplit(url)
-        print(url)
         return '://'.join(url_parts[:2])  # e.g. https://docs.python.org/
 
     def get_path(self, url: str) -> str:
         url_parts = urllib.parse.urlsplit(url)
         return url_parts.path
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/command/run.py` & `AnimeCrawler-0.2.1/AnimeCrawler/cli/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import abc
 import argparse
 from collections import namedtuple
 
-from AnimeCrawler.log import get_logger
+from AnimeCrawler.log import Logger
 from AnimeCrawler.mhyyy.searcher import Searcher
 from AnimeCrawler.mhyyy.spider import AnimeSpider
 from AnimeCrawler.utils import is_url
 
 
 class BaseCommand:
     '''命令的基类
 
     子类必须实现 subcommand_add_arguments, handle, catch_error 方法
     '''
 
-    logger = get_logger('Command')
+    logger = Logger()
 
     @abc.abstractmethod
     def subcommand_add_arguments(self, parser) -> None:
         ...
 
     @abc.abstractmethod
     def handle(self, args) -> None:
@@ -42,14 +42,17 @@
             "--title",
             metavar='Title',
             help="动漫名称",
         )
         parser.add_argument(
             "--del_ts", dest='can_del_ts', help="删除ts文件", action='store_true'
         )
+        parser.add_argument(
+            '--debug', dest='is_debug', help='进入debug模式', action='store_true'
+        )
 
     def handle(self, args) -> None:
         if error := self.catch_error(args):
             raise ValueError(f'{error.output}')
         AnimeSpider.init(args.title, args.url, args.can_del_ts).start()
 
     def catch_error(self, parse):
@@ -63,19 +66,22 @@
     def subcommand_add_arguments(self, parser) -> None:
         parser.add_argument(
             "-t",
             "--title",
             metavar='Title',
             help="动漫名称",
         )
+        parser.add_argument(
+            '--debug', dest='is_debug', help='进入debug模式', action='store_true'
+        )
 
     def handle(self, args) -> None:
         if error := self.catch_error(args):
             raise ValueError(f'{error.output}')
-        Searcher.init(args.title).start()
+        Searcher.init(args.title, is_debug=args.is_debug).start()
 
     def catch_error(self, parse):
         if not parse.title:
             return self.base_error('402', 'null_title', '标题为空')
 
 
 def main():
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/downloader.py` & `AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 from typing import Any, Union
 
 import aiohttp
 import tqdm.asyncio
 
-from AnimeCrawler.log import get_logger
+from AnimeCrawler.log import Logger
 from AnimeCrawler.utils import write
 
 
 class Downloader:
     session = None
-    logger = get_logger('Downloader')
+    logger = Logger().get_logger()
 
     @property
     def current_session(self) -> aiohttp.ClientSession:
         if not self.session:
             self.session = aiohttp.ClientSession(
                 connector=aiohttp.TCPConnector(verify_ssl=False)
             )
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/searcher.py` & `AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/searcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from typing import Generator
 
 from ruia import AttrField, Item, TextField
 
 from AnimeCrawler.base_spider import BaseSpider
 from AnimeCrawler.utils import align
 
@@ -16,48 +17,83 @@
         xpath_select='//div[@class="module-card-item-footer"]/a[@class="play-btn icon-btn"]',
         many=True,
     )
     title = TextField(
         xpath_select='//div[@class="module-card-item-title"]/a[@rel="nofollow"]/strong',
         many=True,
     )
+    info = TextField(
+        xpath_select='//div[@class="module-card-item-info"]/div[last()]/div["module-card-item-content"]',
+        many=True,
+    )
+
+
+class LineItem(Item):
+    target_item = TextField(xpath_select='//div[@class="swiper-wrapper"]')
+    line_name = TextField(
+        xpath_select='//a[@data-hash="slide{1}"]',
+        many=True,
+    )
+    line_url = AttrField(
+        attr='href',
+        xpath_select='//a[@data-hash="slide{1}"]',
+        many=True,
+    )
 
 
 class Searcher(BaseSpider):
     session = None
     downloader = None
     domain = 'https://www.mh620.com'
-    # logger = get_logger('Searcher')
 
     @classmethod
-    def init(cls, anime_title) -> BaseSpider:
+    def init(cls, anime_title, is_debug) -> BaseSpider:
         cls.start_urls = [
             cls.urljoin(cls, cls.domain, f'/search.html?wd={anime_title}')
         ]
-        return super().init()
+        return super().init(is_debug)
 
     async def select_anime(self, animes) -> None:
-        answer = int(input('Which anime do you want to download? >>> '))
-        if answer <= 0:
-            return
-        anime = animes[answer - 1][1]
-        title, url = anime[0].replace(' ', '_'), self.domain + anime[1]
-        print(
-            f'\nDownload Command:\nAnimeCrawler download -t {title} -u {url} --del_ts'
-        )
-
-    async def pretty_print(self, animes) -> None:
-        partten = "{0}| {1}|"
-        print(partten.format('序号', align('标题', 38, 'C')))
-        print('-' * 45)
-        for index, (title, _) in animes:
-            print(partten.format(align(str(index), 4), align(title, 37)))
+        answer = input('Which anime do you want to download? >>> ')
+        if answer.isdigit():
+            answer = int(answer)
+            anime = animes[answer - 1][1]
+            title, url = anime[0].replace(' ', '_'), self.domain + anime[1]
+            html = await self.request(url=url).fetch()
+            await self.select_line(title, html)
+
+    async def select_line(self, title, html):
+        async for item in LineItem.get_items(html=await html.text()):
+            lines = tuple(
+                enumerate(
+                    zip(item.line_name, item.line_url, itertools.repeat(None)),
+                    start=1,
+                )
+            )
+            await self.pretty_print(lines)
+        answer = input('Which line do you expect to download? >>> ')
+        if answer.isdigit():
+            answer = int(answer)
+            line_info = lines[answer - 1][1]
+            print(
+                f'\nDownload Command:\nAnimeCrawler download -t {title} -u {self.domain + line_info[1]} --del_ts'
+            )
+
+    async def pretty_print(self, items) -> None:
+        partten = "{0}| {1}| {2}"
+        print(partten.format('序号', align('标题', 38, 'C'), align('简介', 26, 'C')))
+        print('-' * 75)
+        for index, (title, _, info) in items:
+            info = '无简介' if info is None else info[:12] + '...'
+            print(
+                partten.format(align(str(index), 4), align(title, 37), align(info, 20))
+            )
 
     async def parse(self, response) -> Generator[SearchItem, None, None]:
         async for item in SearchItem.get_items(html=await response.text()):
             yield item
 
     async def process_item(self, item: SearchItem) -> None:
-        animes = tuple(enumerate(zip(item.title, item.url), start=1))
+        animes = tuple(enumerate(zip(item.title, item.url, item.info), start=1))
         # 美化输出
         await self.pretty_print(animes)
         await self.select_anime(animes)
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/spider.py` & `AnimeCrawler-0.2.1/AnimeCrawler/mhyyy/spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,42 +16,44 @@
 
 from .downloader import Downloader
 
 
 class AnimeItem(Item):
     target_item = TextField(xpath_select='//div[@class="player-box-main"]')
     profile = TextField(xpath_select='//div/script[@type="text/javascript"]')
-    episodes = None
+    episodes = TextField(xpath_select='//a[@class="module-play-list-link active"]')
     _base_m3u8_url = None
     mixed_m3u8_url = None
 
 
 class AnimeSpider(BaseSpider):
     _base_ts_url = None
     _mixed_m3u8 = None
     downloader = Downloader()
     headers = {'User-Agent': 'Mozilla/5.0'}
     concurrency: int = 5
 
     @classmethod
-    def init(cls, anime_title: str, urls: str, del_ts: bool = False) -> BaseSpider:
+    def init(
+        cls, anime_title: str, urls: str, del_ts: bool = False, is_debug: bool = False
+    ) -> BaseSpider:
         '''初始化爬虫
 
         Args:
             anime_title (str): 动漫标题，用于取文件夹的名称，利于管理动漫
             urls (str): 第一页的网址
 
         Returns:
             cls: 为了链式调用返回了cls
         '''
         cls.domain = cls.get_domain(cls, urls)
         cls.start_urls = [cls.get_path(cls, urls)]
         cls.PATH = folder_path(Path(get_video_path()) / anime_title)
         cls.del_ts = del_ts
-        return super().init()
+        return super().init(is_debug)
 
     async def _mixed_m3u8_url_parse(self, index_m3u8_url: str, item: AnimeItem) -> None:
         resp = await self.request(index_m3u8_url).fetch()
         text = await resp.text()
         if self._mixed_m3u8 is None:
             self._mixed_m3u8 = text.split('\n')[-1]
         item.mixed_m3u8_url = self.urljoin(item._base_m3u8_url, self._mixed_m3u8)
@@ -79,36 +81,34 @@
 
     async def parse(
         self, response: Response
     ) -> AsyncGenerator[Request | AnimeItem, None]:
         async for item in AnimeItem.get_items(html=await response.text()):
             profile = item.profile
             player_aaaa = eval(re.search('{.*}', profile).group())
-            item.episodes = re.findall('\d+', response.url)[2]
             encoded_url = player_aaaa['url']
             index_m3u8_url = unescape(
                 base64_decode(encoded_url)
             )  # 目标网站的index.m3u8文件地址做了加密
             item._base_m3u8_url = index_m3u8_url[:-10]
             await self._mixed_m3u8_url_parse(index_m3u8_url, item)
-
+            print(item.episodes)
             link_next = player_aaaa.get('link_next', None)
             if link_next:
                 yield await self.have_next_page(link_next)
             yield item
 
     async def process_item(self, item: AnimeItem) -> None:
         resp = await self.request(item.mixed_m3u8_url, headers=self.headers).fetch()
         text = await resp.text()
-        episodes = item.episodes
-        folder_path = self.PATH / f'{episodes}'
+        folder_path = self.PATH / f'{item.episodes}'
         self.logger.info('\033[0;32;40m写入mixed.m3u8\033[0m')
         await write(folder_path, text, 'mixed', 'm3u8', 'w+')
         urls = self._parse_mixed_m3u8(item)
         self.downloader.set_url = urls
-        await self.downloader.download_ts_files(folder_path, episodes)
-        self.logger.info(f"正在把第 {episodes} 集的ts文件转码成 mp4")
-        await merge_ts2mp4(folder_path, episodes, self.del_ts)
+        await self.downloader.download_ts_files(folder_path, item.episodes)
+        self.logger.info(f"正在把 {item.episodes} 的ts文件转码成 mp4")
+        await merge_ts2mp4(folder_path, item.episodes, self.del_ts)
 
     async def stop(self, _signal) -> None:
         await self.downloader.close_session()
         return await super().stop(_signal)
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/utils/decode.py` & `AnimeCrawler-0.2.1/AnimeCrawler/utils/decode.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler/utils/file.py` & `AnimeCrawler-0.2.1/AnimeCrawler/utils/file.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/PKG-INFO` & `AnimeCrawler-0.2.1/AnimeCrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.2.0b0
+Version: 0.2.1
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/SOURCES.txt` & `AnimeCrawler-0.2.1/AnimeCrawler.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 AnimeCrawler/log.py
 AnimeCrawler.egg-info/PKG-INFO
 AnimeCrawler.egg-info/SOURCES.txt
 AnimeCrawler.egg-info/dependency_links.txt
 AnimeCrawler.egg-info/entry_points.txt
 AnimeCrawler.egg-info/requires.txt
 AnimeCrawler.egg-info/top_level.txt
-AnimeCrawler/command/__init__.py
-AnimeCrawler/command/run.py
+AnimeCrawler/cli/__init__.py
+AnimeCrawler/cli/run.py
 AnimeCrawler/mhyyy/__init__.py
 AnimeCrawler/mhyyy/downloader.py
 AnimeCrawler/mhyyy/searcher.py
 AnimeCrawler/mhyyy/spider.py
 AnimeCrawler/utils/__init__.py
 AnimeCrawler/utils/decode.py
 AnimeCrawler/utils/file.py
```

### Comparing `AnimeCrawler-0.2.0b0/LICENSE` & `AnimeCrawler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0b0/PKG-INFO` & `AnimeCrawler-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.2.0b0
+Version: 0.2.1
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AnimeCrawler-0.2.0b0/README.md` & `AnimeCrawler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0b0/setup.py` & `AnimeCrawler-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnimeCrawler",
-    version="v0.2.0b",
+    version="v0.2.1",
     author="Senvlin",
     author_email="2994515402@qq.com",
     description="一个可免费下载动漫的爬虫",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Senvlin/AnimeCrawler",
     packages=setuptools.find_packages(),
```

