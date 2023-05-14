# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.5.1.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.5.1.tar", last modified: Sun May  7 04:19:54 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.6.0.tar", last modified: Sun May 14 08:13:21 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1.tar` & `nonebot-plugin-chatgpt-on-qq-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.585218 nonebot-plugin-chatgpt-on-qq-1.5.1/
--rw-rw-rw-   0        0        0      770 2023-05-07 04:19:54.585218 nonebot-plugin-chatgpt-on-qq-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.570952 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    21908 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py
--rw-rw-rw-   0        0        0    11532 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/sessions.py
-drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.583218 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 04:19:54.586218 nonebot-plugin-chatgpt-on-qq-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-05-07 04:19:33.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.635310 nonebot-plugin-chatgpt-on-qq-1.6.0/
+-rw-rw-rw-   0        0        0      770 2023-05-14 08:13:21.632310 nonebot-plugin-chatgpt-on-qq-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.589033 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    21829 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1293 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    12934 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:13:21.626311 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-14 08:13:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-14 08:13:19.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 08:13:21.635310 nonebot-plugin-chatgpt-on-qq-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-05-14 08:11:32.000000 nonebot-plugin-chatgpt-on-qq-1.6.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.5.1
+Version: 1.6.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import json
 import re
 from datetime import datetime
 from json import JSONDecodeError
-from typing import Dict, List, Any
+from typing import Dict, List, Any, Type
 
+from nonebot.adapters.onebot.v11.utils import unescape
+from nonebot.adapters.onebot.v11.permission import GROUP
 from nonebot.adapters.onebot.v11 import (Bot, MessageEvent,
                                          GroupMessageEvent, PrivateMessageEvent,
                                          GROUP_ADMIN, GROUP_OWNER, MessageSegment, Message)
+from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.plugin import on_regex
 from nonebot.params import ArgPlainText, RegexDict, EventMessage
 from nonebot.permission import SUPERUSER, Permission
 from nonebot.plugin import PluginMetadata
 
 from .config import Config, plugin_config
 from .loadpresets import presets_str
 from .custom_errors import NeedCreatSession
 from .sessions import session_container, Session, get_group_id
 
 __usage__: str = (
     "指令表：\n"
     "    /chat help 获取指令帮助菜单\n"
+    "    /chat auth 获取当前群会话管理权限状态\n"
+    "    /chat auth on 设置当前群仅管理员可以管理会话\n"
+    "    /chat auth off 设置当前群所有人均可管理会话\n"
     "    /talk <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
     ">> 增\n"
     "    /chat new  根据预制模板prompt创建并加入一个新的会话\n"
     "    /chat new <自定义prompt> 根据自定义prompt创建并加入一个新的会话\n"
     "    /chat json 根据历史会话json来创建一个会话，输入该命令后会提示你在下一个消息中输入json\n"
     "    /chat cp 根据当前会话创建并加入一个新的会话\n"
     "    /chat cp <id> 根据会话<id>为模板进行复制新建加入（id为/chat list中的序号）\n"
@@ -48,15 +54,15 @@
     name="多功能ChatGPT插件",
     description="基于chatGPT-3.5-turbo API的nonebot插件",
     usage=__usage__,
     config=Config,
     extra={
         "License": "BSD License",
         "Author": "颜曦",
-        "version": "1.5.1",
+        "version": "1.6.0",
     },
 )
 
 allow_private: bool = plugin_config.allow_private
 api_keys: List[str] = session_container.api_keys
 temperature: float = plugin_config.temperature
 model: str = plugin_config.model_name
