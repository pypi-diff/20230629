# Comparing `tmp/grzegorz-0.4.9.tar.gz` & `tmp/grzegorz-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grzegorz-0.4.9.tar", last modified: Tue Feb 14 20:49:11 2023, max compression
+gzip compressed data, was "grzegorz-0.5.0.tar", last modified: Thu Jun 29 21:04:54 2023, max compression
```

## Comparing `grzegorz-0.4.9.tar` & `grzegorz-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/
--rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.4.9/LICENSE
--rw-------   0 xylous    (1000) xylous    (1001)     7651 2023-02-14 20:49:11.377137 grzegorz-0.4.9/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)     6984 2022-12-31 17:03:16.000000 grzegorz-0.4.9/README.md
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/grzegorz/
--rw-------   0 xylous    (1000) xylous    (1001)        0 2022-06-15 18:44:41.000000 grzegorz-0.4.9/grzegorz/__init__.py
--rw-------   0 xylous    (1000) xylous    (1001)     6375 2023-01-28 17:10:14.000000 grzegorz-0.4.9/grzegorz/__main__.py
--rw-------   0 xylous    (1000) xylous    (1001)     4174 2023-01-28 17:10:01.000000 grzegorz-0.4.9/grzegorz/anki_integration.py
--rw-------   0 xylous    (1000) xylous    (1001)     1837 2023-01-28 17:10:05.000000 grzegorz-0.4.9/grzegorz/fetcher.py
--rw-------   0 xylous    (1000) xylous    (1001)    12711 2023-02-13 13:45:47.000000 grzegorz-0.4.9/grzegorz/generator.py
--rw-------   0 xylous    (1000) xylous    (1001)     2832 2023-02-13 14:30:04.000000 grzegorz-0.4.9/grzegorz/test.py
--rw-------   0 xylous    (1000) xylous    (1001)     4569 2023-02-13 13:04:18.000000 grzegorz-0.4.9/grzegorz/word.py
--rw-------   0 xylous    (1000) xylous    (1001)     3840 2023-01-28 17:10:22.000000 grzegorz-0.4.9/grzegorz/wordlist.py
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-02-14 20:49:11.377137 grzegorz-0.4.9/grzegorz.egg-info/
--rw-------   0 xylous    (1000) xylous    (1001)     7651 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)      404 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/SOURCES.txt
--rw-------   0 xylous    (1000) xylous    (1001)        1 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/dependency_links.txt
--rw-------   0 xylous    (1000) xylous    (1001)       52 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/entry_points.txt
--rw-------   0 xylous    (1000) xylous    (1001)       39 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/requires.txt
--rw-------   0 xylous    (1000) xylous    (1001)        9 2023-02-14 20:49:11.000000 grzegorz-0.4.9/grzegorz.egg-info/top_level.txt
--rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.4.9/pyproject.toml
--rw-------   0 xylous    (1000) xylous    (1001)      835 2023-02-14 20:49:11.377137 grzegorz-0.4.9/setup.cfg
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/
+-rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.5.0/LICENSE
+-rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-06-29 21:04:54.954460 grzegorz-0.5.0/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)     3177 2023-06-29 21:00:50.000000 grzegorz-0.5.0/README.md
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/grzegorz/
+-rw-------   0 xylous    (1000) xylous    (1001)        0 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/__init__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     8531 2023-06-29 18:45:47.000000 grzegorz-0.5.0/grzegorz/__main__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     4156 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/anki_integration.py
+-rw-------   0 xylous    (1000) xylous    (1001)     2823 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/fetcher.py
+-rw-------   0 xylous    (1000) xylous    (1001)     9808 2023-06-29 18:44:05.000000 grzegorz-0.5.0/grzegorz/generator.py
+-rw-------   0 xylous    (1000) xylous    (1001)     3950 2023-06-26 10:32:45.000000 grzegorz-0.5.0/grzegorz/test.py
+-rw-------   0 xylous    (1000) xylous    (1001)     9448 2023-06-26 10:06:56.000000 grzegorz-0.5.0/grzegorz/word.py
+-rw-------   0 xylous    (1000) xylous    (1001)     4024 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/wordlist.py
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/grzegorz.egg-info/
+-rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)      404 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/SOURCES.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        1 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/dependency_links.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       52 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/entry_points.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       39 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/requires.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        9 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/top_level.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.5.0/pyproject.toml
+-rw-------   0 xylous    (1000) xylous    (1001)      852 2023-06-29 21:04:54.954460 grzegorz-0.5.0/setup.cfg
```

### Comparing `grzegorz-0.4.9/LICENSE` & `grzegorz-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grzegorz-0.4.9/grzegorz/__main__.py` & `grzegorz-0.5.0/grzegorz/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,39 +9,62 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-import argparse
-from fetcher import fetchipa
-from generator import MinPairGenerator
-from anki_integration import makedeck
-from wordlist import wordlist
+from grzegorz.fetcher import fetchipa
+from grzegorz.generator import (MinPairGenerator)
+from grzegorz.word import (Word)
+from grzegorz.anki_integration import makedeck
+from grzegorz.wordlist import (wordlist, print_languages_list)
+
 from os import remove
+import argparse
 
 # Why does it have to be this complicated?
 def create_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
             prog='grzegorz',
             description='Generate minimal pairs from a list of words')
     subparsers = parser.add_subparsers(dest='subparser_name')
 
