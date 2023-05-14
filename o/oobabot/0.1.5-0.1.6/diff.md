# Comparing `tmp/oobabot-0.1.5.tar.gz` & `tmp/oobabot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.5.tar", max compression
+gzip compressed data, was "oobabot-0.1.6.tar", max compression
```

## Comparing `oobabot-0.1.5.tar` & `oobabot-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.5/LICENSE
--rw-r--r--   0        0        0    12401 2023-05-12 21:59:07.554398 oobabot-0.1.5/README.md
--rw-r--r--   0        0        0      967 2023-05-12 21:59:53.189975 oobabot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-12 22:00:00.522861 oobabot-0.1.5/src/oobabot/__init__.py
--rw-r--r--   0        0        0       69 2023-05-05 00:57:20.206747 oobabot-0.1.5/src/oobabot/__main__.py
--rw-r--r--   0        0        0     6356 2023-05-12 21:31:34.953554 oobabot-0.1.5/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0     8499 2023-05-12 21:41:24.362388 oobabot-0.1.5/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     1572 2023-05-12 09:20:17.327499 oobabot-0.1.5/src/oobabot/fancy_logging.py
--rw-r--r--   0        0        0     1099 2023-05-12 09:21:18.606212 oobabot-0.1.5/src/oobabot/http_client.py
--rw-r--r--   0        0        0     8134 2023-05-12 20:40:24.610786 oobabot-0.1.5/src/oobabot/image_generator.py
--rw-r--r--   0        0        0     4092 2023-05-12 13:22:04.074586 oobabot-0.1.5/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     5815 2023-05-12 21:26:10.891395 oobabot-0.1.5/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     7520 2023-05-12 10:30:14.671081 oobabot-0.1.5/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     2334 2023-05-12 21:49:59.613778 oobabot-0.1.5/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6605 2023-05-12 09:53:03.857841 oobabot-0.1.5/src/oobabot/response_stats.py
--rw-r--r--   0        0        0    10177 2023-05-12 21:02:06.616260 oobabot-0.1.5/src/oobabot/sd_client.py
--rw-r--r--   0        0        0     2695 2023-05-12 09:19:49.870308 oobabot-0.1.5/src/oobabot/sentence_splitter.py
--rw-r--r--   0        0        0    11050 2023-05-12 22:01:40.925524 oobabot-0.1.5/src/oobabot/settings.py
--rw-r--r--   0        0        0     5512 2023-05-12 21:38:15.155746 oobabot-0.1.5/src/oobabot/templates.py
--rw-r--r--   0        0        0     1572 2023-05-12 10:48:40.662797 oobabot-0.1.5/src/oobabot/types.py
--rw-r--r--   0        0        0    13237 1970-01-01 00:00:00.000000 oobabot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.6/LICENSE
+-rw-r--r--   0        0        0    14255 2023-05-14 08:14:21.162473 oobabot-0.1.6/README.md
+-rw-r--r--   0        0        0      987 2023-05-14 08:29:00.042268 oobabot-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-14 08:28:58.302268 oobabot-0.1.6/src/oobabot/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-14 06:37:29.703837 oobabot-0.1.6/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     6229 2023-05-14 05:49:01.714519 oobabot-0.1.6/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     7043 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    14456 2023-05-14 05:54:37.044441 oobabot-0.1.6/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     2174 2023-05-14 05:55:27.114429 oobabot-0.1.6/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     1558 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     2570 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/http_client.py
+-rw-r--r--   0        0        0     9315 2023-05-14 06:03:07.084322 oobabot-0.1.6/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0     4098 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     7661 2023-05-14 07:24:24.833176 oobabot-0.1.6/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0     8104 2023-05-14 06:03:31.764314 oobabot-0.1.6/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     2861 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6647 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0    10298 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0     2695 2023-05-09 03:46:59.468832 oobabot-0.1.6/src/oobabot/sentence_splitter.py
+-rw-r--r--   0        0        0    12294 2023-05-14 07:23:55.493183 oobabot-0.1.6/src/oobabot/settings.py
+-rw-r--r--   0        0        0     6709 2023-05-14 06:04:39.674301 oobabot-0.1.6/src/oobabot/templates.py
+-rw-r--r--   0        0        0     1113 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/types.py
+-rw-r--r--   0        0        0    15045 1970-01-01 00:00:00.000000 oobabot-0.1.6/PKG-INFO
```

### Comparing `oobabot-0.1.5/LICENSE` & `oobabot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.5/README.md` & `oobabot-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
 | ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
+| ✨**Slash Commands* | coming in v0.1.6... did your bot get confused?  `/lobotomize` it! |
 
 ## Getting Started with **`oobabot`**
 
 ### See the [Installation Guide](./docs/INSTALL.md) for step-by-step instructions
 
 ## Installation tl;dr
 
