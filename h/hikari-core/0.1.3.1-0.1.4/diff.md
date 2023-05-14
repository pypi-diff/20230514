# Comparing `tmp/hikari_core-0.1.3.1.tar.gz` & `tmp/hikari_core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.1.3.1.tar", max compression
+gzip compressed data, was "hikari_core-0.1.4.tar", max compression
```

## Comparing `hikari_core-0.1.3.1.tar` & `hikari_core-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,43 @@
--rw-r--r--   0        0        0     3586 2023-05-13 07:57:00.362890 hikari_core-0.1.3.1/hikari_core/__init__.py
--rw-r--r--   0        0        0     4206 2023-05-13 07:45:38.265891 hikari_core-0.1.3.1/hikari_core/analyze.py
--rw-r--r--   0        0        0     3361 2023-05-12 16:59:43.442417 hikari_core-0.1.3.1/hikari_core/command_select.py
--rw-r--r--   0        0        0    12076 2023-05-13 06:36:00.880449 hikari_core-0.1.3.1/hikari_core/data_source.py
--rw-r--r--   0        0        0      719 2023-05-12 16:14:53.492016 hikari_core-0.1.3.1/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-12 16:29:09.654986 hikari_core-0.1.3.1/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5462 2023-05-12 16:27:10.898314 hikari_core-0.1.3.1/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-12 16:01:25.071577 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-05-12 16:01:25.084174 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-05-12 16:01:25.123214 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-05-12 16:01:25.124230 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      662 2023-05-12 16:01:25.127272 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-12 16:01:25.128288 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-12 16:01:25.129291 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-12 16:01:25.129291 hikari_core-0.1.3.1/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0      937 2023-05-12 17:40:06.718420 hikari_core-0.1.3.1/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     2601 2023-05-13 07:53:57.519505 hikari_core-0.1.3.1/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-12 06:05:30.059172 hikari_core-0.1.3.1/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0      175 2023-05-12 06:05:32.348596 hikari_core-0.1.3.1/hikari_core/moudle/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5400 2023-05-12 06:07:09.234200 hikari_core-0.1.3.1/hikari_core/moudle/__pycache__/publicAPI.cpython-310.pyc
--rw-r--r--   0        0        0     2914 2023-05-12 06:06:54.456117 hikari_core-0.1.3.1/hikari_core/moudle/__pycache__/wws_info.cpython-310.pyc
--rw-r--r--   0        0        0     3105 2023-05-12 06:07:46.904239 hikari_core-0.1.3.1/hikari_core/moudle/__pycache__/wws_recent.cpython-310.pyc
--rw-r--r--   0        0        0     7226 2023-05-12 16:47:03.778682 hikari_core-0.1.3.1/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0     2584 2023-05-13 07:46:24.329769 hikari_core-0.1.3.1/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     4501 2023-05-12 16:56:20.219036 hikari_core-0.1.3.1/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0   173077 2023-05-12 03:16:55.137328 hikari_core-0.1.3.1/hikari_core/Template/Chart.min.js
--rw-r--r--   0        0        0    13279 2023-05-12 03:16:55.058560 hikari_core-0.1.3.1/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js
--rw-r--r--   0        0        0  3313391 2023-05-12 03:16:55.346040 hikari_core-0.1.3.1/hikari_core/Template/echarts.js
--rw-r--r--   0        0        0     3710 2023-05-12 03:16:55.039314 hikari_core-0.1.3.1/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5118 2023-05-12 03:16:55.034251 hikari_core-0.1.3.1/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      225 2023-05-12 03:16:55.063600 hikari_core-0.1.3.1/hikari_core/Template/text-help.css
--rw-r--r--   0        0        0     7293 2023-05-12 03:16:55.073236 hikari_core-0.1.3.1/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16766 2023-05-12 03:16:55.041316 hikari_core-0.1.3.1/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-05-12 03:16:55.029646 hikari_core-0.1.3.1/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    23636 2023-05-12 03:16:55.035273 hikari_core-0.1.3.1/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    25512 2023-05-12 03:16:55.078284 hikari_core-0.1.3.1/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-05-12 03:16:55.070709 hikari_core-0.1.3.1/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21667 2023-05-12 03:16:55.042328 hikari_core-0.1.3.1/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    20760 2023-05-12 03:16:55.061585 hikari_core-0.1.3.1/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9455 2023-05-12 03:16:55.069704 hikari_core-0.1.3.1/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5793 2023-05-12 03:16:55.077269 hikari_core-0.1.3.1/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     3537 2023-05-12 13:08:49.465546 hikari_core-0.1.3.1/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.1.3.1/LICENSE
--rw-r--r--   0        0        0      523 2023-05-13 07:57:36.341674 hikari_core-0.1.3.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.1.3.1/README.md
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 hikari_core-0.1.3.1/setup.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 hikari_core-0.1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3455 2023-05-14 15:01:19.741919 hikari_core-0.1.4/hikari_core/__init__.py
+-rw-r--r--   0        0        0     4191 2023-05-13 14:01:45.601135 hikari_core-0.1.4/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3343 2023-05-13 14:01:40.215538 hikari_core-0.1.4/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1468 2023-05-14 15:00:10.091403 hikari_core-0.1.4/hikari_core/config.py
+-rw-r--r--   0        0        0    10720 2023-05-14 13:29:43.169579 hikari_core-0.1.4/hikari_core/data_source.py
+-rw-r--r--   0        0        0      743 2023-05-13 14:56:23.409562 hikari_core-0.1.4/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2942 2023-05-13 14:55:33.233652 hikari_core-0.1.4/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5462 2023-05-12 16:27:10.898314 hikari_core-0.1.4/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-12 16:01:25.071577 hikari_core-0.1.4/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-05-12 16:01:25.084174 hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-05-12 16:01:25.123214 hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-05-12 16:01:25.124230 hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      662 2023-05-12 16:01:25.127272 hikari_core-0.1.4/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-12 16:01:25.128288 hikari_core-0.1.4/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-12 16:01:25.129291 hikari_core-0.1.4/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-12 16:01:25.129291 hikari_core-0.1.4/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     1873 2023-05-14 14:43:13.477604 hikari_core-0.1.4/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     2601 2023-05-14 15:04:21.196241 hikari_core-0.1.4/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-12 06:05:30.059172 hikari_core-0.1.4/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0     7259 2023-05-14 14:29:25.237345 hikari_core-0.1.4/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0     2579 2023-05-14 14:30:06.290170 hikari_core-0.1.4/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     4556 2023-05-14 14:29:46.686278 hikari_core-0.1.4/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0   173077 2023-05-12 03:16:55.137328 hikari_core-0.1.4/hikari_core/Template/Chart.min.js
+-rw-r--r--   0        0        0    13279 2023-05-12 03:16:55.058560 hikari_core-0.1.4/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js
+-rw-r--r--   0        0        0     3710 2023-05-12 03:16:55.039314 hikari_core-0.1.4/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5118 2023-05-12 03:16:55.034251 hikari_core-0.1.4/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      225 2023-05-12 03:16:55.063600 hikari_core-0.1.4/hikari_core/Template/text-help.css
+-rw-r--r--   0        0        0     7293 2023-05-12 03:16:55.073236 hikari_core-0.1.4/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16766 2023-05-12 03:16:55.041316 hikari_core-0.1.4/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-05-12 03:16:55.029646 hikari_core-0.1.4/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    23636 2023-05-12 03:16:55.035273 hikari_core-0.1.4/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    25512 2023-05-12 03:16:55.078284 hikari_core-0.1.4/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-05-12 03:16:55.070709 hikari_core-0.1.4/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21667 2023-05-12 03:16:55.042328 hikari_core-0.1.4/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    20760 2023-05-12 03:16:55.061585 hikari_core-0.1.4/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9455 2023-05-12 03:16:55.069704 hikari_core-0.1.4/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5793 2023-05-12 03:16:55.077269 hikari_core-0.1.4/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     3429 2023-05-13 13:54:59.163470 hikari_core-0.1.4/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.1.4/LICENSE
+-rw-r--r--   0        0        0      521 2023-05-14 15:14:09.541585 hikari_core-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.1.4/README.md
+-rw-r--r--   0        0        0    11417 1970-01-01 00:00:00.000000 hikari_core-0.1.4/setup.py
+-rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 hikari_core-0.1.4/PKG-INFO
```

### Comparing `hikari_core-0.1.3.1/hikari_core/__init__.py` & `hikari_core-0.1.4/hikari_core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,85 @@
+# fmt: off
 import os
 import time
 import traceback
 
 import jinja2
 from loguru import logger