@@ -94,339 +100,349 @@
 ChatCP = on_regex(rf"^{pattern_str}\s+cp$", permission=ALLOW_PRIVATE)
 ChatWho = on_regex(rf'^{pattern_str}\s+who$', permission=ALLOW_PRIVATE)
 ChatUserList = on_regex(rf"^{pattern_str}\s+list\s*\S+$", permission=ALLOW_PRIVATE)  # 展示群聊天列表
 ReName = on_regex(rf"^{pattern_str}\s+rename\s+(?P<name>.+)$", permission=ALLOW_PRIVATE)  # 重命名当前会话
 ChatPrompt = on_regex(rf"^{pattern_str}\s+prompt$", permission=ALLOW_PRIVATE)
 ChatClear = on_regex(rf"{pattern_str}\s+clear$", permission=ALLOW_PRIVATE)
 ChatClearAt = on_regex(rf"{pattern_str}\s+clear\s*\S+$", permission=ALLOW_PRIVATE)
+SetAuthOn = on_regex(rf'^{pattern_str}\s+auth on$', permission=GROUP)
+SetAuthOff = on_regex(rf'^{pattern_str}\s+auth off$', permission=GROUP)
+ShowAuth = on_regex(rf'^{pattern_str}\s+auth$', permission=GROUP)
+
+
+@ShowAuth.handle()
+async def _(event: GroupMessageEvent):
+    group_id: str = get_group_id(event)
+    if session_container.get_group_auth(group_id):
+        await ShowAuth.finish("当前仅有管理员有权限管理会话")
+    await ShowAuth.finish("当前所有人均有权限管理会话")
+
+
+async def auth_check(matcher: Type[Matcher], bot: Bot, event: MessageEvent, group_id: str) -> None:
+    if isinstance(event, PrivateMessageEvent):
+        return
+    if session_container.get_group_auth(group_id) and not (await admin_check(bot, event)):
+        await matcher.finish('该群仅有管理员可以管理会话')
+
+
+async def admin_check(bot: Bot, event: MessageEvent) -> bool:
+    if not isinstance(event, GroupMessageEvent):
+        return True
+    return (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+
+
+@SetAuthOff.handle()
+async def _(bot: Bot, event: GroupMessageEvent):
+    group_id: str = get_group_id(event)
+    perm_check = await admin_check(bot, event)
+    if not perm_check:
+        await SetAuthOff.finish("只有群主或管理员才能设置权限管理")
+    session_container.set_group_auth(group_id, False)
+    await SetAuthOff.finish("设置成功，当前所有人均有权限管理会话")
+
+
+@SetAuthOn.handle()
+async def _(bot: Bot, event: GroupMessageEvent):
+    group_id: str = get_group_id(event)
+    perm_check = await admin_check(bot, event)
+    if not perm_check:
+        await SetAuthOn.finish("只有群主或管理员才能设置权限管理")
+    session_container.set_group_auth(group_id, True)
+    await SetAuthOn.finish("设置成功，当前仅有管理员有权限管理会话")
 
 
 @ChatClear.handle()
 async def _(bot: Bot, event: MessageEvent):
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if isinstance(event, PrivateMessageEvent):  # 私聊
-        session: Session = group_usage.pop(userId)
-        if not session:
-            await ChatClear.finish("当前不存在会话")
-        session_container.sessions.remove(session)
-        session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
-        await ChatClear.finish("已删除当前会话")
-
-    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+    group_id: str = get_group_id(event)
+    perm_check = await admin_check(bot, event)
     if not perm_check:
         await ChatClear.finish("只有群主或管理员才能清空本群全部会话!")
-    session_list: List[Session] = session_container.get_group_sessions(groupId)
+    session_list: List[Session] = session_container.get_group_sessions(group_id)
     num = len(session_list)
     for session in session_list:
-        await session_container.delete_session(session, groupId)
-    await ChatClear.finish(f"成功删除本群全部共{num}条会话")
+        await session_container.delete_session(session, group_id)
+    await ChatClear.finish(f"成功删除全部共{num}条会话")
 
 
 @ChatClearAt.handle()
 async def _(bot: Bot, event: MessageEvent, message: Message = EventMessage()):
     if isinstance(event, PrivateMessageEvent):
         await ChatClearAt.finish()
     segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
     if not segments:
         await ChatClearAt.finish()
-    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
-    senderId: int = int(event.get_user_id())
-    userId: int = int(segments[0].data.get("qq", ""))
-    groupId: str = get_group_id(event)
-    if userId != senderId and not perm_check:
+    perm_check = await admin_check(bot, event)
+    sender_id: int = int(event.get_user_id())
+    user_id: int = int(segments[0].data.get("qq", ""))
+    group_id: str = get_group_id(event)
+    if user_id != sender_id and not perm_check:
         await ChatClearAt.finish("您不是该会话的创建者或管理员!")
-    session_list: List[Session] = [s for s in session_container.sessions if s.group == groupId and s.creator == userId]
+    session_list: List[Session] = [s for s in session_container.sessions if s.group == group_id and s.creator == user_id]
     num = len(session_list)
     if num == 0:
-        await ChatClearAt.finish(f"本群用户 {userId} 还没有创建过会话哦")
+        await ChatClearAt.finish(f"本群用户 {user_id} 还没有创建过会话哦")
     for session in session_list:
-        await session_container.delete_session(session, groupId)
-    await ChatClearAt.finish(f"成功删除本群用户 {userId} 创建的全部会话共{num}条")
+        await session_container.delete_session(session, group_id)
+    await ChatClearAt.finish(f"成功删除本群用户 {user_id} 创建的全部会话共{num}条")
 
 
 @ChatCP.handle()
-async def _(event: MessageEvent):
-    if isinstance(event, PrivateMessageEvent):
-        await ChatCP.finish('私聊中无法复制会话，如果想导出json字符串请使用 /chat dump')
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if userId not in group_usage:
+async def _(bot: Bot, event: MessageEvent):
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(ChatCP, bot, event, group_id)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    if user_id not in group_usage:
         await ChatCP.finish('请先加入一个会话，再进行复制当前会话 或者使用 /chat cp <id> 进行复制')
-    session: Session = group_usage[userId]
-    group_usage[userId].del_user(userId)
-    new_session: Session = session_container.create_with_session(session, userId, groupId)
+    session: Session = group_usage[user_id]
+    group_usage[user_id].del_user(user_id)
+    new_session: Session = session_container.create_with_session(session, user_id, group_id)
     await ChatCP.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
 
 
 @ChatPrompt.handle()
 async def _(event: MessageEvent):
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if userId not in group_usage:
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    if user_id not in group_usage:
         await ChatPrompt.finish('请先加入一个会话，再进行重命名')
-    session: Session = group_usage[userId]
+    session: Session = group_usage[user_id]
     await ChatPrompt.finish(f'会话：{session.name}\nprompt：{session.prompt}')
 
 
 @ReName.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
-    if isinstance(event, PrivateMessageEvent):
-        await ReName.finish('私聊中只存在一个会话，无法命名，如果想导出json字符串请使用 /chat dump')
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if userId not in group_usage:
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(ReName, bot, event, group_id)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    if user_id not in group_usage:
         await ReName.finish('请先加入一个会话，再进行重命名')
-    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
-    session: Session = group_usage[userId]
-    name: str = info.get('name', '').strip()
-    if session.creator == userId or perm_check:
+    perm_check = await admin_check(bot, event)
+    session: Session = group_usage[user_id]
+    name: str = unescape(info.get('name', '').strip())
+    if session.creator == user_id or perm_check:
         session.rename(name[:32])
         await ReName.finish(f'当前会话已命名为 {session.name}')
-    logger.info(f'重命名群 {groupId} 会话 {session.name} 失败：权限不足')
+    logger.info(f'重命名群 {group_id} 会话 {session.name} 失败：权限不足')
     await ReName.finish("您不是该会话的创建者或管理员!")
 
 
 @ChatUserList.handle()
 async def _(event: MessageEvent, message: Message = EventMessage()):
     if isinstance(event, PrivateMessageEvent):
-        await ChatUserList.finish('私聊只有一个会话，如果想导出json字符串请使用 /chat dump')
+        await ChatUserList.finish()
     segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
     if not segments:
         await ChatUserList.finish()
-    userId: int = int(segments[0].data.get("qq", ""))
-    groupId: str = get_group_id(event)
-    session_list: List[Session] = [s for s in session_container.sessions if s.group == groupId and s.creator == userId]
+    user_id: int = int(segments[0].data.get("qq", ""))
+    group_id: str = get_group_id(event)
+    session_list: List[Session] = [s for s in session_container.sessions if s.group == group_id and s.creator == user_id]
     msg: str = f"在群中创建会话{len(session_list)}条：\n"
     for index, session in enumerate(session_list):
         msg += f" 名称:{session.name[:10]} " \
                f"创建者:{session.creator} " \
                f"时间:{datetime.fromtimestamp(session.creation_time)}\n"
-    await ChatUserList.finish(MessageSegment.at(userId) + msg)
+    await ChatUserList.finish(MessageSegment.at(user_id) + msg)
 
 
 @ChatWho.handle()
 async def _(event: MessageEvent):
-    if isinstance(event, PrivateMessageEvent):
-        await ChatWho.finish('私聊只有一个会话，如果想导出json字符串请使用 /chat dump')
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if userId not in group_usage:
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    if user_id not in group_usage:
         await ChatWho.finish('当前没有加入任何会话，请加入或创建一个会话')
-    session: Session = group_usage[userId]
+    session: Session = group_usage[user_id]
     msg = f'当前所在会话信息:\n' \
           f"名称:{session.name[:10]}\n" \
           f"创建者:{session.creator}\n" \
           f"时间:{datetime.fromtimestamp(session.creation_time)}\n" \
           f"可以使用 /chat dump 导出json字符串格式的上下文信息"
     await ChatWho.finish(msg)
 
 
 @ChatCopy.handle()
-async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
-    if isinstance(event, PrivateMessageEvent):
-        await ChatCopy.finish('私聊中无法复制会话，如果想导出json字符串请使用 /chat dump')
+async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_sessions: List[Session] = session_container.get_group_sessions(groupId)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(ChatCopy, bot, event, group_id)
+    group_sessions: List[Session] = session_container.get_group_sessions(group_id)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if not group_sessions:
         await ChatCopy.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
         await ChatCopy.finish("序号超出!", at_sender=True)
     session: Session = group_sessions[session_id - 1]
-    if userId in group_usage:
-        group_usage[userId].del_user(userId)
-    new_session: Session = session_container.create_with_session(session, userId, groupId)
+    if user_id in group_usage:
+        group_usage[user_id].del_user(user_id)
+    new_session: Session = session_container.create_with_session(session, user_id, group_id)
     await ChatCopy.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
 
 
 @Dump.handle()
 async def _(event: MessageEvent):
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
     try:
-        session: Session = session_container.get_user_usage(groupId, userId)
+        session: Session = session_container.get_user_usage(group_id, user_id)
         await Dump.finish(session.dump2json_str())
     except NeedCreatSession:
         await Dump.finish('请先加入一个会话')
 
 
 @Chat.handle()
 async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
-    content: str = info.get('content', '').strip()
+    content: str = unescape(info.get('content', '').strip())
     if not content:
         await Chat.finish("输入不能为空!", at_sender=True)
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if userId not in group_usage:  # 若用户没有加入任何会话则先创建会话
-        session: Session = session_container.create_with_template('1', userId, groupId)
-        logger.info(f"{userId} 自动创建并加入会话 '{session.name}'")
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    if user_id not in group_usage:  # 若用户没有加入任何会话则先创建会话
+        session: Session = session_container.create_with_template('1', user_id, group_id)
+        logger.info(f"{user_id} 自动创建并加入会话 '{session.name}'")
         if auto_create_preset_info:
             await Chat.send(f"自动创建并加入会话 '{session.name}' 成功", at_sender=True)
     else:
-        session: Session = group_usage[userId]
+        session: Session = group_usage[user_id]
     answer: str = await session.ask_with_content(api_keys, content, 'user', temperature, model, max_tokens)
     if answer:
         await Chat.finish(answer)
     await Chat.finish('连接失败...报错信息请查看日志')
 
 
 @Join.handle()
 async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
-    if isinstance(event, PrivateMessageEvent):
-        await Join.finish("私聊中无法加入会话!")
     session_id: int = int(info.get('id', '').strip())
-    groupId: str = get_group_id(event)
-    group_sessions: List[Session] = session_container.get_group_sessions(groupId)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    group_id: str = get_group_id(event)
+    group_sessions: List[Session] = session_container.get_group_sessions(group_id)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if not group_sessions:
         await Join.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
         await Join.finish("序号超出!", at_sender=True)
-    userId: int = int(event.get_user_id())
+    user_id: int = int(event.get_user_id())
     session: Session = group_sessions[session_id - 1]
-    if userId in group_usage:
-        group_usage[userId].del_user(userId)
-    session.add_user(userId)
-    group_usage[userId] = session
+    if user_id in group_usage:
+        group_usage[user_id].del_user(user_id)
+    session.add_user(user_id)
+    group_usage[user_id] = session
     await Join.finish(f"加入会话 {session_id}:{session.name} 成功!", at_sender=True)
 
 
 @CallMenu.handle()
 async def _():
     menu: str = __usage__
     await CallMenu.finish(menu, at_sender=True)
 
 
 @DelSelf.handle()
 async def _(bot: Bot, event: MessageEvent):
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    session: Session = group_usage.pop(userId)
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(DelSelf, bot, event, group_id)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
+    session: Session = group_usage.pop(user_id, None)
     if not session:
         await DelSelf.finish("当前不存在会话")
-    if isinstance(event, PrivateMessageEvent):  # 私聊
-        session_container.sessions.remove(session)
-        session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
-        await DelSelf.finish("已删除当前会话")
-    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
-    if session.creator == userId or perm_check:
-        await session_container.delete_session(session, groupId)
+    perm_check = await admin_check(bot, event)
+    if session.creator == user_id or perm_check:
+        await session_container.delete_session(session, group_id)
         await DelSelf.finish("删除成功!")
-    logger.info(f'删除群 {groupId} 会话 {session.name} 失败：权限不足')
+    logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足')
     await DelSelf.finish("您不是该会话的创建者或管理员!")
 
 
 @Delete.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
-    if isinstance(event, PrivateMessageEvent):  # 私聊
-        session: Session = group_usage.pop(userId)
-        if not session:
-            await Delete.finish("当前不存在会话")
-        session_container.sessions.remove(session)
-        session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
-        await Delete.finish("已删除当前会话")
-    # 群聊
-    group_sessions: List[Session] = session_container.get_group_sessions(groupId)
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(Delete, bot, event, group_id)
+    group_sessions: List[Session] = session_container.get_group_sessions(group_id)
     if not group_sessions:
-        await Delete.finish("本群尚未创建过会话!", at_sender=True)
+        await Delete.finish("当前不存在会话")
     if session_id < 1 or session_id > len(group_sessions):
         await Delete.finish("序号超出!", at_sender=True)
-    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
     session: Session = group_sessions[session_id - 1]
-    if session.creator == userId or perm_check:
-        await session_container.delete_session(session, groupId)
+    perm_check = await admin_check(bot, event)
+    if session.creator == user_id or perm_check:
+        await session_container.delete_session(session, group_id)
         await Delete.finish("删除成功!")
     else:
-        logger.info(f'删除群 {groupId} 会话 {session.name} 失败：权限不足')
+        logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足')
         await Delete.finish("您不是该会话的创建者或管理员!")
 
 
 # 暂时已完成
 
 
 @ShowList.handle()
 async def _(event: MessageEvent):
-    if isinstance(event, PrivateMessageEvent):
-        await ShowList.finish("私聊中无法展示列表(最多只有一个会话)，如果想导出json字符串请使用 /chat dump")
-    groupId: str = get_group_id(event)
-    session_list: List[Session] = session_container.get_group_sessions(groupId)
+    group_id: str = get_group_id(event)
+    session_list: List[Session] = session_container.get_group_sessions(group_id)
     msg: str = f"本群全部会话共{len(session_list)}条：\n"
     for index, session in enumerate(session_list):
         msg += f"{index + 1}. {session.name} " \
                f"创建者:{session.creator} " \
                f"时间:{datetime.fromtimestamp(session.creation_time)}\n"
     await ShowList.finish(msg, at_sender=True)
 
 
 # 暂时完成
 
 
 @CreateConversationWithPrompt.handle()
-async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
-    customPrompt: str = info.get('prompt', '').strip()
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    if isinstance(event, PrivateMessageEvent):  # 当在私聊中时
-        if userId in session_container.get_group_usage(groupId):
-            await CreateConversationWithPrompt.finish("已存在一个会话,请先删除")
-    session: Session = session_container.create_with_str(customPrompt, userId, groupId, customPrompt[:5])
+async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
+    custom_prompt: str = unescape(info.get('prompt', '').strip())
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    await auth_check(CreateConversationWithPrompt, bot, event, group_id)
+    session: Session = session_container.create_with_str(custom_prompt, user_id, group_id, custom_prompt[:5])
     await CreateConversationWithPrompt.finish(f"成功创建并加入会话 '{session.name}' ", at_sender=True)
 
 
 @CreateConversationWithTemplate.handle()
-async def CreateConversation():
+async def CreateConversation(bot: Bot, event: MessageEvent):
+    group_id: str = get_group_id(event)
+    await auth_check(CreateConversationWithTemplate, bot, event, group_id)
     await CreateConversationWithTemplate.send(presets_str, at_sender=True)
 
 
 # 暂时完成
 
 
 @CreateConversationWithTemplate.got(key="template")
 async def Create(event: MessageEvent, template_id: str = ArgPlainText("template")):
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    if isinstance(event, PrivateMessageEvent):  # 当在私聊中时
-        if userId in session_container.get_group_usage(groupId):
-            await CreateConversationWithPrompt.finish("已存在一个会话，请先删除该会话!")
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
     if not template_id.isdigit():
-        await CreateConversationWithTemplate.reject("输入ID无效!")
-    session: Session = session_container.create_with_template(template_id, userId, groupId)
+        await CreateConversationWithTemplate.finish("输入ID无效！")
+    session: Session = session_container.create_with_template(template_id, user_id, group_id)
     await CreateConversationWithTemplate.send(f"使用模板 '{template_id}' 创建并加入会话 '{session.name}' 成功!",
                                               at_sender=True)
 
 
 @CreateConversationWithJson.handle()
-async def CreateConversation():
+async def CreateConversation(bot: Bot, event: MessageEvent):
+    group_id: str = get_group_id(event)
+    await auth_check(CreateConversationWithTemplate, bot, event, group_id)
     pass
 
 
 @CreateConversationWithJson.got("jsonStr", "请直接输入json")
 async def GetJson(event: MessageEvent, json_str: str = ArgPlainText("jsonStr")):
     try:
         chat_log = json.loads(json_str)
     except JSONDecodeError:
         logger.error("json字符串错误!")
-        await CreateConversationWithJson.reject("Json错误!")
+        await CreateConversationWithJson.finish("Json错误！")
     if not chat_log[0].get("role"):
-        await CreateConversationWithJson.reject("Json错误!")
-    userId: int = int(event.get_user_id())
-    groupId: str = get_group_id(event)
-    session: Session = session_container.create_with_chat_log(chat_log, userId, groupId,
+        await CreateConversationWithJson.finish("Json错误！")
+    user_id: int = int(event.get_user_id())
+    group_id: str = get_group_id(event)
+    session: Session = session_container.create_with_chat_log(chat_log, user_id, group_id,
                                                               name=chat_log[0].get('content', '')[:5])
     await CreateConversationWithJson.send(f"创建并加入会话 '{session}' 成功!", at_sender=True)
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/config.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     allow_private: bool = True
     change_chat_to: str = None
     max_tokens: int = 1024
     auto_create_preset_info: bool = True
     customize_prefix: str = '/'
     customize_talk_cmd: str = 'talk'
     timeout: int = 10
+    default_only_admin: bool = False
 
     @validator('api_key')
     def api_key_validator(cls, v) -> List[str]:
         if not v:
             raise NoApiKeyError('请输入APIKEY')
         if isinstance(v, list):
             return v
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/sessions.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq/sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
 
 from .config import plugin_config
 from .loadpresets import templateDict
 from .custom_errors import NeedCreatSession, NoResponseError
 
-user_id = int
-group_id = str
+type_user_id = int
+type_group_id = str
 PRIVATE_GROUP: str = "Private"
 
 proxy: Optional[str] = plugin_config.openai_proxy
 if proxy:
     openai.proxy = {'http': f"http://{proxy}", 'https': f'http://{proxy}'}
 else:
     logger.warning("没有设置正向代理")
@@ -27,52 +27,86 @@
     openai.api_base = plugin_config.openai_api_base
 
 
 def get_group_id(event: MessageEvent) -> str:
     if isinstance(event, GroupMessageEvent):  # 当在群聊中时
         return str(event.group_id)
     else:  # 当在私聊中时
-        return PRIVATE_GROUP
+        return PRIVATE_GROUP + f'_{event.get_user_id()}'
 
 
 class SessionContainer:
-    def __init__(self, api_keys: List[str], chat_memory_max: int, history_max: int, dir_path: Path):
+    def __init__(self, api_keys: List[str], chat_memory_max: int, history_max: int, dir_path: Path,
+                 default_only_admin: bool):
         self.api_keys: List[str] = api_keys
         self.chat_memory_max: int = chat_memory_max
         self.history_max: int = history_max
         self.dir_path: Path = dir_path
         self.sessions: List[Session] = []
-        self.session_usage: Dict[group_id, Dict[user_id, Session]] = {}
+        self.session_usage: Dict[type_group_id, Dict[type_user_id, Session]] = {}
+        self.default_only_admin: bool = default_only_admin
+        self.group_auth: Dict[str, bool] = {}
         if not dir_path.exists():
             dir_path.mkdir(parents=True)
         self.load()
+        self.load_group_auth()
 
-    async def delete_session(self, session: "Session", groupId: str) -> None:
-        group_usage: Dict[int, Session] = self.get_group_usage(groupId)
+    @property
+    def group_auth_file_path(self) -> Path:
+        return self.dir_path / 'group_auth_file.json'
+
+    def save_group_auth(self):
+        with open(self.group_auth_file_path, 'w', encoding='utf8') as f:
+            json.dump(self.group_auth, f, ensure_ascii=False)
+
+    def load_group_auth(self):
+        if not self.group_auth_file_path.exists():
+            self.save_group_auth()
+            return
+        with open(self.group_auth_file_path, 'r', encoding='utf8') as f:
+            self.group_auth = json.load(f)
+
+    def get_group_auth(self, gid: str) -> bool:
+        return self.group_auth.setdefault(gid, self.default_only_admin)
+
+    def set_group_auth(self, gid: str, auth: bool):
+        self.group_auth[gid] = auth
+        self.save_group_auth()
+
+    async def delete_session(self, session: "Session", gid: str) -> None:
+        group_usage: Dict[int, Session] = self.get_group_usage(gid)
         users = set(uid for uid, s in group_usage.items() if s is session)
         for user in users:
-            group_usage.pop(user)
+            group_usage.pop(user, None)
         self.sessions.remove(session)
         session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
+        logger.success(f'成功删除群 {gid} 会话 {session.name}')
 
     def get_group_sessions(self, group_id: Union[str, int]) -> List["Session"]:
         return [s for s in self.sessions if s.group == str(group_id)]
 
+    @staticmethod
+    def old_version_check(session: "Session"):
+        if session.group == PRIVATE_GROUP:
+            session.file_path.unlink(missing_ok=True)
+            session.group = PRIVATE_GROUP + f'_{session.creator}'
+            session.save()
+
     def load(self) -> None:
-        for file in self.dir_path.glob('*.json'):
+        for file in list(self.dir_path.glob('*.json')):
             session = Session.reload_from_file(file)
             if not session:
                 continue
+            self.old_version_check(session)
             self.sessions.append(session)
             group = self.get_group_usage(session.group)
             for user in session.users:
                 group[user] = session
 
-    def get_group_usage(self, gid: Union[str, int]) -> Dict[user_id, "Session"]:
+    def get_group_usage(self, gid: Union[str, int]) -> Dict[type_user_id, "Session"]:
         return self.session_usage.setdefault(str(gid), {})
 
     def get_user_usage(self, gid: Union[str, int], uid: int) -> "Session":
         try:
             return self.get_group_usage(gid)[uid]
         except KeyError:
             raise NeedCreatSession(f'群{gid} 用户{uid} 需要创建 Session')
@@ -116,15 +150,15 @@
 class Session:
     def __init__(self, chat_log: List[Dict[str, str]], creator: int, group: Union[int, str], name: str,
                  chat_memory_max: int, dir_path: Path, history_max: int = 100,
                  users=None, is_save: bool = True, basic_len: int = None):
         self.history: List[Dict[str, str]] = chat_log
         self.creator: int = creator
         self._users: Set[int] = set(users) if users else set()
-        self.group: str = str(group)
+        self.group: str = group
         self.name: str = name
         self.chat_memory_max: int = chat_memory_max
         self.history_max: int = history_max
         self.creation_time: int = int(datetime.datetime.now().timestamp())
         self.dir_path: Path = dir_path
         if basic_len:
             self.basic_len: int = basic_len
@@ -180,26 +214,26 @@
             model: str = 'gpt-3.5-turbo',
             max_tokens=1024,
     ) -> str:
         if not api_keys:
             logger.error(
                 f'当前不存在api key，请在配置文件里进行配置...')
             return ''
-        if key_load_balancing:
+        if _key_load_balancing:
             random.shuffle(api_keys)
         for num, key in enumerate(api_keys):
             openai.api_key = key
             logger.debug(f'当前使用 Api Key [{key[:4]}...{key[-4:]}]')
             try:
                 completion: dict = await openai.ChatCompletion.acreate(
                     model=model,
                     messages=self.chat_memory,
                     temperature=temperature,
                     max_tokens=max_tokens,
-                    timeout=timeout,
+                    timeout=_timeout,
                 )
                 self.update_from_completion(completion)
                 if completion.get("choices") is None:
                     raise NoResponseError("未返回任何choices")
                 if len(completion["choices"]) == 0:
                     raise NoResponseError("返回的choices长度为0")
                 if completion["choices"][0].get("message") is None:
@@ -265,18 +299,19 @@
         with open(self.file_path, 'w', encoding='utf8') as f:
             json.dump(self.as_dict(), f, ensure_ascii=False)
 
     def dump2json_str(self) -> str:
         return json.dumps(self.chat_memory, ensure_ascii=False)
 
 
-chat_memory_max = plugin_config.chat_memory_max if plugin_config.chat_memory_max > 2 else 2
-history_max = plugin_config.history_max if plugin_config.history_max > chat_memory_max else 100
-timeout = int(plugin_config.timeout) if plugin_config.timeout and plugin_config.timeout > 0 else 10
-key_load_balancing: bool = plugin_config.key_load_balancing
+_chat_memory_max = plugin_config.chat_memory_max if plugin_config.chat_memory_max > 2 else 2
+_history_max = plugin_config.history_max if plugin_config.history_max > _chat_memory_max else 100
+_timeout = int(plugin_config.timeout) if plugin_config.timeout and plugin_config.timeout > 0 else 10
+_key_load_balancing: bool = plugin_config.key_load_balancing
 
 session_container: SessionContainer = SessionContainer(
     dir_path=plugin_config.history_save_path,
-    chat_memory_max=chat_memory_max,
+    chat_memory_max=_chat_memory_max,
     api_keys=plugin_config.api_key,
-    history_max=history_max,
+    history_max=_history_max,
+    default_only_admin=plugin_config.default_only_admin,
 )
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.5.1
+Version: 1.6.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.1/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.5.1',
+    version='1.6.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