+    # 'analyse' subcommand
+    parser_analyse = subparsers.add_parser('analyse',
+            help='Print the result of phonologically parsing of the given IPA transcription')
+    parser_analyse.add_argument('ipa',
+            type=str,
+            help="IPA transcription")
+
+    # 'check' subcommand
+    parser_check = subparsers.add_parser('check',
+            help='Check if the two given IPAs can form minimal pair')
+    parser_check .add_argument('ipa_first',
+            type=str,
+            help="first IPA transcription")
+    parser_check .add_argument('ipa_second',
+            type=str,
+            help="second IPA transcription")
+
+    # 'list-languages' subcommand
+    subparsers.add_parser('list-languages',
+            help='List all languages for which you can fetch a wordlist')
+
     # 'fullmake' command
     parser_fullmake = subparsers.add_parser('fullmake',
             help='Build an Anki deck for a language automatically')
     parser_fullmake.add_argument('language',
             type=str)
     parser_fullmake.add_argument('numwords',
             type=int,
             help='number of words to sample')
     parser_fullmake.add_argument('--clean',
-            dest="clean",
-            action="store_true",
+            dest='clean',
+            action='store_true',
             default=False,
             help='remove temporary files after building the deck')
 
     # 'wordlist' command
     parser_wordlist = subparsers.add_parser('wordlist',
             help='Fetch the word list for a given language, containing a certain number of words')
     parser_wordlist.add_argument('language',
@@ -59,14 +82,19 @@
             help='Fetch all IPA pronunciations for the words into a JSON file')
     parser_fetchipa.add_argument('infile',
             type=str,
             help='file containing the list of words')
     parser_fetchipa.add_argument('outfile',
             type=str,
             help='output file (JSON)')
+    parser_fetchipa.add_argument('--keep-failed',
+            dest='keep_failed',
+            action='store_true',
+            default=False,
+            help='Save the words for which no IPA was found in the output file (default: don\'t)')
 
     # 'generate' subcommand
     parser_generate = subparsers.add_parser('generate',
             help='Create minimal pairs, given a JSON input file')
     parser_generate.add_argument('infile',
             type=str,
             help='JSON file created by fetchipa')
@@ -79,57 +107,67 @@
             dest="nooptimise",
             help="generate all possible minimal pairs (default: optimise)")
     parser_generate.add_argument('--no-phonemes',
             action='store_true',
             default=False,
             dest="no_phonemes",
             help="ignore minimal pairs containing a phoneme contrast")
-    parser_generate.add_argument('--keep-chronemes',
+    parser_generate.add_argument('--no-chronemes',
             action='store_true',
             default=False,
-            dest="keep_chronemes",
-            help="keep minimal pairs containing a chroneme contrast (default: don't)")
-    parser_generate.add_argument('--keep-stress',
+            dest="no_chronemes",
+            help="ignore minimal pairs containing a chroneme contrast")
+    parser_generate.add_argument('--no-stress',
             action='store_true',
             default=False,
-            dest="keep_stress",
-            help="keep minimal pairs with a difference in syllable stress (default: don't)")
+            dest="no_stress",
+            help="ignore minimal pairs with a difference in syllable stress")
+    parser_generate.add_argument('-f', '--filter-file',
+            type=str,
+            dest="path",
+            help="path to the file whose contents determine the phones to keep when optimising")
 
     # 'makedeck' subcommand
     parser_makedeck = subparsers.add_parser('makedeck',
             help='Create an Anki deck package containing all minimal pairs')
     parser_makedeck.add_argument('infile',
             type=str,
             help="Output file of 'generate'")
+    parser_makedeck.add_argument('outfile',
+            type=str,
+            help="Output file; note that it should ideally have the .apkg extension")
+
     return parser
 
 def fullmake(language: str, numwords: int, clean: bool) -> None:
     """
     Practically: wrap all commands into one. If `clean` is True, then
     temporary files created by this function are removed.
     """
     optimise = True
     keep_phonemes = True
-    keep_chronemes = False
-    keep_stress = False
+    keep_chronemes = True
+    keep_stress = True
 
     wordlist_file = language + "-wordlist.txt"
     ipa_json = language + "-ipa.json"
     minpairs_file = language + "-minpairs.json"
+    makedeck_file = "grzegorz-" + language + "-minpairs.apkg"
 
-    wordlist(language, numwords, wordlist_file)
-    fetchipa(wordlist_file, ipa_json)
+    if wordlist(language, numwords, wordlist_file) == 1:
+        exit(1)
+    fetchipa(wordlist_file, ipa_json, False)
     g = MinPairGenerator(
         optimise,
         keep_phonemes,
         keep_chronemes,
         keep_stress,
     )
     g.generate(ipa_json, minpairs_file)
-    makedeck(minpairs_file)
+    makedeck(minpairs_file, makedeck_file)
 
     if clean:
         print("Removing temporary files...")
         remove(wordlist_file)
         remove(ipa_json)
         remove(minpairs_file)
 
@@ -145,34 +183,47 @@
             numwords = args.numwords
             language = args.language.lower()
             fullmake(language, numwords, clean)
         case 'wordlist':
             outfile = args.outfile
             numwords = args.numwords
             language = args.language.lower()
-            wordlist(language, numwords, outfile)
+            status = wordlist(language, numwords, outfile)
+            exit(status)
         case 'fetchipa':
-            infile = args.infile
-            outfile = args.outfile
-            fetchipa(infile, outfile)
+            fetchipa(args.infile, args.outfile, args.keep_failed)
         case 'generate':
             infile = args.infile
             outfile = args.outfile
             nooptimise = args.nooptimise;
             no_phonemes = args.no_phonemes;