@@ -68,54 +69,63 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--history-lines HISTORY_LINES] [--ignore-dms]
-               [--wakewords [WAKEWORDS ...]] [--ai-name AI_NAME] [--base-url BASE_URL]
-               [--log-all-the-things] [--persona PERSONA]
-               [--diffusion-steps DIFFUSION_STEPS] [--image-height IMAGE_HEIGHT]
-               [--image-width IMAGE_WIDTH] [--image-words [IMAGE_WORDS ...]]
+usage: oobabot [-h] [--discord-token] [--dont-split-responses]
+               [--history-lines HISTORY_LINES] [--ignore-dms] [--wakewords [WAKEWORDS ...]]
+               [--ai-name AI_NAME] [--base-url BASE_URL] [--log-all-the-things]
+               [--persona PERSONA] [--reply-in-thread] [--diffusion-steps DIFFUSION_STEPS]
+               [--image-height IMAGE_HEIGHT] [--image-width IMAGE_WIDTH]
+               [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
                [--sd-negative-prompt SD_NEGATIVE_PROMPT]
                [--sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW]
 
 Discord bot for oobabooga's text-generation-webui
 
 options:
   -h, --help            show this help message and exit
 
 Discord Settings:
+  --discord-token       Token to log into Discord with. For security purposes it's strongly
+                        recommended that you set this via the DISCORD_TOKEN environment
+                        variable instead, if possible.
+  --dont-split-responses
+                        If set, the bot post its entire response as a single message,
+                        rather than splitting it into seperate messages by sentence.
   --history-lines HISTORY_LINES
-                        Number of lines of history to supply to the AI. This is the number
-                        of lines of history that the AI will see when generating a response.
-                        The default is 20.
+                        Number of lines of chat history the AI will see when generating a
+                        response. The default is 15.
   --ignore-dms          If set, the bot will ignore direct messages.
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
                         in all discord channels can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
-                        The bot will always reply to @-mentions and direct messages, even if
-                        no wakewords are supplied.
+                        The bot will always reply to @-mentions and direct messages, even
+                        if no wakewords are supplied.
 
 Oobabooga Seetings:
   --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want,
                         but might make sense to be the name of the bot in Discord.
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
                         wss://hostname[:port] for websocket connections over TLS.
   --log-all-the-things  Prints all oobabooga requests and responses in their entirety to
                         STDOUT
   --persona PERSONA     This prefix will be added in front of every user-supplied request.
                         This is useful for setting up a 'character' for the bot to play.
                         Alternatively, this can be set with the OOBABOT_PERSONA environment
                         variable.
+  --reply-in-thread     When set, the bot will generate a new thread for each response it
+                        generates. But it will only do so if the user who prompted the bot
+                        has thread-create permissions.
 
 Stable Diffusion Settings:
   --diffusion-steps DIFFUSION_STEPS
                         Number of diffusion steps to take when generating an image. The
                         default is 30.
   --image-height IMAGE_HEIGHT
                         Size of images to generate. This is the height of the image in
@@ -123,16 +133,16 @@
   --image-width IMAGE_WIDTH
                         Size of images to generate. This is the width of the image in
                         pixels. The default is 512.
   --image-words [IMAGE_WORDS ...]
                         One or more words that will indicate the user is requeting an image
                         to be generated.
   --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER, --sd-sampler STABLE_DIFFUSION_SAMPLER
-                        Sampler to use when generating images. If not specified, the one set
-                        on the AUTOMATIC1111 server will be used.
+                        Sampler to use when generating images. If not specified, the one
+                        set on the AUTOMATIC1111 server will be used.
   --stable-diffusion-url STABLE_DIFFUSION_URL, --sd-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server
   --sd-negative-prompt SD_NEGATIVE_PROMPT
                         Negative prompt to use when generating images. This will discourage
                         Stable Diffusion from generating images with the specified content.
                         By default, this is set to follow Discord's TOS.
   --sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW
@@ -157,14 +167,17 @@
 
     **fish example**
 
     ``` fish
     set -Ux DISCORD_TOKEN ___YOUR_TOKEN___
     ```
 
+    In certain environments, it may be difficult to set an environment variable.  In that case, you can also pass the token in as a command-line argument using `--discord-token`.  But doing so might leak the token to other
+    users on a shared sysem, as it will be visible to anyone who can run `ps`.
+
 - **`--base-url`**
 
     The base URL of oobabooga's streaming web API.  This is
     required if the oobabooga machine is different than where you're running **`oobabot`**.
 
     By default, this will be port 5005 (even though the HTML UI runs on a different port).  The protocol should typically be ws://.
 
@@ -264,14 +277,29 @@
  1. any message containing a provided wakeword (see Optional Settings)
 
 Also, the bot has a random chance of sending follow-up messages within the
 same channel if others reply within 120 seconds of its last post.  The exact
 parameters for this are in flux, but is meant to simulate a natural conversation
 flow, without forcing others to always post a wakeword.
 
+### Slash Commands
+
+As of 0.1.6, the bot now supports slash commands:
+
+| **`/command`**  | what it does |
+|---------------|------------------|
+| **`/lobotomize`** | make the bot forget everything in the channel before the command is run |
+| **`/say "message"`** | speak as the bot |
+
+Oobabot doesn't add any restrictions on who can run these commands, but luckily Discord does!  You can find this inside Discord by visiting "Server Settings" -> Integrations -> Bots and Apps -> hit the icon which looks like [/] next to your bot
+
+If you're running on a large server, you may want to restrict who can run these commands.  I suggest creating a new role, and only allowing that role to run the commands.
+
 ## Known Issues
 
 - detection of requests for photos is very crude, and will likely be improved in the future.
 - some of the default settings are very specific to my use case, and will likely be made
   configurable in the future
+- public threads in 'age restricted' channels are treated as if they
+  were not age-restricted
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

### Comparing `oobabot-0.1.5/src/oobabot/decide_to_respond.py` & `oobabot-0.1.6/src/oobabot/decide_to_respond.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import random
 import re
 import typing
-from typing import List
 
-from oobabot.fancy_logging import get_logger
-from oobabot.types import ChannelMessage
-from oobabot.types import DirectMessage
-from oobabot.types import GenericMessage
+from oobabot import fancy_logger
+from oobabot import types
 
 
 class LastReplyTimes(dict):
     """
     A dictionary that keeps track of the last time we were mentioned
     in a channel.
 
@@ -29,30 +26,30 @@
             channel_id: response_time
             for channel_id, response_time in self.items()
             if response_time >= oldest_time_to_keep
         }
         self.clear()
         self.update(purged)
 
-    def log_mention(self, message: ChannelMessage) -> None:
-        self[message.channel_id] = message.send_timestamp
+    def log_mention(self, channel_id: int, send_timestamp: float) -> None:
+        self[channel_id] = send_timestamp
 
-    def time_since_last_mention(self, message: ChannelMessage) -> float:
+    def time_since_last_mention(self, message: types.ChannelMessage) -> float:
         self.purge_outdated(message.send_timestamp)
         return message.send_timestamp - self.get(message.channel_id, 0)
 
 
 class DecideToRespond:
     """
     Decide whether to respond to a message.
     """
 
     def __init__(
         self,
-        wakewords: List[str],
+        wakewords: typing.List[str],
         ignore_dms: bool,
         interrobang_bonus: float,
         time_vs_response_chance: typing.List[typing.Tuple[float, float]],
     ):
         self.wakewords = wakewords
         self.ignore_dms = ignore_dms
         self.interrobang_bonus = interrobang_bonus
@@ -63,39 +60,43 @@
 
         # match messages that include any `wakeword`, but not as part of
         # another word
         self.wakeword_patterns = [
             re.compile(rf"\b{wakeword}\b", re.IGNORECASE) for wakeword in self.wakewords
         ]
 
-    def is_directly_mentioned(self, our_user_id: int, message: GenericMessage) -> bool:
+    def is_directly_mentioned(
+        self, our_user_id: int, message: types.GenericMessage
+    ) -> bool:
         """
         Returns True if the message is a direct message to us, or if it
         mentions us by @name or wakeword.
         """
 
         # reply to all private messages
-        if isinstance(message, DirectMessage):
+        if isinstance(message, types.DirectMessage):
             if self.ignore_dms:
                 return False
             return True
 
         # reply to all messages in which we're @-mentioned
-        if isinstance(message, ChannelMessage):
+        if isinstance(message, types.ChannelMessage):
             if message.is_mentioned(our_user_id):
                 return True
 
         # reply to all messages that include a wakeword
         for wakeword_pattern in self.wakeword_patterns:
             if wakeword_pattern.search(message.body_text):
                 return True
 
         return False
 
-    def calc_base_chance_of_unsolicited_reply(self, message: ChannelMessage) -> float:
+    def calc_base_chance_of_unsolicited_reply(
+        self, message: types.ChannelMessage
+    ) -> float:
         """
         Calculate base chance of unsolicited reply using the
         TIME_VS_RESPONSE_CHANCE table.
         """
         # return a base chance that we'll respond to a message that wasn't
         # addressed to us, based on the table in TIME_VS_RESPONSE_CHANCE.
         # other factors might increase this chance.
@@ -104,15 +105,15 @@
         for duration, chance in self.time_vs_response_chance:
             if time_since_last_send < duration:
                 response_chance = chance
                 break
         return response_chance
 
     def provide_unsolicited_reply_in_channel(
-        self, our_user_id: int, message: ChannelMessage
+        self, our_user_id: int, message: types.ChannelMessage
     ) -> bool:
         # if we're not at-mentioned but others are, don't reply
         if message.mentions and not message.is_mentioned(our_user_id):
             return False
 
         # if message is empty, don't reply.  This can happen if someone
         # posts an image or an attachment without a comment.
@@ -133,44 +134,60 @@
             response_chance += self.interrobang_bonus
 
         # if the new message ends with an exclamation point, we'll respond
         if message.body_text.endswith("!"):
             response_chance += self.interrobang_bonus
 
         time_since_last_mention = self.last_reply_times.time_since_last_mention(message)
-        get_logger().debug(
-            f"Considering unsolicited message in channel {message.channel_id} "
+        fancy_logger.get().debug(
+            f"Considering unsolicited message in channel {message.channel_name} "
             f"after {time_since_last_mention:2.0f} seconds, "
             f"with chance {response_chance*100.0:2.0f}%."
         )
 
         if random.random() < response_chance:
             return True
 
         return False
 
     def should_reply_to_message(
-        self, our_user_id: int, message: GenericMessage
-    ) -> bool:
+        self, our_user_id: int, message: types.GenericMessage
+    ) -> typing.Tuple[bool, bool]:
+        """
+        Returns a tuple of (should_reply, is_direct_mention).
+
+        Direct mentions are always replied to, but also, the
+        caller should log the mention later by calling log_mention().
+
+        The only reason this method doesn't to so itself is that
+        in the case of us generating a thread to reply on, the
+        channel ID we want to track will be that of the thread
+        we create, not the channel the message was posted in.
+        """
+
         # ignore messages from other bots, out of fear of infinite loops,
         # as well as world domination
         if message.author_is_bot:
-            return False
+            return (False, False)
 
         # we do not want the bot to reply to itself.  This is redundant
         # with the previous check, except it won't be if someone decides
         # to run this under their own user token, rather than a proper
         # bot token.
         if message.author_id == our_user_id:
-            return False
+            return (False, False)
 
         if self.is_directly_mentioned(our_user_id, message):
-            if isinstance(message, ChannelMessage):
-                self.last_reply_times.log_mention(message)
-            return True
+            return (True, True)
 
-        if isinstance(message, ChannelMessage):
+        if isinstance(message, types.ChannelMessage):
             if self.provide_unsolicited_reply_in_channel(our_user_id, message):
-                return True
+                return (True, False)
 
         # ignore anything else
-        return False
+        return (False, False)
+
+    def log_mention(self, message: types.ChannelMessage) -> None:
+        self.last_reply_times.log_mention(message.channel_id, message.send_timestamp)
+
+    def log_mention_raw(self, channel_id: int, send_timestamp: float) -> None:
+        self.last_reply_times.log_mention(channel_id, send_timestamp)
```

### Comparing `oobabot-0.1.5/src/oobabot/discord_bot.py` & `oobabot-0.1.6/src/oobabot/image_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,240 +1,275 @@
-# Purpose: Discord client for Rosie
-#
-
 import asyncio
+import io
 import re
 import typing
 
 import discord
 
-from oobabot.decide_to_respond import DecideToRespond
-from oobabot.fancy_logging import get_logger
-from oobabot.image_generator import ImageGenerator
-from oobabot.ooba_client import OobaClient
-from oobabot.prompt_generator import PromptGenerator
-from oobabot.repetition_tracker import RepetitionTracker
-from oobabot.response_stats import AggregateResponseStats
-from oobabot.types import ChannelMessage
-from oobabot.types import DirectMessage
-from oobabot.types import GenericMessage
-
-FORBIDDEN_CHARACTERS = r"[\n\r\t]"
-FORBIDDEN_CHARACTERS_PATTERN = re.compile(FORBIDDEN_CHARACTERS)
-
-
-def sanitize_string(raw_string: str) -> str:
-    """
-    Filter out any characters that would confuse the AI
-    """
-    return FORBIDDEN_CHARACTERS_PATTERN.sub(" ", raw_string)
+from oobabot import fancy_logger
+from oobabot import sd_client
+from oobabot import templates
+
+
+async def image_task_to_file(image_task: "asyncio.Task[bytes]", image_request: str):
+    await image_task
+    img_bytes = image_task.result()
+    file_of_bytes = io.BytesIO(img_bytes)
+    file = discord.File(file_of_bytes)
+    file.filename = "photo.png"
+    file.description = f"image generated from '{image_request}'"
+    return file
 
 
-def discord_message_to_generic_message(raw_message: discord.Message) -> GenericMessage:
+class StableDiffusionImageView(discord.ui.View):
     """
-    Convert a discord message to a GenericMessage or subclass thereof
+    A View that displays buttons to regenerate an image
+    from Stable Diffusion with a new seed, or to lock
+    in the current image.
     """
-    generic_args = {
-        "author_id": raw_message.author.id,
-        "author_name": sanitize_string(raw_message.author.name),
-        "message_id": raw_message.id,
-        "body_text": sanitize_string(raw_message.content),
-        "author_is_bot": raw_message.author.bot,
-        "send_timestamp": raw_message.created_at.timestamp(),
-    }
-    if isinstance(raw_message.channel, discord.DMChannel):
-        return DirectMessage(**generic_args)
-    if isinstance(raw_message.channel, discord.TextChannel) or isinstance(
-        raw_message.channel, discord.GroupChannel
-    ):
-        return ChannelMessage(
-            channel_id=raw_message.channel.id,
-            mentions=[mention.id for mention in raw_message.mentions],
-            **generic_args,
-        )
-    get_logger().warning(
-        f"Unknown channel type {type(raw_message.channel)}, "
-        + f"unsolicited replies disabled.: {raw_message.channel}"
-    )
-    return GenericMessage(**generic_args)
-
-
-async def discord_to_generic_async(
-    raw_messages: typing.AsyncIterator[discord.Message],
-) -> typing.AsyncIterator[GenericMessage]:
-    async for raw_message in raw_messages:
-        message = discord_message_to_generic_message(raw_message)
-        yield message
-
-
-class DiscordBot(discord.Client):
-    # seconds after which we'll lazily purge a channel
-    # from channel_last_direct_response
 
     def __init__(
         self,
-        ooba_client: OobaClient,
-        decide_to_respond: DecideToRespond,
-        prompt_generator: PromptGenerator,
-        repetition_tracker: RepetitionTracker,
-        aggregate_response_stats: AggregateResponseStats,
-        image_generator: ImageGenerator | None,
-        ai_name: str,
-        persona: str,
-        ignore_dms: bool,
-        log_all_the_things: bool,
+        sd_client: sd_client.StableDiffusionClient,
+        is_channel_nsfw: bool,
+        image_prompt: str,
+        requesting_user_id: int,
+        requesting_user_name: str,
+        template_store: templates.TemplateStore,
     ):
-        self.ooba_client = ooba_client
-        self.decide_to_respond = decide_to_respond
-        self.prompt_generator = prompt_generator
-        self.repetition_tracker = repetition_tracker
-        self.aggregate_response_stats = aggregate_response_stats
+        super().__init__(timeout=120.0)
 
-        self.ai_name = ai_name
-        self.persona = persona
-        self.ai_user_id = -1
-        self.image_generator = image_generator
+        self.template_store = template_store
 
-        self.ignore_dms = ignore_dms
-        self.log_all_the_things = log_all_the_things
+        # only the user who requested generation of the image
+        # can have it replaced
+        self.requesting_user_id = requesting_user_id
+        self.requesting_user_name = requesting_user_name
+        self.image_prompt = image_prompt
+        self.photo_accepted = False
+
+        #####################################################
+        # "Try Again" button
+        #
+        btn_try_again = discord.ui.Button(
+            label="Try Again",
+            style=discord.ButtonStyle.blurple,
+            row=1,
+        )
+        self.image_message = None
+
+        async def on_try_again(interaction: discord.Interaction):
+            result = await self.diy_interaction_check(interaction)
+            if not result:
+                # unauthorized user
+                return
+
+            try:
+                # generate a new image
+                regen_task = sd_client.generate_image(image_prompt, is_channel_nsfw)
+                regen_file = await image_task_to_file(regen_task, image_prompt)
+                await interaction.response.defer()
+                await self.get_image_message().edit(attachments=[regen_file])
+            except Exception as e:
+                fancy_logger.get().error(f"Could not regenerate image: {e}")
+
+        btn_try_again.callback = on_try_again
+
+        #####################################################
+        # "Accept" button
+        #
+        btn_lock_in = discord.ui.Button(
+            label="Accept",
+            style=discord.ButtonStyle.success,
+            row=1,
+        )
+
+        async def on_lock_in(interaction: discord.Interaction):
+            result = await self.diy_interaction_check(interaction)
+            if not result:
+                # unauthorized user
+                return
+            await interaction.response.defer()
+            await self.detach_view_keep_img()
+
+        btn_lock_in.callback = on_lock_in
+
+        #####################################################
+        # "Delete" button
+        #
+        btn_delete = discord.ui.Button(
+            label="Delete",
+            style=discord.ButtonStyle.danger,
+            row=1,
+        )
+
+        async def on_delete(interaction: discord.Interaction):
+            result = await self.diy_interaction_check(interaction)
+            if not result:
+                # unauthorized user
+                return
+            await interaction.response.defer()
+            await self.delete_image()
 
-        # a list of timestamps in which we last posted to a channel
-        self.channel_last_direct_response = {}
+        btn_delete.callback = on_delete
 
-        intents = discord.Intents.default()
-        intents.message_content = True
+        super().add_item(btn_try_again).add_item(btn_lock_in).add_item(btn_delete)
 
-        super().__init__(intents=intents)
+    def set_image_message(self, image_message: discord.Message):
+        self.image_message = image_message
 
-    async def on_ready(self) -> None:
-        guilds = self.guilds
-        num_guilds = len(guilds)
-        num_channels = sum([len(guild.channels) for guild in guilds])
+    def get_image_message(self) -> discord.Message:
+        if self.image_message is None:
+            raise ValueError("image_message is None")
+        return self.image_message
 
-        if self.user:
-            self.ai_user_id = self.user.id
-            user_id_str = str(self.ai_user_id)
-        else:
-            user_id_str = "<unknown>"
+    async def delete_image(self):
+        await self.detach_view_delete_img(self.get_detach_message())
 
-        get_logger().info(f"Connected to discord as {self.user} (ID: {user_id_str})")
-        get_logger().debug(
-            f"monitoring {num_channels} channels across " + f"{num_guilds} server(s)"
+    async def detach_view_delete_img(self, detach_msg: str):
+        await self.get_image_message().edit(
+            content=detach_msg,
+            view=None,
+            attachments=[],
         )
-        if self.ignore_dms:
-            get_logger().debug("Ignoring DMs")
-        else:
-            get_logger().debug("listening to DMs")
 
-        get_logger().debug(f"AI name: {self.ai_name}")
-        get_logger().debug(f"AI persona: {self.persona}")
+    async def detach_view_keep_img(self):
+        self.photo_accepted = True
+        await self.get_image_message().edit(
+            content=None,
+            view=None,
+        )
+
+    async def on_timeout(self):
+        if not self.photo_accepted:
+            await self.delete_image()
+
+    async def diy_interaction_check(self, interaction: discord.Interaction) -> bool:
+        """
+        Only allow the requesting user to interact with this view.
+        """
+        if interaction.user.id == self.requesting_user_id:
+            return True
+        error_mesage = self._get_message(templates.Templates.IMAGE_UNAUTHORIZED)
+        await interaction.response.send_message(
+            content=error_mesage,
+            ephemeral=True,
+        )
+        return False
 
-        get_logger().debug(f"History: {self.prompt_generator.history_lines} lines ")
+    def get_image_message_text(self) -> str:
+        return self._get_message(templates.Templates.IMAGE_CONFIRMATION)
 
-        str_wakewords = (
-            ", ".join(self.decide_to_respond.wakewords)
-            if self.decide_to_respond.wakewords
-            else "<none>"
+    def get_detach_message(self) -> str:
+        return self._get_message(templates.Templates.IMAGE_DETACH)
+
+    def _get_message(self, message_type: templates.Templates) -> str:
+        return self.template_store.format(
+            message_type,
+            {
+                templates.TemplateToken.USER_NAME: self.requesting_user_name,
+                templates.TemplateToken.IMAGE_PROMPT: self.image_prompt,
+            },
         )
-        get_logger().debug(f"Wakewords: {str_wakewords}")
 
-    async def on_message(self, raw_message: discord.Message) -> None:
-        try:
-            message = discord_message_to_generic_message(raw_message)
-            if not self.decide_to_respond.should_reply_to_message(
-                self.ai_user_id, message
-            ):
-                return
-            async with raw_message.channel.typing():
-                image_task = None
-                if self.image_generator is not None:
-                    image_task = (
-                        await self.image_generator.maybe_generate_image_from_message(
-                            raw_message
-                        )
-                    )
-
-                message_task = self.send_response(
-                    message=message,
-                    raw_message=raw_message,
-                    image_requested=image_task is not None,
-                )
-
-                response_tasks = [
-                    task for task in [message_task, image_task] if task is not None
-                ]
-                await asyncio.wait(response_tasks)
 
-        except Exception as e:
-            get_logger().error(
-                f"Exception while processing message: {e}", exc_info=True
+class ImageGenerator:
+    def __init__(
+        self,
+        stable_diffusion_client: sd_client.StableDiffusionClient,
+        image_words: typing.List[str],
+        template_store: templates.TemplateStore,
+    ):
+        self.stable_diffusion_client = stable_diffusion_client
+        self.template_store = template_store
+        self.image_patterns = [
+            re.compile(
+                r"^.*\b" + image_word + r"\b[\s]*(of|with)?[\s]*[:]?(.*)$",
+                re.IGNORECASE,
             )
+            for image_word in image_words
+        ]
 
-    async def send_response(
+    async def _generate_image(
         self,
-        message: GenericMessage,
+        image_prompt: str,
         raw_message: discord.Message,
-        image_requested: bool,
-    ) -> None:
-        get_logger().debug(f"Request from {message.author_name}")
+        response_channel: discord.abc.Messageable,
+    ) -> discord.Message:
+        is_channel_nsfw = False
+
+        # note: public threads in NSFW chanels are not considered here
+        if isinstance(raw_message.channel, discord.TextChannel):
+            is_channel_nsfw = raw_message.channel.is_nsfw()
 
-        recent_messages = raw_message.channel.history(
-            limit=self.prompt_generator.history_lines
+        image_task = self.stable_diffusion_client.generate_image(
+            image_prompt, is_channel_nsfw=is_channel_nsfw
         )
+        try:
+            file = await image_task_to_file(image_task, image_prompt)
+        except Exception as e:
+            fancy_logger.get().error(f"Could not generate image: {e}")
+            error_message = self.template_store.format(
+                templates.Templates.IMAGE_GENERATION_ERROR,
+                {
+                    templates.TemplateToken.USER_NAME: raw_message.author.display_name,
+                    templates.TemplateToken.IMAGE_PROMPT: image_prompt,
+                },
+            )
+            return await response_channel.send(error_message, reference=raw_message)
 
-        repeated_id = self.repetition_tracker.get_throttle_message_id(
-            raw_message.channel.id
+        regen_view = StableDiffusionImageView(
+            self.stable_diffusion_client,
+            is_channel_nsfw=is_channel_nsfw,
+            image_prompt=image_prompt,
+            requesting_user_id=raw_message.author.id,
+            requesting_user_name=raw_message.author.display_name,
+            template_store=self.template_store,
         )
 
-        prompt_prefix = await self.prompt_generator.generate(
-            ai_user_id=self.ai_user_id,
-            message_history=discord_to_generic_async(recent_messages),
-            image_requested=image_requested,
-            throttle_message_id=repeated_id,
+        kwargs = {}
+        # we can only pass a reference if the message is in the same channel
+        # as the original request.  Also, send() won't take None of this
+        # argument, so we need to conditionally add it.
+        if raw_message.channel == response_channel:
+            kwargs["reference"] = raw_message
+
+        image_message = await response_channel.send(
+            content=regen_view.get_image_message_text(),
+            file=file,
+            view=regen_view,
+            **kwargs,
         )
+        regen_view.image_message = image_message
+        return image_message
 
-        response_stats = self.aggregate_response_stats.log_request_arrived(
-            prompt_prefix
-        )
-        if self.log_all_the_things:
-            print("prompt_prefix:\n----------\n")
-            print(prompt_prefix)
-            print("Response:\n----------\n")
+    def maybe_get_image_prompt(
+        self, raw_message: discord.Message
+    ) -> typing.Optional[str]:
+        image_prompt = None
+        for image_pattern in self.image_patterns:
+            match = image_pattern.search(raw_message.content)
+            if match:
+                image_prompt = match.group(2)
+                return image_prompt
+        if image_prompt is None:
+            return None
 
-        try:
-            async for sentence in self.ooba_client.request_by_sentence(prompt_prefix):
-                if self.log_all_the_things:
-                    print(sentence)
-
-                # if the AI gives itself a second line, just ignore
-                # the line instruction and continue
-                if self.prompt_generator.bot_prompt_line == sentence:
-                    get_logger().warning(
-                        f'Filtered out "{sentence}" from response, continuing'
-                    )
-                    continue
-
-                # hack: abort response if it looks like the AI is
-                # continuing the conversation as someone else
-                if sentence.endswith(" says:"):
-                    get_logger().warning(
-                        f'Filtered out "{sentence}" from response, aborting'
-                    )
-                    break
-
-                response_message = await raw_message.channel.send(sentence)
-                generic_response_message = discord_message_to_generic_message(
-                    response_message
-                )
-                self.repetition_tracker.log_message(
-                    raw_message.channel.id, generic_response_message
-                )
-
-                response_stats.log_response_part()
-
-        except Exception as err:
-            get_logger().error(f"Error: {str(err)}")
-            self.aggregate_response_stats.log_response_failure()
-            return
+        fancy_logger.get().debug("Found image prompt: %s", image_prompt)
 
-        response_stats.write_to_log(f"Response to {message.author_name} done!  ")
-        self.aggregate_response_stats.log_response_success(response_stats)
+    async def generate_image(
+        self,
+        image_prompt: str,
+        raw_message: discord.Message,
+        response_channel: discord.abc.Messageable,
+    ) -> typing.Optional["asyncio.Task[discord.Message]"]:
+        """
+        If the message contains a photo word, kick off a task
+        to generate an image, post it to the channel, and return
+        the generated message.
+
+        If the message does not contain a photo word, return None.
+        """
+        create_image_task = asyncio.create_task(
+            self._generate_image(image_prompt, raw_message, response_channel)
+        )
+        return create_image_task
```

### Comparing `oobabot-0.1.5/src/oobabot/fancy_logging.py` & `oobabot-0.1.6/src/oobabot/fancy_logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,20 +40,20 @@
         formatter = self.formatters.get(record.levelno)
         if formatter:
             return formatter.format(record)
         else:
             return record.getMessage()
 
 
-def get_logger(name: str = "oobabot") -> logging.Logger:
+def get(name: str = "oobabot") -> logging.Logger:
     return logging.getLogger(name)
 
 
 def init_logging() -> logging.Logger:
-    logger = get_logger()
+    logger = get()
     logger.setLevel(logging.DEBUG)
 
     console_handler = logging.StreamHandler()
     console_handler.setLevel(logging.DEBUG)
     console_handler.setFormatter(ColorfulLoggingFormatter())
     logger.addHandler(console_handler)
```

### Comparing `oobabot-0.1.5/src/oobabot/ooba_client.py` & `oobabot-0.1.6/src/oobabot/ooba_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 # Purpose: Streaming client for the Ooba API.
 # Can provide the response by token or by sentence.
 #
 
-from asyncio.exceptions import TimeoutError
-from socket import gaierror
 import typing
 
 import aiohttp
 
-from oobabot.fancy_logging import get_logger
-from oobabot.http_client import OobaClientError
-from oobabot.http_client import SerializedHttpClient
-from oobabot.sentence_splitter import SentenceSplitter
-from oobabot.settings import Settings
+from oobabot import fancy_logger
+from oobabot import http_client
+from oobabot import sentence_splitter
 
 
-class OobaClient(SerializedHttpClient):
+class OobaClient(http_client.SerializedHttpClient):
     # Purpose: Streaming client for the Ooba API.
     # Can provide the response by token or by sentence.
 
+    SERVICE_NAME = "Oobabooga"
+
     OOBABOOGA_STREAMING_URI_PATH: str = "/api/v1/stream"
 
     END_OF_INPUT = ""
 
-    def __init__(self, base_url: str):
-        super().__init__(base_url)
+    def __init__(
+        self, base_url: str, default_oobabooga_params: typing.Dict[str, typing.Any]
+    ):
+        super().__init__(self.SERVICE_NAME, base_url)
         self.total_response_tokens = 0
+        self.default_oobabooga_params = default_oobabooga_params
 
-    async def setup(self):
-        """
-        Attempt to connect to the oobabooga server.
-
-        Returns:
-            nothing, if the connection test was successful
-
-        Raises:
-            OobaClientError, if the connection fails
-        """
-        try:
-            async with self.get_session().ws_connect(self.OOBABOOGA_STREAMING_URI_PATH):
-                return
-        except (
-            ConnectionRefusedError,
-            gaierror,
-            TimeoutError,
-        ) as e:
-            raise OobaClientError(f"Failed to connect to {self.base_url}: {e}", e)
+    async def _setup(self):
+        async with self.get_session().ws_connect(self.OOBABOOGA_STREAMING_URI_PATH):
+            return
 
     async def request_by_sentence(self, prompt: str) -> typing.AsyncIterator[str]:
         """
         Yields each complete sentence of the response as it arrives.
         """
 
-        splitter = SentenceSplitter()
+        splitter = sentence_splitter.SentenceSplitter()
         async for new_token in self.request_by_token(prompt):
             for sentence in splitter.by_sentence(new_token):
                 yield sentence
 
+    async def request_as_string(self, prompt: str) -> typing.AsyncIterator[str]:
+        """
+        Yields the entire response as a single string.
+        """
+
+        response = ""
+        async for token in self.request_by_token(prompt):
+            response += token
+        yield response
+
     async def request_by_token(self, prompt: str) -> typing.AsyncIterator[str]:
         """
         Yields each token of the response as it arrives.
         """
 
-        request: dict[str, bool | float | int | str | typing.List[typing.Any]] = {
+        request: dict[
+            str, typing.Union[bool, float, int, str, typing.List[typing.Any]]
+        ] = {
             "prompt": prompt,
         }
-        request.update(Settings.OOBABOOGA_DEFAULT_REQUEST_PARAMS)
+        request.update(self.default_oobabooga_params)
 
         async with self.get_session().ws_connect(
             self.OOBABOOGA_STREAMING_URI_PATH
         ) as websocket:
             await websocket.send_json(request)
 
             async for msg in websocket:
@@ -94,17 +91,21 @@
 
                     elif "stream_end" == incoming_data["event"]:
                         # Make sure any unprinted text is flushed.
                         yield self.END_OF_INPUT
                         return
 
                     else:
-                        get_logger().warning(f"Unexpected event: {incoming_data}")
+                        fancy_logger.get().warning(f"Unexpected event: {incoming_data}")
 
                 elif msg.type == aiohttp.WSMsgType.ERROR:
-                    get_logger().error(f"WebSocket connection closed with error: {msg}")
-                    raise OobaClientError(
+                    fancy_logger.get().error(
+                        f"WebSocket connection closed with error: {msg}"
+                    )
+                    raise http_client.OobaHttpClientError(
                         f"WebSocket connection closed with error {msg}"
                     )
                 elif msg.type == aiohttp.WSMsgType.CLOSED:
-                    get_logger().info(f"WebSocket connection closed normally: {msg}")
+                    fancy_logger.get().info(
+                        f"WebSocket connection closed normally: {msg}"
+                    )
                     return
```

### Comparing `oobabot-0.1.5/src/oobabot/prompt_generator.py` & `oobabot-0.1.6/src/oobabot/prompt_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 # purpose: generate a prompt for the AI to respond to, given
 # the message history and persona.
 import typing
 
-from oobabot.fancy_logging import get_logger
-from oobabot.templates import TemplateStore
-from oobabot.types import GenericMessage
-from oobabot.types import TemplateToken
-from oobabot.types import Templates
+from oobabot import fancy_logger
+from oobabot import templates
+from oobabot import types
 
 
 class PromptGenerator:
     """
     Purpose: generate a prompt for the AI to use, given
     the message history and persona.
     """
 
     # this is set by the AI, and is the maximum length
     # it will understand before it starts to ignore
     # the rest of the prompt_prefix
     # note: we don't currently measure tokens, we just
     # count characters. This is a rough estimate.
-    EST_CHARACTERS_PER_TOKEN = 4
+    EST_CHARACTERS_PER_TOKEN = 3
 
     # the estimated number of characters in a line of message history
     # this is used to rougly calculate whether we'll have enough space
     # to supply the requested number of lines of history.
     #
     # in practice, we will look at the actual number of characters to
     # see what we can fit.
     #
     # note that we're doing calculations in characters, not in tokens,
     # so even counting characters exactly is still an estimate.
     EST_CHARACTERS_PER_HISTORY_LINE = 30
 
+    # when we're not splitting responses, each history line is
+    # much larger, and it's easier to run out of token space,
+    # so we use a different estimate
+    EST_CHARACTERS_PER_HISTORY_LINE_NOT_SPLITTING_RESPONSES = 180
+
     def __init__(
         self,
         ai_name: str,
         persona: str,
         history_lines: int,
         token_space: int,
-        template_store: TemplateStore,
+        template_store: templates.TemplateStore,
+        dont_split_responses: bool,
     ):
         self.ai_name = ai_name
         self.persona = persona
         self.history_lines = history_lines
         self.token_space = token_space
         self.template_store = template_store
+        self.dont_split_responses = dont_split_responses
 
         # this will be also used when sending message
         # to suppress sending the prompt text to the user
         self.bot_prompt_line = self.template_store.format(
-            Templates.PROMPT_HISTORY_LINE,
+            templates.Templates.PROMPT_HISTORY_LINE,
             {
-                TemplateToken.USER_NAME: self.ai_name,
-                TemplateToken.USER_MESSAGE: "",
+                templates.TemplateToken.USER_NAME: self.ai_name,
+                templates.TemplateToken.USER_MESSAGE: "",
             },
         ).strip()
 
         self.image_request_made = self.template_store.format(
-            Templates.PROMPT_IMAGE_COMING,
+            templates.Templates.PROMPT_IMAGE_COMING,
             {
-                TemplateToken.AI_NAME: self.ai_name,
+                templates.TemplateToken.AI_NAME: self.ai_name,
             },
         )
         self._init_history_available_chars()
 
     def _init_history_available_chars(self) -> None:
         """
         Calculate the number of characters we have available
@@ -87,17 +92,21 @@
 
         # how many chars might we have available for history?
         available_chars_for_history = est_chars_in_token_space - len(
             prompt_without_history
         )
         # how many chars do we need for the requested number of
         # lines of history?
-        required_history_size_chars = (
-            self.history_lines * self.EST_CHARACTERS_PER_HISTORY_LINE
-        )
+        chars_per_history_line = self.EST_CHARACTERS_PER_HISTORY_LINE
+        if self.dont_split_responses:
+            chars_per_history_line = (
+                self.EST_CHARACTERS_PER_HISTORY_LINE_NOT_SPLITTING_RESPONSES
+            )
+
+        required_history_size_chars = self.history_lines * chars_per_history_line
 
         if available_chars_for_history < required_history_size_chars:
             raise ValueError(
                 "AI token space is too small for prompt_prefix and history "
                 + "by an estimated "
                 + f"{required_history_size_chars - available_chars_for_history}"
                 + " characters.  You may lose history context.  You can save space"
@@ -105,16 +114,16 @@
                 + " lines of history."
             )
         self.max_history_chars = available_chars_for_history
 
     async def _render_history(
         self,
         ai_user_id: int,
-        message_history: typing.AsyncIterator[GenericMessage],
-        stop_before_message_id: int | None,
+        message_history: typing.AsyncIterator[types.GenericMessage],
+        stop_before_message_id: typing.Optional[int],
     ) -> str:
         # add on more history, but only if we have room
         # if we don't have room, we'll just truncate the history
         # by discarding the oldest messages first
         # this is s
         # it will understand before ignore
         #
@@ -144,24 +153,24 @@
                 if "tried to make an image with the prompt" in message.body_text:
                     continue
 
             if not message.body_text:
                 continue
 
             line = self.template_store.format(
-                Templates.PROMPT_HISTORY_LINE,
+                templates.Templates.PROMPT_HISTORY_LINE,
                 {
-                    TemplateToken.USER_NAME: adjusted_author_name,
-                    TemplateToken.USER_MESSAGE: message.body_text,
+                    templates.TemplateToken.USER_NAME: adjusted_author_name,
+                    templates.TemplateToken.USER_MESSAGE: message.body_text,
                 },
             )
 
             if len(line) > prompt_len_remaining:
                 num_discarded_lines = self.history_lines - len(history_lines)
-                get_logger().warn(
+                fancy_logger.get().warn(
                     "ran out of prompt space, discarding "
                     + f"{num_discarded_lines} lines "
                     + "of chat history"
                 )
                 break
 
             prompt_len_remaining -= len(line)
@@ -172,30 +181,30 @@
 
     def _generate(
         self,
         message_history_txt: str,
         image_coming: str,
     ) -> str:
         prompt = self.template_store.format(
-            Templates.PROMPT,
+            templates.Templates.PROMPT,
             {
-                TemplateToken.AI_NAME: self.ai_name,
-                TemplateToken.PERSONA: self.persona,
-                TemplateToken.MESSAGE_HISTORY: message_history_txt,
-                TemplateToken.IMAGE_COMING: image_coming,
+                templates.TemplateToken.AI_NAME: self.ai_name,
+                templates.TemplateToken.PERSONA: self.persona,
+                templates.TemplateToken.MESSAGE_HISTORY: message_history_txt,
+                templates.TemplateToken.IMAGE_COMING: image_coming,
             },
         )
         # todo: make this part of the template?
         prompt += self.bot_prompt_line + "\n"
         return prompt
 
     async def generate(
         self,
         ai_user_id: int,
-        message_history: typing.AsyncIterator[GenericMessage] | None,
+        message_history: typing.Optional[typing.AsyncIterator[types.GenericMessage]],
         image_requested: bool,
         throttle_message_id: int,
     ) -> str:
         """
         Generate a prompt for the AI to respond to.
         """
         message_history_txt = ""
```

### Comparing `oobabot-0.1.5/src/oobabot/repetition_tracker.py` & `oobabot-0.1.6/src/oobabot/repetition_tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
-from oobabot.fancy_logging import get_logger
-from oobabot.types import GenericMessage
+from oobabot import fancy_logger
+from oobabot import types
 
 
 class RepetitionTracker:
     # how many times the bot can repeat the same thing before we
     # throttle history
 
     def __init__(self, repetition_threshold: int) -> None:
@@ -22,15 +22,17 @@
         if no throttling is needed
         """
         _, throttle_message_id, _ = self.repetition_count.get(
             channel_id, (None, 0, None)
         )
         return throttle_message_id
 
-    def log_message(self, channel_id: int, response_message: GenericMessage) -> None:
+    def log_message(
+        self, channel_id: int, response_message: types.GenericMessage
+    ) -> None:
         """
         Logs a message sent by the bot, to be used for repetition tracking
         """
         # make string into canonical form
         sentence = self.make_canonical(response_message.body_text)
 
         last_message, throttle_message_id, repetition_count = self.repetition_count.get(
@@ -38,31 +40,44 @@
         )
         if last_message == sentence:
             repetition_count += 1
         else:
             repetition_count = 0
 
         if repetition_count > 0:
-            get_logger().debug(
+            fancy_logger.get().debug(
                 f"Repetition count for channel {channel_id} is {repetition_count}"
             )
 
         if self.should_throttle(repetition_count):
-            get_logger().warning(
+            fancy_logger.get().warning(
                 "Repetition found, will throttle history for channel "
                 + f"{channel_id} in next request"
             )
             throttle_message_id = response_message.message_id
 
         self.repetition_count[channel_id] = (
             sentence,
             throttle_message_id,
             repetition_count,
         )
 
+    def hide_messages_before(self, channel_id: int, message_id: int) -> None:
+        """
+        Hides all messages before the given message ID in the given channel
+        """
+        sentence, _, repetition_count = self.repetition_count.get(
+            channel_id, ("", 0, 0)
+        )
+        fancy_logger.get().info(
+            "Hiding messages before message ID "
+            + f"{message_id} in channel {channel_id}"
+        )
+        self.repetition_count[channel_id] = (sentence, message_id, repetition_count)
+
     def should_throttle(self, repetition_count: int) -> bool:
         """
         Returns whether the bot should throttle history for a given repetition count
         """
         return repetition_count >= self.repetition_threshold
 
     def make_canonical(self, content: str) -> str:
```

### Comparing `oobabot-0.1.5/src/oobabot/response_stats.py` & `oobabot-0.1.6/src/oobabot/response_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
-from typing import Callable
+import typing
 
-from oobabot.fancy_logging import get_logger
+from oobabot import fancy_logger
 
 
 class ResponseStats:
     """
     Purpose: collects timing and rate statistics for a single response
     """
 
-    def __init__(self, fn_get_total_tokens: Callable[[], int], prompt: str):
+    def __init__(self, fn_get_total_tokens: typing.Callable[[], int], prompt: str):
         self.fn_get_total_tokens = fn_get_total_tokens
         self.start_time = time.time()
         self.start_tokens = fn_get_total_tokens()
         self.duration = 0
         self.latency = 0
         self.tokens = 0
         self.prompt_len = len(prompt)
@@ -38,29 +38,29 @@
         return self.tokens / self.duration
 
     def write_to_log(self, log_prefix: str) -> None:
         """
         This writes the statistics for this specific
         request to the log.
         """
-        get_logger().debug(
+        fancy_logger.get().debug(
             log_prefix
             + f"tokens: {self.tokens}, "
             + f"time: {self.duration:.2f}s, "
             + f"latency: {self.latency:.2f}s, "
             + f"rate: {self.tokens_per_second():.2f} tok/s"
         )
 
 
 class AggregateResponseStats:
     """
     Purpose: collects timing and rate statistics for all AggregateResponseStats
     """
 
-    def __init__(self, fn_get_total_tokens: Callable[[], int]):
+    def __init__(self, fn_get_total_tokens: typing.Callable[[], int]):
         self.total_requests_received = 0
         self.total_successful_responses = 0
         self.total_failed_responses = 0
         self.total_response_time_seconds = 0
         self.total_response_latency_seconds = 0
         self.prompt_max_chars = 0
         self.prompt_min_chars = 0
@@ -148,47 +148,47 @@
 
     def write_stat_summary_to_log(self) -> None:
         """
         This writes a summary of the statistics to the log.
         Call this after all AggregateResponseStats have been handled.
         """
         if 0 == self.total_requests_received:
-            get_logger().info("No requests handled")
+            fancy_logger.get().info("No requests handled")
             return
 
-        get_logger().info(
+        fancy_logger.get().info(
             f"Recevied {self.total_requests_received} request(s), "
             + f"sent {self.total_successful_responses} successful responses "
             + f"and failed to send one {self.total_failed_responses} times(s)"
         )
 
         if self.total_failed_responses > 0:
-            get_logger().error(
+            fancy_logger.get().error(
                 "Error rate:                  " + f"{self.error_rate()}%"
             )
 
         if self.total_successful_responses > 0:
-            get_logger().debug(
+            fancy_logger.get().debug(
                 "Average response time:       "
                 + f"{self.average_response_time():6.2f}s"
             )
-            get_logger().debug(
+            fancy_logger.get().debug(
                 "Average response latency:    "
                 + f"{self.average_response_latency():6.2f}s"
             )
-            get_logger().debug(
+            fancy_logger.get().debug(
                 "Average tokens per response: "
                 + f"{self.average_tokens_per_second():6.2f}"
             )
 
         if self.total_response_time_seconds > 0:
-            get_logger().debug(
+            fancy_logger.get().debug(
                 "Average tokens per second:   "
                 + f"{self.average_tokens_per_second():6.2f}"
             )
 
-        get_logger().debug(
+        fancy_logger.get().debug(
             "Prompt length: "
             + f"max: {self.prompt_max_chars}, "
             + f"min: {self.prompt_min_chars}, "
             + f"avg: {self.average_prompt_length():.2f}"
         )
```

### Comparing `oobabot-0.1.5/src/oobabot/sd_client.py` & `oobabot-0.1.6/src/oobabot/sd_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Purpose: Client for generating images using the AUTOMATIC1111
 # API.  Takes a prompt and returns image binary data in PNG format.
 #
 
 import asyncio
 import base64
 import time
-from typing import Dict
+import typing
 
 import aiohttp
 
-from oobabot.fancy_logging import get_logger
-from oobabot.http_client import SerializedHttpClient
-
-
-class StableDiffusionClientError(Exception):
-    pass
-
+from oobabot import fancy_logger
+from oobabot import http_client
 
 # todo: response stats for SD client
 
 
-class StableDiffusionClient(SerializedHttpClient):
+class StableDiffusionClient(http_client.SerializedHttpClient):
     """
     Purpose: Client for generating images using the AUTOMATIC1111
     API.  Takes a prompt and returns image binary data in PNG format.
     """
 
-    LOG_PREFIX = "Stable Diffusion: "
+    SERVICE_NAME = "Stable Diffusion"
+    LOG_PREFIX = SERVICE_NAME + ": "
     STABLE_DIFFUSION_API_URI_PATH: str = "/sdapi/v1/"
 
     API_COMMAND_URLS = {
         "get_samplers": STABLE_DIFFUSION_API_URI_PATH + "samplers",
         # get_samplers: GET only
         #   returns a list of samplers which we can use
         #   in text2img
@@ -51,17 +47,17 @@
         self,
         base_url: str,
         negative_prompt: str,
         negative_prompt_nsfw: str,
         image_width: int,
         image_height: int,
         steps: int,
-        desired_sampler: str | None = None,
+        desired_sampler: typing.Optional[str] = None,
     ):
-        super().__init__(base_url)
+        super().__init__(self.SERVICE_NAME, base_url)
 
         self.negative_prompt = negative_prompt
         self.negative_prompt_nsfw = negative_prompt_nsfw
 
         self._sampler = None
         self.desired_sampler = desired_sampler
 
@@ -70,15 +66,15 @@
 
         self._steps = steps
 
     # set default negative prompts to make it more difficult
     # to create content against the discord TOS
     # https://discord.com/guidelines
 
-    DEFAULT_REQUEST_PARAMS: Dict[str, bool | int | str] = {
+    DEFAULT_REQUEST_PARAMS: typing.Dict[str, typing.Union[bool, int, str]] = {
         # default values are commented out
         #
         # "do_not_save_samples": False,
         #    This is a privacy concern for the users of the service.
         #    We don't want to save the generated images anyway, since they
         #    are going to be on Discord.  Also, we don't want to use the
         #    disk space.
@@ -128,68 +124,68 @@
         #  - some versions of the API don't support the
         #    "do_not_add_watermark" option, so we need to
         #    check if it's there before we try to set it
         #
         current_options = None
         async with self.get_session().get(url) as response:
             if response.status != 200:
-                raise StableDiffusionClientError(response)
+                raise http_client.OobaHttpClientError(response)
             current_options = await response.json()
 
         # now, set the options
         options_to_set = {}
         for k, v in self.DEFAULT_OPTIONS.items():
             if k not in current_options:
                 continue
             if v == current_options[k]:
                 continue
             options_to_set[k] = v
-            get_logger().info(
+            fancy_logger.get().info(
                 self.LOG_PREFIX
                 + f" changing option '{k}' from to "
                 + f"'{current_options[k]}' to '{v}'"
             )
 
         if not options_to_set:
-            get_logger().debug(
+            fancy_logger.get().debug(
                 self.LOG_PREFIX + "Options are already set correctly, no changes made."
             )
             return
 
         async with self.get_session().post(url, json=options_to_set) as response:
             if response.status != 200:
-                raise StableDiffusionClientError(response)
+                raise http_client.OobaHttpClientError(response)
             await response.json()
 
-    async def get_samplers(self) -> list[str]:
+    async def get_samplers(self) -> typing.List[str]:
         url = self.API_COMMAND_URLS["get_samplers"]
         async with self.get_session().get(url) as response:
             if response.status != 200:
-                raise StableDiffusionClientError(response)
+                raise http_client.OobaHttpClientError(response)
             response = await response.json()
             samplers = [str(sampler["name"]) for sampler in response]
             return samplers
 
     def generate_image(
         self,
         prompt: str,
         is_channel_nsfw: bool = False,
-    ) -> asyncio.Task[bytes]:
+    ) -> "asyncio.Task[bytes]":
         # Purpose: Generate an image from a prompt.
         # Args:
         #     prompt: The prompt to generate an image from.
         #     negative_prompt: The negative prompt to use.
         #     sampler_name: The sampler to use.
         #     steps: The number of steps to use.
         #     width: The width of the image.
         #     height: The height of the image.
         # Returns:
         #     The image as bytes.
         # Raises:
-        #     OobaClientError, if the request fails.
+        #     OobaHttpClientError, if the request fails.
         request = self.DEFAULT_REQUEST_PARAMS.copy()
         negative_prompt = self.negative_prompt
         if is_channel_nsfw:
             negative_prompt = self.negative_prompt_nsfw
         request.update(
             {
                 "prompt": prompt,
@@ -199,30 +195,30 @@
                 "height": self.image_height,
             }
         )
         if self._sampler is not None:
             request["sampler_name"] = self._sampler
 
         async def do_post() -> bytes:
-            get_logger().debug(
+            fancy_logger.get().debug(
                 self.LOG_PREFIX
                 + f"Image request (nsfw: {is_channel_nsfw}): {request['prompt']}"
             )
             start_time = time.time()
 
             async with self.get_session().post(
                 self.API_COMMAND_URLS["txt2img"],
                 json=request,
             ) as response:
                 if response.status != 200:
-                    raise StableDiffusionClientError(response)
+                    raise http_client.OobaHttpClientError(response)
                 duration = time.time() - start_time
                 json_body = await response.json()
                 bytes = base64.b64decode(json_body["images"][0])
-                get_logger().debug(
+                fancy_logger.get().debug(
                     self.LOG_PREFIX
                     + "Image generated, {} bytes in {:.2f} seconds".format(
                         len(bytes), duration
                     )
                 )
                 return bytes
 
@@ -233,47 +229,49 @@
                 try:
                     return await do_post()
                 except aiohttp.ClientOSError as e:
                     if e.__cause__ is not ConnectionResetError:
                         raise e
                     if tries > 2:
                         raise e
-                    get_logger().warning(
+                    fancy_logger.get().warning(
                         self.LOG_PREFIX
                         + f"Connection reset error: {e}, retrying in 1 second"
                     )
                     await asyncio.sleep(1)
                     tries += 1
 
         return asyncio.create_task(do_post_with_retry())
 
     async def set_sampler(self):
         """Sets the sampler to use, if it is available."""
         samplers = await self.get_samplers()
         if self.desired_sampler is not None:
             if self.desired_sampler in samplers:
-                get_logger().debug(
+                fancy_logger.get().debug(
                     self.LOG_PREFIX + "Using desired sampler '%s'", self.desired_sampler
                 )
                 self._sampler = self.desired_sampler
             else:
-                get_logger().warn(
+                fancy_logger.get().warn(
                     self.LOG_PREFIX + "Desired sampler '%s' not available",
                     self.desired_sampler,
                 )
                 self._sampler = None
         if self._sampler is None:
-            get_logger().debug(self.LOG_PREFIX + "Using default sampler on SD server")
-            get_logger().debug(
+            fancy_logger.get().debug(
+                self.LOG_PREFIX + "Using default sampler on SD server"
+            )
+            fancy_logger.get().debug(
                 self.LOG_PREFIX + "Available samplers: %s", ", ".join(samplers)
             )
             self._sampler = None
 
-    async def setup(self):
+    async def _setup(self):
         await self.set_sampler()
         await self.set_options()
-        get_logger().debug(
+        fancy_logger.get().debug(
             self.LOG_PREFIX
             + "Using negative prompt: "
             + self.negative_prompt[:20]
             + "..."
         )
```

### Comparing `oobabot-0.1.5/src/oobabot/sentence_splitter.py` & `oobabot-0.1.6/src/oobabot/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.5/src/oobabot/settings.py` & `oobabot-0.1.6/src/oobabot/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # this is the number of tokens we reserve for the AI
     # to respond with.
     OOBABOT_MAX_NEW_TOKENS: int = 250
 
     # this is the number of tokens the AI has available
     # across its entire request + response
-    OOBABOT_MAX_AI_TOKEN_SPACE: int = 2048
+    OOBABOT_MAX_AI_TOKEN_SPACE: int = 730
 
     # This is a table of the probability that the bot will respond
     # in an unsolicited manner (i.e. it isn't specifically pinged)
     # to a message, based on how long ago it was pinged in that
     # same channel.
     DECIDE_TO_RESPOND_TIME_VS_RESPONSE_CHANCE: typing.List[
         typing.Tuple[float, float]
@@ -38,16 +38,16 @@
     # a question mark or exclamation point
     DECIDE_TO_RESPOND_INTERROBANG_BONUS = 0.3
 
     # number of times in a row that the bot will repeat itself
     # before the repetition tracker will take action
     REPETITION_TRACKER_THRESHOLD = 1
 
-    OOBABOOGA_DEFAULT_REQUEST_PARAMS: dict[
-        str, bool | float | int | str | typing.List[typing.Any]
+    OOBABOOGA_DEFAULT_REQUEST_PARAMS: typing.Dict[
+        str, typing.Union[bool, float, int, str, typing.List[typing.Any]]
     ] = {
         "max_new_tokens": OOBABOT_MAX_NEW_TOKENS,
         "do_sample": True,
         "temperature": 1.3,
         "top_p": 0.1,
         "typical_p": 1,
         "repetition_penalty": 1.18,
@@ -67,15 +67,15 @@
     }
 
     ############################################################
     # These are the default settings for the bot.  They can be
     # overridden by environment variables or command line arguments.
 
     # number lines back in the message history to include in the prompt
-    DEFAULT_HISTORY_LINES_TO_SUPPLY = 20
+    DEFAULT_HISTORY_LINES_TO_SUPPLY = 7
 
     # words to look for in the prompt to indicate that the user
     # wants to generate an image
     DEFAULT_IMAGE_WORDS: typing.List[str] = [
         "drawing",
         "photo",
         "pic",
@@ -89,15 +89,15 @@
 
     # 30 steps of diffusion
     DEFAULT_STABLE_DIFFUSION_STEPS: int = 30
 
     # ENVIRONMENT VARIABLES ####
 
     DISCORD_TOKEN_ENV_VAR: str = "DISCORD_TOKEN"
-    DISCORD_TOKEN: str = os.environ.get(DISCORD_TOKEN_ENV_VAR, "")
+    DISCORD_TOKEN_ENV: str = os.environ.get(DISCORD_TOKEN_ENV_VAR, "")
 
     OOBABOT_PERSONA_ENV_VAR: str = "OOBABOT_PERSONA"
     OOBABOT_PERSONA: str = os.environ.get(OOBABOT_PERSONA_ENV_VAR, "")
 
     DEFAULT_WAKEWORDS: typing.List[str] = ["oobabot"]
     DEFAULT_URL: str = "ws://localhost:5005"
 
@@ -126,20 +126,36 @@
         )
 
         ###########################################################
         # Discord Settings
 
         discord_group = self.add_argument_group("Discord Settings")
         discord_group.add_argument(
+            "--discord-token",
+            type=str,
+            default=self.DISCORD_TOKEN_ENV,
+            help="Token to log into Discord with.  For security "
+            + "purposes it's strongly recommended that you set "
+            + f"this via the {self.DISCORD_TOKEN_ENV_VAR} environment "
+            + "variable instead, if possible.",
+        )
+        discord_group.add_argument(
+            "--dont-split-responses",
+            default=False,
+            help="If set, the bot post its entire response as a single "
+            + "message, rather than splitting it into seperate "
+            + "messages by sentence.",
+            action="store_true",
+        )
+        discord_group.add_argument(
             "--history-lines",
             type=int,
             default=self.DEFAULT_HISTORY_LINES_TO_SUPPLY,
-            help="Number of lines of history to supply to the AI.  "
-            + "This is the number of lines of history that the AI will "
-            + "see when generating a response.  The default is "
+            help="Number of lines of chat history the AI will see "
+            + "when generating a response.  The default is "
             + f"{self.DEFAULT_HISTORY_LINES_TO_SUPPLY}.",
         )
         discord_group.add_argument(
             "--ignore-dms",
             default=False,
             help="If set, the bot will ignore direct messages.",
             action="store_true",
@@ -190,15 +206,22 @@
             type=str,
             default=self.OOBABOT_PERSONA,
             help="This prefix will be added in front of every user-supplied "
             + "request.  This is useful for setting up a 'character' for the "
             + "bot to play.  Alternatively, this can be set with the "
             + f"{self.OOBABOT_PERSONA_ENV_VAR} environment variable.",
         )
-
+        oobabooga_group.add_argument(
+            "--reply-in-thread",
+            default=False,
+            help="When set, the bot will generate a new thread for each "
+            + "response it generates.  But it will only do so if the "
+            + "user who prompted the bot has thread-create permissions.",
+            action="store_true",
+        )
         ###########################################################
         # Stable Diffusion Settings
 
         stable_diffusion_group = self.add_argument_group("Stable Diffusion Settings")
         stable_diffusion_group.add_argument(
             "--diffusion-steps",
             type=int,
@@ -253,24 +276,27 @@
             + " Stable Diffusion from generating images with the specified content.  "
             + "By default, this is set to follow Discord's TOS.",
         )
         stable_diffusion_group.add_argument(
             "--sd-negative-prompt-nsfw",
             type=str,
             default=self.DEFAULT_SD_NEGATIVE_PROMPT_NSFW,
-            help="Negative prompt to use when generating images in a channel marked as"
+            help="Negative prompt to use when generating images in a channel marked as "
             + "'Age-Restricted'.",
         )
 
-    def load(self) -> None:
-        self._settings = self.parse_args().__dict__
+    def load(self, args) -> None:
+        self._settings = self.parse_args(args=args).__dict__
 
         # Discord Settings
+        self.discord_token = self._settings.pop("discord_token")
+        self.dont_split_responses = self._settings.pop("dont_split_responses")
         self.history_lines = self._settings.pop("history_lines")
         self.ignore_dms = self._settings.pop("ignore_dms")
+        self.reply_in_thread = self._settings.pop("reply_in_thread")
         self.wakewords = self._settings.pop("wakewords")
 
         # OogaBooga Settings
         self.ai_name = self._settings.pop("ai_name")
         self.base_url = self._settings.pop("base_url")
         print(self.base_url)
         self.log_all_the_things = self._settings.pop("log_all_the_things")
```

### Comparing `oobabot-0.1.5/src/oobabot/templates.py` & `oobabot-0.1.6/src/oobabot/templates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,44 @@
+import enum
 import textwrap
 import typing
 
-from oobabot.types import TemplateToken
-from oobabot.types import Templates
 
+class Templates(enum.Enum):
+    COMMAND_LOBOTOMIZE_RESPONSE = "command_lobotomize_response"
 
-class TemplateMessageFormatter:
-    # Purpose: format messages using a template string
-
-    def __init__(
-        self,
-        template_name: Templates,
-        template: str,
-        allowed_tokens: typing.List[TemplateToken],
-    ):
-        self._validate_format_string(template_name, template, allowed_tokens)
-        self.template_name = template_name
-        self.template = template
-        self.allowed_tokens = allowed_tokens
-
-    def format(self, format_args: dict[TemplateToken, str]) -> str:
-        return self.template.format(**format_args)
-
-    @staticmethod
-    def _validate_format_string(
-        template_name: Templates,
-        format_str: str,
-        allowed_args: typing.List[TemplateToken],
-    ):
-        def find_all_ch(s: str, ch: str) -> typing.Generator[int, None, None]:
-            # find all indices of ch in s
-            for i, ltr in enumerate(s):
-                if ltr == ch:
-                    yield i
-
-        # raises if fmt_string contains any args not in allowed_args
-        allowed_close_brace_indices: typing.Set[int] = set()
-
-        for open_brace_idx in find_all_ch(format_str, "{"):
-            for allowed_arg in allowed_args:
-                idx_end = open_brace_idx + len(allowed_arg) + 1
-                next_substr = format_str[open_brace_idx : idx_end + 1]
-                if next_substr == "{" + allowed_arg + "}":
-                    allowed_close_brace_indices.add(idx_end)
-                    break
-            else:
-                raise ValueError(
-                    f"invalid template: {template_name} contains "
-                    + f"an argument not in {allowed_args}"
-                )
-        for close_brace_idx in find_all_ch(format_str, "}"):
-            if close_brace_idx not in allowed_close_brace_indices:
-                raise ValueError(
-                    f"invalid template: {template_name} contains "
-                    + f"an argument not in {allowed_args}"
-                )
+    IMAGE_DETACH = "image_detach"
+    IMAGE_CONFIRMATION = "image_confirmation"
+    IMAGE_GENERATION_ERROR = "image_generation_error"
+    IMAGE_UNAUTHORIZED = "image_unauthorized"
+
+    PROMPT = "prompt"
+    PROMPT_HISTORY_LINE = "prompt_history_line"
+    PROMPT_IMAGE_COMING = "prompt_image_coming"
+
+
+class TemplateToken(str, enum.Enum):
+    AI_NAME = "AI_NAME"
+    PERSONA = "PERSONA"
+    IMAGE_COMING = "IMAGE_COMING"
+    IMAGE_PROMPT = "IMAGE_PROMPT"
+    MESSAGE_HISTORY = "MESSAGE_HISTORY"
+    USER_MESSAGE = "USER_MESSAGE"
+    USER_NAME = "USER_NAME"
 
 
 class TemplateStore:
     # Purpose: store templates and format messages using them
 
     # mapping of template names to tokens allowed in that template
     TEMPLATES: typing.Dict[Templates, typing.List[TemplateToken]] = {
+        Templates.COMMAND_LOBOTOMIZE_RESPONSE: [
+            TemplateToken.AI_NAME,
+            TemplateToken.USER_NAME,
+        ],
         Templates.PROMPT: [
             TemplateToken.AI_NAME,
             TemplateToken.IMAGE_COMING,
             TemplateToken.MESSAGE_HISTORY,
             TemplateToken.PERSONA,
         ],
         Templates.PROMPT_HISTORY_LINE: [
@@ -79,14 +52,18 @@
             TemplateToken.IMAGE_PROMPT,
             TemplateToken.USER_NAME,
         ],
         Templates.IMAGE_CONFIRMATION: [
             TemplateToken.IMAGE_PROMPT,
             TemplateToken.USER_NAME,
         ],
+        Templates.IMAGE_GENERATION_ERROR: [
+            TemplateToken.IMAGE_PROMPT,
+            TemplateToken.USER_NAME,
+        ],
         Templates.IMAGE_UNAUTHORIZED: [TemplateToken.USER_NAME],
     }
 
     DEFAULT_TEMPLATES: typing.Dict[Templates, str] = {
         Templates.PROMPT: textwrap.dedent(
             """
             You are in a chat room with multiple participants.
@@ -125,19 +102,29 @@
         ),
         Templates.IMAGE_CONFIRMATION: textwrap.dedent(
             """
             {USER_NAME}, is this what you wanted?
             If no choice is made, this message will 💣 self-destuct 💣 in 3 minutes.
             """
         ),
+        Templates.IMAGE_GENERATION_ERROR: textwrap.dedent(
+            """
+            Something went wrong generating your image.  Sorry about that!
+            """
+        ),
         Templates.IMAGE_UNAUTHORIZED: textwrap.dedent(
             """
             Sorry, only {USER_NAME} can press the buttons.
             """
         ),
+        Templates.COMMAND_LOBOTOMIZE_RESPONSE: textwrap.dedent(
+            """
+            Ummmm... what were we talking about?
+            """
+        ),
     }
 
     def __init__(self):
         self.templates: typing.Dict[Templates, TemplateMessageFormatter] = {}
         for template, tokens in self.TEMPLATES.items():
             template_fmt = TemplateStore.DEFAULT_TEMPLATES.get(template)
             if template_fmt is None:
