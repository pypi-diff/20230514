# Comparing `tmp/anicli_api-0.3.8.tar.gz` & `tmp/anicli_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.3.8.tar", max compression
+gzip compressed data, was "anicli_api-0.4.0.tar", max compression
```

## Comparing `anicli_api-0.3.8.tar` & `anicli_api-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,25 @@
--rw-r--r--   0        0        0     4280 2023-01-11 22:09:51.971819 anicli_api-0.3.8/README.MD
--rw-r--r--   0        0        0      297 2023-01-25 23:19:25.546656 anicli_api-0.3.8/anicli_api/__init__.py
--rw-r--r--   0        0        0     1544 2023-01-12 14:34:11.166425 anicli_api-0.3.8/anicli_api/__template_decoder__.py
--rw-r--r--   0        0        0     6713 2023-01-25 23:19:25.547656 anicli_api-0.3.8/anicli_api/__template_extractor__.py
--rw-r--r--   0        0        0     2790 2023-01-25 23:19:25.547656 anicli_api-0.3.8/anicli_api/_http.py
--rw-r--r--   0        0        0    16187 2023-01-30 08:44:18.702827 anicli_api-0.3.8/anicli_api/base.py
--rw-r--r--   0        0        0     4021 2023-01-12 14:34:11.167425 anicli_api-0.3.8/anicli_api/base_decoder.py
--rw-r--r--   0        0        0      520 2023-01-25 23:19:37.198751 anicli_api-0.3.8/anicli_api/decoders/__init__.py
--rw-r--r--   0        0        0     3086 2023-01-17 10:13:30.159217 anicli_api-0.3.8/anicli_api/decoders/aniboom.py
--rw-r--r--   0        0        0     1232 2023-01-12 14:34:11.168425 anicli_api-0.3.8/anicli_api/decoders/animejoy.py
--rw-r--r--   0        0        0     1500 2023-01-12 14:34:11.168425 anicli_api-0.3.8/anicli_api/decoders/csst.py
--rw-r--r--   0        0        0     1686 2023-01-12 14:34:11.168425 anicli_api-0.3.8/anicli_api/decoders/dzen.py
--rw-r--r--   0        0        0       84 2022-12-06 17:11:19.673846 anicli_api-0.3.8/anicli_api/decoders/exceptions.py
--rw-r--r--   0        0        0     4769 2022-12-06 17:11:19.674847 anicli_api-0.3.8/anicli_api/decoders/kodik.py
--rw-r--r--   0        0        0     1360 2023-01-12 14:34:11.168425 anicli_api-0.3.8/anicli_api/decoders/okru.py
--rw-r--r--   0        0        0     1227 2022-12-06 17:11:19.674847 anicli_api-0.3.8/anicli_api/decoders/sibnet.py
--rw-r--r--   0        0        0     1522 2023-01-12 14:34:11.169425 anicli_api-0.3.8/anicli_api/decoders/vkcom.py
--rw-r--r--   0        0        0     1666 2023-01-25 23:19:25.547656 anicli_api-0.3.8/anicli_api/decoders/yt_dlp_decoder.py
--rw-r--r--   0        0        0       42 2022-12-06 17:11:19.674847 anicli_api-0.3.8/anicli_api/extractors/__init__.py
--rw-r--r--   0        0        0     8737 2023-01-27 17:40:28.784899 anicli_api-0.3.8/anicli_api/extractors/anilibria.py
--rw-r--r--   0        0        0     8481 2023-01-25 23:19:38.038758 anicli_api-0.3.8/anicli_api/extractors/animania.py
--rw-r--r--   0        0        0    13223 2023-01-25 23:19:38.427761 anicli_api-0.3.8/anicli_api/extractors/animego.py
--rw-r--r--   0        0        0     9784 2023-01-25 23:19:25.549656 anicli_api-0.3.8/anicli_api/extractors/animejoy.py
--rw-r--r--   0        0        0     7500 2023-01-25 23:19:38.532762 anicli_api-0.3.8/anicli_api/extractors/animevost.py
--rw-r--r--   0        0        0     5799 2023-01-25 23:19:25.549656 anicli_api-0.3.8/anicli_api/loader.py
--rw-r--r--   0        0        0      670 2023-01-25 23:19:25.549656 anicli_api-0.3.8/anicli_api/logging_config.py
--rw-r--r--   0        0        0     9783 2022-12-06 17:11:19.675846 anicli_api-0.3.8/anicli_api/re_models.py
--rw-r--r--   0        0        0       58 2023-01-25 23:19:25.549656 anicli_api-0.3.8/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-06 17:11:19.675846 anicli_api-0.3.8/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0     2369 2023-01-30 08:45:33.760573 anicli_api-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5098 1970-01-01 00:00:00.000000 anicli_api-0.3.8/setup.py
--rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 anicli_api-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-14 13:28:38.026999 anicli_api-0.4.0/README.MD
+-rw-r--r--   0        0        0     2987 2023-05-14 10:56:27.746746 anicli_api-0.4.0/anicli_api/_http.py
+-rw-r--r--   0        0        0     1511 2023-05-14 12:55:53.852480 anicli_api-0.4.0/anicli_api/_logger.py
+-rw-r--r--   0        0        0     2474 2023-05-14 10:57:20.152356 anicli_api-0.4.0/anicli_api/base.py
+-rw-r--r--   0        0        0      482 2023-05-14 10:57:20.189357 anicli_api-0.4.0/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-14 08:49:09.675438 anicli_api-0.4.0/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2280 2023-05-14 10:43:11.345457 anicli_api-0.4.0/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1179 2023-05-14 08:42:33.397571 anicli_api-0.4.0/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3430 2023-05-14 10:42:29.255965 anicli_api-0.4.0/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1282 2023-05-14 08:42:33.398571 anicli_api-0.4.0/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1394 2023-05-14 10:44:03.105062 anicli_api-0.4.0/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     3930 2023-05-14 08:42:33.389571 anicli_api-0.4.0/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1875 2023-05-14 08:42:33.399571 anicli_api-0.4.0/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1290 2023-05-14 10:44:26.183332 anicli_api-0.4.0/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1089 2023-05-14 08:42:33.392571 anicli_api-0.4.0/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1256 2023-05-14 08:42:33.395571 anicli_api-0.4.0/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0     1254 2023-05-14 08:42:33.376571 anicli_api-0.4.0/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     5942 2023-05-14 12:54:38.982765 anicli_api-0.4.0/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0     9301 2023-05-14 12:37:34.938773 anicli_api-0.4.0/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8427 2023-05-14 12:37:34.892773 anicli_api-0.4.0/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5358 2023-05-14 12:54:38.962765 anicli_api-0.4.0/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0       58 2023-01-25 23:19:25.549656 anicli_api-0.4.0/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-06 17:11:19.675846 anicli_api-0.4.0/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0     2050 2023-05-14 13:28:49.200112 anicli_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 anicli_api-0.4.0/PKG-INFO
```

### Comparing `anicli_api-0.3.8/anicli_api/_http.py` & `anicli_api-0.4.0/anicli_api/_http.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,74 +2,78 @@
 This module contains httpx.Client and httpx.AsyncClient classes with the following settings:
 
 1. User-agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.114
 
 2. x-requested-with: XMLHttpRequest
 
 """
-import logging
+import ssl
 from typing import Dict
 
 from httpx import AsyncClient, Client, Response
 
-logger = logging.getLogger("anicli-api._http")
+from anicli_api._logger import logger
+
 HEADERS: Dict[str, str] = {
     "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) "
-    "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.114"
-    "Mobile Safari/537.36",
+    "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
     # XMLHttpRequest required
     "x-requested-with": "XMLHttpRequest",
 }
 # DDoS protection check by "Server" key header
 DDOS_SERVICES = ("cloudflare", "ddos-guard")
 
 __all__ = ("BaseHTTPSync", "BaseHTTPAsync", "HTTPSync", "HTTPAsync", "Singleton")
 
 
 class Singleton:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
-            cls._instance = super().__new__(cls, *args, **kwargs)
+            cls._instance = super().__new__(cls)
         return cls._instance
 
 
 class BaseHTTPSync(Client):
     """httpx.Client class with configured user agent and enabled redirects"""
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__(http2=True, **kwargs)
         self.headers.update(HEADERS)
         self.follow_redirects = True
 
 
 class BaseHTTPAsync(AsyncClient):
     """httpx.AsyncClient class with configured user agent and enabled redirects"""
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, http2: bool = True, **kwargs):
+        super().__init__(http2=http2, **kwargs)
         self.headers.update(HEADERS)
         self.follow_redirects = True
 
 
 def check_ddos_protect_hook(resp: Response):
     """
     Simple ddos protect check hook.
 
     If response return 403 code or server headers contains *cloudflare* or *ddos-guard* strings and
     **Connection = close,** throw ConnectionError traceback
     """
+    logger.debug(
+        "{} check DDOS protect :\nstatus [{}] {}", resp.url, resp.status_code, resp.headers
+    )
     if (
         resp.headers.get("Server") in DDOS_SERVICES
-        and resp.headers["Connection"] == "close"
+        and resp.headers.get("Connection", None) == "close"
         or resp.status_code == 403
     ):
+        logger.error("Ooops, {} have ddos protect :(", resp.url)
         raise ConnectionError(
-            f"{resp.url} have ddos protect {resp.headers.get('Server')} and return 403 code."
+            f"{resp.url} have '{resp.headers.get('Server', 'unknown')}' and return 403 code."
         )
 
 
 class HTTPSync(Singleton, BaseHTTPSync):
     """
     Base singleton **sync** HTTP class with recommended config.