-            keep_chronemes = args.keep_chronemes;
-            keep_stress = args.keep_stress;
+            no_chronemes = args.no_chronemes;
+            no_stress = args.no_stress;
+            filter_file_path = args.path
             g = MinPairGenerator(
                 not nooptimise,
                 not no_phonemes,
-                keep_chronemes,
-                keep_stress
+                not no_chronemes,
+                not no_stress
             )
+            if filter_file_path is not None:
+                g.set_filter_pairs_from_file(filter_file_path)
             g.generate(infile, outfile)
         case 'makedeck':
             infile = args.infile
-            makedeck(infile)
+            outfile = args.outfile
+            makedeck(infile, outfile)
+        case 'analyse':
+            Word("", args.ipa).print_human_readable()
+        case 'check':
+            word1 = Word("", args.ipa_first)
+            word2 = Word("", args.ipa_second)
+            generator = MinPairGenerator(False, True, True, True)
+            if not generator.print_human_readable_check(word1, word2):
+                exit(1)
+        case 'list-languages':
+            print_languages_list()
         case _:
             parser.print_help()
 
 if __name__ == "__main__":
     main()
```

### Comparing `grzegorz-0.4.9/grzegorz/anki_integration.py` & `grzegorz-0.5.0/grzegorz/anki_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from word import MinPair, readfile
+from grzegorz.word import MinPair, readfile
+
 import genanki
 from genanki import Note, Deck
 import json
 
 """The model used for the flashcards is rather simple"""
 grzegorz_minpair_model = genanki.Model(
     1958583115, # Randomly generated Model ID. Needs to be hardcoded!
@@ -116,22 +117,22 @@
 
 .center {
     display: inline;
     padding: 10px;
 }""",
 )
 
-def makedeck(infile: str) -> None:
+def makedeck(infile: str, outfile: str) -> None:
     """Create an Anki deck given a file full of minimal pairs"""
     json_str = readfile(infile)
     dict = json.loads(json_str)
     minpairs = list(map(MinPair.from_dict, dict))
     notes = list(map(minpair_to_anki_note, minpairs))
     deck = notes_to_deck(notes)
-    export_deck(deck)
+    export_deck(deck, outfile)
 
 ### HELPER FUNCTIONS ###
 
 def minpair_to_anki_note(minpair: MinPair) -> Note:
     """
     Given a minimal pair, create an Anki note from it, with grzegorz_minpair_model
     as its model.
@@ -159,12 +160,11 @@
         1597757363,
         "grzegorz's minimal pairs",
     )
     for note in notes:
         deck.add_note(note)
     return deck
 
-def export_deck(deck: Deck) -> None:
-    """Package the given deck and write it to a file: grzegorz-anki-deck.apkg"""
-    outfile = 'grzegorz-anki-deck.apkg'
+def export_deck(deck: Deck, outfile: str) -> None:
+    """Package the given deck and write it to a file"""
     genanki.Package(deck).write_to_file(outfile)
     print('Done! Now import', outfile, 'in your Anki')
```

#### html2text {}

```diff
@@ -4,21 +4,22 @@
 Public License as published by the Free Software # Foundation, either version 3
 of the License, or (at your option) any later # version. # # grzegorz is
 distributed in the hope that it will be useful, but WITHOUT ANY # WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR # A
 PARTICULAR PURPOSE. See the GNU General Public License for more details. # #
 You should have received a copy of the GNU General Public License along with #
 grzegorz. If not, see