+from pydantic import ValidationError
 
 from .analyze import analyze_command
-from .data_source import (hikari_config, set_config, set_render_params,
-                          template_path)
+from .config import hikari_config, set_hikari_config
+from .data_source import set_render_params, template_path
 from .Html_Render import html_to_pic
 from .model import Hikari_Model, Input_Model, UserInfo_Model
 from .utils import startup
-from pydantic import ValidationError
 
-env = jinja2.Environment(
-    loader=jinja2.FileSystemLoader(template_path), enable_async=True
-)
+# fmt : on
+env = jinja2.Environment(loader=jinja2.FileSystemLoader(template_path), enable_async=True)
 env.globals.update(
     time=time,
     abs=abs,
     enumerate=enumerate,
 )
 
 
 async def init_hikari(
     platform: str,
     PlatformId: str,
     command_text: str = None,
-    auto_rendering: bool = True,
-    auto_image: bool = True,
-    use_broswer: str = "chromium"
 ) -> Hikari_Model:
     """Hikari初始化，如果进行过set_config，则会覆盖这边的对应配置
 
     Args:
         platform (str): 平台类型
         PlatformId (str): 平台ID
         command_text (str): 传入指令，不带wws
-        auto_rendering (bool): 自动填充模板，默认启用
-        auto_image (bool): 是否自动渲染，默认启用，若auto_rending未启用则该项配置无效
-        use_broswer (str): chromium/firefox，默认chromium，性能大约为firefox三倍
 
     Returns:
-        Hikari: 可通过Hikari.Output.Data内数据判断是否输出
+        Hikari_Model: 可通过Hikari.Output.Data内数据判断是否输出
     """
     try:
         userinfo = UserInfo_Model(Platform=platform, PlatformId=PlatformId)
         input = Input_Model(Command_Text=command_text)
         hikari = Hikari_Model(UserInfo=userinfo, Input=input)
         hikari = await analyze_command(hikari)
         if not hikari.Status == "error" and hikari.Function:
             hikari: Hikari_Model = await hikari.Function(hikari)
