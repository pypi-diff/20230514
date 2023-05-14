# Comparing `tmp/midoTrim-0.0.0.dev0.tar.gz` & `tmp/midoTrim-1.2.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midoTrim-0.0.0.dev0.tar", last modified: Sun May 14 04:44:45 2023, max compression
+gzip compressed data, was "midoTrim-1.2.10.tar", last modified: Sun May 14 04:39:58 2023, max compression
```

## Comparing `midoTrim-0.0.0.dev0.tar` & `midoTrim-1.2.10.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.273572 midoTrim-0.0.0.dev0/
--rw-rw-rw-   0        0        0      257 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/.flake8
--rw-rw-rw-   0        0        0     1078 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/LICENSE
--rw-rw-rw-   0        0        0      496 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     3486 2023-05-14 04:44:45.271775 midoTrim-0.0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2452 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.009600 midoTrim-0.0.0.dev0/docs/
--rw-rw-rw-   0        0        0     5556 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.012596 midoTrim-0.0.0.dev0/docs/_static/
--rw-rw-rw-   0        0        0       56 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/_static/PLACEHOLDER
--rw-rw-rw-   0        0        0     2962 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/about_midi.rst
--rw-rw-rw-   0        0        0      239 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/acknowledgements.rst
--rw-rw-rw-   0        0        0      254 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/authors.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.031527 midoTrim-0.0.0.dev0/docs/backends/
--rw-rw-rw-   0        0        0     1014 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/amidi.rst
--rw-rw-rw-   0        0        0     2233 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/index.rst
--rw-rw-rw-   0        0        0      920 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/portmidi.rst
--rw-rw-rw-   0        0        0      223 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/pygame.rst
--rw-rw-rw-   0        0        0     3635 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/rtmidi.rst
--rw-rw-rw-   0        0        0      509 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/backends/rtmidi_python.rst
--rw-rw-rw-   0        0        0     1365 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/bin.rst
--rw-rw-rw-   0        0        0    24677 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/changes.rst
--rw-rw-rw-   0        0        0     6161 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/code_of_conduct.rst
--rw-rw-rw-   0        0        0     8117 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/conf.py
--rw-rw-rw-   0        0        0     2257 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/contributing.rst
--rw-rw-rw-   0        0        0     1142 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/freezing.rst
--rw-rw-rw-   0        0        0     1273 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/frozen_messages.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.035514 midoTrim-0.0.0.dev0/docs/images/
--rw-rw-rw-   0        0        0    20327 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/images/midi_time.svg
--rw-rw-rw-   0        0        0     1220 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/implementing_backends.rst
--rw-rw-rw-   0        0        0     6533 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/implementing_ports.rst
--rw-rw-rw-   0        0        0     1790 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/index.rst
--rw-rw-rw-   0        0        0      783 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/installing.rst
--rw-rw-rw-   0        0        0     5133 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/intro.rst
--rw-rw-rw-   0        0        0     2345 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/lib.rst
--rw-rw-rw-   0        0        0     1115 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/license.rst
--rwxrwxrwx   0        0        0     5092 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/make.bat
--rw-rw-rw-   0        0        0     2400 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/message_types.rst
--rw-rw-rw-   0        0        0     4356 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/messages.rst
--rw-rw-rw-   0        0        0     9085 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/meta_message_types.rst
--rw-rw-rw-   0        0        0     7770 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/midi_files.rst
--rw-rw-rw-   0        0        0     2239 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/parsing.rst
--rw-rw-rw-   0        0        0     7355 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/ports.rst
--rw-rw-rw-   0        0        0     1646 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/resources.rst
--rw-rw-rw-   0        0        0     5876 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/roadmap.rst
--rw-rw-rw-   0        0        0     3857 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/socket_ports.rst
--rw-rw-rw-   0        0        0     3239 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/string_encoding.rst
--rw-rw-rw-   0        0        0      864 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/docs/syx.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.038503 midoTrim-0.0.0.dev0/examples/
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.047475 midoTrim-0.0.0.dev0/examples/backends/
--rw-rw-rw-   0        0        0      568 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/backends/printer.py
--rw-rw-rw-   0        0        0     3004 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/backends/rtm.py
--rw-rw-rw-   0        0        0      521 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/backends/use_printer.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.067426 midoTrim-0.0.0.dev0/examples/midifiles/
--rw-rw-rw-   0        0        0      836 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/create_midi_file.py
--rw-rw-rw-   0        0        0      347 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/midifile_to_json.py
--rw-rw-rw-   0        0        0      697 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/play_midi_file.py
--rw-rw-rw-   0        0        0      438 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/print_midi_file.py
--rw-rw-rw-   0        0        0      270 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/show_midifile.py
--rw-rw-rw-   0        0        0      135 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/midifiles/test.sh
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.090941 midoTrim-0.0.0.dev0/examples/ports/
--rw-rw-rw-   0        0        0      811 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/input_filter.py
--rw-rw-rw-   0        0        0      352 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/list_ports.py
--rw-rw-rw-   0        0        0      413 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/multi_receive.py
--rw-rw-rw-   0        0        0      529 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/nonblocking_receive.py
--rw-rw-rw-   0        0        0      778 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/queue_port.py
--rw-rw-rw-   0        0        0      466 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/receive.py
--rw-rw-rw-   0        0        0      777 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/ports/send.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.102867 midoTrim-0.0.0.dev0/examples/sockets/
--rw-rw-rw-   0        0        0      495 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/sockets/forward_ports.py
--rw-rw-rw-   0        0        0      817 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/sockets/serve_ports.py
--rw-rw-rw-   0        0        0      895 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/sockets/simple_client.py
--rw-rw-rw-   0        0        0      499 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/sockets/simple_server.py
--rw-rw-rw-   0        0        0      674 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/examples/using_rtmidi_directly.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.108438 midoTrim-0.0.0.dev0/extras/
--rw-rw-rw-   0        0        0      279 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/extras/README.rst
--rw-rw-rw-   0        0        0     6812 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/extras/hid_joystick.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.131371 midoTrim-0.0.0.dev0/midoTrim/
--rw-rw-rw-   0        0        0     4131 2023-05-14 04:38:50.000000 midoTrim-0.0.0.dev0/midoTrim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.172774 midoTrim-0.0.0.dev0/midoTrim/backends/
--rw-rw-rw-   0        0        0        0 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/_parser_queue.py
--rw-rw-rw-   0        0        0     3081 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/amidi.py
--rw-rw-rw-   0        0        0     6667 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/backend.py
--rw-rw-rw-   0        0        0     8869 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/portmidi.py
--rw-rw-rw-   0        0        0     4127 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/portmidi_init.py
--rw-rw-rw-   0        0        0     3645 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/pygame.py
--rw-rw-rw-   0        0        0     5345 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi.py
--rw-rw-rw-   0        0        0     3745 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi_python.py
--rw-rw-rw-   0        0        0     1351 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi_utils.py
--rw-rw-rw-   0        0        0     2295 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/frozen.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.192747 midoTrim-0.0.0.dev0/midoTrim/messages/
--rw-rw-rw-   0        0        0      293 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/checks.py
--rw-rw-rw-   0        0        0     2665 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/decode.py
--rw-rw-rw-   0        0        0     1700 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/encode.py
--rw-rw-rw-   0        0        0     7785 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/messages.py
--rw-rw-rw-   0        0        0     3368 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/specs.py
--rw-rw-rw-   0        0        0     1588 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/messages/strings.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.207373 midoTrim-0.0.0.dev0/midoTrim/midifiles/
--rw-rw-rw-   0        0        0      211 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/midifiles/__init__.py
--rw-rw-rw-   0        0        0    16200 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/midifiles/meta.py
--rw-rw-rw-   0        0        0    14207 2023-05-14 04:42:54.000000 midoTrim-0.0.0.dev0/midoTrim/midifiles/midifiles.py
--rw-rw-rw-   0        0        0     3362 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/midifiles/tracks.py
--rw-rw-rw-   0        0        0     1593 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/midifiles/units.py
--rw-rw-rw-   0        0        0     2682 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/parser.py
--rw-rw-rw-   0        0        0    11740 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/ports.py
--rw-rw-rw-   0        0        0     4386 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/sockets.py
--rw-rw-rw-   0        0        0     1496 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/syx.py
--rw-rw-rw-   0        0        0     2777 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/midoTrim/tokenizer.py
--rw-rw-rw-   0        0        0      413 2023-05-14 04:44:40.000000 midoTrim-0.0.0.dev0/midoTrim/version.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.144093 midoTrim-0.0.0.dev0/midoTrim.egg-info/
--rw-rw-rw-   0        0        0     3486 2023-05-14 04:44:44.000000 midoTrim-0.0.0.dev0/midoTrim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3069 2023-05-14 04:44:44.000000 midoTrim-0.0.0.dev0/midoTrim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:44:44.000000 midoTrim-0.0.0.dev0/midoTrim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-14 04:44:44.000000 midoTrim-0.0.0.dev0/midoTrim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.221060 midoTrim-0.0.0.dev0/scripts/
--rw-rw-rw-   0        0        0        0 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/scripts/__init__.py
--rw-rw-rw-   0        0        0      949 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/scripts/mido_connect.py
--rw-rw-rw-   0        0        0     2171 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/scripts/mido_play.py
--rw-rw-rw-   0        0        0      798 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/scripts/mido_ports.py
--rw-rw-rw-   0        0        0     1004 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/scripts/mido_serve.py
--rw-rw-rw-   0        0        0       42 2023-05-14 04:44:45.273572 midoTrim-0.0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-05-14 04:42:54.000000 midoTrim-0.0.0.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.238013 midoTrim-0.0.0.dev0/tests/
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.242859 midoTrim-0.0.0.dev0/tests/backends/
--rw-rw-rw-   0        0        0      264 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/backends/test_backend.py
--rw-rw-rw-   0        0        0      762 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/backends/test_rtmidi.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.256820 midoTrim-0.0.0.dev0/tests/messages/
--rw-rw-rw-   0        0        0      351 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/messages/test_checks.py
--rw-rw-rw-   0        0        0     1011 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/messages/test_decode.py
--rw-rw-rw-   0        0        0      685 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/messages/test_encode.py
--rw-rw-rw-   0        0        0     3435 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/messages/test_messages.py
--rw-rw-rw-   0        0        0      570 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/messages/test_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:44:45.268793 midoTrim-0.0.0.dev0/tests/midifiles/
--rw-rw-rw-   0        0        0     2848 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/midifiles/test_meta.py
--rw-rw-rw-   0        0        0     5358 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/midifiles/test_midifiles.py
--rw-rw-rw-   0        0        0      841 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/midifiles/test_tracks.py
--rw-rw-rw-   0        0        0     3495 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/midifiles/test_units.py
--rw-rw-rw-   0        0        0     1608 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_frozen.py
--rw-rw-rw-   0        0        0     3311 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_parser.py
--rw-rw-rw-   0        0        0     2168 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_ports.py
--rw-rw-rw-   0        0        0     1316 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_sockets.py
--rw-rw-rw-   0        0        0     1290 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_syx.py
--rw-rw-rw-   0        0        0     1516 2023-05-14 04:30:31.000000 midoTrim-0.0.0.dev0/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.967154 midoTrim-1.2.10/
+-rw-rw-rw-   0        0        0      257 2023-05-14 04:30:31.000000 midoTrim-1.2.10/.flake8
+-rw-rw-rw-   0        0        0     1078 2023-05-14 04:30:31.000000 midoTrim-1.2.10/LICENSE
+-rw-rw-rw-   0        0        0      496 2023-05-14 04:30:31.000000 midoTrim-1.2.10/MANIFEST.in
+-rw-rw-rw-   0        0        0     3482 2023-05-14 04:39:58.966157 midoTrim-1.2.10/PKG-INFO
+-rw-rw-rw-   0        0        0     2452 2023-05-14 04:30:31.000000 midoTrim-1.2.10/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.700077 midoTrim-1.2.10/docs/
+-rw-rw-rw-   0        0        0     5556 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.702746 midoTrim-1.2.10/docs/_static/
+-rw-rw-rw-   0        0        0       56 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/_static/PLACEHOLDER
+-rw-rw-rw-   0        0        0     2962 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/about_midi.rst
+-rw-rw-rw-   0        0        0      239 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/acknowledgements.rst
+-rw-rw-rw-   0        0        0      254 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/authors.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.720615 midoTrim-1.2.10/docs/backends/
+-rw-rw-rw-   0        0        0     1014 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/amidi.rst
+-rw-rw-rw-   0        0        0     2233 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/index.rst
+-rw-rw-rw-   0        0        0      920 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/portmidi.rst
+-rw-rw-rw-   0        0        0      223 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/pygame.rst
+-rw-rw-rw-   0        0        0     3635 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/rtmidi.rst
+-rw-rw-rw-   0        0        0      509 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/backends/rtmidi_python.rst
+-rw-rw-rw-   0        0        0     1365 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/bin.rst
+-rw-rw-rw-   0        0        0    24677 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/changes.rst
+-rw-rw-rw-   0        0        0     6161 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/code_of_conduct.rst
+-rw-rw-rw-   0        0        0     8117 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/conf.py
+-rw-rw-rw-   0        0        0     2257 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1142 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/freezing.rst
+-rw-rw-rw-   0        0        0     1273 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/frozen_messages.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.723598 midoTrim-1.2.10/docs/images/
+-rw-rw-rw-   0        0        0    20327 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/images/midi_time.svg
+-rw-rw-rw-   0        0        0     1220 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/implementing_backends.rst
+-rw-rw-rw-   0        0        0     6533 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/implementing_ports.rst
+-rw-rw-rw-   0        0        0     1790 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/index.rst
+-rw-rw-rw-   0        0        0      783 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/installing.rst
+-rw-rw-rw-   0        0        0     5133 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/intro.rst
+-rw-rw-rw-   0        0        0     2345 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/lib.rst
+-rw-rw-rw-   0        0        0     1115 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/license.rst
+-rwxrwxrwx   0        0        0     5092 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/make.bat
+-rw-rw-rw-   0        0        0     2400 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/message_types.rst
+-rw-rw-rw-   0        0        0     4356 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/messages.rst
+-rw-rw-rw-   0        0        0     9085 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/meta_message_types.rst
+-rw-rw-rw-   0        0        0     7770 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/midi_files.rst
+-rw-rw-rw-   0        0        0     2239 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/parsing.rst
+-rw-rw-rw-   0        0        0     7355 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/ports.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/resources.rst
+-rw-rw-rw-   0        0        0     5876 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/roadmap.rst
+-rw-rw-rw-   0        0        0     3857 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/socket_ports.rst
+-rw-rw-rw-   0        0        0     3239 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/string_encoding.rst
+-rw-rw-rw-   0        0        0      864 2023-05-14 04:30:31.000000 midoTrim-1.2.10/docs/syx.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.727370 midoTrim-1.2.10/examples/
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.735348 midoTrim-1.2.10/examples/backends/
+-rw-rw-rw-   0        0        0      568 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/backends/printer.py
+-rw-rw-rw-   0        0        0     3004 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/backends/rtm.py
+-rw-rw-rw-   0        0        0      521 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/backends/use_printer.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.752265 midoTrim-1.2.10/examples/midifiles/
+-rw-rw-rw-   0        0        0      836 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/create_midi_file.py
+-rw-rw-rw-   0        0        0      347 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/midifile_to_json.py
+-rw-rw-rw-   0        0        0      697 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/play_midi_file.py
+-rw-rw-rw-   0        0        0      438 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/print_midi_file.py
+-rw-rw-rw-   0        0        0      270 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/show_midifile.py
+-rw-rw-rw-   0        0        0      135 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/midifiles/test.sh
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.773810 midoTrim-1.2.10/examples/ports/
+-rw-rw-rw-   0        0        0      811 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/input_filter.py
+-rw-rw-rw-   0        0        0      352 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/list_ports.py
+-rw-rw-rw-   0        0        0      413 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/multi_receive.py
+-rw-rw-rw-   0        0        0      529 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/nonblocking_receive.py
+-rw-rw-rw-   0        0        0      778 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/queue_port.py
+-rw-rw-rw-   0        0        0      466 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/receive.py
+-rw-rw-rw-   0        0        0      777 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/ports/send.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.784784 midoTrim-1.2.10/examples/sockets/
+-rw-rw-rw-   0        0        0      495 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/sockets/forward_ports.py
+-rw-rw-rw-   0        0        0      817 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/sockets/serve_ports.py
+-rw-rw-rw-   0        0        0      895 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/sockets/simple_client.py
+-rw-rw-rw-   0        0        0      499 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/sockets/simple_server.py
+-rw-rw-rw-   0        0        0      674 2023-05-14 04:30:31.000000 midoTrim-1.2.10/examples/using_rtmidi_directly.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.790431 midoTrim-1.2.10/extras/
+-rw-rw-rw-   0        0        0      279 2023-05-14 04:30:31.000000 midoTrim-1.2.10/extras/README.rst
+-rw-rw-rw-   0        0        0     6812 2023-05-14 04:30:31.000000 midoTrim-1.2.10/extras/hid_joystick.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.814248 midoTrim-1.2.10/midoTrim/
+-rw-rw-rw-   0        0        0     4131 2023-05-14 04:38:50.000000 midoTrim-1.2.10/midoTrim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.855254 midoTrim-1.2.10/midoTrim/backends/
+-rw-rw-rw-   0        0        0        0 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/_parser_queue.py
+-rw-rw-rw-   0        0        0     3081 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/amidi.py
+-rw-rw-rw-   0        0        0     6667 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/backend.py
+-rw-rw-rw-   0        0        0     8869 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/portmidi.py
+-rw-rw-rw-   0        0        0     4127 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/portmidi_init.py
+-rw-rw-rw-   0        0        0     3645 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/pygame.py
+-rw-rw-rw-   0        0        0     5345 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/rtmidi.py
+-rw-rw-rw-   0        0        0     3745 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/rtmidi_python.py
+-rw-rw-rw-   0        0        0     1351 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/backends/rtmidi_utils.py
+-rw-rw-rw-   0        0        0     2295 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/frozen.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.873938 midoTrim-1.2.10/midoTrim/messages/
+-rw-rw-rw-   0        0        0      293 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/checks.py
+-rw-rw-rw-   0        0        0     2665 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/decode.py
+-rw-rw-rw-   0        0        0     1700 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/encode.py
+-rw-rw-rw-   0        0        0     7785 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/messages.py
+-rw-rw-rw-   0        0        0     3368 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/specs.py
+-rw-rw-rw-   0        0        0     1588 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/messages/strings.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.888557 midoTrim-1.2.10/midoTrim/midifiles/
+-rw-rw-rw-   0        0        0      211 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/midifiles/__init__.py
+-rw-rw-rw-   0        0        0    16200 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/midifiles/meta.py
+-rw-rw-rw-   0        0        0    14152 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/midifiles/midifiles.py
+-rw-rw-rw-   0        0        0     3362 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/midifiles/tracks.py
+-rw-rw-rw-   0        0        0     1593 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/midifiles/units.py
+-rw-rw-rw-   0        0        0     2682 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/parser.py
+-rw-rw-rw-   0        0        0    11740 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/ports.py
+-rw-rw-rw-   0        0        0     4386 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/sockets.py
+-rw-rw-rw-   0        0        0     1496 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/syx.py
+-rw-rw-rw-   0        0        0     2777 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/tokenizer.py
+-rw-rw-rw-   0        0        0      409 2023-05-14 04:30:31.000000 midoTrim-1.2.10/midoTrim/version.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.825556 midoTrim-1.2.10/midoTrim.egg-info/
+-rw-rw-rw-   0        0        0     3482 2023-05-14 04:39:58.000000 midoTrim-1.2.10/midoTrim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3069 2023-05-14 04:39:58.000000 midoTrim-1.2.10/midoTrim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 04:39:58.000000 midoTrim-1.2.10/midoTrim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-14 04:39:58.000000 midoTrim-1.2.10/midoTrim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.901273 midoTrim-1.2.10/scripts/
+-rw-rw-rw-   0        0        0        0 2023-05-14 04:30:31.000000 midoTrim-1.2.10/scripts/__init__.py
+-rw-rw-rw-   0        0        0      949 2023-05-14 04:30:31.000000 midoTrim-1.2.10/scripts/mido_connect.py
+-rw-rw-rw-   0        0        0     2171 2023-05-14 04:30:31.000000 midoTrim-1.2.10/scripts/mido_play.py
+-rw-rw-rw-   0        0        0      798 2023-05-14 04:30:31.000000 midoTrim-1.2.10/scripts/mido_ports.py
+-rw-rw-rw-   0        0        0     1004 2023-05-14 04:30:31.000000 midoTrim-1.2.10/scripts/mido_serve.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 04:39:58.967154 midoTrim-1.2.10/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-05-14 04:36:38.000000 midoTrim-1.2.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.918356 midoTrim-1.2.10/tests/
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.923627 midoTrim-1.2.10/tests/backends/
+-rw-rw-rw-   0        0        0      264 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/backends/test_backend.py
+-rw-rw-rw-   0        0        0      762 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/backends/test_rtmidi.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.937609 midoTrim-1.2.10/tests/messages/
+-rw-rw-rw-   0        0        0      351 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/messages/test_checks.py
+-rw-rw-rw-   0        0        0     1011 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/messages/test_decode.py
+-rw-rw-rw-   0        0        0      685 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/messages/test_encode.py
+-rw-rw-rw-   0        0        0     3435 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/messages/test_messages.py
+-rw-rw-rw-   0        0        0      570 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/messages/test_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:39:58.963168 midoTrim-1.2.10/tests/midifiles/
+-rw-rw-rw-   0        0        0     2848 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/midifiles/test_meta.py
+-rw-rw-rw-   0        0        0     5358 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/midifiles/test_midifiles.py
+-rw-rw-rw-   0        0        0      841 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/midifiles/test_tracks.py
+-rw-rw-rw-   0        0        0     3495 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/midifiles/test_units.py
+-rw-rw-rw-   0        0        0     1608 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_frozen.py
+-rw-rw-rw-   0        0        0     3311 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_parser.py
+-rw-rw-rw-   0        0        0     2168 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_ports.py
+-rw-rw-rw-   0        0        0     1316 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_sockets.py
+-rw-rw-rw-   0        0        0     1290 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_syx.py
+-rw-rw-rw-   0        0        0     1516 2023-05-14 04:30:31.000000 midoTrim-1.2.10/tests/test_tokenizer.py
```

### Comparing `midoTrim-0.0.0.dev0/LICENSE` & `midoTrim-1.2.10/LICENSE`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/PKG-INFO` & `midoTrim-1.2.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midoTrim
-Version: 0.0.0.dev0
+Version: 1.2.10
 Summary: Python的mid对象处理
 Home-page: https://github.com/TriM-Organization/mido
 Author: Ole Martin Bjørndalen, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `midoTrim-0.0.0.dev0/README.rst` & `midoTrim-1.2.10/README.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/Makefile` & `midoTrim-1.2.10/docs/Makefile`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/about_midi.rst` & `midoTrim-1.2.10/docs/about_midi.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/backends/amidi.rst` & `midoTrim-1.2.10/docs/backends/amidi.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/backends/index.rst` & `midoTrim-1.2.10/docs/backends/index.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/backends/portmidi.rst` & `midoTrim-1.2.10/docs/backends/portmidi.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/backends/rtmidi.rst` & `midoTrim-1.2.10/docs/backends/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/bin.rst` & `midoTrim-1.2.10/docs/bin.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/changes.rst` & `midoTrim-1.2.10/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/code_of_conduct.rst` & `midoTrim-1.2.10/docs/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/conf.py` & `midoTrim-1.2.10/docs/conf.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/contributing.rst` & `midoTrim-1.2.10/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/freezing.rst` & `midoTrim-1.2.10/docs/freezing.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/frozen_messages.rst` & `midoTrim-1.2.10/docs/frozen_messages.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/images/midi_time.svg` & `midoTrim-1.2.10/docs/images/midi_time.svg`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/implementing_backends.rst` & `midoTrim-1.2.10/docs/implementing_backends.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/implementing_ports.rst` & `midoTrim-1.2.10/docs/implementing_ports.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/index.rst` & `midoTrim-1.2.10/docs/index.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/installing.rst` & `midoTrim-1.2.10/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/intro.rst` & `midoTrim-1.2.10/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/lib.rst` & `midoTrim-1.2.10/docs/lib.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/license.rst` & `midoTrim-1.2.10/docs/license.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/make.bat` & `midoTrim-1.2.10/docs/make.bat`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/message_types.rst` & `midoTrim-1.2.10/docs/message_types.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/messages.rst` & `midoTrim-1.2.10/docs/messages.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/meta_message_types.rst` & `midoTrim-1.2.10/docs/meta_message_types.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/midi_files.rst` & `midoTrim-1.2.10/docs/midi_files.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/parsing.rst` & `midoTrim-1.2.10/docs/parsing.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/ports.rst` & `midoTrim-1.2.10/docs/ports.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/resources.rst` & `midoTrim-1.2.10/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/roadmap.rst` & `midoTrim-1.2.10/docs/roadmap.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/socket_ports.rst` & `midoTrim-1.2.10/docs/socket_ports.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/string_encoding.rst` & `midoTrim-1.2.10/docs/string_encoding.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/docs/syx.rst` & `midoTrim-1.2.10/docs/syx.rst`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/backends/printer.py` & `midoTrim-1.2.10/examples/backends/printer.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/backends/rtm.py` & `midoTrim-1.2.10/examples/backends/rtm.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/backends/use_printer.py` & `midoTrim-1.2.10/examples/backends/use_printer.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/midifiles/create_midi_file.py` & `midoTrim-1.2.10/examples/midifiles/create_midi_file.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/midifiles/play_midi_file.py` & `midoTrim-1.2.10/examples/midifiles/play_midi_file.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/ports/input_filter.py` & `midoTrim-1.2.10/examples/ports/input_filter.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/ports/nonblocking_receive.py` & `midoTrim-1.2.10/examples/ports/nonblocking_receive.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/ports/queue_port.py` & `midoTrim-1.2.10/examples/ports/queue_port.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/ports/send.py` & `midoTrim-1.2.10/examples/ports/send.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/sockets/serve_ports.py` & `midoTrim-1.2.10/examples/sockets/serve_ports.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/sockets/simple_client.py` & `midoTrim-1.2.10/examples/sockets/simple_client.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/examples/using_rtmidi_directly.py` & `midoTrim-1.2.10/examples/using_rtmidi_directly.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/extras/hid_joystick.py` & `midoTrim-1.2.10/extras/hid_joystick.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/__init__.py` & `midoTrim-1.2.10/midoTrim/__init__.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/_parser_queue.py` & `midoTrim-1.2.10/midoTrim/backends/_parser_queue.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/amidi.py` & `midoTrim-1.2.10/midoTrim/backends/amidi.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/backend.py` & `midoTrim-1.2.10/midoTrim/backends/backend.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/portmidi.py` & `midoTrim-1.2.10/midoTrim/backends/portmidi.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/portmidi_init.py` & `midoTrim-1.2.10/midoTrim/backends/portmidi_init.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/pygame.py` & `midoTrim-1.2.10/midoTrim/backends/pygame.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi.py` & `midoTrim-1.2.10/midoTrim/backends/rtmidi.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi_python.py` & `midoTrim-1.2.10/midoTrim/backends/rtmidi_python.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/backends/rtmidi_utils.py` & `midoTrim-1.2.10/midoTrim/backends/rtmidi_utils.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/frozen.py` & `midoTrim-1.2.10/midoTrim/frozen.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/checks.py` & `midoTrim-1.2.10/midoTrim/messages/checks.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/decode.py` & `midoTrim-1.2.10/midoTrim/messages/decode.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/encode.py` & `midoTrim-1.2.10/midoTrim/messages/encode.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/messages.py` & `midoTrim-1.2.10/midoTrim/messages/messages.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/specs.py` & `midoTrim-1.2.10/midoTrim/messages/specs.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/messages/strings.py` & `midoTrim-1.2.10/midoTrim/messages/strings.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/midifiles/meta.py` & `midoTrim-1.2.10/midoTrim/midifiles/meta.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/midifiles/midifiles.py` & `midoTrim-1.2.10/midoTrim/midifiles/midifiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
                 delta = 0
 
             yield msg.copy(time=delta)
 
             if msg.type == 'set_tempo':
                 tempo = msg.tempo
 