@@ -151,10 +138,62 @@
         allowed_tokens: typing.List[TemplateToken],
     ):
         self.templates[template_name] = TemplateMessageFormatter(
             template_name, format_str, allowed_tokens
         )
 
     def format(
-        self, template_name: Templates, format_args: dict[TemplateToken, str]
+        self, template_name: Templates, format_args: typing.Dict[TemplateToken, str]
     ) -> str:
         return self.templates[template_name].format(format_args)
+
+
+class TemplateMessageFormatter:
+    # Purpose: format messages using a template string
+
+    def __init__(
+        self,
+        template_name: Templates,
+        template: str,
+        allowed_tokens: typing.List[TemplateToken],
+    ):
+        self._validate_format_string(template_name, template, allowed_tokens)
+        self.template_name = template_name
+        self.template = template
+        self.allowed_tokens = allowed_tokens
+
+    def format(self, format_args: typing.Dict[TemplateToken, str]) -> str:
+        return self.template.format(**format_args)
+
+    @staticmethod
+    def _validate_format_string(
+        template_name: Templates,
+        format_str: str,
+        allowed_args: typing.List[TemplateToken],
+    ):
+        def find_all_ch(s: str, ch: str) -> typing.Generator[int, None, None]:
+            # find all indices of ch in s
+            for i, ltr in enumerate(s):
+                if ltr == ch:
+                    yield i
+
+        # raises if fmt_string contains any args not in allowed_args
+        allowed_close_brace_indices: typing.Set[int] = set()
+
+        for open_brace_idx in find_all_ch(format_str, "{"):
+            for allowed_arg in allowed_args:
+                idx_end = open_brace_idx + len(allowed_arg) + 1
+                next_substr = format_str[open_brace_idx : idx_end + 1]
+                if next_substr == "{" + allowed_arg + "}":
+                    allowed_close_brace_indices.add(idx_end)
+                    break
+            else:
+                raise ValueError(
+                    f"invalid template: {template_name} contains "
+                    + f"an argument not in {allowed_args}"
+                )
+        for close_brace_idx in find_all_ch(format_str, "}"):
+            if close_brace_idx not in allowed_close_brace_indices:
+                raise ValueError(
+                    f"invalid template: {template_name} contains "
+                    + f"an argument not in {allowed_args}"
+                )
```

### Comparing `oobabot-0.1.5/PKG-INFO` & `oobabot-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: discord.py (>=2.2.2,<3.0.0)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
 Project-URL: Repository, https://github.com/chrisrude/oobabot