-            if hikari.Output.Data_Type == '''<class 'str'>''':
+            if hikari.Output.Data_Type == """<class 'str'>""":
                 logger.info(hikari.Output.Data)
                 return hikari
             else:
-                if auto_rendering:
+                if hikari_config.auto_rendering:
                     template = env.get_template(hikari.Output.Template)
                     template_data = await set_render_params(hikari.Output.Data)
                     content = await template.render_async(template_data)
-                    if auto_image:
+                    if hikari_config.auto_image:
                         hikari.success(
-                            await html_to_pic(content, wait=0, viewport={"width": hikari.Output.Width, "height": hikari.Output.Height}, use_browser=use_broswer))
+                            await html_to_pic(
+                                content,
+                                wait=0,
+                                viewport={"width": hikari.Output.Width, "height": hikari.Output.Height},
+                                use_browser=hikari_config.use_broswer,
+                            )
+                        )
                 logger.info(hikari.Output.Data_Type)
-        if hikari.Output.Data_Type == '''<class 'str'>''':
+        if hikari.Output.Data_Type == """<class 'str'>""":
             logger.info(hikari.Output.Data)
         return hikari
     except ValidationError:
         logger.error(traceback.format_exc())
         return Hikari_Model().error("参数校验错误，请联系开发者确认入参是否符合Model")
     except Exception:
         logger.error(traceback.format_exc())