```

### Comparing `anicli_api-0.3.8/anicli_api/base_decoder.py` & `anicli_api-0.4.0/anicli_api/player/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,114 @@
-"""
-Decoders class for video hostings
-
-Decoder structure:
-
-- class DecoderName(BaseDecoder) - base decoder structure.
-
-- URL_RULE - link validation regex.
-
-- def parse - List[MetaVideo]: synchronous video parser class method.
-
-- async def async_parse -> List[MetaVideo]: asynchronous video parser class method.
-
-
-Video Dataclass with reference values
-
-MetaVideo
-
-- type file type (m3u8, mpd, mp4...)
-
-- quality video quality, int (144,240,360,480,720,1080)
-
-- url video link
-
-- extra_headers - if the video stream does not work without them (like aniboom, sibnet) or set default value.
-"""
-
 import re
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
 from typing import Any, Dict, List, Literal, Optional, Union
 from urllib.parse import urlparse
 
 from anicli_api._http import BaseHTTPAsync, BaseHTTPSync
 
 ALL_QUALITIES = (144, 240, 360, 480, 720, 1080)
 
 
-@dataclass
-class MetaVideo:
+def url_validator(pattern: Union[str, re.Pattern]):
+    if isinstance(pattern, str):
+        pattern = re.compile(pattern)
+
+    def decorator(func):
+        def wrapper(_, url, **kwargs):
+            if not pattern.match(url):
+                raise TypeError(f"Uncorrected url for {_.__class__.__name__} player")
+            return func(_, url, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+class Video:
     """MetaVideo class contains direct link and information like type, quality
 
     - type - video format type (mp4, m3u8 or mpd)
 
     - quality - video quality [144, 240, 360, 480, 720, 1080]
 
     - url - direct video link
 
     - extra_headers - required UserAgent values for play or download this video. If not needed, default dict is empty
     """
 
-    type: Literal["mp4", "m3u8", "mpd", "audio", "webm"]
-    quality: Literal[0, 144, 240, 360, 480, 720, 1080]
-    url: str
-    extra_headers: Optional[Dict] = field(default_factory=dict)
+    def __init__(
+        self,
+        type: Literal["mp4", "m3u8", "mpd", "audio", "webm"],
+        quality: Literal[0, 144, 240, 360, 480, 720, 1080],
+        url: str,
+        headers: Optional[Dict[str, str]] = None,
+    ):
+        self.type = type
+        self.quality = quality
+        self.url = url
+        self.headers = headers or {}
 
     def dict(self) -> Dict[str, Any]:
-        return self.__dict__
+        return {
+            "type": self.type,
+            "quality": self.quality,
+            "url": self.url,
+            "headers": self.headers,
+        }
 
     def __str__(self):
         return f"{self.type} {self.quality} {urlparse(self.url).netloc}"
 
     def __hash__(self):
         return hash((self.type, self.quality, urlparse(self.url).netloc))
 
+    def __repr__(self):
+        return self.__str__()
+
     def __eq__(self, other):
-        if isinstance(other, MetaVideo):
+        if isinstance(other, Video):
             return hash(self) == hash(other)
         raise TypeError(f"MetaVideo object required, not {type(other)}")
 
 
-class ABCDecoder(ABC):
-    def __init__(self, **kwargs):
-        if kwargs:
-            self.http = BaseHTTPSync(**kwargs)
-            self.a_http = BaseHTTPAsync(**kwargs)
-        else:
-            self.http = BaseHTTPSync()
-            self.a_http = BaseHTTPAsync()
+class ABCVideoExtractor(ABC):
+    URL_RULE: Union[str, re.Pattern] = NotImplemented
+    DEFAULT_HTTP_CONFIG: Dict[str, Any] = {}
+
+    def __init__(self, **httpx_kwargs):
+        self.http = BaseHTTPSync(**self.DEFAULT_HTTP_CONFIG, **httpx_kwargs)
+        self.a_http = BaseHTTPAsync(**self.DEFAULT_HTTP_CONFIG, **httpx_kwargs)
 
-    @classmethod
     @abstractmethod
-    def parse(cls, url: str, **kwargs) -> List[MetaVideo]:
-        ...
+    def parse(self, url: str, **kwargs) -> List[Video]:
+        pass
 
-    @classmethod
     @abstractmethod
-    async def async_parse(cls, url: str, **kwargs) -> List[MetaVideo]:
-        ...
+    async def a_parse(self, url: str, **kwargs) -> List[Video]:
+        pass
 
     @classmethod
     @abstractmethod
     def _compare_url(cls, url: str) -> bool:
         ...
 
     def __eq__(self, other: str):  # type: ignore
         """compare class instance with url string"""
+        if not isinstance(other, str):
+            raise TypeError(f"{other} should be str not {type(other).__name__}")
         return self._compare_url(other)
 
 
-class BaseDecoder(ABCDecoder):
-    """Abstract decoder class
-
-    - URL_RULE - regular expression to validate link
-
-    - cls.parse - get videos synchronously
-
-    - cls.async_parse - get videos asynchronously
-    """
-
-    URL_RULE: Union[str, re.Pattern]
-
+class BaseVideoExtractor(ABCVideoExtractor, ABC):
     @classmethod
     def _validate_url(cls, url: str):
         if url != cls():
             raise TypeError(f"Incorrect decoder. {url} if not {cls.__class__.__name__}")
 
     @classmethod
-    @abstractmethod
-    def parse(cls, url: str, **kwargs) -> List[MetaVideo]:
-        """get video synchronously
-
-        :param url: video url
-        :param kwargs: optional params for httpx.Client instance
-        :return: List of MetaVideo dataclasses
-        """
-        ...
-
-    @classmethod
-    @abstractmethod
-    async def async_parse(cls, url: str, **kwargs) -> List[MetaVideo]:
-        """get video asynchronously
-
-        :param url: video url
-        :param kwargs: optional params for httpx.AsyncClient instance
-        :return: List of MetaVideo dataclasses
-        """
-        ...
-
-    @classmethod
     def _compare_url(cls, url: str) -> bool:
         """
         :param url: link
         :return: True, if link valid else False
         """
         return (
             bool(cls.URL_RULE.search(url))
```

### Comparing `anicli_api-0.3.8/anicli_api/extractors/anilibria.py` & `anicli_api-0.4.0/anicli_api/source/anilibria.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,29 @@
-"""
-TODO sort keys for objects
-"""
-from __future__ import annotations
-
-from typing import Any, AsyncGenerator, Generator, Optional, Protocol
-
-from anicli_api.base import *
-from anicli_api.base_decoder import MetaVideo
-
-__all__ = (
-    "Extractor",
-    "SearchResult",
-    "Ongoing",
-    "AnimeInfo",
-    "Episode",
-    "Video",
-    "TestCollections",
-)
-
-
-class SearchIterData(Protocol):
-    search: SearchResult
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
+from typing import Any, List, Optional
+from urllib.parse import urlsplit
 
-
-class OngoingIterData(Protocol):
-    search: Ongoing
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
+from anicli_api.base import (
+    BaseAnime,
+    BaseEpisode,
+    BaseExtractor,
+    BaseOngoing,
+    BaseSearch,
+    BaseSource,
+    MainSchema,
+)
+from anicli_api.player.base import Video
 
 
 class Anilibria:
-    """For details see docs on https://github.com/anilibria/docs/blob/master/api_v2.md"""
+    """Dummmy API interface
+    https://github.com/anilibria/docs/blob/master/api_v2.md
+    """
 
-    HTTP = BaseAnimeExtractor.HTTP
-    HTTP_ASYNC = BaseAnimeExtractor.HTTP_ASYNC
+    HTTP = BaseExtractor.HTTP
+    HTTP_ASYNC = BaseExtractor.HTTP_ASYNC
 
     BASE_URL = "https://api.anilibria.tv/v2/"
 
     def api_request(self, method: str = "GET", *, api_method: str, **kwargs) -> dict:
         response = self.HTTP().request(method=method, url=f"{self.BASE_URL}{api_method}", **kwargs)
         return response.json()
 
@@ -74,46 +56,36 @@
         return self.api_request(api_method="getUpdates", data=params, **kwargs)
 
     async def a_get_updates(self, *, limit: int = -1, **kwargs) -> dict:
         params = self._kwargs_pop_params(kwargs, limit=limit)
         return await self.a_api_request(api_method="getUpdates", data=params, **kwargs)
 
 
-class Extractor(BaseAnimeExtractor):
-    # optional constants, HTTP configuration here
-    """For details see docs on https://github.com/anilibria/docs/blob/master/api_v2.md"""
-    BASE_URL = "https://api.anilibria.tv/v2/"
-    ANILIBRIA = Anilibria()
-
-    def async_walk_search(self, query: str) -> AsyncGenerator[SearchIterData, None]:
-        return super().async_walk_search(query)
-
-    def async_walk_ongoing(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().async_walk_ongoing()
-
-    def walk_search(self, query: str) -> Generator[SearchIterData, None, None]:
-        return super().walk_search(query)
-
-    def walk_ongoing(self) -> Generator[OngoingIterData, None, None]:
-        return super().walk_ongoing()
-
-    def search(self, query: str) -> List["SearchResult"]:
-        return [SearchResult(**kw) for kw in self.ANILIBRIA.search_titles(search=query)]
+class Extractor(BaseExtractor):
+    BASE_URL = ""  # BASEURL
+    API = Anilibria()
+
+    def search(self, query: str) -> List["Search"]:
+        # search entrypoint
+        return [Search.from_kwargs(**kw) for kw in self.API.search_titles(search=query)]
+
+    async def a_search(self, query: str) -> List["Search"]:
+        # async search entrypoint
+        return [Search.from_kwargs(**kw) for kw in (await self.API.a_search_titles(search=query))]
 
     def ongoing(self) -> List["Ongoing"]:
-        return [Ongoing(**kw) for kw in self.ANILIBRIA.get_updates()]
-
-    async def async_search(self, query: str) -> List["SearchResult"]:
-        return [SearchResult(**kw) for kw in (await self.ANILIBRIA.a_search_titles(search=query))]
+        # ongoing entrypoint
+        return [Ongoing.from_kwargs(**kw) for kw in self.API.get_updates()]
 
-    async def async_ongoing(self) -> List["Ongoing"]:
-        return [Ongoing(**kw) for kw in (await self.ANILIBRIA.a_get_updates())]
+    async def a_ongoing(self) -> List["Ongoing"]:
+        # async ongoing entrypoint
+        return [Ongoing.from_kwargs(**kw) for kw in (await self.API.a_get_updates())]
 
 
-class SResult(BaseModel):
+class _SearchOrOngoing(MainSchema):
     id: int
     code: str
     names: dict
     announce: Optional[Any]
     status: dict
     posters: dict
     updated: int
@@ -124,42 +96,33 @@
     season: dict
     description: str
     in_favorites: int
     blocked: dict
     player: dict
     torrents: dict
 
-    async def a_get_anime(self) -> "AnimeInfo":
-        return AnimeInfo(**self.dict())
+    async def a_get_anime(self) -> "Anime":
+        return self.get_anime()
 
-    def get_anime(self) -> "AnimeInfo":
-        return AnimeInfo(**self.dict())
+    def get_anime(self) -> "Anime":
+        return Anime.from_kwargs(**self.dict())
 
     def __str__(self):
         return f"{list(self.names.values())[0]}"
 
 
-class SearchResult(SResult, BaseSearchResult):
-    def __iter__(self) -> Generator[SearchIterData, None, None]:
-        return super().__iter__()
+class Search(_SearchOrOngoing, BaseSearch):
+    pass
 
-    def __aiter__(self) -> AsyncGenerator[SearchIterData, None]:
-        return super().__aiter__()
 
+class Ongoing(_SearchOrOngoing, BaseOngoing):
+    pass
 
-class Ongoing(SResult, BaseOngoing):
-    def __iter__(self) -> Generator[OngoingIterData, None, None]:
-        return super().__iter__()
 
-    def __aiter__(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().__aiter__()
-
-
-class AnimeInfo(BaseAnimeInfo):
-    # TODO typing keys better
+class Anime(BaseAnime):
     id: int
     code: str
     names: dict
     announce: Optional[Any]
     status: dict
     posters: dict
     updated: int
@@ -170,118 +133,75 @@
     season: dict
     description: str
     in_favorites: int
     blocked: dict
     player: dict
     torrents: dict
 
-    async def a_get_episodes(self) -> List["Episode"]:
-        return [
-            Episode(
-                alternative_player=self.player["alternative_player"],
-                host=self.player["host"],
-                torrents=self.torrents["list"],
-                **p,
-            )
-            for p in self.player["playlist"].values()
-        ]
+    def __str__(self):
+        return f"{list(self.names.values())}"
 
     def get_episodes(self) -> List["Episode"]:
         return [
-            Episode(
+            Episode.from_kwargs(
                 alternative_player=self.player["alternative_player"],
                 host=self.player["host"],
                 torrents=self.torrents["list"],
                 **p,
             )
             for p in self.player["playlist"].values()
         ]
 
-    def __str__(self):
-        return f"{list(self.names.values())[0]}\n{self.genres}\n{self.description}"
+    async def a_get_episodes(self) -> List["Episode"]:
+        return self.get_episodes()
 
 
 class Episode(BaseEpisode):
     alternative_player: Optional[str]
     host: str
     serie: int
     created_timestamp: int
     preview: Optional[Any]
     skips: dict
     hls: dict
     torrents: dict
 
-    async def a_get_videos(self) -> List["Video"]:
-        return [
-            Video(
-                torrents=self.torrents,
-                # dirty hack for success url validate for decoder.anilibria :D
-                url=self.hls["sd"],
-                **{k: f"https://{self.host}{v}" if v else None for k, v in self.hls.items()},
-            )
-        ]
+    def __str__(self):
+        return f"{self.host} {self.serie}"
 
-    def get_videos(self) -> List["Video"]:
+    def get_sources(self) -> List["Source"]:
         return [
-            Video(
+            Source.from_kwargs(
                 torrents=self.torrents,
                 # dirty hack for success url validate for decoder.anilibria :D
                 url=self.hls["sd"],
                 **{k: f"https://{self.host}{v}" if v else None for k, v in self.hls.items()},
             )
         ]
 
-    def __str__(self):
-        return f"{self.serie} episode"
+    async def a_get_sources(self) -> List["Source"]:
+        return self.get_sources()
 
 
-class Video(BaseVideo):
+class Source(BaseSource):
     torrents: dict
     fhd: Optional[str]
     hd: str
     sd: str
 
-    def _source(self) -> List[MetaVideo]:
+    def __str__(self):
+        return f"{urlsplit(self.fhd).netloc or urlsplit(self.hd).netloc}"
+
+    def get_videos(self) -> List["Video"]:
         if self.fhd:
             return [
-                MetaVideo(type="m3u8", quality=480, url=self.sd),
-                MetaVideo(type="m3u8", quality=720, url=self.hd),
-                MetaVideo(type="m3u8", quality=1080, url=self.fhd),
+                Video(type="m3u8", quality=480, url=self.sd),
+                Video(type="m3u8", quality=720, url=self.hd),
+                Video(type="m3u8", quality=1080, url=self.fhd),
             ]
         return [
-            MetaVideo(type="m3u8", quality=480, url=self.sd),
-            MetaVideo(type="m3u8", quality=720, url=self.hd),
+            Video(type="m3u8", quality=480, url=self.sd),
+            Video(type="m3u8", quality=720, url=self.hd),
         ]
 
-    def get_source(self) -> List[MetaVideo]:
-        return self._source()
-
-    async def a_get_source(self) -> List[MetaVideo]:
-        return self._source()
-
-    def __hash__(self):
-        return hash(tuple(self.get_source()))
-
-
-class TestCollections(BaseTestCollections):
-    def test_search(self):
-        resp = Extractor().search("Зомбиленд")
-        assert resp[0].id == 7474
-        assert resp[1].id == 8960
-
-    def test_ongoing(self):
-        resp = Extractor().ongoing()
-        assert len(resp) > 1
-
-    def test_extract_metadata(self):
-        for meta in Extractor().search("Зомбиленд")[0]:
-            assert meta.search.id == 7474
-            assert meta.search.code == "zombieland-saga"
-            assert meta.search.genres == ["Комедия", "Сверхъестественное", "Ужасы", "Экшен"]
-            break
-
-    def test_extract_video(self):
-        search = Extractor().search("Зомбиленд")[0]
-        anime = search.get_anime()
-        episodes = anime.get_episodes()
-        video = episodes[0].get_videos()[0]
-        assert "libria.fun" in video.get_source()[0].url
+    async def a_get_videos(self) -> List["Video"]:
+        return self.get_videos()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anicli_api-0.3.8/anicli_api/extractors/animania.py` & `anicli_api-0.4.0/anicli_api/source/animejoy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,256 +1,235 @@
-"""Animania Extractor"""
-from __future__ import annotations
+from typing import Dict, List, TypedDict
+from urllib.parse import urlsplit
 
-from typing import AsyncGenerator, Dict, Generator, Protocol
-
-from anicli_api.base import *
-
-__all__ = (
-    "Extractor",
-    "SearchResult",
-    "Ongoing",
-    "AnimeInfo",
-    "Episode",
-    "Video",
-    "TestCollections",
+from parsel import Selector
+from scrape_schema import ScField
+from scrape_schema.callbacks.parsel import crop_by_xpath_all as cbxa
+from scrape_schema.callbacks.parsel import get_attr, get_text
+from scrape_schema.fields.parsel import ParselXPath, ParselXPathList
+
+from anicli_api.base import (
+    BaseAnime,
+    BaseEpisode,
+    BaseExtractor,
+    BaseOngoing,
+    BaseSearch,
+    BaseSource,
 )
 
+_SourceDict = TypedDict("_SourceDict", {"player_id": str, "url": str, "name": str})
 
-class SearchIterData(Protocol):
-    search: SearchResult
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
-
-
-class OngoingIterData(Protocol):
-    search: Ongoing
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
-
-
-class Extractor(BaseAnimeExtractor):
-    BASE_URL = "https://animania.online"
-
-    def async_walk_search(self, query: str) -> AsyncGenerator[SearchIterData, None]:
-        return super().async_walk_search(query)
-
-    def walk_search(self, query: str) -> Generator[SearchIterData, None, None]:
-        return super().walk_search(query)
-
-    def async_walk_ongoing(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().async_walk_ongoing()
-
-    def walk_ongoing(self) -> Generator[OngoingIterData, None, None]:
-        return super().walk_ongoing()
-
-    def _search_parse(self, markup: str) -> List["SearchResult"]:
-        soup = self._soup(markup)
-        lst = []
-        for article in soup.find("div", class_="floats clearfix").find_all(
-            "article", attrs={"class": "short clearfix", "id": "short"}
-        ):
-            for tc_item, short_poster in zip(
-                article.find_all("a", class_="tc-item"),
-                article.find_all("a", attrs={"class": "short-poster img-box"}),
-            ):
-                data = {
-                    "url": tc_item["href"],
-                    "title": tc_item.find("div", class_="tc-title").get_text(strip=True),
-                    "poster": "https://animania.online" + short_poster.find("img")["src"],
-                }
-                lst.append(SearchResult(**data))
-        return lst
 
-    def search(self, query: str) -> List["SearchResult"]:
+class Extractor(BaseExtractor):
+    BASE_URL = "https://animejoy.ru"
+
+    def search(self, query: str) -> List["Search"]:
+        # search entrypoint
         response = (
             self.HTTP()
-            .get(
-                f"{self.BASE_URL}/index.php",
-                params={"do": "search", "subaction": "search", "story": query},
+            .post(
+                self.BASE_URL,
+                data={"story": query, "do": "search", "subaction": "search"},
             )
             .text
         )
-        return self._search_parse(response)
-
-    def _ongoing_parse(self, response: str):
-        divs_ksupdate = self._soup(response).find_all(
-            "div", class_="ksupdate_block_list_item_inner"
+        return Search.from_crop_rule_list(
+            response,
+            crop_rule=cbxa('//*[@id="dle-content"]/article[@class="block story shortstory"]'),
         )
-        ongs = []
-        for div in divs_ksupdate:
-            ksupdate_block = div.find("a", class_="ksupdate_block_list_link")
-            data = {
-                "url": "https://animania.online" + ksupdate_block["href"],
-                "name": ksupdate_block.get_text(strip=True),
-                "info": div.find("span").get_text(strip=True),
-            }
-            ongs.append(Ongoing(**data))
-        return ongs
 
-    def ongoing(self) -> List["Ongoing"]:
-        response = self.HTTP().get(f"{self.BASE_URL}/index.php")
-        return self._ongoing_parse(response.text)
+    async def a_search(self, query: str) -> List["Search"]:
+        async with self.HTTP_ASYNC() as client:
+            response = await client.post(
+                self.BASE_URL, data={"story": query, "do": "search", "subaction": "search"}
+            )
+            return Search.from_crop_rule_list(
+                response,
+                crop_rule=cbxa('//*[@id="dle-content"]/article[@class="block story shortstory"]'),
+            )
 
-    async def async_search(self, query: str) -> List["SearchResult"]:
-        async with self.HTTP_ASYNC() as session:
-            response = (
-                await session.get(
-                    f"{self.BASE_URL}/index.php",
-                    params={"do": "search", "subaction": "search", "story": query},
-                )
-            ).text
-            return self._search_parse(response)
+    def ongoing(self) -> List["Ongoing"]:
+        # ongoing entrypoint
+        response = self.HTTP().get(self.BASE_URL).text
+        return Ongoing.from_crop_rule_list(
+            response, crop_rule=cbxa('//div[@id="dle-content"]/article')
+        )
 
-    async def async_ongoing(self) -> List["Ongoing"]:
-        async with self.HTTP_ASYNC() as session:
-            response = await session.get(f"{self.BASE_URL}/index.php")
-            return self._ongoing_parse(response.text)
+    async def a_ongoing(self) -> List["Ongoing"]:
+        async with self.HTTP_ASYNC() as client:
+            response = await client.get(self.BASE_URL)
+            return Ongoing.from_crop_rule_list(
+                response.text, crop_rule=cbxa('//div[@id="dle-content"]/article')
+            )
 
 
-class AnimeInfoParser(BaseModel):
-    url: str
+class Search(BaseSearch):
+    url: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a', callback=get_attr("href"))]
+    title: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a')]
+    alt_name: ScField[
+        str, ParselXPath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]')
+    ]
+    _thumbnail_path: ScField[str, ParselXPath('//div[@class="text"]/picture/img')]
+    _metadata: ScField[
+        List[str],
+        ParselXPathList(
+            '//div[@class="blkdesc"]/p[@class="zerop"]', callback=get_text(strip=True, deep=True)
+        ),
+    ]
+    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+
+    def get_anime(self) -> "Anime":
+        response = self.HTTP().get(self.url).text
+        return Anime(response)
+
+    async def a_get_anime(self) -> "Anime":
+        async with self.HTTP_ASYNC() as client:
+            response = await client.get(self.url)
+            return Anime(response.text)
 
-    def _parse_meta(self, response: str) -> "AnimeInfo":
-        soup = self._soup(response)
-        info = soup.find("div", class_="fmright")
-        meta_data = {
-            "poster": "https://animania.online"
-            + soup.find("div", class_="fmid")
-            .find("div", attrs={"class": "fposterik-l"})
-            .find("img")["data-src"],
-            "title": info.find("div", attrs={"class": "fdesc-title"}).get_text(),
-            "description": info.find(
-                "div", attrs={"class": "fdesc slice-this ficon clearfix"}
-            ).get_text(strip=True),
-            "meta": [
-                li.get_text(strip=True)
-                for li in info.find("div", class_="flist clearfix").find_all("li")
-            ],
-        }
-        # dubs_meta
-        dubs_id_table = {
-            int(
-                span["onclick"].replace("kodikSlider.season('", "").replace("', this)", "")
-            ): span.get_text()
-            for span in soup.find("div", id="ks-translations").find_all("span")
-        }
-
-        # video
-        # episodes = {name: [{id: 0, video, dub}, ...], ...}
-        episodes: dict[str, list[dict]] = {}
-        for ul in soup.find("ul", id="ks-episodes"):
-            for span in ul.find_all("span"):
-                data = {
-                    "id": int(ul["id"].replace("season", "")),
-                    "name": span.get_text(strip=True),
-                    "url": "https:"
-                    + span["onclick"].replace("kodikSlider.player('", "").replace("', this);", ""),
-                }
-                data["dub"] = dubs_id_table.get(data["id"])
-                if episodes.get(data["name"]):
-                    episodes[data["name"]].append(data)
-                else:
-                    episodes[data["name"]] = [data]
-        return AnimeInfo(**meta_data, _episodes=episodes)
-
-    def get_anime(self) -> "AnimeInfo":
-        response = self._HTTP().get(self.url).text
-        return self._parse_meta(response)
-
-    async def a_get_anime(self) -> "AnimeInfo":
-        async with self._HTTP_ASYNC() as session:
-            response = (await session.get(self.url)).text
-            return self._parse_meta(response)
-
-
-class SearchResult(AnimeInfoParser, BaseSearchResult):
-    title: str
-    poster: str
+    def __str__(self):
+        return f"{self.title} ({self.alt_name})"
 
-    def __iter__(self) -> Generator[SearchIterData, None, None]:
-        return super().__iter__()
 
-    def __aiter__(self) -> AsyncGenerator[SearchIterData, None]:
-        return super().__aiter__()
+class Ongoing(BaseOngoing):
+    url: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a', callback=get_attr("href"))]
+    title: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a')]
+    alt_name: ScField[
+        str, ParselXPath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]')
+    ]
+    _thumbnail_path: ScField[str, ParselXPath('//div[@class="text"]/picture/img', callback=get_attr('src'))]
+    _metadata: ScField[
+        List[str],
+        ParselXPathList(
+            '//div[@class="blkdesc"]/p[@class="zerop"]', callback=get_text(strip=True, deep=True)
+        ),
+    ]
+    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+
+    def get_anime(self) -> "Anime":
+        response = self.HTTP().get(self.url)
+        return Anime(response)
+
+    async def a_get_anime(self) -> "Anime":
+        async with self.HTTP_ASYNC() as client:
+            response = await client.get(self.url)
+            return Anime(response)
 
     def __str__(self):
-        return f"{self.title}"
-
+        return f"{self.title} ({self.alt_name})"
 
-class Ongoing(AnimeInfoParser, BaseOngoing):
-    name: str
-    info: str
 
-    def __iter__(self) -> Generator[OngoingIterData, None, None]:
-        return super().__iter__()
-
-    def __aiter__(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().__aiter__()
+class Anime(BaseAnime):
+    title: ScField[str, ParselXPath('//h1[@class="h2 ntitle"]')]
+    alt_name: ScField[str, ParselXPath('//h2[@class="romanji"]')]
+    _thumbnail_path: ScField[str, ParselXPath('//div[@class="text"]/picture/img', callback=get_attr('src'))]
+    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+    _metadata: ScField[List[str], ParselXPathList('//div[@class="blkdesc"]/p[@class="zerop"]')]
+    description: ScField[
+        str, ParselXPath('//div[@class="pcdescrf"]', callback=get_text(deep=True))
+    ]
+    screenshots: ScField[
+        List[str],
+        ParselXPathList('//div[@class="photo-row clearfix"]/a', callback=get_attr("href")),
+    ]
+    url: ScField[str, ParselXPath('//meta[@property="og:url"]', callback=get_attr("content"))]
+    news_id = property(lambda self: self.url.split("/")[-1].split("-")[0])
 
     def __str__(self):
-        return f"{self.name}"
-
+        return f"{self.title} ({self.alt_name})"
 
-class AnimeInfo(BaseAnimeInfo):
-    title: str
-    description: str
-    meta: str
-    _episodes: Dict[str, List[Dict]]
-
-    async def a_get_episodes(self) -> List["Episode"]:
-        return [Episode(name=name, _video_meta=meta) for name, meta in self._episodes.items()]
+    def _extract_episode_meta(self, response: str) -> List["Episode"]:
+        sel = Selector(response)
+        # get player ids and names for better output
+        players_ids = sel.xpath(
+            '//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/@data-id'
+        ).getall()
+        players_names = sel.xpath(
+            '//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/text()'
+        ).getall()
+        players_table = dict(zip(players_ids, players_names))
+
+        # extract episodes names, video urls, and player ids
+        series_names = sel.xpath(
+            '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/text()'
+        ).getall()
+        series_urls = sel.xpath(
+            '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/@data-file'
+        ).getall()
+        series_player_id = sel.xpath(
+            '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/@data-id'
+        ).getall()
+        episodes_dict: Dict[str, List[Dict[str, str]]] = {}
+        for name, url, player_id in zip(series_names, series_urls, series_player_id):
+            if not episodes_dict.get(name):
+                episodes_dict[name] = []
+            if url.startswith("//"):
+                url = f"https:{url}"
+
+            episodes_dict[name].append(
+                {
+                    "url": url,
+                    "name": players_table.get(player_id, "unknown"),
+                    "player_id": player_id,
+                }
+            )
+        return [
+            Episode.from_kwargs(name=name, _video_meta=video_meta)
+            for name, video_meta in episodes_dict.items()
+        ]
 
     def get_episodes(self) -> List["Episode"]:
-        return [Episode(name=name, _video_meta=meta) for name, meta in self._episodes.items()]
+        response = (
+            self.HTTP()
+            .get(
+                "https://animejoy.ru/engine/ajax/playlists.php",
+                params={"news_id": self.news_id, "xfield": "playlist"},
+            )
+            .json()["response"]
+        )
+        return self._extract_episode_meta(response)
 
-    def __str__(self):
-        return f"{self.title}\n{self.description}"
+    async def a_get_episodes(self) -> List["Episode"]:
+        async with self.HTTP_ASYNC() as client:
+            response = (
+                await client.get(
+                    "https://animejoy.ru/engine/ajax/playlists.php",
+                    params={"news_id": self.news_id, "xfield": "playlist"},
+                )
+            ).json()["response"]
+            return self._extract_episode_meta(response)
 
 
 class Episode(BaseEpisode):
+    _video_meta: List[_SourceDict]
     name: str
-    _video_meta: List[Dict]
-
-    async def a_get_videos(self) -> List["Video"]:
-        return [Video(**meta) for meta in self._video_meta]
-
-    def get_videos(self) -> List["Video"]:
-        return [Video(**meta) for meta in self._video_meta]
 
     def __str__(self):
         return self.name
 
+    def get_sources(self) -> List["Source"]:
+        return [
+            Source.from_kwargs(url=meta["url"], name=meta["name"], player_id=meta["player_id"])
+            for meta in self._video_meta
+        ]
+
+    async def a_get_sources(self) -> List["Source"]:
+        return self.get_sources()
 
-class Video(BaseVideo):
-    id: int
+
+class Source(BaseSource):
+    url: str
     name: str
-    dub: str
-    __CMP_KEYS__ = ("dub",)
+    player_id: str
 
+    def __str__(self):
+        return f"{urlsplit(self.url).netloc} ({self.name})"
 
-class TestCollections(BaseTestCollections):
-    def test_search(self):
-        result = Extractor().search("serial experiments lain")
-        res = result[0].get_anime().dict()
-        assert res.get("poster")
-        assert "Эксперименты Лэйн" in res.get("title")
-
-    def test_ongoing(self):
-        assert len(Extractor().ongoing()) > 1
-
-    def test_extract_metadata(self):
-        for meta in Extractor().search("serial experiments lain")[0]:
-            assert (
-                meta.search.url
-                == "https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html"
-            )
-            assert meta.anime.title == 'Сюжет аниме "Эксперименты Лэйн":'
-            assert meta.episode.name == "1 серия"
-            break
-
-    def test_extract_video(self):
-        for meta in Extractor().search("serial experiments lain")[0]:
-            assert "kodik" in meta.video.url
-            assert meta.video.get_source()[0].url.endswith(".m3u8")
+
+if __name__ == "__main__":
+    ex = Extractor()
+    res = ex.search("lai")
+    an = res[0].get_anime()
+    eps = an.get_episodes()
+    vids = eps[0].get_sources()
+    print(*[v.raw_dict() for v in vids], sep="\n")
+    print(vids[1].get_videos())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anicli_api-0.3.8/anicli_api/extractors/animevost.py` & `anicli_api-0.4.0/anicli_api/source/animevost.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-"""Animevost extractor"""
-from __future__ import annotations
+from typing import Dict, List, Union
 
-from typing import AsyncGenerator, Generator, Protocol, Union
-
-from anicli_api.base import *
-
-__all__ = (
-    "Extractor",
-    "SearchResult",
-    "Ongoing",
-    "AnimeInfo",
-    "Episode",
-    "Video",
-    "TestCollections",
+from anicli_api.base import (
+    BaseAnime,
+    BaseEpisode,
+    BaseExtractor,
+    BaseOngoing,
+    BaseSearch,
+    BaseSource,
+    MainSchema,
 )
-
-from anicli_api.base_decoder import MetaVideo
-
-
-class SearchIterData(Protocol):
-    search: SearchResult
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
-
-
-class OngoingIterData(Protocol):
-    search: Ongoing
-    anime: AnimeInfo
-    episode: Episode
-    video: Video
+from anicli_api.player.base import Video
 
 
 class VostAPI:
-    HTTP = BaseAnimeExtractor.HTTP
-    HTTP_ASYNC = BaseAnimeExtractor.HTTP_ASYNC
+    """dummy animevost API implementation"""
 
+    HTTP = BaseExtractor.HTTP
+    HTTP_ASYNC = BaseExtractor.HTTP_ASYNC
     BASE_URL = "https://api.animevost.org/v1/"
 
-    def api_request(self, method: str, *, api_method: str, **kwargs) -> Union[dict, list[dict]]:
+    def api_request(self, method: str, *, api_method: str, **kwargs) -> Union[Dict, List[Dict]]:
         response = self.HTTP().request(method, self.BASE_URL + api_method, **kwargs)
         return response.json()
 
     async def a_api_request(
         self, method: str, *, api_method: str, **kwargs
-    ) -> Union[dict, list[dict]]:
+    ) -> Union[Dict, List[Dict]]:
         async with self.HTTP_ASYNC() as session:
             response = await session.request(method, self.BASE_URL + api_method, **kwargs)
             return response.json()
 
     @staticmethod
     def _kwargs_pop_params(kwargs, **params) -> dict:
         data = kwargs.pop("params") if kwargs.get("params") else {}
@@ -67,179 +48,134 @@
         params = self._kwargs_pop_params(kwargs, page=1, quantity=limit)
         return self.api_request("GET", api_method="last", params=params, **kwargs)  # type: ignore
 
     async def a_last(self, *, limit: int = 20, **kwargs) -> dict:
         params = self._kwargs_pop_params(kwargs, page=1, quantity=limit)
         return await self.a_api_request("GET", api_method="last", params=params, **kwargs)  # type: ignore
 
-    def playlist(self, id: int) -> list[dict]:
+    def playlist(self, id: int) -> List[Dict]:
         return self.api_request("POST", api_method="playlist", data={"id": id})  # type: ignore
 
-    async def a_playlist(self, id: int) -> list[dict]:
+    async def a_playlist(self, id: int) -> List[Dict]:
         return await self.a_api_request("POST", api_method="playlist", data={"id": id})  # type: ignore
 
 
-class Extractor(BaseAnimeExtractor):
-    def async_walk_search(self, query: str) -> AsyncGenerator[SearchIterData, None]:
-        return super().async_walk_search(query)
-
-    def walk_search(self, query: str) -> Generator[SearchIterData, None, None]:
-        return super().walk_search(query)
-
-    def async_walk_ongoing(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().async_walk_ongoing()
+class Extractor(BaseExtractor):
+    API = VostAPI()
 
-    def walk_ongoing(self) -> Generator[OngoingIterData, None, None]:
-        return super().walk_ongoing()
+    def search(self, query: str) -> List["Search"]:
+        # search entrypoint
+        return [Search.from_kwargs(**kw) for kw in VostAPI().search(query)["data"]]
 
-    def search(self, query: str) -> List[SearchResult]:
-        # past code here
-        response = VostAPI().search(query)
-        return [SearchResult(**kw) for kw in response["data"]]
+    async def a_search(self, query: str) -> List["Search"]:
+        # async search entrypoint
+        return [Search.from_kwargs(**kw) for kw in (await VostAPI().a_search(query))["data"]]
 
-    def ongoing(self) -> List[Ongoing]:
-        response = VostAPI().last()
-        return [Ongoing(**kw) for kw in response["data"]]
+    def ongoing(self) -> List["Ongoing"]:
+        # ongoing entrypoint
+        return [Ongoing.from_kwargs(**kw) for kw in VostAPI().last()["data"]]
 
-    async def async_search(self, query: str) -> List[SearchResult]:
-        # past async code here
-        response = await VostAPI().a_search(query)
-        return [SearchResult(**kw) for kw in response["data"]]
+    async def a_ongoing(self) -> List["Ongoing"]:
+        # async ongoing entrypoint
+        return [Ongoing.from_kwargs(**kw) for kw in (await VostAPI().a_last())["data"]]
 
-    async def async_ongoing(self) -> List[Ongoing]:
-        response = await VostAPI().a_last()
-        return [Ongoing(**kw) for kw in response["data"]]
 
-
-class SResult(BaseModel):
+class _SearchOrOngoing(MainSchema):
     # TODO add convert camel case to snake case
     id: int
     title: str
     description: str
     genre: str
     year: str
     urlImagePreview: str
-    screenImage: list[str]
+    screenImage: List[str]
     isFavorite: int
     isLikes: int
     rating: int
     votes: int
     timer: int
     type: str
     director: str
     series: str  # '{\'1 серия\':\'147459278\ ...'
 
-    async def a_get_anime(self) -> "AnimeInfo":
-        # past async code here
-        response = await VostAPI().a_playlist(self.id)
-        return AnimeInfo(**self.dict(), playlist=response)
-
-    def get_anime(self) -> "AnimeInfo":
-        response = VostAPI().playlist(self.id)
-        return AnimeInfo(**self.dict(), playlist=response)
-
     def __str__(self):
-        return f"{self.title}"
+        return f"{self.title} {self.year} ({self.rating}) {self.type}"
 
+    def get_anime(self) -> "Anime":
+        response = VostAPI().playlist(self.id)
+        return Anime.from_kwargs(**self.dict(), playlist=response)
 
-class SearchResult(SResult, BaseSearchResult):
-    def __iter__(self) -> Generator[SearchIterData, None, None]:
-        return super().__iter__()
+    async def a_get_anime(self) -> "Anime":
+        response = await VostAPI().a_playlist(self.id)
+        return Anime.from_kwargs(**self.dict(), playlist=response)
 
-    def __aiter__(self) -> AsyncGenerator[SearchIterData, None]:
-        return super().__aiter__()
 
+class Search(_SearchOrOngoing, BaseSearch):
+    pass
 
-class Ongoing(SResult, BaseOngoing):
-    def __iter__(self) -> Generator[OngoingIterData, None, None]:
-        return super().__iter__()
 
-    def __aiter__(self) -> AsyncGenerator[OngoingIterData, None]:
-        return super().__aiter__()
+class Ongoing(_SearchOrOngoing, BaseOngoing):
+    pass
 
 
-class AnimeInfo(BaseAnimeInfo):
+class Anime(BaseAnime):
     id: int
     title: str
     description: str
     genre: str
     year: str
     urlImagePreview: str
-    screenImage: list[str]
+    screenImage: List[str]
     isFavorite: int
     isLikes: int
     rating: int
     votes: int
     timer: int
     type: str
     director: str
     series: str  # '{\'1 серия\':\'147459278\ ...'
-    playlist: list[dict]
+    playlist: List[Dict]
+
+    def __str__(self):
+        return f"{self.title} [{self.year}] {self.type} {self.rating}"
 
     async def a_get_episodes(self) -> List["Episode"]:
-        return [Episode(**kw) for kw in self.playlist]
+        return self.get_episodes()
 
     def get_episodes(self) -> List["Episode"]:
-        return [Episode(**kw) for kw in self.playlist]
+        return [Episode.from_kwargs(**kw) for kw in self.playlist]
 
-    def __str__(self):
-        return f"{self.title} {self.year} {self.rating}\n{self.genre}\n{self.description}"
 
 
 class Episode(BaseEpisode):
     name: str
     preview: str
 
     # video meta
     hd: str
     std: str
 
-    async def a_get_videos(self) -> List["Video"]:
-        return [Video(hd=self.hd, std=self.std)]
+    async def a_get_sources(self) -> List["Source"]:
+        return self.get_sources()
 
-    def get_videos(self) -> List["Video"]:
-        return [Video(hd=self.hd, std=self.std)]
+    def get_sources(self) -> List["Source"]:
+        return [Source.from_kwargs(hd=self.hd, std=self.std)]
 
     def __str__(self):
         return f"{self.name}"
 
 
-class Video(BaseVideo):
+class Source(BaseSource):
     hd: str
     std: str
 
-    def get_source(self) -> List[MetaVideo]:
-        return [
-            MetaVideo(type="mp4", quality=480, url=self.std),
-            MetaVideo(type="mp4", quality=720, url=self.hd),
-        ]
+    def __str__(self):
+        return "Animevost"
 
-    async def a_get_source(self) -> List[MetaVideo]:
+    def get_videos(self) -> List[Video]:
         return [
-            MetaVideo(type="mp4", quality=480, url=self.std),
-            MetaVideo(type="mp4", quality=720, url=self.hd),
+            Video(type="mp4", quality=480, url=self.std),
+            Video(type="mp4", quality=720, url=self.hd),
         ]
 
-
-class TestCollections(BaseTestCollections):
-    def test_search(self):
-        # rewrite testcase search here
-        result = Extractor().search("serial experiments lain")
-        assert result[0].get_anime().id == 558
-
-    def test_ongoing(self):
-        # test get ongoing
-        assert len(Extractor().ongoing()) > 1
-
-    def test_extract_metadata(self):
-        # rewrite testcase get metadata here
-        for meta in Extractor().search("serial experiments lain")[0]:
-            # past metadata dict here
-            assert meta.search.id == 558
-            assert meta.anime.id == 558
-            assert meta.episode.name == "1 серия"
-            break
-
-    def test_extract_video(self):
-        # rewrite testcase extract video here
-        for meta in Extractor().search("serial experiments lain")[0]:
-            assert meta.video.get_source()[0].url.endswith(".mp4")
+    async def a_get_videos(self) -> List[Video]:
+        return self.get_videos()
```

### Comparing `anicli_api-0.3.8/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.0/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.3.8/pyproject.toml` & `anicli_api-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.3.8"
+version = "0.4.0"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
@@ -25,71 +25,68 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed"
 ]
 
-
-
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vypivshiy/anicli-api/issues"
 "Cli app" = "https://github.com/vypivshiy/ani-cli-ru"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.0"
-bs4 = "^0.0.1"
-yt-dlp = "^2023.1.6"
+httpx = {extras = ["http2"], version = "^0.24.0"}
+scrape-schema = {extras = ["parsel"], version = "^0.2.3"}
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = {extras = ["coverage"], version = "^7.2.0"}
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.0"
+pyproject-flake8 = "5.0.4"
 mypy = "^0.982"
 pytest-asyncio = "^0.20.2"
 twine = "^4.0.1"
 isort = "^5.10.1"
 black = "^22.10.0"
+urllib3 = "1.26.15"
 
 [tool.poetry.group.doc.dependencies]
 sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 
 
-
 [tool.poetry.group.codegen.dependencies]
 jinja2 = "^3.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
-addopts = "--ignore='anicli_api.extractors.*' --cov='anicli_api._http' --cov='anicli_api.base' --cov='anicli_api.decoders' --cov='anicli_api.loader' --cov='anicli_api.random_useragent' --cov='anicli_api.re_models'"
-
-
-[tool.mypy]
-python_version = 3.8
-exclude="(tests|venv|setup.py|anicli_api/__template_extractor__.py|anicli_api/__template_decoder__.py)"
-ignore_missing_imports = true
-warn_no_return = false
-warn_return_any = false
-warn_unused_configs = true
 
 [tool.flake8]
-exclude = '.git,__pycache__,dist,env,venv,tests,.venv,docs/conf.py,anicli_api/extractors/__template__.py,anicli_api/decoders/__template__.py'
+exclude = [
+'.git',
+'__pycache__',
+'dist',
+'env',
+'venv',
+'.venv',
+'__template__.py']
 max-line-length = 120
 max-complexity = 8
-ignore = 'F405, F403, W503, E501, F401, E203'
+ignore = ['F405', 'F403', 'W503', 'E501', 'F401', 'E203', 'F722', 'F821']
 
-[[tool.mypy.overrides]]
-module = "tests.*"
-ignore_errors = true
+[tool.mypy]
+python_version = 3.8
+pretty = true
+ignore_missing_imports = true
+exclude = ["env", ".env", "venv", "__pycache__", "examples", "__template__.py"]
+files=["anicli_api/*"]
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
```

### Comparing `anicli_api-0.3.8/setup.py` & `anicli_api-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: anicli-api
+Version: 0.4.0
+Summary: Anime extractor api implementation
+License: MIT
+Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
+Author: Georgiy aka Vypivshiy
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Typing :: Typed
+Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
+Requires-Dist: scrape-schema[parsel] (>=0.2.3,<0.3.0)
+Project-URL: Bug Tracker, https://github.com/vypivshiy/anicli-api/issues
+Project-URL: Cli app, https://github.com/vypivshiy/ani-cli-ru
+Description-Content-Type: text/plain
+
+# anicli-api
+
+Программный интерфейс набора парсеров аниме с различных источников.
+
+# requirements
+```python
+ht
+```
+Присутствует поддержка sync и async методов с помощью `httpx` библиотеки
+Парсеры работают на REST-API (если у источника есть доступ), parsel и обёртки scrape-schema
+
+# install
+`pip install anicli-api`
+
+# Overview
+Структура проекта
+```
+anicli_api
+├── base.py - базовый класс модуля-парсера
+├── _http.py - сконфигурированный классы httpx
+├── _logger.py - логгер
+├── player - модули получения ссылок на видео
+│     ├── __template__.py - шаблон модуля PlayerExtractor
+│     ├── ...  ready-made модули
+│     ...
+├── source - модули парсеров с источников
+│     ├── __template__.py
+│     ├─ ... ready-made парсеры
+│     ...
+└── tools - прочие модули
+
+```
+Модули имеют следующий алгоритм пошагового получения объектов:
+
+```shell
+# Extractor works schema:
+    [Extractor]
+        | search(<query>)/ongoing()  -> List[Search | Ongoing]
+        V                           
+  [Search | Ongoing]          
+         | get_anime()  -> AnimeInfo
+         V                          
+    [Anime]                     
+        | get_episodes()  -> List[Episode]  
+        V                           
+    [Episode]                      
+        | get_videos()  -> List[Video]              
+        V                           
+    [Source]
+        | get_source()  -> MetaVideo or Str
+        V
+    Video(type, quality, url, extra_headers) or url
+```
+
+# Quickstart example
+Демонстрация простого prompt-line приложения.
+```python
+from anicli_api.source.animejoy import Extractor # или любой другой источник
+
+
+if __name__ == '__main__':
+    ex = Extractor()
+    while True:
+        print("PRESS CTRL + C for exit")
+        results = ex.search(input("search query > "))
+        print(*[f"{i}) {r}" for i, r in enumerate(results)], sep="\n")
+        anime = results[int(input("anime > "))].get_anime()
+        episodes = anime.get_episodes()
+        print(*[f"{i}) {ep}" for i, ep in enumerate(episodes)], sep="\n")
+        episode = episodes[int(input("episode > "))]
+        sources = episode.get_sources()
+        print(*[f"{i}) {source}" for i, source in enumerate(sources)])
+        source = sources[int(input("source > "))]
+        videos = source.get_videos()
+        print(*videos, sep="\n")
+        video = videos[int(input("video > "))]
+        print(video.type, video.quality, video.url, video.headers)
+```
+С asyncio аналогично, но методы получения объектов имеют префикс `a_` 
+# Video
+Объект `Video` (полученный из `Source.get_video` или `Source.a_get_video`) имеет следующую структуру:
+* type - тип видео
+* quality - разрешение видео
+* url - прямая ссылка на видео
+* headers - заголовки требуемые для воспроизведения видео. 
+Если возвращает пустой словарь - заголовки не нужны
+# Примечания
+
+Проект разработан преимущественно на личное, некоммерческое использование с client-side 
+стороны. 
+Автор проекта не несет ответственности за поломки, убытки в высоко нагруженных проектах и решение
+предоставляется "Как есть" в соответствии с [MIT](LIENSE) лицензией.
 
-packages = \
-['anicli_api',
- 'anicli_api.decoders',
- 'anicli_api.extractors',
- 'anicli_api.tools']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bs4>=0.0.1,<0.0.2', 'httpx>=0.23.0,<0.24.0', 'yt-dlp>=2023.1.6,<2024.0.0']
-
-setup_kwargs = {
-    'name': 'anicli-api',
-    'version': '0.3.8',
-    'description': 'Anime extractor api implementation',
-    'long_description': '# anicli-api\n[![CI](https://github.com/vypivshiy/anicli-api/actions/workflows/ci.yml/badge.svg)](https://github.com/vypivshiy/anicli-api/actions/workflows/ci.yml)\n[![Documentation Status](https://readthedocs.org/projects/anicli-api/badge/?version=latest)](https://anicli-api.readthedocs.io/en/latest/?badge=latest)\n\nПрограммный интерфейс парсера аниме с различных источников.\n\nПрисутствует поддержка sync и async методов с помощью `httpx` библиотеки, для получения информации и прямых ссылок \nна видео.\n\n# install\n`pip install anicli-api`\n\n# Overview\nМодуль экстрактора имеют следующую структуру пошагового получения объекта:\n```shell\n# Extractor works schema:\n    [Extractor]\n        | search(<query>)/ongoing()  -> List[SearchResult | Ongoing]\n        V                           \n  [SearchResult | Ongoing]          \n         | get_anime()  -> AnimeInfo\n         V                          \n    [AnimeInfo]                     \n        | get_episodes()  -> List[Episode]  \n        V                           \n    [Episode]                      \n        | get_videos()  -> List[Video]              \n        V                           \n    [Video]\n        | get_source()  -> MetaVideo or Str\n        V\n    MetaVideo(type, quality, url, extra_headers) or url\n```\n\n# Quickstart example\nСмотрите примеры [examples](examples) и [документации](https://anicli-api.readthedocs.io/en/latest/index.html)!\n\n# Примечания\n\nПроект разработан преимущественно на личное, некоммерческое использование на стороне клиента. \nАвтор проекта не несет ответственности за поломки, убытки в высоко нагруженных проектах и решение\nпредоставляется "Как есть" в соответствии с [MIT](LIENSE) лицензией.\n\nЕсли вы всё же решили этот проект использовать в **production** условиях, \nто выстаивайте архитектуру своих проектов **на предварительный сбор информации** \n(например, полученные данные сохранять в базу данных и оттуда позже получать), \nтак как большинство парсеров работает в обход официальных методов и применяются такие библиотеки как re, bs4. \n\nСледовательно, могут быть проблемы от производительности, до получения ошибок по типу 403 (срабатывание ddos защиты) или \n502 (доступа к сайту запрещён).\n\n**Этот проект не включает инструменты кеширования и сохранения всех полученных данных, только эндпоинты \nс готовой реализацией архитектуры парсеров**\n\n# DEV\n [DEV](DEV.MD)\n\n# Contributing\n[CONTRIBUTING](CONTRIBUTING.MD)\n\n# TODO\n* ~~CI CD автотестов~~\n~~* Поправить sphinx документацию~~\n* Получение видео по ссылке (like yt-dlp)\n* расширенный поиск (по жанрам, годам, etc)\n* улучшение документации\n* Продумать стандартизацию атрибутов в экстракторах (если такое реально?)\n* ~~asyncio tests~~\n* ~~coverage~~\n* ~~добавить примеры~~\n* ~~Написать документацию для high level применения пока на уровне example примеров~~\n* ~~Написать документацию для low level разработки экстракторов~~\n* ~~Дописать asyncio методы для animego~~\n* ~~Портировать anilibria, animevost, animania экстракторы из старого проекта~~\n',
-    'author': 'Georgiy aka Vypivshiy',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
 
+**Этот проект не включает инструменты кеширования и сохранения всех полученных данных, 
+только готовые реализации парсеров**
 
-setup(**setup_kwargs)
```

