# Comparing `tmp/grzegorz-0.4.8.tar.gz` & `tmp/grzegorz-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grzegorz-0.4.8.tar", last modified: Thu Aug 11 09:20:45 2022, max compression
+gzip compressed data, was "grzegorz-0.4.9.tar", last modified: Tue Feb 14 20:49:11 2023, max compression
```

## Comparing `grzegorz-0.4.8.tar` & `grzegorz-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwx------   0 xylous    (1000) xylous    (1001)        0 2022-08-11 09:20:45.222780 grzegorz-0.4.8/
--rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.4.8/LICENSE
--rw-------   0 xylous    (1000) xylous    (1001)     7584 2022-08-11 09:20:45.222780 grzegorz-0.4.8/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)     6917 2022-06-24 14:58:39.000000 grzegorz-0.4.8/README.md
-drwx------   0 xylous    (1000) xylous    (1001)        0 2022-08-11 09:20:45.219447 grzegorz-0.4.8/grzegorz/
--rw-------   0 xylous    (1000) xylous    (1001)        0 2022-06-15 18:44:41.000000 grzegorz-0.4.8/grzegorz/__init__.py
--rw-------   0 xylous    (1000) xylous    (1001)     6379 2022-06-25 08:52:45.000000 grzegorz-0.4.8/grzegorz/__main__.py
--rw-------   0 xylous    (1000) xylous    (1001)     4175 2022-08-11 09:15:14.000000 grzegorz-0.4.8/grzegorz/anki_integration.py
--rw-------   0 xylous    (1000) xylous    (1001)     1838 2022-07-11 08:38:44.000000 grzegorz-0.4.8/grzegorz/fetcher.py
--rw-------   0 xylous    (1000) xylous    (1001)    11509 2022-07-09 17:58:35.000000 grzegorz-0.4.8/grzegorz/generator.py
--rw-------   0 xylous    (1000) xylous    (1001)     3719 2022-07-11 13:55:54.000000 grzegorz-0.4.8/grzegorz/word.py
--rw-------   0 xylous    (1000) xylous    (1001)     3841 2022-06-25 08:54:30.000000 grzegorz-0.4.8/grzegorz/wordlist.py
-drwx------   0 xylous    (1000) xylous    (1001)        0 2022-08-11 09:20:45.222780 grzegorz-0.4.8/grzegorz.egg-info/
--rw-------   0 xylous    (1000) xylous    (1001)     7584 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)      387 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/SOURCES.txt
--rw-------   0 xylous    (1000) xylous    (1001)        1 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/dependency_links.txt
--rw-------   0 xylous    (1000) xylous    (1001)       52 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/entry_points.txt
--rw-------   0 xylous    (1000) xylous    (1001)       39 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/requires.txt
--rw-------   0 xylous    (1000) xylous    (1001)        9 2022-08-11 09:20:45.000000 grzegorz-0.4.8/grzegorz.egg-info/top_level.txt
--rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.4.8/pyproject.toml
--rw-------   0 xylous    (1000) xylous    (1001)      835 2022-08-11 09:20:45.222780 grzegorz-0.4.8/setup.cfg
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/
+-rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.4.9/LICENSE
+-rw-------   0 xylous    (1000) xylous    (1001)     7651 2023-02-14 20:49:11.377137 grzegorz-0.4.9/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)     6984 2022-12-31 17:03:16.000000 grzegorz-0.4.9/README.md
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/grzegorz/
+-rw-------   0 xylous    (1000) xylous    (1001)        0 2022-06-15 18:44:41.000000 grzegorz-0.4.9/grzegorz/__init__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     6375 2023-01-28 17:10:14.000000 grzegorz-0.4.9/grzegorz/__main__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     4174 2023-01-28 17:10:01.000000 grzegorz-0.4.9/grzegorz/anki_integration.py
+-rw-------   0 xylous    (1000) xylous    (1001)     1837 2023-01-28 17:10:05.000000 grzegorz-0.4.9/grzegorz/fetcher.py
+-rw-------   0 xylous    (1000) xylous    (1001)    12711 2023-02-13 13:45:47.000000 grzegorz-0.4.9/grzegorz/generator.py
+-rw-------   0 xylous    (1000) xylous    (1001)     2832 2023-02-13 14:30:04.000000 grzegorz-0.4.9/grzegorz/test.py
+-rw-------   0 xylous    (1000) xylous    (1001)     4569 2023-02-13 13:04:18.000000 grzegorz-0.4.9/grzegorz/word.py
+-rw-------   0 xylous    (1000) xylous    (1001)     3840 2023-01-28 17:10:22.000000 grzegorz-0.4.9/grzegorz/wordlist.py
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/grzegorz.egg-info/
+-rw-------   0 xylous    (1000) xylous    (1001)     7651 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)      404 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/SOURCES.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        1 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/dependency_links.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       52 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/entry_points.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       39 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/requires.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        9 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/top_level.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.4.9/pyproject.toml
+-rw-------   0 xylous    (1000) xylous    (1001)      835 2023-02-14 20:49:11.377137 grzegorz-0.4.9/setup.cfg
```

### Comparing `grzegorz-0.4.8/LICENSE` & `grzegorz-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grzegorz-0.4.8/PKG-INFO` & `grzegorz-0.4.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grzegorz
-Version: 0.4.8
+Version: 0.4.9
 Summary: A minimal pair generator
 Home-page: https://github.com/xylous/grzegorz
 Author: xylous
 Author-email: xylous.e@gmail.com
 Project-URL: Bug Tracker, https://github.com/xylous/grzegorz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,38 +15,44 @@
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # grzegorz
 
-`grzegorz` - a minimal pair generator. For a detailed history of the project,
-check the [Changelog](./Changelog.md)
+`grzegorz` is a minimal pair generator. For a detailed history of the project's
+development, check the [Changelog](./Changelog.md)
 