-        return Hikari_Model().error("解析指令时发生错误，请确认输入参数无误")
+        return Hikari_Model().error("Hikari-core顶层错误，请检查log")
 
 
-mtime = os.path.getmtime(template_path/"wws-info.html")
-if time.time()-mtime > 86400:
+mtime = os.path.getmtime(template_path / "wws-info.html")
+if time.time() - mtime > 86400:
     startup()
 
 logger.add(
     "hikari-core-logs/error.log",
     rotation="00:00",
     retention="1 week",
     diagnose=False,
```

### Comparing `hikari_core-0.1.3.1/hikari_core/analyze.py` & `hikari_core-0.1.4/hikari_core/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,34 @@
 from .moudle.wws_info import get_AccountInfo
 from .moudle.wws_recent import get_RecentInfo
 from .utils import match_keywords
 
 
 async def analyze_command(hikari: Hikari_Model) -> Hikari_Model:
     try:
-        if hikari.Status == 'init':  # 状态为init时才解析
+        if hikari.Status == "init":  # 状态为init时才解析
             if not hikari.Input.Command_Text:
                 return hikari.error("请发送wws help查看帮助")
-            hikari.Input.Command_Text = html.unescape(
-                str(hikari.Input.Command_Text)).strip()
+            hikari.Input.Command_Text = html.unescape(str(hikari.Input.Command_Text)).strip()
             hikari = await extract_with_special_name(hikari)
             hikari.Function, hikari.Input.Command_List = await select_command(hikari.Input.Command_List)
             hikari = await extract_with_me_or_at(hikari)
             hikari = await extract_with_function(hikari)
         return hikari
     except Exception:
         logger.error(traceback.format_exc())
         return hikari.error("解析指令时发生错误，请确认输入参数无误")
 
 
 async def extract_with_special_name(hikari: Hikari_Model) -> Hikari_Model:
     try:
-        match = re.search(r"(\(|（)(.*?)(\)|）)",
-                          hikari.Input.Command_Text)  # 是否存在（），存在则需提取出来
+        match = re.search(r"(\(|（)(.*?)(\)|）)", hikari.Input.Command_Text)  # 是否存在（），存在则需提取出来
         if match:
             hikari.Input.AccountName = match.group(2)
-            hikari.Input.Command_List = hikari.Input.Command_Text.replace(
-                match.group(0), "").split()
+            hikari.Input.Command_List = hikari.Input.Command_Text.replace(match.group(0), "").split()
         else:
             hikari.Input.Command_List = hikari.Input.Command_Text.split()
         return hikari
     except Exception:
         logger.error(traceback.format_exc())
         return hikari.error("解析指令时发生错误，请确认输入参数无误")
 
@@ -75,15 +72,17 @@
                 hikari.Input.Recent_Day = 1
             for i in hikari.Input.Command_List:
                 if str(i).isdigit() and len(i) <= 3:
                     hikari.Input.Recent_Day = int(i)
                     hikari.Input.Command_List.remove(i)
             if hikari.Input.Search_Type == 3:
                 if len(hikari.Input.Command_List) == 2:
-                    hikari.Input.Server, hikari.Input.Command_List = await match_keywords(hikari.Input.Command_List, servers)
+                    hikari.Input.Server, hikari.Input.Command_List = await match_keywords(
+                        hikari.Input.Command_List, servers
+                    )
                     if hikari.Input.Server:
                         hikari.Input.AccountName = str(hikari.Input.Command_List[0])
                         hikari.Input.Command_List.remove(hikari.Input.Command_List[0])
                     else:
                         return hikari.error("服务器参数输入错误")
                 else:
                     return hikari.error("您似乎准备用游戏昵称查询水表，请检查参数中是否包含服务器和游戏昵称，以空格区分")
```

### Comparing `hikari_core-0.1.3.1/hikari_core/command_select.py` & `hikari_core-0.1.4/hikari_core/command_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Protocol, Tuple, runtime_checkable, List
+from typing import List, Protocol, Tuple, runtime_checkable
 
 # from .game.ban_search import get_BanInfo
 # from .game.box_check import check_christmas_box
 # from .game.ocr import get_Random_Ocr_Pic
 # from .game.roll import roll_ship
 # from .game.sx import get_sx_info
 # from .moudle.publicAPI import get_ship_name
@@ -34,15 +34,15 @@
 first_command_list = [  # 同指令中越长的匹配词越靠前
     # command(("切换绑定", "更换绑定", "更改绑定"), change_BindInfo),
     # command(("查询绑定", "绑定查询", "绑定列表", "查绑定"), get_BindInfo),
     # command(("删除绑定",), delete_BindInfo),
     # command(("特殊绑定",), set_special_BindInfo),
     # command(("ship.rank", "rank"), get_ShipRank),
     # command(("bind", "绑定", "set"), set_BindInfo),
-    command(("recent", "近期",), None, get_RecentInfo,),
+    command(("recent", "近期"), None, get_RecentInfo),
     # command(("ship","单船",),None,get_ShipInfo,),
     # command(("record", "历史记录"), None, get_record),
     # command(("clan", "军团", "公会", "工会"), None, get_ClanInfo),
     # command(("随机表情包",), get_Random_Ocr_Pic),
     # command(("roll", "随机"), roll_ship),
     # command(("sx", "扫雪"), get_sx_info),
     # command(("ban","封号记录"),get_BanInfo),
@@ -67,15 +67,13 @@
                     if match_list[i] == "":  # 为空时才删除，防止未加空格没有被split切割
                         match_list.remove("")
                     return com, match_list
     return command(None, default_func, None), match_list
 
 
 async def select_command(search_list) -> Tuple[Func, List]:
-    command, search_list = await findFunction_and_replaceKeywords(
-        search_list, first_command_list, get_AccountInfo
-    )
-    if command.func == None:
+    command, search_list = await findFunction_and_replaceKeywords(search_list, first_command_list, get_AccountInfo)
+    if command.func is None:
         command, search_list = await findFunction_and_replaceKeywords(
             search_list, second_command_list, command.default_func
         )
     return command.func, search_list
```

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/__init__.py` & `hikari_core-0.1.4/hikari_core/Html_Render/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# fmt: off
 from loguru import logger
 
 from .browser import get_browser, get_new_page, shutdown_browser
 from .data_source import (capture_element, html_to_pic, template_to_html,
                           template_to_pic, text_to_pic)
 
+# fmt:on
+
 
 async def init(**kwargs):
     """Start Browser
 
     Returns:
         Browser: Browser
     """
```

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/browser.py` & `hikari_core-0.1.4/hikari_core/Html_Render/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 @Date           : 2021-03-12 13:42:43
 @LastEditors    : yanyongyu
 @LastEditTime   : 2021-11-01 14:05:41
 @Description    : None
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
-
-from typing import Optional, AsyncIterator
+# fmt: off
 from contextlib import asynccontextmanager
+from typing import AsyncIterator, Optional
 
 from loguru import logger
-from playwright.async_api import Page, Error, Browser, Playwright, async_playwright
-
+from playwright.async_api import (Browser, Error, Page, Playwright,
+                                  async_playwright)
 
+# fmt:on
 _browser: Optional[Browser] = None
 _playwright: Optional[Playwright] = None
 
 
 async def init(use_browser, **kwargs) -> Browser:
     global _browser
     global _playwright
@@ -71,18 +72,17 @@
 
 
 async def install_browser(use_browser):
     import os
     import sys
 
     from playwright.__main__ import main
+
     logger.info("使用镜像源进行下载")
-    os.environ[
-        "PLAYWRIGHT_DOWNLOAD_HOST"
-    ] = "https://npmmirror.com/mirrors/playwright/"
+    os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = "https://npmmirror.com/mirrors/playwright/"
     success = False
 
     if use_browser == "firefox":
         logger.info("正在安装 firefox")
         sys.argv = ["", "install", "firefox"]
     else:
         # 默认使用 chromium
```

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/data_source.py` & `hikari_core-0.1.4/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/katex.min.b64_fonts.css` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/katex.min.js` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/katex/mathtex-script-type.min.js` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.1.4/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/model.py` & `hikari_core-0.1.4/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/moudle/publicAPI.py` & `hikari_core-0.1.4/hikari_core/moudle/publicAPI.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from typing import List
 
 import orjson
 from httpx import ConnectTimeout
 from loguru import logger
 
 from ..data_source import levels, nations, shiptypes
-from ..HttpClient_Pool import client_wg, client_yuyuko
+from ..HttpClient_Pool import get_client_wg, get_client_yuyuko
 from ..utils import match_keywords
 
 
 async def get_nation_list():
     try:
         msg = ""
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/nation/list"
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, timeout=None)
         result = orjson.loads(resp.content)
         for nation in result["data"]:
             msg: str = msg + f"{nation['cn']}：{nation['nation']}\n"
         return msg
     except Exception:
         logger.error(traceback.format_exc())
@@ -44,14 +45,15 @@
         params = {
             "county": param_nation,
             "level": param_level,
             "shipName": "",
             "shipType": param_shiptype,
         }
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         if result["data"]:
             for ship in result["data"]:
                 msg += f"{ship['shipNameCn']}：{ship['shipNameNumbers']}\n"
         else:
             msg = "没有符合的船只"
@@ -63,56 +65,51 @@
         return "wuwuwu出了点问题，请联系麻麻解决"
 
 
 async def get_ship_byName(shipname: str):
     try:
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
         params = {"county": "", "level": "", "shipName": shipname, "shipType": ""}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         List = []
         if result["code"] == 200 and result["data"]:
             for each in result["data"]:
-                List.append(
-                    [
-                        each["id"],
-                        each["shipNameCn"],
-                        each["shipNameNumbers"],
-                        each["tier"],
-                        each['shipType']
-                    ]
-                )
+                List.append([each["id"], each["shipNameCn"], each["shipNameNumbers"], each["tier"], each["shipType"]])
             return List
         else:
             return None
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def get_all_shipList():
     try:
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
         params = {"county": "", "level": "", "shipName": "", "shipType": ""}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         if result["code"] == 200 and result["data"]:
             return result["data"]
         else:
             return None
     except Exception:
         return None
 
 
 async def get_AccountIdByName(server: str, name: str) -> str:
     try:
         url = "https://api.wows.shinoaki.com/public/wows/account/search/user"
         params = {"server": server, "userName": name}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         if result["code"] == 200 and result["data"]:
             return int(result["data"]["accountId"])
         else:
             return result["message"]
     except (TimeoutError, ConnectTimeout):
@@ -123,14 +120,15 @@
         return "好像出了点问题呢，可能是网络问题，如果重试几次还不行的话，请联系麻麻解决"
 
 
 async def get_ClanIdByName(server: str, tag: str):
     try:
         url = "https://api.wows.shinoaki.com/public/wows/clan/search"
         params = {"server": server, "tag": tag, "type": 1}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         List = []
         if result["code"] == 200 and result["data"]:
             # for each in result['data']:
             #    List.append([each['clanId'],each['name'],each['serverName'],each['tag']])
             return result["data"]
@@ -141,35 +139,29 @@
         return None
 
 
 async def check_yuyuko_cache(server, id):
     try:
         yuyuko_cache_url = "https://api.wows.shinoaki.com/api/wows/cache/check"
         params = {"accountId": id, "server": server}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.post(yuyuko_cache_url, json=params, timeout=5)
         result = orjson.loads(resp.content)
         cache_data = {}
         if result["code"] == 201:
             if "DEV" in result["data"]:
                 await get_wg_info(cache_data, "DEV", result["data"]["DEV"])
             elif "pvp" in result["data"]:
                 tasks = []
-                loop = asyncio.get_running_loop()
                 for key in result["data"]:
-                    tasks.append(
-                        asyncio.ensure_future(
-                            get_wg_info(cache_data, key, result["data"][key])
-                        )
-                    )
+                    tasks.append(asyncio.ensure_future(get_wg_info(cache_data, key, result["data"][key])))
                 await asyncio.gather(*tasks)
             if not cache_data:
                 return False
-            data_base64 = b64encode(
-                gzip.compress(orjson.dumps(cache_data))
-            ).decode()
+            data_base64 = b64encode(gzip.compress(orjson.dumps(cache_data))).decode()
             params["data"] = data_base64
             resp = await client_yuyuko.post(yuyuko_cache_url, json=params, timeout=5)
             result = orjson.loads(resp.content)
             logger.success(result)
             if result["code"] == 200:
                 return True
             else:
@@ -178,14 +170,15 @@
     except Exception:
         logger.error(traceback.format_exc())
         return False
 
 
 async def get_wg_info(params, key, url):
     try:
+        client_wg = await get_client_wg()
         resp = await client_wg.get(url, timeout=5, follow_redirects=True)
         wg_result = orjson.loads(resp.content)
         if resp.status_code == 200 and wg_result["status"] == "ok":
             params[key] = resp.text
     except Exception:
         logger.error(traceback.format_exc())
         logger.error(f"上报url：{url}")
```

### Comparing `hikari_core-0.1.3.1/hikari_core/moudle/wws_info.py` & `hikari_core-0.1.4/hikari_core/moudle/wws_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import traceback
 from asyncio.exceptions import TimeoutError
 
 import orjson
 from httpx import ConnectTimeout
 from loguru import logger
 
-from ..HttpClient_Pool import client_yuyuko
+from ..HttpClient_Pool import get_client_yuyuko
 from ..model import Hikari_Model
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName
 
 
 async def get_AccountInfo(hikari: Hikari_Model) -> Hikari_Model:
     try:
         if hikari.Status == "init":
@@ -22,23 +22,21 @@
         is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com/public/wows/account/user/info"
         if hikari.Input.Search_Type == 3:
-            params = {"server": hikari.Input.Server,
-                      "accountId": hikari.Input.AccountId}
+            params = {"server": hikari.Input.Server, "accountId": hikari.Input.AccountId}
         else:
-            params = {"server": hikari.Input.Platform,
-                      "accountId": hikari.Input.PlatformId}
+            params = {"server": hikari.Input.Platform, "accountId": hikari.Input.PlatformId}
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        logger.success(
-            f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         hikari.Output.Yuyuko_Code = result["code"]
         if result["code"] == 200 and result["data"]:
             hikari.Output.Template = "wws-info.html"
             hikari.Output.Width = 920
             hikari.Output.Height = 1000
             return hikari.success(result["data"])
         elif result["code"] == 403:
```

### Comparing `hikari_core-0.1.3.1/hikari_core/moudle/wws_recent.py` & `hikari_core-0.1.4/hikari_core/moudle/wws_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import httpx
 import jinja2
 import orjson
 from httpx import ConnectTimeout
 from loguru import logger
 
-from ..data_source import (servers, set_damageColor,
-                           set_upinfo_color, set_winColor, template_path)
-from ..HttpClient_Pool import client_yuyuko
+from ..data_source import (servers, set_damageColor, set_upinfo_color,
+                           set_winColor, template_path)
+from ..HttpClient_Pool import get_client_yuyuko
 from ..utils import match_keywords
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName
 
 #from nonebot_plugin_htmlrender import html_to_pic
 
 
 env = jinja2.Environment(
@@ -86,14 +86,15 @@
             return "参数似乎出了问题呢"
         is_cache = await check_yuyuko_cache(params["server"], params["accountId"])
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com//api/wows/recent/v2/recent/info"
+        client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         if result["code"] == 200:
             if result["data"]["shipData"][0]["shipData"]:
                 template = env.get_template("wws-info-recent.html")
             else:
                 return "该日期数据记录不存在"
```

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/Chart.min.js` & `hikari_core-0.1.4/hikari_core/Template/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js` & `hikari_core-0.1.4/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/select-ship.html` & `hikari_core-0.1.4/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/ship-rank.html` & `hikari_core-0.1.4/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-ban.html` & `hikari_core-0.1.4/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.1.4/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-clan.html` & `hikari_core-0.1.4/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.1.4/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-info.html` & `hikari_core-0.1.4/hikari_core/Template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.1.4/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.1.4/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-ship.html` & `hikari_core-0.1.4/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-sx.html` & `hikari_core-0.1.4/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/Template/wws-unban.html` & `hikari_core-0.1.4/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/hikari_core/utils.py` & `hikari_core-0.1.4/hikari_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,15 @@
         return
 
 
 async def match_keywords(match_list, Lists):
     for List in Lists:
         for kw in List.keywords:
             for match_kw in match_list:
-                if (
-                    match_kw == kw
-                    or match_kw.upper() == kw.upper()
-                    or match_kw.lower() == kw.lower()
-                ):
+                if match_kw == kw or match_kw.upper() == kw.upper() or match_kw.lower() == kw.lower():
                     match_list.remove(match_kw)
                     return List.match_keywords, match_list
     return None, match_list
 
 
 async def find_and_replace_keywords(match_list, Lists):
     for List in Lists:
@@ -68,17 +64,15 @@
         self.next_time = defaultdict(float)
         self.default_cd = default_cd_seconds
 
     def check(self, key) -> bool:
         return bool(time.time() >= self.next_time[key])
 
     def start_cd(self, key, cd_time=0):
-        self.next_time[key] = time.time() + (
-            cd_time if cd_time > 0 else self.default_cd
-        )
+        self.next_time[key] = time.time() + (cd_time if cd_time > 0 else self.default_cd)
 
     def left_time(self, key) -> float:
         return self.next_time[key] - time.time()
 
 
 class DailyNumberLimiter:
     tz = pytz.timezone("Asia/Shanghai")
```

### Comparing `hikari_core-0.1.3.1/LICENSE` & `hikari_core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.3.1/pyproject.toml` & `hikari_core-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.1.3.1"
+version = "0.1.4"
 description = ""
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `hikari_core-0.1.3.1/PKG-INFO` & `hikari_core-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: 
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

