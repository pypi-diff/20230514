# Comparing `tmp/discord_pretty_help-2.0.3.tar.gz` & `tmp/discord_pretty_help-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_pretty_help-2.0.3.tar", max compression
+gzip compressed data, was "discord_pretty_help-2.0.4.tar", max compression
```

## Comparing `discord_pretty_help-2.0.3.tar` & `discord_pretty_help-2.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-05-11 00:54:19.082441 discord_pretty_help-2.0.3/LICENSE
--rw-r--r--   0        0        0      105 2023-05-12 22:33:28.714632 discord_pretty_help-2.0.3/pretty_help/__init__.py
--rw-r--r--   0        0        0      500 2023-05-11 00:54:19.096444 discord_pretty_help-2.0.3/pretty_help/abc_menu.py
--rw-r--r--   0        0        0     4197 2023-05-12 22:24:49.371197 discord_pretty_help-2.0.3/pretty_help/app_menu.py
--rw-r--r--   0        0        0     5332 2023-05-11 00:54:19.097444 discord_pretty_help-2.0.3/pretty_help/emoji_menu.py
--rw-r--r--   0        0        0    22753 2023-05-12 22:23:41.300783 discord_pretty_help-2.0.3/pretty_help/pretty_help.py
--rw-r--r--   0        0        0      748 2023-05-12 22:32:31.632523 discord_pretty_help-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3784 2023-05-12 22:34:44.353758 discord_pretty_help-2.0.3/README.md
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-29 11:31:31.530107 discord_pretty_help-2.0.4/LICENSE
+-rw-r--r--   0        0        0      105 2023-05-14 10:50:13.591307 discord_pretty_help-2.0.4/pretty_help/__init__.py
+-rw-r--r--   0        0        0      500 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.4/pretty_help/abc_menu.py
+-rw-r--r--   0        0        0     4197 2023-05-14 04:50:39.398654 discord_pretty_help-2.0.4/pretty_help/app_menu.py
+-rw-r--r--   0        0        0     5332 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.4/pretty_help/emoji_menu.py
+-rw-r--r--   0        0        0    23111 2023-05-14 10:49:47.368955 discord_pretty_help-2.0.4/pretty_help/pretty_help.py
+-rw-r--r--   0        0        0      748 2023-05-14 08:41:21.929133 discord_pretty_help-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3952 2023-05-14 10:49:13.991504 discord_pretty_help-2.0.4/README.md
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.4/PKG-INFO
```

### Comparing `discord_pretty_help-2.0.3/LICENSE` & `discord_pretty_help-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.3/pretty_help/app_menu.py` & `discord_pretty_help-2.0.4/pretty_help/app_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.3/pretty_help/emoji_menu.py` & `discord_pretty_help-2.0.4/pretty_help/emoji_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.3/pretty_help/pretty_help.py` & `discord_pretty_help-2.0.4/pretty_help/pretty_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,31 +129,34 @@
         Args:
             embed (discord.Embed): The page to add command descriptions
             page_title (str): The title of the page
             commands_list(List[Union[commands.Command, app_commands.commands.Command]]): The list of commands for the fields
         """
 
         for command in command_list:
+            command_name = command.name
+            if group or isinstance(command, commands.Group):
+                command_name = "🔗 " + command_name
             if isinstance(command, commands.Command):
                 short_doc = command.short_doc
             else:
                 short_doc = command.description.split("\n", 1)[0]
             if not self._check_embed(
                 embed,
                 self.ending_note,
-                command.name,
+                command_name,
                 short_doc,
                 self.prefix,
                 self.suffix,
             ):
                 self._add_page(embed)
                 embed = self._new_page(page_title, embed.description)
 
             embed.add_field(
-                name=f"🔗 {command.name}" if group else command.name,
+                name=command_name, 
                 value=f'{self.prefix}{short_doc or "No Description"}{self.suffix}',
                 inline=False,
             )
 
         self._add_page(embed)
 
     @staticmethod
@@ -311,31 +314,35 @@
     dm_help: Optional[:class:`bool`]
         A tribool that indicates if the help command should DM the user instead of
         sending it to the channel it received it from. If the boolean is set to
         ``True``, then all help output is DM'd. If ``False``, none of the help
         output is DM'd. If ``None``, then the bot will only DM when the help
         message becomes too long (dictated by more than :attr:`dm_help_threshold` characters).
         Defaults to ``False``.
-    menu: Optional[:class:`pretty_help.PrettyMenu`]
-        The menu to use for navigating pages. Default is :class:`pretty_help.DefaultMenu`
-        Custom menus should inherit from :class:`pretty_help.PrettyMenu`
     ending_note: Optional[:class:`str`]
         The footer in of the help embed
+    image_url: Optional[:class:`str`]
+        The url of the image to be used on the embed
     index_title: :class: `str`
         The string used when the index page is shown. Defaults to ``"Categories"``
+    menu: Optional[:class:`pretty_help.PrettyMenu`]
+        The menu to use for navigating pages. Default is :class:`pretty_help.DefaultMenu`
+        Custom menus should inherit from :class:`pretty_help.PrettyMenu`
     no_category: :class:`str`
         The string used when there is a command which does not belong to any category(cog).
         Useful for i18n. Defaults to ``"No Category"``
-    sort_commands: :class:`bool`
-        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
+    paginator: :class: `pretty_help.Paginator`
+        The paginator to use. One is created by default.
+    send_typing: :class: `bool`
+        A bool that indicates if the bot will send a typing indicator. Defaults to ``True``
     show_index: class: `bool`
         A bool that indicates if the index page should be shown listing the available cogs
         Defaults to ``True``.
-    image_url: Optional[:class:`str`]
-        The url of the image to be used on the embed
+    sort_commands: :class:`bool`
+        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
     thumbnail_url: Optional[:class:`str`]
         The url of the thumbnail to be used on the embed
     """
 
     def __init__(
         self,
         case_insensitive: Optional[bool] = False,
@@ -346,18 +353,20 @@
         dm_help: Optional[bool] = False,
         ending_note: Optional[str] = "",
         image_url: Optional[str] = None,
         index_title: Optional[str] = "Categories",
         menu: Optional[PrettyMenu] = AppMenu(),
         no_category: Optional[str] = "No Category",
         paginator: Optional[Paginator] = None,
+        send_typing:Optional[bool] = True,
         show_index: Optional[bool] = True,
         sort_commands: Optional[bool] = True,
         thumbnail_url: Optional[str] = None,
         **options,
+
     ):
         self.dm_help = dm_help
         self.index_title = index_title
         self.no_category = no_category
         self.sort_commands = sort_commands
         self.menu = menu
         self.paginator = paginator or Paginator(
@@ -365,14 +374,15 @@
             color=color,
             image_url=image_url,
             thumbnail_url=thumbnail_url,
         )
         self.case_insensitive = case_insensitive
         self.ending_note = ending_note
         self.delete_invoke = delete_invoke