@@ -67,14 +66,15 @@
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
 | ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
+| ✨**Slash Commands* | coming in v0.1.6... did your bot get confused?  `/lobotomize` it! |
 
 ## Getting Started with **`oobabot`**
 
 ### See the [Installation Guide](./docs/INSTALL.md) for step-by-step instructions
 
 ## Installation tl;dr
 
@@ -89,54 +89,63 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--history-lines HISTORY_LINES] [--ignore-dms]
-               [--wakewords [WAKEWORDS ...]] [--ai-name AI_NAME] [--base-url BASE_URL]
-               [--log-all-the-things] [--persona PERSONA]
-               [--diffusion-steps DIFFUSION_STEPS] [--image-height IMAGE_HEIGHT]
-               [--image-width IMAGE_WIDTH] [--image-words [IMAGE_WORDS ...]]
+usage: oobabot [-h] [--discord-token] [--dont-split-responses]
+               [--history-lines HISTORY_LINES] [--ignore-dms] [--wakewords [WAKEWORDS ...]]
+               [--ai-name AI_NAME] [--base-url BASE_URL] [--log-all-the-things]
+               [--persona PERSONA] [--reply-in-thread] [--diffusion-steps DIFFUSION_STEPS]
+               [--image-height IMAGE_HEIGHT] [--image-width IMAGE_WIDTH]
+               [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
                [--sd-negative-prompt SD_NEGATIVE_PROMPT]
                [--sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW]
 
 Discord bot for oobabooga's text-generation-webui
 
 options:
   -h, --help            show this help message and exit
 
 Discord Settings:
+  --discord-token       Token to log into Discord with. For security purposes it's strongly
+                        recommended that you set this via the DISCORD_TOKEN environment
+                        variable instead, if possible.
+  --dont-split-responses
+                        If set, the bot post its entire response as a single message,
+                        rather than splitting it into seperate messages by sentence.
   --history-lines HISTORY_LINES
-                        Number of lines of history to supply to the AI. This is the number
-                        of lines of history that the AI will see when generating a response.
-                        The default is 20.
+                        Number of lines of chat history the AI will see when generating a
+                        response. The default is 15.
   --ignore-dms          If set, the bot will ignore direct messages.
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
                         in all discord channels can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
-                        The bot will always reply to @-mentions and direct messages, even if
-                        no wakewords are supplied.
+                        The bot will always reply to @-mentions and direct messages, even
+                        if no wakewords are supplied.
 
 Oobabooga Seetings:
   --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want,
                         but might make sense to be the name of the bot in Discord.
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
                         wss://hostname[:port] for websocket connections over TLS.
   --log-all-the-things  Prints all oobabooga requests and responses in their entirety to
                         STDOUT
   --persona PERSONA     This prefix will be added in front of every user-supplied request.
                         This is useful for setting up a 'character' for the bot to play.
                         Alternatively, this can be set with the OOBABOT_PERSONA environment
                         variable.
+  --reply-in-thread     When set, the bot will generate a new thread for each response it
+                        generates. But it will only do so if the user who prompted the bot
+                        has thread-create permissions.
 
 Stable Diffusion Settings:
   --diffusion-steps DIFFUSION_STEPS
                         Number of diffusion steps to take when generating an image. The
                         default is 30.
   --image-height IMAGE_HEIGHT
                         Size of images to generate. This is the height of the image in
@@ -144,16 +153,16 @@
   --image-width IMAGE_WIDTH
                         Size of images to generate. This is the width of the image in
                         pixels. The default is 512.
   --image-words [IMAGE_WORDS ...]
                         One or more words that will indicate the user is requeting an image
                         to be generated.
   --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER, --sd-sampler STABLE_DIFFUSION_SAMPLER
-                        Sampler to use when generating images. If not specified, the one set
-                        on the AUTOMATIC1111 server will be used.
+                        Sampler to use when generating images. If not specified, the one
+                        set on the AUTOMATIC1111 server will be used.
   --stable-diffusion-url STABLE_DIFFUSION_URL, --sd-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server
   --sd-negative-prompt SD_NEGATIVE_PROMPT
                         Negative prompt to use when generating images. This will discourage
                         Stable Diffusion from generating images with the specified content.
                         By default, this is set to follow Discord's TOS.
   --sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW
@@ -178,14 +187,17 @@
 
     **fish example**
 
     ``` fish
     set -Ux DISCORD_TOKEN ___YOUR_TOKEN___
     ```
 
+    In certain environments, it may be difficult to set an environment variable.  In that case, you can also pass the token in as a command-line argument using `--discord-token`.  But doing so might leak the token to other
+    users on a shared sysem, as it will be visible to anyone who can run `ps`.
+
 - **`--base-url`**
 
     The base URL of oobabooga's streaming web API.  This is
     required if the oobabooga machine is different than where you're running **`oobabot`**.
 
     By default, this will be port 5005 (even though the HTML UI runs on a different port).  The protocol should typically be ws://.
 
@@ -285,15 +297,30 @@
  1. any message containing a provided wakeword (see Optional Settings)
 
 Also, the bot has a random chance of sending follow-up messages within the
 same channel if others reply within 120 seconds of its last post.  The exact
 parameters for this are in flux, but is meant to simulate a natural conversation
 flow, without forcing others to always post a wakeword.
 
+### Slash Commands
+
+As of 0.1.6, the bot now supports slash commands:
+
+| **`/command`**  | what it does |
+|---------------|------------------|
+| **`/lobotomize`** | make the bot forget everything in the channel before the command is run |
+| **`/say "message"`** | speak as the bot |
+
+Oobabot doesn't add any restrictions on who can run these commands, but luckily Discord does!  You can find this inside Discord by visiting "Server Settings" -> Integrations -> Bots and Apps -> hit the icon which looks like [/] next to your bot
+
+If you're running on a large server, you may want to restrict who can run these commands.  I suggest creating a new role, and only allowing that role to run the commands.
+
 ## Known Issues
 
 - detection of requests for photos is very crude, and will likely be improved in the future.
 - some of the default settings are very specific to my use case, and will likely be made
   configurable in the future
+- public threads in 'age restricted' channels are treated as if they
+  were not age-restricted
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