-    def play(self, meta_messages=False, no_delays=False):
+    def play(self, meta_messages=False):
         """Play back all tracks.
 
         The generator will sleep between each message by
         default. Messages are yielded with correct timing. The time
         attribute is set to the number of seconds slept since the
         previous message.
 
@@ -407,16 +407,15 @@
         for msg in self:
             input_time += msg.time
 
             playback_time = time.time() - start_time
             duration_to_next_event = input_time - playback_time
 
             if duration_to_next_event > 0.0:
-                if not no_delays:
-                    time.sleep(duration_to_next_event)
+                time.sleep(duration_to_next_event)
 
             if isinstance(msg, MetaMessage) and not meta_messages:
                 continue
             else:
                 yield msg
 
     def save(self, filename=None, file=None):
```

### Comparing `midoTrim-0.0.0.dev0/midoTrim/midifiles/tracks.py` & `midoTrim-1.2.10/midoTrim/midifiles/tracks.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/midifiles/units.py` & `midoTrim-1.2.10/midoTrim/midifiles/units.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/parser.py` & `midoTrim-1.2.10/midoTrim/parser.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/ports.py` & `midoTrim-1.2.10/midoTrim/ports.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/sockets.py` & `midoTrim-1.2.10/midoTrim/sockets.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/syx.py` & `midoTrim-1.2.10/midoTrim/syx.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim/tokenizer.py` & `midoTrim-1.2.10/midoTrim/tokenizer.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/midoTrim.egg-info/PKG-INFO` & `midoTrim-1.2.10/midoTrim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midoTrim
-Version: 0.0.0.dev0
+Version: 1.2.10
 Summary: Python的mid对象处理
 Home-page: https://github.com/TriM-Organization/mido
 Author: Ole Martin Bjørndalen, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `midoTrim-0.0.0.dev0/midoTrim.egg-info/SOURCES.txt` & `midoTrim-1.2.10/midoTrim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/scripts/mido_connect.py` & `midoTrim-1.2.10/scripts/mido_connect.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/scripts/mido_play.py` & `midoTrim-1.2.10/scripts/mido_play.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/scripts/mido_ports.py` & `midoTrim-1.2.10/scripts/mido_ports.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/scripts/mido_serve.py` & `midoTrim-1.2.10/scripts/mido_serve.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/setup.py` & `midoTrim-1.2.10/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 import setuptools
 import midoTrim
 
-midoTrim.midifiles.midifiles.MidiFile().play()
-
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="midoTrim",
     version=midoTrim.version.__version__,
     author="Ole Martin Bjørndalen, bgArray",
```

### Comparing `midoTrim-0.0.0.dev0/tests/backends/test_rtmidi.py` & `midoTrim-1.2.10/tests/backends/test_rtmidi.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/messages/test_decode.py` & `midoTrim-1.2.10/tests/messages/test_decode.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/messages/test_encode.py` & `midoTrim-1.2.10/tests/messages/test_encode.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/messages/test_messages.py` & `midoTrim-1.2.10/tests/messages/test_messages.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/messages/test_strings.py` & `midoTrim-1.2.10/tests/messages/test_strings.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/midifiles/test_meta.py` & `midoTrim-1.2.10/tests/midifiles/test_meta.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/midifiles/test_midifiles.py` & `midoTrim-1.2.10/tests/midifiles/test_midifiles.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/midifiles/test_tracks.py` & `midoTrim-1.2.10/tests/midifiles/test_tracks.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/midifiles/test_units.py` & `midoTrim-1.2.10/tests/midifiles/test_units.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_frozen.py` & `midoTrim-1.2.10/tests/test_frozen.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_parser.py` & `midoTrim-1.2.10/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_ports.py` & `midoTrim-1.2.10/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_sockets.py` & `midoTrim-1.2.10/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_syx.py` & `midoTrim-1.2.10/tests/test_syx.py`

 * *Files identical despite different names*

### Comparing `midoTrim-0.0.0.dev0/tests/test_tokenizer.py` & `midoTrim-1.2.10/tests/test_tokenizer.py`

 * *Files identical despite different names*