-www.gnu.org/licenses/>. from word import MinPair, readfile import genanki from
-genanki import Note, Deck import json """The model used for the flashcards is
-rather simple""" grzegorz_minpair_model = genanki.Model( 1958583115, # Randomly
-generated Model ID. Needs to be hardcoded! 'Grzegorz Minimal Pairs', fields=[
-{'name': 'Word 1 text'}, {'name': 'Word 1 audio'}, {'name': 'Word 1 IPA'},
-{'name': 'Word 2 text'}, {'name': 'Word 2 audio'}, {'name': 'Word 2 IPA'}, ],
-templates=[ { 'name': 'Card 1', 'qfmt': """What did you hear?
+www.gnu.org/licenses/>. from grzegorz.word import MinPair, readfile import
+genanki from genanki import Note, Deck import json """The model used for the
+flashcards is rather simple""" grzegorz_minpair_model = genanki.Model
+( 1958583115, # Randomly generated Model ID. Needs to be hardcoded! 'Grzegorz
+Minimal Pairs', fields=[ {'name': 'Word 1 text'}, {'name': 'Word 1 audio'},
+{'name': 'Word 1 IPA'}, {'name': 'Word 2 text'}, {'name': 'Word 2 audio'},
+{'name': 'Word 2 IPA'}, ], templates=[ { 'name': 'Card 1', 'qfmt': """What did
+you hear?
 {{Word 1 audio}}
 {{Word 1 text}}
 {{Word 1 IPA}}
 or
 {{Word 2 text}}
 {{Word 2 IPA}}
 """, 'afmt': """{{FrontSide}}
@@ -37,23 +38,23 @@
 You heard:
 {{Word 2 text}}
 """, }, ], css= """.card { font-family: arial; font-size: 20px; text-align:
 center; color: black; background-color: white; } .word { text-align: center;
 border: 3px outset black; display: inline-block; box-sizing: border-box; }
 .nightMode .word { border: 3px outset white; } .minpair { display: flex;
 justify-content: center; align-items: center; } .center { display: inline;
-padding: 10px; }""", ) def makedeck(infile: str) -> None: """Create an Anki
-deck given a file full of minimal pairs""" json_str = readfile(infile) dict =
-json.loads(json_str) minpairs = list(map(MinPair.from_dict, dict)) notes = list
-(map(minpair_to_anki_note, minpairs)) deck = notes_to_deck(notes) export_deck
-(deck) ### HELPER FUNCTIONS ### def minpair_to_anki_note(minpair: MinPair) -
-> Note: """ Given a minimal pair, create an Anki note from it, with
-grzegorz_minpair_model as its model. """ first = minpair.first last =
-minpair.last note = genanki.Note( model=grzegorz_minpair_model, fields=
-[ first.text, '', first.ipa, last.text, '', last.ipa, ] ) return note def
-notes_to_deck(notes: list[Note]) -> Deck: """ Add a list of notes into a deck
-called "grzegorz's minimal pairs" """ deck = genanki.Deck( 1597757363,
-"grzegorz's minimal pairs", ) for note in notes: deck.add_note(note) return
-deck def export_deck(deck: Deck) -> None: """Package the given deck and write
-it to a file: grzegorz-anki-deck.apkg""" outfile = 'grzegorz-anki-deck.apkg'
-genanki.Package(deck).write_to_file(outfile) print('Done! Now import', outfile,
-'in your Anki')
+padding: 10px; }""", ) def makedeck(infile: str, outfile: str) -> None:
+"""Create an Anki deck given a file full of minimal pairs""" json_str =
+readfile(infile) dict = json.loads(json_str) minpairs = list(map
+(MinPair.from_dict, dict)) notes = list(map(minpair_to_anki_note, minpairs))
+deck = notes_to_deck(notes) export_deck(deck, outfile) ### HELPER FUNCTIONS ###
+def minpair_to_anki_note(minpair: MinPair) -> Note: """ Given a minimal pair,
+create an Anki note from it, with grzegorz_minpair_model as its model. """
+first = minpair.first last = minpair.last note = genanki.Note
+( model=grzegorz_minpair_model, fields=[ first.text, '', first.ipa, last.text,
+'', last.ipa, ] ) return note def notes_to_deck(notes: list[Note]) -> Deck: """
+Add a list of notes into a deck called "grzegorz's minimal pairs" """ deck =
+genanki.Deck( 1597757363, "grzegorz's minimal pairs", ) for note in notes:
+deck.add_note(note) return deck def export_deck(deck: Deck, outfile: str) -
+> None: """Package the given deck and write it to a file""" genanki.Package
+(deck).write_to_file(outfile) print('Done! Now import', outfile, 'in your
+Anki')
```

### Comparing `grzegorz-0.4.9/grzegorz/fetcher.py` & `grzegorz-0.5.0/grzegorz/fetcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,41 +9,71 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from word import Word, readfile, writefile
+from grzegorz.word import Word, readfile, writefile
+
+from wiktionaryparser import WiktionaryParser
 from multiprocessing import Pool, cpu_count
 from functools import partial
-import json
 from tqdm import tqdm
+import json
+import re
 
-def fetchipa(infile: str, outfile: str) -> None:
+def fetchipa(infile: str, outfile: str, keep_failed: bool) -> None:
     """
     Given an input file containing a list of words separated, fetch the IPAs and
     create a JSON file with their IPA spellings matched to their text
     """
 
     # For speed reasons, we use parallelism
     numproc = 10 * cpu_count()
 
     contents = readfile(infile).splitlines()
     language = contents.pop(0)
-    words = [Word(line, '') for line in contents if line]
+    words = [line for line in contents if line]
     wds = []
     numwords = len(words)
 
     print("Fetching IPA spellings for", numwords, language, "words...")
     if numwords > 500:
         print("If you cancel, all progress will be lost!")
     with Pool(numproc) as p:
-        for x in tqdm(p.imap_unordered(partial(Word.get_ipa, language=language),
+        for x in tqdm(p.imap_unordered(partial(get_ipa_for_word, language=language),
             words), total=numwords):
             wds.append(x)
 
     # Don't keep entries with no IPA pronunciation
-    wds = [w for w in wds if w.ipa]
+    if not keep_failed:
+        wds = [w for w in wds if w.ipa]
 
     jsonlog = json.dumps([Word.obj_dict(word) for word in wds])
     writefile(outfile, jsonlog)
+
+### HELPER FUNCTIONS ###
+
+def get_ipa_for_word(word: str, language: str) -> Word:
+    """
+    Look on the English Wiktionary for the IPA of the given word
+    """
+    parser = WiktionaryParser()
+    parser.set_default_language(language)
+    ipa = ""
+    # If we get no result, skip.
+    try:
+        ipa = first_ipa_pronunciation(parser.fetch(word)[0]['pronunciations']['text'][0])
+        # Not all words have their IPAs on wiktionary, but they might have a
+        # "Rhymes" section (try German wordlists). If we did fetch a rhyme,
+        # don't add it as a valid IPA
+        if ipa[0] == '-':
+            ipa = ""
+    except (IndexError, AttributeError, KeyError) as _:
+        pass
+
+    return Word(word, ipa)
+
+def first_ipa_pronunciation(ipa_str: str) -> str:
+    """Find the first IPA spelling in the given string"""
+    return re.findall(r"[/\[].*?[/\]]", ipa_str)[0]
```

### Comparing `grzegorz-0.4.9/grzegorz/generator.py` & `grzegorz-0.5.0/grzegorz/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,393 +9,253 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from word import Word, MinPair, Sound, Syllable, readfile, writefile
+from grzegorz.word import (Word, MinPair, readfile, writefile,
+                           PHONEME_MINPAIR, CHRONEME_MINPAIR, STRESS_MINPAIR,
+                           NOT_MINPAIR)
+
 import json
 from tqdm import tqdm
 from itertools import chain, combinations
-import re
 
 class MinPairGenerator:
     def __init__(
         self,
         optimise: bool,
         keep_phonemes: bool,
         keep_chronemes: bool,
         keep_stress: bool,
     ) -> None:
         self.optimise = optimise
+        # used for phonemes only; maybe rename?
+        self.filter_pairs = DEFAULT_FILTER_PAIRS
         self.keep_phonemes = keep_phonemes
         self.keep_chronemes = keep_chronemes
         self.keep_stress = keep_stress
 
+    def set_filter_pairs_from_file(self, path: str) -> None:
+        """NOTE: the file must have comma-separated values, with the phones that
+        form chains together on the same line"""
+        contents = readfile(path).split("\n")
+        lists_of_phonemes = []
+        for line in contents:
+            if line != "":
+                lists_of_phonemes.append(line.replace(" ", "").split(","))
+        self.filter_pairs = phoneme_lists_to_phoneme_pairs(lists_of_phonemes)
+
     def generate(self, infile: str, outfile: str) -> None:
         """
         Given the path to a file containing JSON data about serialised `Word`s, create
         a file `outfile` with all the minimal pairs found, in JSON format
         """
         jsonstr = readfile(infile)
         words = json.loads(jsonstr, object_hook=Word.from_dict)
-        words = list(map(word_with_delimited_ipa, words))
         minpairs = []
 
         if not self.keep_phonemes and not self.keep_chronemes and not self.keep_stress:
             print("Generator: skipping all contrasts means no minimal pairs will be generated; abort")
             return
         if not self.keep_phonemes:
             print("Generator: phoneme contrasts will be ignored")
-        if self.keep_chronemes:
-            print("Generator: chroneme contrasts will be kept")
-        if self.keep_stress:
-            print("Generator: syllable stress contrasts will be kept")
+        if not self.keep_chronemes:
+            print("Generator: chroneme contrasts will be ignored")
+        if not self.keep_stress:
+            print("Generator: syllable stress contrasts will be ignored")
 
         for i in tqdm(range(0,len(words))):
             for j in range(i+1,len(words)):
                 pair = MinPair(words[i], words[j])
                 if self.check_minpair(pair):
                     minpairs.append(pair)
 
         json_out = json.dumps([MinPair.obj_dict(pair) for pair in minpairs])
         writefile(outfile, json_out)
         print('Done! Generated', len(minpairs), 'minimal pairs')
 
-    def check_minpair(self, pair: MinPair) -> bool:
+    def check_minpair(self, pair: MinPair) -> int:
         """
-        Return True if the given pair is a minimal pair as per our options/rules,
-        and False otherwise
+        If the given pair si not a minpair, return NOT_MINPAIR; otherwise,
+        return, per case, PHONEME_MINPAIR, CHRONEME_MINPAIR and STRESS_MINPAIR
         """
         # Skip empty entries
         if not pair.first.phonology or not pair.last.phonology:
             return False
         # A minimal pair is kept if it has an interesting difference.
-        return ((self.keep_phonemes and has_phoneme_contrast(pair, self.optimise))
-                or (self.keep_chronemes and has_chroneme_contrast(pair))
-                or (self.keep_stress and has_stress_contrast(pair)))
-
-### Helper functions ###
+        if self.keep_phonemes and self.check_phoneme_contrast(pair):
+            return PHONEME_MINPAIR
+        elif self.keep_chronemes and self.check_chroneme_contrast(pair):
+            return CHRONEME_MINPAIR
+        elif self.keep_stress and self.check_stress_contrast(pair):
+            return STRESS_MINPAIR
+        else:
+            return NOT_MINPAIR
 
-def has_phoneme_contrast(pair: MinPair, optimise: bool) -> bool:
-    first = pair.first.phonology
-    last = pair.last.phonology
-
-    # we have to work with same number of syllables
-    if len(first) != len(last):
-        return False
+    def check_optimised_phone_pair(self, s1: str, s2: str) -> bool:
+        """
+        Two sounds are interestingly different if they are likely to be confused
+        """
+        for diff in self.filter_pairs:
+            if s1 in diff and s2 in diff and s1 != s2:
+                return True
+        return False
+
+    def print_human_readable_check(self, word1: Word, word2: Word) -> int:
+        word1.print_human_readable()
+        print("")
+        word2.print_human_readable()
+        print("")
+        verdict = self.check_minpair(MinPair(word1, word2))
+        if verdict == PHONEME_MINPAIR:
+            print("minimal pair based on phoneme difference")
+        elif verdict == CHRONEME_MINPAIR:
+            print("minimal pair based on chroneme difference")
+        elif verdict == STRESS_MINPAIR:
+            print("minimal pair based on syllable stress difference")
+        else:
+            print("not minimal pair")
+        return verdict
+
+    def check_phoneme_contrast(self, pair: MinPair) -> bool:
+        first = pair.first.phonology
+        last = pair.last.phonology
 
-    syl_diffs = differences(first, last)
-    # abort if more (or less) than one syllable is different
-    if len(syl_diffs) != 1:
-        return False
-    syl_diffs = syl_diffs[0]
+        # we have to work with same number of syllables
+        if len(first) != len(last):
+            return False
 
-    # get the number of phones different in the matched syllable
-    phones_diffs = differences(syl_diffs[0].contents, syl_diffs[1].contents)
-    if len(phones_diffs) != 1 or len(syl_diffs[0].contents) != len(syl_diffs[1].contents):
-        return False
+        diffs = []
+        for i in range(0, len(first)):
+            syl1 = first[i].contents
+            syl2 = last[i].contents
+            if len(syl1) != len(syl2):
+                return False
+            for j in range(0, len(syl1)):
+                if syl1[j].sound != syl2[j].sound:
+                    diffs.append((syl1[j].sound, syl2[j].sound))
 
-    # make sure that the differences between sounds are based on phonemes, and
-    # not chronemes
-    diff = phones_diffs[0]
-    return diff[0].long == diff[1].long and \
-            (not optimise or are_interestingly_different(diff[0], diff[1]))
-
-def has_chroneme_contrast(pair: MinPair) -> bool:
-    first = pair.first.phonology
-    last = pair.last.phonology
+        if len(diffs) != 1:
+            return False
 
-    # we have to work with same number of syllables
-    if len(first) != len(last):
-        return False
+        return (not self.optimise or self.check_optimised_phone_pair(diffs[0][0], diffs[0][1]))
 
-    syl_diffs = differences(first, last)
-    # abort if more (or less) than one syllable is different
-    if len(syl_diffs) != 1:
-        return False
-    syl_diffs = syl_diffs[0]
+    def check_chroneme_contrast(self, pair: MinPair) -> bool:
+        first = pair.first.phonology
+        last = pair.last.phonology
 
-    # get the number of phones different in the matched syllable
-    phones_diffs = differences(syl_diffs[0].contents, syl_diffs[1].contents)
-    if len(phones_diffs) != 1 or len(syl_diffs[0].contents) != len(syl_diffs[1].contents):
-        return False
-
-    # make sure that the differences between sounds is based on sound length
-    diff = phones_diffs[0]
-    return diff[0].long != diff[1].long and diff[0].sound == diff[1].sound
-
-def has_stress_contrast(pair: MinPair) -> bool:
-    first = pair.first.phonology
-    last = pair.last.phonology
+        # we have to work with same number of syllables
+        if len(first) != len(last):
+            return False
 
-    # we have to work with same number of syllables
-    if len(first) != len(last):
-        return False
+        # find the number of chroneme differences; if, at any point, we
+        # encounter a differnt sound, then we know the words are too different
+        # apart, and so return False
+        chroneme_diffs = 0
+        for i in range(0, len(first)):
+            syl1 = first[i].contents
+            syl2 = last[i].contents
+            if len(syl1) != len(syl2):
+                return False
+            for j in range(0, len(syl1)):
+                if syl1[j].sound != syl2[j].sound:
+                    return False
+                elif syl1[j].long != syl2[j].long:
+                    chroneme_diffs += 1
+
+        return chroneme_diffs >= 1
+
+    def check_stress_contrast(self, pair: MinPair) -> bool:
+        first = pair.first.phonology
+        last = pair.last.phonology
 
-    syl_diffs = differences(first, last)
-    # abort if more (or less) than one syllable is different
-    if len(syl_diffs) != 1:
-        return False
-    diff = syl_diffs[0]
+        # we have to work with same number of syllables
+        if len(first) != len(last):
+            return False
 
-    return diff[0].stress != diff[1].stress \
-            and diff[0].contents == diff[1].contents
+        fst_stress = []
+        snd_stress = []
+        for i in range(0, len(first)):
+            if first[i].contents != last[i].contents:
+                return False
+            fst_stress += first[i].stress
+            snd_stress += last[i].stress
 
-def strip_stress(sounds: list[str]) -> list[str]:
-    """Remove stress marks from a list of sounds"""
-    return [x for x in sounds if not x in ['.', 'ˈ', 'ˌ', '̯', '']]
+        return fst_stress != snd_stress
 
-def word_with_delimited_ipa(word: Word) -> Word:
-    """
-    Return the same word, except its `sounds` property is filled with all the
-    sounds of the IPA
-    """
-    word.phonology = parse_phonologically(word.ipa)
-    return word
+### Helper functions ###
 
 def differences(A: list, B: list) -> list:
     """Given two lists, return pairs of elements that differ at the same index"""
     return [(a, b) for a, b in zip(A, B) if a != b]
 
-def are_interestingly_different(s1: Sound, s2: Sound) -> bool:
-    """
-    Two sounds are interestingly different if they are likely to be
-    confused
-    """
-    for diff in INTERESTING_DIFFERENCES:
-        if s1.sound in diff and s2.sound in diff \
-                and s1.sound != s2.sound and s1.long == s2.long:
-            return True
-    return False
-
-def parse_ipa_characters(ipa: str) -> list[str]:
-    """ Given an IPA transliteration, return all the IPA characters in it """
-    # Remove starting and ending '/'
-    chars = ipa.replace("/", "")
-    # Some scripts use `ː` to denote vowel length, some use `:`. Don't be
-    # fooled: they're not the same character! We use `ː`.
-    chars = chars.replace(":", "ː")
-    # Also, remove the diphthong tie, as that can break things.
-    chars = chars.replace('̯', '')
-
-    # Do the actual splitting
-    IPA_CHARACTERS = IPA_SOUNDS + IPA_CHRONEMES + IPA_SYLLABLES
-    chars = re.split("(" + '|'.join(IPA_CHARACTERS) + "|[a-z])", chars)
-
-    return [process_transliteration(ch) for ch in chars if ch != ""]
-
-def parse_phonologically(ipa: str) -> list[Syllable]:
-    """
-    Given an IPA transliteration, parse it into a very convenient format, from a
-    phonological point of view
-    """
-    chars = parse_ipa_characters(ipa)
-    syllables = []
-    stress = "." # assume the first syllable is unemphasised
-    sounds = []
-
-    # sometimes we need to skip characters, namely chronemes: the same sound
-    # appearing consecutively is marked as one sound, but long in length
-    skip = False
-    for i in range(0, len(chars)):
-        if skip:
-            skip = False
-            continue
-
-        crnt = chars[i]
-        next = peek(chars[i :])
-
-        # If the current character isn't a syllable (stress) mark, then that
-        # means we've encountered a sound (or a chroneme character, by accident,
-        # but that's skipped). Next, figure out if the current sound is short or
-        # long
-        if not crnt in IPA_SYLLABLES:
-            is_long_sound = False
-            if next == crnt or next in IPA_CHRONEMES:
-                is_long_sound = True
-                skip = True
-            # skip chroneme characters if we've accidentally encountered them
-            if not crnt in IPA_CHRONEMES:
-                s = Sound(crnt, is_long_sound)
-                sounds.append(s)
-
-        # If we found a syllable mark, or the transcription ended, then we know
-        # that the previous syllable ends here. Thus, add all the sounds we've
-        # encountered so far to it, and prepare for a new syllable. NOTE: if
-        # we've encountered the end, then processing ends anyways
-        if crnt in IPA_SYLLABLES or i == len(chars) - 1:
-            if len(sounds) != 0:
-                syllable = Syllable(stress, sounds)
-                syllables.append(syllable)
-            stress = crnt
-            sounds = []
-
-    return syllables
-
-def peek(xs: list):
-    """
-    Return the second element in the list if that index exists, otherwise empty
-    string
-    """
-    if len(xs) <= 1:
-        return ""
-    else:
-        return xs[1]
-
-def process_transliteration(sound: str) -> str:
-    """
-    Return the given sound, except, if it's badly transliterated, modify
-    it
-    """
-    if sound in BAD_TRANSLITERATIONS:
-        # evil unicode hack
-        sound = sound[0] + 't͡ɕ'[1] + sound[1]
-    return sound
-
-def parse_differences_chain(diffs_chain: list[str]) -> list[tuple[str]]:
+def phoneme_list_to_pairs(phoneme_list: list[str]) -> list[tuple[str]]:
     """
     Hardcoding is a bad practice. And tiresome as well. Especially when you add a
     new sound: you have to manually add so many pairs!
 
-    Thus, we use chains of sounds: ['a', 'e', 'o'] returns the list of
-    interesting differences `('a', 'e')`, `('a', 'o')`, `('e', 'o')` so
-    basically all powersets of range two.
+    Thus, we use lists of phonemes to group similar sounds together. For
+    example, ['a', 'e', 'o'] gets turned into the following pairs of phonemes:
+    `('a', 'e')`, `('a', 'o')`, `('e', 'o')`. Practically, this functions
+    returns  all powersets of range two.
     """
-    s = list(diffs_chain)
+    s = list(phoneme_list)
     # range(2, 2+1) returns all tuples that are exactly 2 in length - exactly
     # what we need
     pairs = chain.from_iterable(combinations(s, r) for r in range(2, 2+1))
     return list(pairs)
 
 def flatten(lst: list[list]) -> set[list]:
     """Return the set of all elements belonging to the sublists of the list"""
     return set(chain(*lst))
 
-### CONSTANTS ###
-
-"""
-The list of unicode characters that denote sounds in IPA text
-"""
-IPA_SOUNDS = [
-    # Consonants
-    't͡ɕ', 'tɕ',
-    't͡ʂ', 'tʂ',
-    't͡s', 'ts',
-    't͡ʃ', 'tʃ',
-    'd͡ʐ', 'dʐ',
-    'd͡ʑ', 'dʑ',
-    'd͡z', 'dz',
-    'd͡ʒ', 'dʒ',
-    'ʂ',
-    'ɕ',
-    'ɲ',
-    'ŋ',
-    'ɡʲ',
-    'xʲ',
-    'ʐ',
-    'ʑ',
-    'ś',
-    'ɡ',
-    'ʁ',
-    'ʃ',
-    'ʒ',
-    'ɟ',
-    'ɫ',
-    'ʎ',
-    'ç',
-    'ɣ',
-    'sʲ',
-    'zʲ',
-
-    # Oral vowels
-    'ɔ',
-    'ɛ',
-    'ɪ',
-    'ɨ',
-    'ø',
-    'ə',
-    'ɑ',
-    'œ',
-    'æ',
-    'ʌ',
-    'ɐ',
-    'ɤ',
-    'ɒ',
-    'ʊ',
-    'ʉ',
-    'ɵ',
-
-    # Nasal vowels
-    'ɑ̃',
-    'ɛ̃',
-    'œ̃',
-    'ɔ̃',
-
-    # Semi-vowels
-    'ɥ',
-    # diphthong tie
-    '̯',
-]
-
-"""
-The list of unicode characters that denote syllables (and stress) in IPA text
-"""
-IPA_SYLLABLES = [
-    '.',
-    'ˈ',
-    'ˌ',
-]
-
-"""
-The list of unicode characters that denote sound length in IPA text
-"""
-IPA_CHRONEMES = [
-    'ː',
-]
+def phoneme_lists_to_phoneme_pairs(phoneme_lists: list[list[str]]) -> set[list]:
+    """
+    Given a list of lists of phonemes, return the combined set of all phoneme
+    pairs made from every individual list.
+    """
+    return flatten(list(map(phoneme_list_to_pairs, phoneme_lists)))
 
-"""
-We only want to deal with transliterations of these sounds that *don't* have a
-tie above them. This is the proper way to represent affricates.
-"""
-BAD_TRANSLITERATIONS = ['tɕ', 'tʂ', 'ts', 'tʃ', 'dʐ', 'dʑ', 'dz', 'dʒ']
+### CONSTANTS ###
 
 """
 All sounds in a particular chain are hard to be distinguished from each other.
 
 Therefore, they form pairs of "interesting differences", which are used to
 filter out all other "boring" minimal pairs: for example, "i" and "l" are so
 far away phonetically they're easily distinguishable by anyone!
 """
-INTERESTING_DIFFERENCES_CHAINS = [
+DEFAULT_FILTER_PAIRS_PHONEME_LISTS = [
     # Consonants
     ['t͡ɕ', 't͡ʂ', 't͡s', 't͡ʃ', 'd͡ʐ', 'd͡ʑ', 'd͡z', 'd͡ʒ',
         'ʂ', 'ʒ', 'ʃ', 'ɕ', 'zʲ', 'sʲ'],
     ['n', 'ɲ', 'ŋ'],
     ['v', 'f'],
     ['x', 'h', 'xʲ', 'ç'],
     ['z', 'ʑ', 'ʐ', 's', 'ś', 'ʂ'],
     ['ʎ', 'ɫ', 'l'],
-    ['ɟ', 'j', 'g', 'ɡʲ', 'g'],
+    ['ɟ', 'j', 'g', 'ɡʲ', 'g', 'ç'],
+    ['tʲ', 'tʰ', 't' ,'d', 'dʲ', 'dʰ'],
+    ['r', 'ʁ'],
 
     # Oral vowels (and semi-vowels)
-    ['ɑ', 'a', 'ɐ', 'ə', 'ʌ', 'æ'],
+    ['ɑ', 'a', 'ɐ', 'ə', 'ʌ', 'æ', 'ä', 'ɐ̯'],
+    ['ɑ', 'ə', 'œ'],
     ['e', 'ɛ', 'ɪ', 'æ'],
     ['ɨ', 'i', 'j', 'ɪ'],
     ['ɔ', 'o', 'ø', 'œ', 'ɵ'],
     ['ɥ', 'j'],
-    ['ɥ', 'u', 'ɤ', 'y', 'w', 'ɒ', 'ʊ', 'ʉ'],
+    ['ɥ', 'u', 'ɤ', 'y', 'w', 'ɒ', 'ʊ', 'ʉ', 'ʊ̯'],
     ['i', 'e'],
 
     # Nasal vowels
     ['ɛ̃', 'ɛ'],
     ['ɛ̃', 'ə'],
     ['ɔ̃', 'ɔ'],
     ['œ̃', 'œ', 'ɔ'],
     ['ɛ̃', 'ɔ̃', 'œ̃', 'ɑ̃'],
 ]
 
 """Precomputed constant, to avoid hardcoding everything."""
-INTERESTING_DIFFERENCES = flatten(list(
-                            map(parse_differences_chain,
-                                INTERESTING_DIFFERENCES_CHAINS)))
+DEFAULT_FILTER_PAIRS = phoneme_lists_to_phoneme_pairs(DEFAULT_FILTER_PAIRS_PHONEME_LISTS)
```

### Comparing `grzegorz-0.4.9/grzegorz/wordlist.py` & `grzegorz-0.5.0/grzegorz/wordlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
+from grzegorz.word import writefile
+
 import requests
-from word import writefile
 
 """List of languages for which word lists can be fetched"""
 VALID_LANGUAGES = [
     # Germanic languages
     ('english', 'en'),
     ('german', 'de'),
     ('norwegian', 'no'),
@@ -61,32 +62,36 @@
     ('chinese', 'zh'),
     ('japanese', 'ja'),
 ]
 
 """This is where all the lists are fetched from"""
 RESOURCES_REPO_LINK = 'https://raw.githubusercontent.com/hermitdave/FrequencyWords/master/content/2016'
 
-def wordlist(lang, numwords, outfile):
+def wordlist(lang, numwords, outfile) -> int:
     """
     Fetch a word list of `numwords` and put it into `outfile` for the given
     language, if it's valid
-    NOTE: the language name should be all lowercase
+    If the operation failed, then return 1, otherwise return 0
     """
     language = lang_name(lang)
     if not valid_lang(lang):
         print(lang, "? I can't fetch a wordlist for that", sep='')
-        return
+        return 1
     link = wordlist_link_for_lang(lang)
     words_kept_slice = slice(0, numwords)
     raw_words = fetch_contents(link).splitlines()[words_kept_slice]
     raw_words = list(map(format_line, raw_words))
     raw_words.insert(0, language)
     writefile(outfile, '\n'.join(raw_words))
     print("Fetched", numwords, language, "words into", outfile)
-    return
+    return 0
+
+def print_languages_list() -> None:
+    for (lang, code) in sorted(VALID_LANGUAGES, key=lambda pair: pair[1]):
+        print(code, ", ", lang, sep="")
 
 ### HELPER FUNCTIONS ###
 
 def valid_lang(lang):
     """We only accept languages that are on the list"""
     for pair in VALID_LANGUAGES:
         if lang in pair:
```

### Comparing `grzegorz-0.4.9/setup.cfg` & `grzegorz-0.5.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = grzegorz
-version = 0.4.9
+version = 0.5.0
 author = xylous
 author_email = xylous.e@gmail.com
-description = A minimal pair generator
+description = Minimal pair generator and phonetics tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/xylous/grzegorz
 project_urls = 
 	Bug Tracker = https://github.com/xylous/grzegorz/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