-If you already know about minimal pairs, or are just interested in linguistics,
-you can use this project as learning material.
-
-If use Anki to learn languages, you can use `grzegorz` to make an Anki deck full
-of minimal pairs, helping you learn the sounds of your target language faster.
-Check the [Usage](#usage) section!
-
-But if you're not sure what minimal pairs are and what they're used for:
-
-Consider that you're learning a new (real) language: like any beginner, you want
-to learn the phonetics, both to be able to hear words and to be able to speak
-(Tip: if you learn to it at the beginning of your journey, you won't have to
-struggle fixing bad pronunciation habits later on). But, in order to learn the
-sounds, you have to be able to differentiate between them. You won't get far if
-you keep messing up your `ou`s and `u`s in French.
-
-Enter: minimal pairs - pairs of words that differ by only *one* sound. Think:
-bit - pit (english), rue - roux (french) etc. Or, more abstractly, when you test
-yourself, a sound is played and then you have to choose between two very
-similarly spelled words. After a few tests, your ability to *know* what sound
-you heard increases, even outside of said tests.
+Minimal pairs are pairs of words that differ only very slightly, or, as
+linguists say, by one *phonological unit*, although that's just jargon. Case in
+point, they can differ:
+
+- by one sound (linguist jargon: *phoneme*) - e.g. English "bat" and "pat",
+    French "rue" and "roux"
+- by one tone (linguist jargon: *toneme*) - languages like Mandarin and
+    Vietnamese have tones
+- by the length of a sound (linguist jargon: *chroneme*) - e.g. Italian "vile"
+    and "ville",
+- when the stress is put on different syllables - e.g. English "address" (noun
+    and verb), Greek "παπά" (priest) and "πάπα" (Pope).
+
+For linguists, minimal pairs are most often used to "prove" that two
+phonological units are different within a language.
+
+But, for the average person, minimal pairs have a more practical use - language
+learning! You can make tests with them: being given the audio pronunciation of a
+word, you'll have to choose the word that you think was pronounced. Remember,
+the more similar the sounds, the harder it is to get it correct! Also, note that
+this "test" is made for both words, so you get to hear both pronunciations. With
+time, after testing yourself consistently, you'll be able to better distinguish
+the seemingly similar sounds of your target language.
+
+Luckily, `grzegorz` can make Anki flashcards with exactly these kinds of tests,
+helping you learn the sounds of your target language faster. Check the
+[Usage](#usage) section!
 
 ## Getting started
 
 ### Requirements
 
 For building:
 
@@ -61,46 +67,45 @@
 ```
 export PATH="${HOME}/.local/bin:${PATH}"
 ```
 
 #### From PyPi
 
 ```
-pip install grzegorz
+$ pip install grzegorz
 ```
 
 #### From source
 
 Clone this repository and run pip:
 
 ```
-git clone https://github.com/xylous/grzegorz grzegorz
-cd grzegorz
-pip install .
+$ git clone https://github.com/xylous/grzegorz grzegorz
+$ cd grzegorz
+$ pip install .
 ```
 
 ### Usage
 
 If you want an to get an Anki deck full of minimal pairs without having to
 bother too much with boring details, use `fullmake`:
 
 ```
-grzegorz fullmake <language> <numwords> [--clean]
+$ grzegorz fullmake <language> <numwords> [--clean]
 ```
 
 In other words, you tell it what language you want your minimal pairs in, and
 the number of words to sample (the higher the sample, the more possible minimal
 pairs found, although the runtime is longer), and, optionally, if it should
 remove the files it made when running (`--clean` option).
 
-So if you wanted to sample the 5000 most common Polish words (like me), you'd
-do:
+So if you wanted to sample the 5000 most common Polish words, you'd do:
 
 ```
-grzegorz fullmake "Polish" 5000
+$ grzegorz fullmake Polish 5000
 ```
 
 Check the "[Importing into Anki](#importing-into-anki)" section for information
 on how you can use the deck in Anki-proper.
 
 But if you want to manually go through the processes of creating a minimal pair
 deck, then read ahead.
@@ -118,58 +123,52 @@
 
 - `fetchipa <wordlist> <output-file>`, which takes the output of `wordlist` and
     creates a JSON file where all words are paired with their International
     Phonetic Alphabet spelling, which is fetched from Wiktionary.
 
 - `generate <ipa-json> <output-file> [--no-optimise | --no-phonemes |
     --keep-chronemes | --keep-stress]`, which takes the JSON file created by
-    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format
-    as well.
+    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format.
 
     Note that, by default, it's optimised: it filters out pairs with "boring"
     differences which are easy to tell apart by most people ('q' and 't', 't'
     and 'd', 'e' and 'o' etc.). Give it the `--no-optimise` option to not curate
     the list.
 
     If you would like to keep minimal pairs based on chroneme and syllable
     stress differences, use the `--keep-chronemes` and `--keep-stress` options
     respectively. They're not enabled by default since they're computationally
     intensive.
 
     In a similar fashion, you can use the `--no-phomenes` option to discard
-    minimal pairs containing a difference in sounds.
+    minimal pairs based on phoneme differences.
 
 - `makedeck <minpairs-list>`, which takes the output file of `generate` and
     creates an Anki deck package (`./grzegorz-anki-deck.apkg`) which you can
     import from inside Anki
 
 ##### Concrete example
 
-Let's assume you want to make a deck full of minimal pairs in French.
-and let's assume you didn't leave the installation directory (or else python
-won't find the `grzegorz` module):
+Let's say you want to make a deck full of minimal pairs in French, without the
+generator filtering out the "boring" pairs. Simple:
 
 ```
-grzegorz wordlist "french" 5000 wordlist.txt
-grzegorz fetchipa french-wordlist.txt french-ipas.json
-grzegorz generate french-ipas.json minpairs.json --ignore-stress
+$ grzegorz wordlist french 5000 french-wordlist.txt
+$ grzegorz fetchipa french-wordlist.txt french-ipas.json
+$ grzegorz generate --no-optimise french-ipas.json french-minpairs.json
 ```
 
-If you were to specify the wrong wordlist language, shame on you: you'll likely
-end up with the wrong International Phonetic Alphabet spellings or, worse, none
-at all.
-
 Then you could generate an Anki deck (output file: `grzegorz-anki-deck.apkg`, in
 the current directory, no matter where the input file is located):
 
 ```
-grzegorz makedeck minpairs.txt
+$ grzegorz makedeck french-minpairs.txt
 ```
 
-## Importing into Anki
+### Importing into Anki
 
 NOTE: the flashcards made don't have any audio, not because of a lack of
 interest, but because of a lack of free (as in beer) APIs or libraries that can
 (legally) furnish audio pronunciations. Forvo's API is paid! You must therefore
 add it yourself, but it won't take a lot of time.
 
 After you've created a deck package, open Anki, click on `Files` in the top left
@@ -179,23 +178,23 @@
 often you review it and whatnot.
 
 ## Roadmap
 
 - [x] fetch a wordlist of most used words in a given language
 - [x] fetch the International Phonetic Alphabet spelling for a given wordlist
 - [x] generate minimal pairs
-    - [x] optimise: look for interesting differences
-    - [x] optimise: ignore stressed syllables
-    - [x] look for phoneme contrasts
+    - [x] look for phoneme differences
+        - [x] optimise: look for interesting differences
+        - [x] optimise: ignore stressed syllables
     - [x] look for chroneme differences
     - [x] look for syllable stress differences
-- [ ] Anki integration
+- [x] Anki integration
     - [x] create Anki flashcards from the generated minimal pairs
     - [x] export a deck containing the created flashcards
-    - [ ] add audio pronunciations for every flashcard
+    - [ ] ~~add audio pronunciations for every flashcard~~
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to
 discuss what you would like to change.
 
 But, honestly, the greatest contribution you can make is to add International
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grzegorz-0.4.8/README.md` & `grzegorz-0.4.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # grzegorz
 
-`grzegorz` - a minimal pair generator. For a detailed history of the project,
-check the [Changelog](./Changelog.md)
+`grzegorz` is a minimal pair generator. For a detailed history of the project's
+development, check the [Changelog](./Changelog.md)
 
-If you already know about minimal pairs, or are just interested in linguistics,
-you can use this project as learning material.
-
-If use Anki to learn languages, you can use `grzegorz` to make an Anki deck full
-of minimal pairs, helping you learn the sounds of your target language faster.
-Check the [Usage](#usage) section!
-
-But if you're not sure what minimal pairs are and what they're used for:
-
-Consider that you're learning a new (real) language: like any beginner, you want
-to learn the phonetics, both to be able to hear words and to be able to speak
-(Tip: if you learn to it at the beginning of your journey, you won't have to
-struggle fixing bad pronunciation habits later on). But, in order to learn the
-sounds, you have to be able to differentiate between them. You won't get far if
-you keep messing up your `ou`s and `u`s in French.
-
-Enter: minimal pairs - pairs of words that differ by only *one* sound. Think:
-bit - pit (english), rue - roux (french) etc. Or, more abstractly, when you test
-yourself, a sound is played and then you have to choose between two very
-similarly spelled words. After a few tests, your ability to *know* what sound
-you heard increases, even outside of said tests.
+Minimal pairs are pairs of words that differ only very slightly, or, as
+linguists say, by one *phonological unit*, although that's just jargon. Case in
+point, they can differ:
+
+- by one sound (linguist jargon: *phoneme*) - e.g. English "bat" and "pat",
+    French "rue" and "roux"
+- by one tone (linguist jargon: *toneme*) - languages like Mandarin and
+    Vietnamese have tones
+- by the length of a sound (linguist jargon: *chroneme*) - e.g. Italian "vile"
+    and "ville",
+- when the stress is put on different syllables - e.g. English "address" (noun
+    and verb), Greek "παπά" (priest) and "πάπα" (Pope).
+
+For linguists, minimal pairs are most often used to "prove" that two
+phonological units are different within a language.
+
+But, for the average person, minimal pairs have a more practical use - language
+learning! You can make tests with them: being given the audio pronunciation of a
+word, you'll have to choose the word that you think was pronounced. Remember,
+the more similar the sounds, the harder it is to get it correct! Also, note that
+this "test" is made for both words, so you get to hear both pronunciations. With
+time, after testing yourself consistently, you'll be able to better distinguish
+the seemingly similar sounds of your target language.
+
+Luckily, `grzegorz` can make Anki flashcards with exactly these kinds of tests,
+helping you learn the sounds of your target language faster. Check the
+[Usage](#usage) section!
 
 ## Getting started
 
 ### Requirements
 
 For building:
 
@@ -42,46 +48,45 @@
 ```
 export PATH="${HOME}/.local/bin:${PATH}"
 ```
 
 #### From PyPi
 
 ```
-pip install grzegorz
+$ pip install grzegorz
 ```
 
 #### From source
 
 Clone this repository and run pip:
 
 ```
-git clone https://github.com/xylous/grzegorz grzegorz
-cd grzegorz
-pip install .
+$ git clone https://github.com/xylous/grzegorz grzegorz
+$ cd grzegorz
+$ pip install .
 ```
 
 ### Usage
 
 If you want an to get an Anki deck full of minimal pairs without having to
 bother too much with boring details, use `fullmake`:
 
 ```
-grzegorz fullmake <language> <numwords> [--clean]
+$ grzegorz fullmake <language> <numwords> [--clean]
 ```
 
 In other words, you tell it what language you want your minimal pairs in, and
 the number of words to sample (the higher the sample, the more possible minimal
 pairs found, although the runtime is longer), and, optionally, if it should
 remove the files it made when running (`--clean` option).
 
-So if you wanted to sample the 5000 most common Polish words (like me), you'd
-do:
+So if you wanted to sample the 5000 most common Polish words, you'd do:
 
 ```
-grzegorz fullmake "Polish" 5000
+$ grzegorz fullmake Polish 5000
 ```
 
 Check the "[Importing into Anki](#importing-into-anki)" section for information
 on how you can use the deck in Anki-proper.
 
 But if you want to manually go through the processes of creating a minimal pair
 deck, then read ahead.
@@ -99,58 +104,52 @@
 
 - `fetchipa <wordlist> <output-file>`, which takes the output of `wordlist` and
     creates a JSON file where all words are paired with their International
     Phonetic Alphabet spelling, which is fetched from Wiktionary.
 
 - `generate <ipa-json> <output-file> [--no-optimise | --no-phonemes |
     --keep-chronemes | --keep-stress]`, which takes the JSON file created by
-    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format
-    as well.
+    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format.
 
     Note that, by default, it's optimised: it filters out pairs with "boring"
     differences which are easy to tell apart by most people ('q' and 't', 't'
     and 'd', 'e' and 'o' etc.). Give it the `--no-optimise` option to not curate
     the list.
 
     If you would like to keep minimal pairs based on chroneme and syllable
     stress differences, use the `--keep-chronemes` and `--keep-stress` options
     respectively. They're not enabled by default since they're computationally
     intensive.
 
     In a similar fashion, you can use the `--no-phomenes` option to discard
-    minimal pairs containing a difference in sounds.
+    minimal pairs based on phoneme differences.
 
 - `makedeck <minpairs-list>`, which takes the output file of `generate` and
     creates an Anki deck package (`./grzegorz-anki-deck.apkg`) which you can
     import from inside Anki
 
 ##### Concrete example
 
-Let's assume you want to make a deck full of minimal pairs in French.
-and let's assume you didn't leave the installation directory (or else python
-won't find the `grzegorz` module):
+Let's say you want to make a deck full of minimal pairs in French, without the
+generator filtering out the "boring" pairs. Simple:
 
 ```
-grzegorz wordlist "french" 5000 wordlist.txt
-grzegorz fetchipa french-wordlist.txt french-ipas.json
-grzegorz generate french-ipas.json minpairs.json --ignore-stress
+$ grzegorz wordlist french 5000 french-wordlist.txt
+$ grzegorz fetchipa french-wordlist.txt french-ipas.json
+$ grzegorz generate --no-optimise french-ipas.json french-minpairs.json
 ```
 
-If you were to specify the wrong wordlist language, shame on you: you'll likely
-end up with the wrong International Phonetic Alphabet spellings or, worse, none
-at all.
-
 Then you could generate an Anki deck (output file: `grzegorz-anki-deck.apkg`, in
 the current directory, no matter where the input file is located):
 
 ```
-grzegorz makedeck minpairs.txt
+$ grzegorz makedeck french-minpairs.txt
 ```
 
-## Importing into Anki
+### Importing into Anki
 
 NOTE: the flashcards made don't have any audio, not because of a lack of
 interest, but because of a lack of free (as in beer) APIs or libraries that can
 (legally) furnish audio pronunciations. Forvo's API is paid! You must therefore
 add it yourself, but it won't take a lot of time.
 
 After you've created a deck package, open Anki, click on `Files` in the top left
@@ -160,23 +159,23 @@
 often you review it and whatnot.
 
 ## Roadmap
 
 - [x] fetch a wordlist of most used words in a given language
 - [x] fetch the International Phonetic Alphabet spelling for a given wordlist
 - [x] generate minimal pairs
-    - [x] optimise: look for interesting differences
-    - [x] optimise: ignore stressed syllables
-    - [x] look for phoneme contrasts
+    - [x] look for phoneme differences
+        - [x] optimise: look for interesting differences
+        - [x] optimise: ignore stressed syllables
     - [x] look for chroneme differences
     - [x] look for syllable stress differences
-- [ ] Anki integration
+- [x] Anki integration
     - [x] create Anki flashcards from the generated minimal pairs
     - [x] export a deck containing the created flashcards
-    - [ ] add audio pronunciations for every flashcard
+    - [ ] ~~add audio pronunciations for every flashcard~~
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to
 discuss what you would like to change.
 
 But, honestly, the greatest contribution you can make is to add International
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grzegorz-0.4.8/grzegorz/__main__.py` & `grzegorz-0.4.9/grzegorz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
-from .fetcher import fetchipa
-from .generator import MinPairGenerator
-from .anki_integration import makedeck
-from .wordlist import wordlist
+from fetcher import fetchipa
+from generator import MinPairGenerator
+from anki_integration import makedeck
+from wordlist import wordlist
 from os import remove
 
 # Why does it have to be this complicated?
 def create_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
             prog='grzegorz',
             description='Generate minimal pairs from a list of words')
```

### Comparing `grzegorz-0.4.8/grzegorz/anki_integration.py` & `grzegorz-0.4.9/grzegorz/anki_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from .word import MinPair, readfile
+from word import MinPair, readfile
 import genanki
 from genanki import Note, Deck
 import json
 
 """The model used for the flashcards is rather simple"""
 grzegorz_minpair_model = genanki.Model(
     1958583115, # Randomly generated Model ID. Needs to be hardcoded!
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 Public License as published by the Free Software # Foundation, either version 3
 of the License, or (at your option) any later # version. # # grzegorz is
 distributed in the hope that it will be useful, but WITHOUT ANY # WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR # A
 PARTICULAR PURPOSE. See the GNU General Public License for more details. # #
 You should have received a copy of the GNU General Public License along with #
 grzegorz. If not, see
-www.gnu.org/licenses/>. from .word import MinPair, readfile import genanki from
+www.gnu.org/licenses/>. from word import MinPair, readfile import genanki from
 genanki import Note, Deck import json """The model used for the flashcards is
 rather simple""" grzegorz_minpair_model = genanki.Model( 1958583115, # Randomly
 generated Model ID. Needs to be hardcoded! 'Grzegorz Minimal Pairs', fields=[
 {'name': 'Word 1 text'}, {'name': 'Word 1 audio'}, {'name': 'Word 1 IPA'},
 {'name': 'Word 2 text'}, {'name': 'Word 2 audio'}, {'name': 'Word 2 IPA'}, ],
 templates=[ { 'name': 'Card 1', 'qfmt': """What did you hear?
 {{Word 1 audio}}
```

### Comparing `grzegorz-0.4.8/grzegorz/fetcher.py` & `grzegorz-0.4.9/grzegorz/fetcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from .word import Word, readfile, writefile
+from word import Word, readfile, writefile
 from multiprocessing import Pool, cpu_count
 from functools import partial
 import json
 from tqdm import tqdm
 
 def fetchipa(infile: str, outfile: str) -> None:
     """
```

### Comparing `grzegorz-0.4.8/grzegorz/generator.py` & `grzegorz-0.4.9/grzegorz/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from .word import Word, MinPair, readfile, writefile
+from word import Word, MinPair, Sound, Syllable, readfile, writefile
 import json
 from tqdm import tqdm
 from itertools import chain, combinations
 import re
 
 class MinPairGenerator:
     def __init__(
@@ -64,167 +64,188 @@
 
     def check_minpair(self, pair: MinPair) -> bool:
         """
         Return True if the given pair is a minimal pair as per our options/rules,
         and False otherwise
         """
         # Skip empty entries
-        if not pair.first.sounds or not pair.last.sounds:
+        if not pair.first.phonology or not pair.last.phonology:
             return False
         # A minimal pair is kept if it has an interesting difference.
         return ((self.keep_phonemes and has_phoneme_contrast(pair, self.optimise))
                 or (self.keep_chronemes and has_chroneme_contrast(pair))
                 or (self.keep_stress and has_stress_contrast(pair)))
 
 ### Helper functions ###
 
 def has_phoneme_contrast(pair: MinPair, optimise: bool) -> bool:
-    """
-    A phoneme contrast occurs when the words in a pair are of equal length and
-    have at least one difference. If `nooptimise` is False, then, additionally, it
-    must have an interesting difference. If the above conditions are met, return
-    True, otherwise False.
-    """
-    first = pair.first
-    last = pair.last
+    first = pair.first.phonology
+    last = pair.last.phonology
+
+    # we have to work with same number of syllables
+    if len(first) != len(last):
+        return False
 
-    if len(first.sounds) != len(last.sounds):
+    syl_diffs = differences(first, last)
+    # abort if more (or less) than one syllable is different
+    if len(syl_diffs) != 1:
         return False
+    syl_diffs = syl_diffs[0]
 
-    return (differences(first, last) == 1
-            and (not optimise or is_interesting_pair(pair)))
+    # get the number of phones different in the matched syllable
+    phones_diffs = differences(syl_diffs[0].contents, syl_diffs[1].contents)
+    if len(phones_diffs) != 1 or len(syl_diffs[0].contents) != len(syl_diffs[1].contents):
+        return False
+
+    # make sure that the differences between sounds are based on phonemes, and
+    # not chronemes
+    diff = phones_diffs[0]
+    return diff[0].long == diff[1].long and \
+            (not optimise or are_interestingly_different(diff[0], diff[1]))
 
 def has_chroneme_contrast(pair: MinPair) -> bool:
-    """
-    A chroneme is a (theoretical) unit of sound that can distinguish the same
-    sound by their duration. In other words, check if the given pair has a
-    short-long sound length contrast, such as `pala` and `palla` in Italian
-    """
-    first = pair.first
-    last = pair.last
-    sounds1 = strip_stress(first.sounds)
-    sounds2 = strip_stress(last.sounds)
-
-    # Not a chroneme if they're the same length, or if the length differs by
-    # more than one sound: it's not a minimal pair
-    if len(sounds1) == len(sounds2) or abs(len(sounds1) - len(sounds2)) > 1:
+    first = pair.first.phonology
+    last = pair.last.phonology
+
+    # we have to work with same number of syllables
+    if len(first) != len(last):
         return False
 
-    # Swap, as to have the longer string in sounds1
-    if len(sounds2) > len(sounds1):
-        sounds1, sounds2 = sounds2, sounds1
-
-    num_same_sounds = 0
-    seen_chroneme = False
-    i = 0
-    j = 0
-    while(i < len(sounds1) and j < len(sounds2)):
-        s1 = sounds1[i]
-        s2 = sounds2[j]
-        try:
-            sn1 = sounds1[i+1]
-            sn2 = sounds2[j+1]
-        except IndexError:
-            sn1 = ''
-            sn2 = ''
-        # If we encounter a `ː`, or some characters are doubled, then we've
-        # encountered a chroneme
-        if s1 == s2 == sn1 != sn2 or (sn1 == s2 and sn1 == 'ː'):
-            seen_chroneme = True
-        elif s1 != s2:
-            i += 1
-            num_same_sounds -= 1
-        i += 1
-        j += 1
-        num_same_sounds += 1
-
-    # We need the words to differ only by one single sound and to know that
-    # there's a chroneme contrast between the words
-    return seen_chroneme and num_same_sounds == len(sounds2)
+    syl_diffs = differences(first, last)
+    # abort if more (or less) than one syllable is different
+    if len(syl_diffs) != 1:
+        return False
+    syl_diffs = syl_diffs[0]
+
+    # get the number of phones different in the matched syllable
+    phones_diffs = differences(syl_diffs[0].contents, syl_diffs[1].contents)
+    if len(phones_diffs) != 1 or len(syl_diffs[0].contents) != len(syl_diffs[1].contents):
+        return False
+
+    # make sure that the differences between sounds is based on sound length
+    diff = phones_diffs[0]
+    return diff[0].long != diff[1].long and diff[0].sound == diff[1].sound
 
 def has_stress_contrast(pair: MinPair) -> bool:
-    """
-    Multiple words have almost the same IPA transcription, but the stress falls
-    on different syllables.
+    first = pair.first.phonology
+    last = pair.last.phonology
 
-    If the stressless sounds of both words are the same and the words' IPAs are
-    different, then return True (i.e., it is a stress contrast)
+    # we have to work with same number of syllables
+    if len(first) != len(last):
+        return False
 
-    Concretely: /poˈte/ and /ˈpote/ (Greek) both get de-stressed to /pote/, and so
-    they form a minimal pair based on a stress contrast
-    """
-    sounds1 = pair.first.sounds
-    sounds2 = pair.last.sounds
-
-    try:
-        stress1 = sounds1.index("ˈ")
-        stress2 = sounds2.index("ˈ")
-        if (stress1 != stress2
-                and strip_stress(sounds1) == strip_stress(sounds2)):
-            return True
-    except ValueError:
-        pass
+    syl_diffs = differences(first, last)
+    # abort if more (or less) than one syllable is different
+    if len(syl_diffs) != 1:
+        return False
+    diff = syl_diffs[0]
 
-    return False
+    return diff[0].stress != diff[1].stress \
+            and diff[0].contents == diff[1].contents
 
 def strip_stress(sounds: list[str]) -> list[str]:
     """Remove stress marks from a list of sounds"""
     return [x for x in sounds if not x in ['.', 'ˈ', 'ˌ', '̯', '']]
 
 def word_with_delimited_ipa(word: Word) -> Word:
     """
     Return the same word, except its `sounds` property is filled with all the
     sounds of the IPA
     """
-    word.sounds = delimit_into_sounds(word.ipa)
+    word.phonology = parse_phonologically(word.ipa)
     return word
 
-def differences(word1: Word, word2: Word) -> int:
-    """Return the number of differences between two word's sounds"""
-    sound1 = word1.sounds
-    sound2 = word2.sounds
-    if len(sound1) != len(sound2):
-        return 0
-    count = sum(1 for a, b in zip(sound1, sound2) if a != b)
-    return count
+def differences(A: list, B: list) -> list:
+    """Given two lists, return pairs of elements that differ at the same index"""
+    return [(a, b) for a, b in zip(A, B) if a != b]
 
-def are_interestingly_different(s1: str, s2: str) -> bool:
+def are_interestingly_different(s1: Sound, s2: Sound) -> bool:
     """
     Two sounds are interestingly different if they are likely to be
     confused
     """
     for diff in INTERESTING_DIFFERENCES:
-        if s1 in diff and s2 in diff and s1 != s2:
-            return True
-    return False
-
-def is_interesting_pair(minpair: MinPair) -> bool:
-    """
-    If the given pair has an interesting difference, return True, otherwise
-    False
-    """
-    sounds1 = minpair.first.sounds
-    sounds2 = minpair.last.sounds
-    for a, b in zip(sounds1, sounds2):
-        if are_interestingly_different(a, b):
+        if s1.sound in diff and s2.sound in diff \
+                and s1.sound != s2.sound and s1.long == s2.long:
             return True
     return False
 
-def delimit_into_sounds(ipa: str) -> list[str]:
-    """Given the IPA pronunciaion of a word, return all the sounds in it"""
+def parse_ipa_characters(ipa: str) -> list[str]:
+    """ Given an IPA transliteration, return all the IPA characters in it """
     # Remove starting and ending '/'
-    sounds = ipa
+    chars = ipa.replace("/", "")
     # Some scripts use `ː` to denote vowel length, some use `:`. Don't be
     # fooled: they're not the same character! We use `ː`.
-    # Also: remove semivowel tie, as that can break things.
-    sounds = sounds.replace(":", "ː")
-    sounds = sounds.replace('̯', '')
-    sounds = re.split("(" + '|'.join(IPA_CHARACTERS) + "|[a-z])", sounds)
-    sounds = [process_transliteration(s) for s in sounds if s]
-    return sounds
+    chars = chars.replace(":", "ː")
+    # Also, remove the diphthong tie, as that can break things.
+    chars = chars.replace('̯', '')
+
+    # Do the actual splitting
+    IPA_CHARACTERS = IPA_SOUNDS + IPA_CHRONEMES + IPA_SYLLABLES
+    chars = re.split("(" + '|'.join(IPA_CHARACTERS) + "|[a-z])", chars)
+
+    return [process_transliteration(ch) for ch in chars if ch != ""]
+
+def parse_phonologically(ipa: str) -> list[Syllable]:
+    """
+    Given an IPA transliteration, parse it into a very convenient format, from a
+    phonological point of view
+    """
+    chars = parse_ipa_characters(ipa)
+    syllables = []
+    stress = "." # assume the first syllable is unemphasised
+    sounds = []
+
+    # sometimes we need to skip characters, namely chronemes: the same sound
+    # appearing consecutively is marked as one sound, but long in length
+    skip = False
+    for i in range(0, len(chars)):
+        if skip:
+            skip = False
+            continue
+
+        crnt = chars[i]
+        next = peek(chars[i :])
+
+        # If the current character isn't a syllable (stress) mark, then that
+        # means we've encountered a sound (or a chroneme character, by accident,
+        # but that's skipped). Next, figure out if the current sound is short or
+        # long
+        if not crnt in IPA_SYLLABLES:
+            is_long_sound = False
+            if next == crnt or next in IPA_CHRONEMES:
+                is_long_sound = True
+                skip = True
+            # skip chroneme characters if we've accidentally encountered them
+            if not crnt in IPA_CHRONEMES:
+                s = Sound(crnt, is_long_sound)
+                sounds.append(s)
+
+        # If we found a syllable mark, or the transcription ended, then we know
+        # that the previous syllable ends here. Thus, add all the sounds we've
+        # encountered so far to it, and prepare for a new syllable. NOTE: if
+        # we've encountered the end, then processing ends anyways
+        if crnt in IPA_SYLLABLES or i == len(chars) - 1:
+            if len(sounds) != 0:
+                syllable = Syllable(stress, sounds)
+                syllables.append(syllable)
+            stress = crnt
+            sounds = []
+
+    return syllables
+
+def peek(xs: list):
+    """
+    Return the second element in the list if that index exists, otherwise empty
+    string
+    """
+    if len(xs) <= 1:
+        return ""
+    else:
+        return xs[1]
 
 def process_transliteration(sound: str) -> str:
     """
     Return the given sound, except, if it's badly transliterated, modify
     it
     """
     if sound in BAD_TRANSLITERATIONS:
@@ -250,18 +271,17 @@
 def flatten(lst: list[list]) -> set[list]:
     """Return the set of all elements belonging to the sublists of the list"""
     return set(chain(*lst))
 
 ### CONSTANTS ###
 
 """
-The list of unicode characters that are used in IPA text and should be delimited
-correctly
+The list of unicode characters that denote sounds in IPA text
 """
-IPA_CHARACTERS = [
+IPA_SOUNDS = [
     # Consonants
     't͡ɕ', 'tɕ',
     't͡ʂ', 'tʂ',
     't͡s', 'ts',
     't͡ʃ', 'tʃ',
     'd͡ʐ', 'dʐ',
     'd͡ʑ', 'dʑ',
@@ -310,21 +330,32 @@
     'ɑ̃',
     'ɛ̃',
     'œ̃',
     'ɔ̃',
 
     # Semi-vowels
     'ɥ',
+    # diphthong tie
+    '̯',
+]
 
-    # Punctuation-related
+"""
+The list of unicode characters that denote syllables (and stress) in IPA text
+"""
+IPA_SYLLABLES = [
     '.',
     'ˈ',
     'ˌ',
+]
+
+"""
+The list of unicode characters that denote sound length in IPA text
+"""
+IPA_CHRONEMES = [
     'ː',
-    '̯',
 ]
 
 """
 We only want to deal with transliterations of these sounds that *don't* have a
 tie above them. This is the proper way to represent affricates.
 """
 BAD_TRANSLITERATIONS = ['tɕ', 'tʂ', 'ts', 'tʃ', 'dʐ', 'dʑ', 'dz', 'dʒ']
```

### Comparing `grzegorz-0.4.8/grzegorz/word.py` & `grzegorz-0.4.9/grzegorz/word.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,36 +12,65 @@
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
 from wiktionaryparser import WiktionaryParser
 import re
 
+class Sound:
+    """ Aside from a mere noise, a sound can also be long or short """
+    def __init__(self, sound: str, long: bool):
+        self.sound = sound
+        self.long = long
+
+    def __eq__(self, other) -> bool:
+        return self.sound == other.sound and \
+                self.long == other.long
+
+    def __str__(self) -> str:
+        long = ""
+        if self.long:
+            long = ":"
+        return '"' + self.sound + long + '"'
+
+class Syllable:
+    """
+    A syllable is composed of one or several sounds and can have various types
+    of stress
+    """
+    def __init__(self, stress: str, sounds: list[Sound]):
+        self.stress = stress
+        self.contents = sounds
+
+    def __eq__(self, other) -> bool:
+        return self.stress == other.stress and \
+                self.contents == other.contents
+
+    def __str__(self) -> str:
+        return "(" + repr(self.contents) + "; " + self.stress + ")"
+
 class Word:
     """
     All we care about is the word's text and its IPA
     """
     def __init__(self, text: str, ipa: str) -> None:
         self.text = text
         self.ipa = ipa
-        self.sounds = []
-
-    def set_sounds(self, sounds: list[str]) -> None:
-        self.sounds = sounds
+        self.phonology = []
 
     def get_ipa(self, language: str):
         """
         Look on the English Wiktionary for the IPA of the current word; if it
         has one, then fill its `ipa` property, otherwise don't
         """
         parser = WiktionaryParser()
         parser.set_default_language(language)
         # If we get no result, skip.
         try:
-            ipa = parse_ipa_pronunciation(parser.fetch(self.text)[0]['pronunciations']['text'][0])
+            ipa = first_ipa_pronunciation(parser.fetch(self.text)[0]['pronunciations']['text'][0])
             # Remove leading and trailing `/`, `[` and `]`
             ipa = re.sub(r"[/\[\]]", "", ipa)
             # Not all words have their IPAs on wiktionary, but they might have a
             # "Rhymes" section (try German wordlists). If we did fetch a rhyme,
             # don't add it as a valid IPA
             if ipa[0] != '-':
                 self.ipa = ipa
@@ -54,15 +83,15 @@
         """Return this class as a dictionary"""
         dict = word.__dict__
         # this might fail since the dictionary is mutated, and the same Word
         # might be converted more than one time
         try:
             # We don't need to know about the sounds of the word; those can be
             # computed
-            dict.pop('sounds')
+            dict.pop('phonology')
         except KeyError:
             pass
         return dict
 
     @staticmethod
     def from_dict(dict) -> 'Word':
         """Deserialise this class from JSON"""
@@ -87,15 +116,15 @@
         """Construct this class from a dictionary"""
         word1 = Word.from_dict(dict['first'])
         word2 = Word.from_dict(dict['last'])
         return MinPair(word1, word2)
 
 ### Helper functions ###
 
-def parse_ipa_pronunciation(ipa_str: str) -> str:
+def first_ipa_pronunciation(ipa_str: str) -> str:
     """Find the first IPA spelling in the given string"""
     return re.findall(r"[/\[].*?[/\]]", ipa_str)[0]
 
 def readfile(path: str) -> str:
     """Return the contents of a file"""
     with open(path, 'r', encoding='utf-8') as f:
         return f.read()
```

### Comparing `grzegorz-0.4.8/grzegorz/wordlist.py` & `grzegorz-0.4.9/grzegorz/wordlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
 import requests
-from .word import writefile
+from word import writefile
 
 """List of languages for which word lists can be fetched"""
 VALID_LANGUAGES = [
     # Germanic languages
     ('english', 'en'),
     ('german', 'de'),
     ('norwegian', 'no'),
```

### Comparing `grzegorz-0.4.8/grzegorz.egg-info/PKG-INFO` & `grzegorz-0.4.9/grzegorz.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grzegorz
-Version: 0.4.8
+Version: 0.4.9
 Summary: A minimal pair generator
 Home-page: https://github.com/xylous/grzegorz
 Author: xylous
 Author-email: xylous.e@gmail.com
 Project-URL: Bug Tracker, https://github.com/xylous/grzegorz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,38 +15,44 @@
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # grzegorz
 
-`grzegorz` - a minimal pair generator. For a detailed history of the project,
-check the [Changelog](./Changelog.md)
+`grzegorz` is a minimal pair generator. For a detailed history of the project's
+development, check the [Changelog](./Changelog.md)
 
-If you already know about minimal pairs, or are just interested in linguistics,
-you can use this project as learning material.
-
-If use Anki to learn languages, you can use `grzegorz` to make an Anki deck full
-of minimal pairs, helping you learn the sounds of your target language faster.
-Check the [Usage](#usage) section!
-
-But if you're not sure what minimal pairs are and what they're used for:
-
-Consider that you're learning a new (real) language: like any beginner, you want
-to learn the phonetics, both to be able to hear words and to be able to speak
-(Tip: if you learn to it at the beginning of your journey, you won't have to
-struggle fixing bad pronunciation habits later on). But, in order to learn the
-sounds, you have to be able to differentiate between them. You won't get far if
-you keep messing up your `ou`s and `u`s in French.
-
-Enter: minimal pairs - pairs of words that differ by only *one* sound. Think:
-bit - pit (english), rue - roux (french) etc. Or, more abstractly, when you test
-yourself, a sound is played and then you have to choose between two very
-similarly spelled words. After a few tests, your ability to *know* what sound
-you heard increases, even outside of said tests.
+Minimal pairs are pairs of words that differ only very slightly, or, as
+linguists say, by one *phonological unit*, although that's just jargon. Case in
+point, they can differ:
+
+- by one sound (linguist jargon: *phoneme*) - e.g. English "bat" and "pat",
+    French "rue" and "roux"
+- by one tone (linguist jargon: *toneme*) - languages like Mandarin and
+    Vietnamese have tones
+- by the length of a sound (linguist jargon: *chroneme*) - e.g. Italian "vile"
+    and "ville",
+- when the stress is put on different syllables - e.g. English "address" (noun
+    and verb), Greek "παπά" (priest) and "πάπα" (Pope).
+
+For linguists, minimal pairs are most often used to "prove" that two
+phonological units are different within a language.
+
+But, for the average person, minimal pairs have a more practical use - language
+learning! You can make tests with them: being given the audio pronunciation of a
+word, you'll have to choose the word that you think was pronounced. Remember,
+the more similar the sounds, the harder it is to get it correct! Also, note that
+this "test" is made for both words, so you get to hear both pronunciations. With
+time, after testing yourself consistently, you'll be able to better distinguish
+the seemingly similar sounds of your target language.
+
+Luckily, `grzegorz` can make Anki flashcards with exactly these kinds of tests,
+helping you learn the sounds of your target language faster. Check the
+[Usage](#usage) section!
 
 ## Getting started
 
 ### Requirements
 
 For building:
 
@@ -61,46 +67,45 @@
 ```
 export PATH="${HOME}/.local/bin:${PATH}"
 ```
 
 #### From PyPi
 
 ```
-pip install grzegorz
+$ pip install grzegorz
 ```
 
 #### From source
 
 Clone this repository and run pip:
 
 ```
-git clone https://github.com/xylous/grzegorz grzegorz
-cd grzegorz
-pip install .
+$ git clone https://github.com/xylous/grzegorz grzegorz
+$ cd grzegorz
+$ pip install .
 ```
 
 ### Usage
 
 If you want an to get an Anki deck full of minimal pairs without having to
 bother too much with boring details, use `fullmake`:
 
 ```
-grzegorz fullmake <language> <numwords> [--clean]
+$ grzegorz fullmake <language> <numwords> [--clean]
 ```
 
 In other words, you tell it what language you want your minimal pairs in, and
 the number of words to sample (the higher the sample, the more possible minimal
 pairs found, although the runtime is longer), and, optionally, if it should
 remove the files it made when running (`--clean` option).
 
-So if you wanted to sample the 5000 most common Polish words (like me), you'd
-do:
+So if you wanted to sample the 5000 most common Polish words, you'd do:
 
 ```
-grzegorz fullmake "Polish" 5000
+$ grzegorz fullmake Polish 5000
 ```
 
 Check the "[Importing into Anki](#importing-into-anki)" section for information
 on how you can use the deck in Anki-proper.
 
 But if you want to manually go through the processes of creating a minimal pair
 deck, then read ahead.
@@ -118,58 +123,52 @@
 
 - `fetchipa <wordlist> <output-file>`, which takes the output of `wordlist` and
     creates a JSON file where all words are paired with their International
     Phonetic Alphabet spelling, which is fetched from Wiktionary.
 
 - `generate <ipa-json> <output-file> [--no-optimise | --no-phonemes |
     --keep-chronemes | --keep-stress]`, which takes the JSON file created by
-    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format
-    as well.
+    `fetchipa`, and outputs the list of minimal pairs it found, in JSON format.
 
     Note that, by default, it's optimised: it filters out pairs with "boring"
     differences which are easy to tell apart by most people ('q' and 't', 't'
     and 'd', 'e' and 'o' etc.). Give it the `--no-optimise` option to not curate
     the list.
 
     If you would like to keep minimal pairs based on chroneme and syllable
     stress differences, use the `--keep-chronemes` and `--keep-stress` options
     respectively. They're not enabled by default since they're computationally
     intensive.
 
     In a similar fashion, you can use the `--no-phomenes` option to discard
-    minimal pairs containing a difference in sounds.
+    minimal pairs based on phoneme differences.
 
 - `makedeck <minpairs-list>`, which takes the output file of `generate` and
     creates an Anki deck package (`./grzegorz-anki-deck.apkg`) which you can
     import from inside Anki
 
 ##### Concrete example
 
-Let's assume you want to make a deck full of minimal pairs in French.
-and let's assume you didn't leave the installation directory (or else python
-won't find the `grzegorz` module):
+Let's say you want to make a deck full of minimal pairs in French, without the
+generator filtering out the "boring" pairs. Simple:
 
 ```
-grzegorz wordlist "french" 5000 wordlist.txt
-grzegorz fetchipa french-wordlist.txt french-ipas.json
-grzegorz generate french-ipas.json minpairs.json --ignore-stress
+$ grzegorz wordlist french 5000 french-wordlist.txt
+$ grzegorz fetchipa french-wordlist.txt french-ipas.json
+$ grzegorz generate --no-optimise french-ipas.json french-minpairs.json
 ```
 
-If you were to specify the wrong wordlist language, shame on you: you'll likely
-end up with the wrong International Phonetic Alphabet spellings or, worse, none
-at all.
-
 Then you could generate an Anki deck (output file: `grzegorz-anki-deck.apkg`, in
 the current directory, no matter where the input file is located):
 
 ```
-grzegorz makedeck minpairs.txt
+$ grzegorz makedeck french-minpairs.txt
 ```
 
-## Importing into Anki
+### Importing into Anki
 
 NOTE: the flashcards made don't have any audio, not because of a lack of
 interest, but because of a lack of free (as in beer) APIs or libraries that can
 (legally) furnish audio pronunciations. Forvo's API is paid! You must therefore
 add it yourself, but it won't take a lot of time.
 
 After you've created a deck package, open Anki, click on `Files` in the top left
@@ -179,23 +178,23 @@
 often you review it and whatnot.
 
 ## Roadmap
 
 - [x] fetch a wordlist of most used words in a given language
 - [x] fetch the International Phonetic Alphabet spelling for a given wordlist
 - [x] generate minimal pairs
-    - [x] optimise: look for interesting differences
-    - [x] optimise: ignore stressed syllables
-    - [x] look for phoneme contrasts
+    - [x] look for phoneme differences
+        - [x] optimise: look for interesting differences
+        - [x] optimise: ignore stressed syllables
     - [x] look for chroneme differences
     - [x] look for syllable stress differences
-- [ ] Anki integration
+- [x] Anki integration
     - [x] create Anki flashcards from the generated minimal pairs
     - [x] export a deck containing the created flashcards
-    - [ ] add audio pronunciations for every flashcard
+    - [ ] ~~add audio pronunciations for every flashcard~~
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to
 discuss what you would like to change.
 
 But, honestly, the greatest contribution you can make is to add International
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grzegorz-0.4.8/setup.cfg` & `grzegorz-0.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = grzegorz
-version = 0.4.8
+version = 0.4.9
 author = xylous
 author_email = xylous.e@gmail.com
 description = A minimal pair generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/xylous/grzegorz
 project_urls =
```