+        self.send_typing = send_typing
 
         super().__init__(**options)
 
     def _add_to_bot(self, bot: commands.Bot) -> None:
         super()._add_to_bot(bot)
         self.bot = bot
         bot.tree.add_command(self._app_command_callback)
@@ -484,46 +494,46 @@
             filter(
                 lambda cmd: isinstance(cmd, app_commands.commands.Command)
                 and not isinstance(cmd, commands.hybrid.HybridAppCommand)
                 and cmd.name != "help",
                 bot.tree.get_commands(),
             )
         )
-        async with channel.typing():
-            mapping = {name: [] for name in mapping}
-            help_filtered = (
-                filter(lambda c: c.name != "help", bot.commands)
-                if len(bot.commands) > 1
-                else bot.commands
-            )
-            for cmd in (
-                await self.filter_commands(
-                    help_filtered,
-                    sort=self.sort_commands,
-                )
-                + app_mapping
-            ):
-                if hasattr(cmd, "binding"):
-                    mapping[cmd.binding].append(cmd)
-                else:
-                    mapping[cmd.cog].append(cmd)
-
-            self.paginator.add_cog(self.no_category, mapping.pop(None))
-            sorted_map = sorted(
-                mapping.items(),
-                key=lambda cg: cg[0].qualified_name
-                if isinstance(cg[0], commands.Cog)
-                else str(cg[0]),
+        if self.send_typing:
+            await channel.typing()
+        mapping = {name: [] for name in mapping}
+        help_filtered = (
+            filter(lambda c: c.name != "help", bot.commands)
+            if len(bot.commands) > 1
+            else bot.commands
+        )
+        for cmd in (
+            await self.filter_commands(
+                help_filtered,
+                sort=self.sort_commands,
             )
-            for cog, command_list in sorted_map:
-                # if a cog has the app_command attribute, it's an AppGroup Cog
-                if cog.app_command:
-                    command_list += cog.app_command.commands
-                self.paginator.add_cog(cog, command_list)
-            self.paginator.add_index(self.index_title, bot)
+            + app_mapping
+        ):
+            if hasattr(cmd, "binding"):
+                mapping[cmd.binding].append(cmd)
+            else:
+                mapping[cmd.cog].append(cmd)
+        self.paginator.add_cog(self.no_category, mapping.pop(None))
+        sorted_map = sorted(
+            mapping.items(),
+            key=lambda cg: cg[0].qualified_name
+            if isinstance(cg[0], commands.Cog)
+            else str(cg[0]),
+        )
+        for cog, command_list in sorted_map:
+            # if a cog has the app_command attribute, it's an AppGroup Cog
+            if cog.app_command:
+                command_list += cog.app_command.commands
+            self.paginator.add_cog(cog, command_list)
+        self.paginator.add_index(self.index_title, bot)
         await self.send_pages()
 
     def get_app_command_signature(self, command: app_commands.commands.Command):
         """
         Returns the application command signature
 
         Args:
@@ -565,30 +575,32 @@
     async def send_command_help(self, command: commands.Command):
         filtered = await self.filter_commands([command])
         if filtered:
             self.paginator.add_command(command, self.get_command_signature(command))
             await self.send_pages()
 
     async def send_group_help(self, group: commands.Group):
-        async with self.get_destination().typing():
-            filtered = await self.filter_commands(
-                group.commands, sort=self.sort_commands
-            )
-            self.paginator.add_group(group, filtered)
+        if self.send_typing:
+            await self.get_destination().typing()
+        filtered = await self.filter_commands(
+            group.commands, sort=self.sort_commands
+        )
+        self.paginator.add_group(group, filtered)
         await self.send_pages()
 
     async def send_cog_help(self, cog: commands.Cog):
-        async with self.get_destination().typing():
-            filtered = await self.filter_commands(
-                cog.get_commands(), sort=self.sort_commands
-            )
-            filtered += await self.filter_app_commands(cog.get_app_commands())
-            if cog.app_command:
-                filtered += await self.filter_app_commands(cog.app_command.commands)
-            self.paginator.add_cog(cog, filtered)
+        if self.send_typing:
+            await self.get_destination().typing()
+        filtered = await self.filter_commands(
+            cog.get_commands(), sort=self.sort_commands
+        )
+        filtered += await self.filter_app_commands(cog.get_app_commands())
+        if cog.app_command:
+            filtered += await self.filter_app_commands(cog.app_command.commands)
+        self.paginator.add_cog(cog, filtered)
         await self.send_pages()
 
     async def send_error_message(self, error: str, /) -> None:
         """Check if the context is from an app command or text command and send an error message"""
         if self.context.interaction:
             return await self.context.interaction.response.send_message(
                 error, ephemeral=True
```

### Comparing `discord_pretty_help-2.0.3/pyproject.toml` & `discord_pretty_help-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-pretty-help"
-version = "2.0.3"
+version = "2.0.4"
 description = "And nicer looking interactive help menu for discord.py"
 authors = ["CasuallyCalm <29642143+casuallycalm@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/casuallycalm/discord-pretty-help"
 keywords=["discord", "discord.py", "discord bot"]
 packages = [
```

### Comparing `discord_pretty_help-2.0.3/README.md` & `discord_pretty_help-2.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 - `color` - Set the default embed color
 - `delete_invoke` - Delete the message that invoked the help command. Requires message delete permission. Defaults is `False`
 - `ending_note` - Set the footer of the embed. Ending notes are fed a `commands.Context` (`ctx`) and a `PrettyHelp` (`help`) instance for more advanced customization.
 - `image_url` - The url of the image to be used on the embed
 - `index_title` - Set the index page name default is *"Categories"*
 - `menu` - The menu to use for navigating pages. Uses a `pretty_help.PrettyMenu()` instance. Default is `pretty_help.AppMenu()`
 - `no_category` - Set the name of the page with commands not part of a category. Default is "*No Category*"
-- `sort_commands` - Sort commands and categories alphabetically
+- `paginator`- The paginator to use. One is created by default.
+- `send_typing` - A bool that indicates if the bot will send a typing indicator. Defaults to ``True``
 - `show_index` - Show the index page or not
+- `sort_commands` - Sort commands and categories alphabetically
 - `thumbnail_url` - The url of the thumbnail to be used on the embed
 
 ## Menus
 
 ### pretty_help.EmojiMenu 
 - Uses Emojis to navigate
 - `active_time` - Set the time (in seconds) that the message will be active. Default is 30s
```

### Comparing `discord_pretty_help-2.0.3/PKG-INFO` & `discord_pretty_help-2.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-pretty-help
-Version: 2.0.3
+Version: 2.0.4
 Summary: And nicer looking interactive help menu for discord.py
 Home-page: https://github.com/casuallycalm/discord-pretty-help
 License: MIT
 Keywords: discord,discord.py,discord bot
 Author: CasuallyCalm
 Author-email: 29642143+casuallycalm@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -49,16 +49,18 @@
 - `color` - Set the default embed color
 - `delete_invoke` - Delete the message that invoked the help command. Requires message delete permission. Defaults is `False`
 - `ending_note` - Set the footer of the embed. Ending notes are fed a `commands.Context` (`ctx`) and a `PrettyHelp` (`help`) instance for more advanced customization.
 - `image_url` - The url of the image to be used on the embed
 - `index_title` - Set the index page name default is *"Categories"*
 - `menu` - The menu to use for navigating pages. Uses a `pretty_help.PrettyMenu()` instance. Default is `pretty_help.AppMenu()`
 - `no_category` - Set the name of the page with commands not part of a category. Default is "*No Category*"
-- `sort_commands` - Sort commands and categories alphabetically
+- `paginator`- The paginator to use. One is created by default.
+- `send_typing` - A bool that indicates if the bot will send a typing indicator. Defaults to ``True``
 - `show_index` - Show the index page or not
+- `sort_commands` - Sort commands and categories alphabetically
 - `thumbnail_url` - The url of the thumbnail to be used on the embed
 
 ## Menus
 
 ### pretty_help.EmojiMenu 
 - Uses Emojis to navigate
 - `active_time` - Set the time (in seconds) that the message will be active. Default is 30s
```

