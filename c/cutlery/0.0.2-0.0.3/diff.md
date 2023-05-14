# Comparing `tmp/cutlery-0.0.2.tar.gz` & `tmp/cutlery-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutlery-0.0.2.tar", last modified: Tue Oct 18 11:31:03 2022, max compression
+gzip compressed data, was "cutlery-0.0.3.tar", last modified: Tue Oct 18 13:52:33 2022, max compression
```

## Comparing `cutlery-0.0.2.tar` & `cutlery-0.0.3.tar`

### file list

```diff
@@ -1,229 +1,230 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.952883 cutlery-0.0.2/
--rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-10-18 11:30:50.000000 cutlery-0.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-10-18 11:31:03.952883 cutlery-0.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      893 2022-10-18 11:30:50.000000 cutlery-0.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.920883 cutlery-0.0.2/cutlery/
--rw-r--r--   0 vsts      (1001) docker     (121)      120 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      333 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_bbpe.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     5099 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_bbpe.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_spp.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_spp.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_wordpiece.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/_wordpiece.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)      156 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/config.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/merges.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1470 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/merges.hh
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.920883 cutlery-0.0.2/cutlery/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)       19 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/incorrect-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     6291 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/robbert-merges-1000.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    16815 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/robbert-vocab-1000.json
--rw-r--r--   0 vsts      (1001) docker     (121)     1741 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/test_bbpe_processor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3640 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/test_sp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1095 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/test_word_piece_processor.py
--rw-r--r--   0 vsts      (1001) docker     (121)       31 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/toy-word-pieces.txt
--rw-r--r--   0 vsts      (1001) docker     (121)   253270 2022-10-18 11:30:50.000000 cutlery-0.0.2/cutlery/tests/toy.model
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.920883 cutlery-0.0.2/cutlery.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-10-18 11:31:03.000000 cutlery-0.0.2/cutlery.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    10016 2022-10-18 11:31:03.000000 cutlery-0.0.2/cutlery.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-18 11:31:03.000000 cutlery-0.0.2/cutlery.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-10-18 11:31:03.000000 cutlery-0.0.2/cutlery.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-18 11:31:03.000000 cutlery-0.0.2/cutlery.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-10-18 11:30:50.000000 cutlery-0.0.2/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.916883 cutlery-0.0.2/sentencepiece/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.920883 cutlery-0.0.2/sentencepiece/python/
--rw-r--r--   0 vsts      (1001) docker     (121)     5858 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/python/once.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/src/
--rw-r--r--   0 vsts      (1001) docker     (121)     6648 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9294 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    10322 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4416 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4850 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    18401 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builder.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     5102 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builder.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7354 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/src/builtin_pb/
--rw-r--r--   0 vsts      (1001) docker     (121)    35154 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    40648 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 vsts      (1001) docker     (121)   130839 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (121)   189303 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1304 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1061 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3525 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1782 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1265 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2506 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6007 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/common.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5713 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4167 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/error.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     3563 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/filesystem.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1577 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2345 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/freelist.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1221 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1341 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/init.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5359 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/init_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1644 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (121)      972 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1743 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6609 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     9527 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_interface.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15932 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)  7198605 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11633 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/normalizer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     5835 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/normalizer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16156 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2024 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    30990 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    19673 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 vsts      (1001) docker     (121)    47605 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     9966 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6527 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13402 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    10493 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spec_parser.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6557 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2035 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4163 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    12142 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1026 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/test_main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1899 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/testharness.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     8718 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/testharness.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2103 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1104 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1656 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    25917 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     5727 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19808 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2807 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unicode_script.h
--rw-r--r--   0 vsts      (1001) docker     (121)   106446 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1525 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    31219 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6912 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32258 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    18625 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     3879 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3321 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     7746 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/util.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    11414 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12866 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/util_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1124 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2101 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1372 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2464 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.916883 cutlery-0.0.2/sentencepiece/third_party/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.916883 cutlery-0.0.2/sentencepiece/third_party/absl/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/third_party/absl/container/
--rw-r--r--   0 vsts      (1001) docker     (121)     1001 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)      966 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 vsts      (1001) docker     (121)     5614 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1673 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 vsts      (1001) docker     (121)      799 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 vsts      (1001) docker     (121)     2592 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.940883 cutlery-0.0.2/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 vsts      (1001) docker     (121)     1309 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1012 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1447 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1088 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2413 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2127 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7856 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/string_view.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    20934 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.944883 cutlery-0.0.2/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 vsts      (1001) docker     (121)    51750 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.944883 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 vsts      (1001) docker     (121)    15726 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     8985 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     5975 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    30847 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    10999 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    82338 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     3573 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    30000 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.916883 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.948883 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 vsts      (1001) docker     (121)     6215 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29756 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18092 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15918 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 vsts      (1001) docker     (121)    96637 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 vsts      (1001) docker     (121)    78585 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12437 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3993 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3266 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12532 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31313 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10023 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3542 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7024 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.948883 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 vsts      (1001) docker     (121)    69376 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5384 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10258 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12750 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16950 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    48107 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24921 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7104 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31973 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27172 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8270 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32754 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2050 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20834 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 vsts      (1001) docker     (121)     4209 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 vsts      (1001) docker     (121)   101600 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 11:31:03.952883 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 vsts      (1001) docker     (121)    11769 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17098 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5733 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7283 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3911 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11971 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8915 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4903 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31213 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6157 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5108 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12765 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3949 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8558 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3293 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17861 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3615 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    39629 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3356 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14401 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)    83648 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2756 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6587 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    20751 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    20703 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     5500 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4197 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2096 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     9193 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     6283 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    26415 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    88575 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    10168 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    27892 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2392 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    11345 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 vsts      (1001) docker     (121)    13255 2022-10-18 11:30:53.000000 cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-10-18 11:31:03.952883 cutlery-0.0.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5856 2022-10-18 11:30:50.000000 cutlery-0.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.676983 cutlery-0.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-10-18 13:52:14.000000 cutlery-0.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-10-18 13:52:33.676983 cutlery-0.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      893 2022-10-18 13:52:14.000000 cutlery-0.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/cutlery/
+-rw-r--r--   0 vsts      (1001) docker     (121)      120 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      333 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (121)     5099 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (121)      156 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/config.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1470 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/merges.hh
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/cutlery/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       19 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     6291 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    16815 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (121)     1741 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3640 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1095 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       31 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)   253270 2022-10-18 13:52:14.000000 cutlery-0.0.3/cutlery/tests/toy.model
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/cutlery.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    10046 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       12 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-18 13:52:33.000000 cutlery-0.0.3/cutlery.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-10-18 13:52:14.000000 cutlery-0.0.3/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.648983 cutlery-0.0.3/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/sentencepiece/python/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5858 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/python/once.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6648 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9294 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    10322 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4416 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4850 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    18401 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     5102 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7354 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (121)    35154 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    40648 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   130839 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)   189303 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1304 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1061 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3525 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1782 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1265 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2506 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6007 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5713 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4167 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     3563 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1577 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2345 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1221 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1341 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5359 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1644 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)      972 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1743 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6609 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     9527 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15932 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)  7198605 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11633 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     5835 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16156 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2024 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    30990 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    19673 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    47605 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     9966 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6527 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13402 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    10493 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6557 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2035 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4163 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    12142 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1026 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1899 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     8718 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2103 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1104 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1656 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    25917 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     5727 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19808 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2807 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   106446 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1525 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    31219 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6912 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32258 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    18625 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     3879 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3321 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     7746 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    11414 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12866 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1124 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2101 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1372 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2464 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.648983 cutlery-0.0.3/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1001 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      966 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5614 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1673 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      799 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2592 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1309 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1012 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1447 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1088 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2413 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2127 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7856 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/string_view.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    20934 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.668983 cutlery-0.0.3/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (121)    51750 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.672983 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (121)    15726 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     8985 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     5975 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    30847 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    10999 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    82338 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     3573 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    30000 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.652983 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.676983 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6215 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29756 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18092 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15918 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    96637 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    78585 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12437 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3993 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3266 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12532 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31313 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10023 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3542 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7024 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.676983 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (121)    69376 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5384 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10258 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12750 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16950 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    48107 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24921 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7104 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31973 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27172 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8270 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32754 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2050 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20834 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4209 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (121)   101600 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-18 13:52:33.676983 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11769 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17098 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5733 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7283 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3911 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11971 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8915 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4903 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31213 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6157 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5108 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12765 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3949 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8558 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3293 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17861 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3615 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    39629 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3356 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14401 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    83648 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2756 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6587 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    20751 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    20703 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     5500 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     4197 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2096 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     9193 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     6283 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    26415 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    88575 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    10168 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    27892 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     2392 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    11345 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)    13255 2022-10-18 13:52:18.000000 cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1197 2022-10-18 13:52:33.680983 cutlery-0.0.3/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     5856 2022-10-18 13:52:14.000000 cutlery-0.0.3/setup.py
```

### Comparing `cutlery-0.0.2/LICENSE` & `cutlery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/PKG-INFO` & `cutlery-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlery
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/danieldk/cutlery
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cutlery-0.0.2/README.md` & `cutlery-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/_bbpe.pyx` & `cutlery-0.0.3/cutlery/_bbpe.pyx`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/_spp.pxd` & `cutlery-0.0.3/cutlery/_spp.pxd`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/_spp.pyx` & `cutlery-0.0.3/cutlery/_spp.pyx`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/_wordpiece.pyx` & `cutlery-0.0.3/cutlery/_wordpiece.pyx`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/merges.cc` & `cutlery-0.0.3/cutlery/merges.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/merges.hh` & `cutlery-0.0.3/cutlery/merges.hh`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/robbert-merges-1000.txt` & `cutlery-0.0.3/cutlery/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/robbert-vocab-1000.json` & `cutlery-0.0.3/cutlery/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/test_bbpe_processor.py` & `cutlery-0.0.3/cutlery/tests/test_bbpe_processor.py`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/test_sp.py` & `cutlery-0.0.3/cutlery/tests/test_sp.py`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/test_word_piece_processor.py` & `cutlery-0.0.3/cutlery/tests/test_word_piece_processor.py`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery/tests/toy.model` & `cutlery-0.0.3/cutlery/tests/toy.model`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/cutlery.egg-info/PKG-INFO` & `cutlery-0.0.3/cutlery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlery
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/danieldk/cutlery
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cutlery-0.0.2/cutlery.egg-info/SOURCES.txt` & `cutlery-0.0.3/cutlery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 cutlery/_wordpiece.pyx
 cutlery/config.h
 cutlery/merges.cc
 cutlery/merges.hh
 cutlery.egg-info/PKG-INFO
 cutlery.egg-info/SOURCES.txt
 cutlery.egg-info/dependency_links.txt
+cutlery.egg-info/requires.txt
 cutlery.egg-info/top_level.txt
 cutlery.egg-info/zip-safe
 cutlery/tests/__init__.py
 cutlery/tests/incorrect-merges.txt
 cutlery/tests/robbert-merges-1000.txt
 cutlery/tests/robbert-vocab-1000.json
 cutlery/tests/test_bbpe_processor.py
```

### Comparing `cutlery-0.0.2/sentencepiece/python/once.h` & `cutlery-0.0.3/sentencepiece/python/once.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model.cc` & `cutlery-0.0.3/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model.h` & `cutlery-0.0.3/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model_test.cc` & `cutlery-0.0.3/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model_trainer.cc` & `cutlery-0.0.3/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model_trainer.h` & `cutlery-0.0.3/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/bpe_model_trainer_test.cc` & `cutlery-0.0.3/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builder.cc` & `cutlery-0.0.3/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builder.h` & `cutlery-0.0.3/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builder_test.cc` & `cutlery-0.0.3/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `cutlery-0.0.3/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model.cc` & `cutlery-0.0.3/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model.h` & `cutlery-0.0.3/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model_test.cc` & `cutlery-0.0.3/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model_trainer.cc` & `cutlery-0.0.3/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model_trainer.h` & `cutlery-0.0.3/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/char_model_trainer_test.cc` & `cutlery-0.0.3/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/common.h` & `cutlery-0.0.3/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/compile_charsmap_main.cc` & `cutlery-0.0.3/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/error.cc` & `cutlery-0.0.3/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/filesystem.cc` & `cutlery-0.0.3/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/filesystem.h` & `cutlery-0.0.3/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/filesystem_test.cc` & `cutlery-0.0.3/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/freelist.h` & `cutlery-0.0.3/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/freelist_test.cc` & `cutlery-0.0.3/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/init.h` & `cutlery-0.0.3/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/init_test.cc` & `cutlery-0.0.3/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_factory.cc` & `cutlery-0.0.3/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_factory.h` & `cutlery-0.0.3/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_factory_test.cc` & `cutlery-0.0.3/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_interface.cc` & `cutlery-0.0.3/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_interface.h` & `cutlery-0.0.3/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/model_interface_test.cc` & `cutlery-0.0.3/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/normalization_rule.h` & `cutlery-0.0.3/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/normalizer.cc` & `cutlery-0.0.3/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/normalizer.h` & `cutlery-0.0.3/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/normalizer_test.cc` & `cutlery-0.0.3/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training.cc` & `cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training.h` & `cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/pretokenizer_for_training_test.cc` & `cutlery-0.0.3/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_processor.cc` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_processor.h` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_processor_test.cc` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer.cc` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer.h` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/sentencepiece_trainer_test.cc` & `cutlery-0.0.3/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spec_parser.h` & `cutlery-0.0.3/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spm_decode_main.cc` & `cutlery-0.0.3/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spm_encode_main.cc` & `cutlery-0.0.3/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spm_export_vocab_main.cc` & `cutlery-0.0.3/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spm_normalize_main.cc` & `cutlery-0.0.3/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/spm_train_main.cc` & `cutlery-0.0.3/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/test_main.cc` & `cutlery-0.0.3/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/testharness.cc` & `cutlery-0.0.3/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/testharness.h` & `cutlery-0.0.3/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_factory.cc` & `cutlery-0.0.3/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_factory.h` & `cutlery-0.0.3/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_factory_test.cc` & `cutlery-0.0.3/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_interface.cc` & `cutlery-0.0.3/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_interface.h` & `cutlery-0.0.3/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/trainer_interface_test.cc` & `cutlery-0.0.3/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unicode_script.cc` & `cutlery-0.0.3/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unicode_script.h` & `cutlery-0.0.3/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unicode_script_map.h` & `cutlery-0.0.3/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unicode_script_test.cc` & `cutlery-0.0.3/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model.cc` & `cutlery-0.0.3/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model.h` & `cutlery-0.0.3/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model_test.cc` & `cutlery-0.0.3/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model_trainer.cc` & `cutlery-0.0.3/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model_trainer.h` & `cutlery-0.0.3/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/unigram_model_trainer_test.cc` & `cutlery-0.0.3/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/util.cc` & `cutlery-0.0.3/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/util.h` & `cutlery-0.0.3/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/util_test.cc` & `cutlery-0.0.3/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model.cc` & `cutlery-0.0.3/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model.h` & `cutlery-0.0.3/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model_test.cc` & `cutlery-0.0.3/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model_trainer.cc` & `cutlery-0.0.3/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model_trainer.h` & `cutlery-0.0.3/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/src/word_model_trainer_test.cc` & `cutlery-0.0.3/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/container/flat_hash_map.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/container/flat_hash_set.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/flags/flag.cc` & `cutlery-0.0.3/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/flags/flag.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/flags/parse.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/memory/memory.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/ascii.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/match.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/numbers.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_cat.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_format.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_join.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_replace.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/str_split.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/string_view.cc` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/string_view.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/string_view.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/absl/strings/strip.h` & `cutlery-0.0.3/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/darts_clone/darts.h` & `cutlery-0.0.3/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/arena.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/common.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/int128.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/status.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/statusor.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/strutil.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/time.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `cutlery-0.0.3/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.2/setup.cfg` & `cutlery-0.0.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.0.2
+version = 0.0.3
 url = https://github.com/danieldk/cutlery
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -22,14 +22,16 @@
 	Programming Language :: Python :: 3.9
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
+install_requires = 
+	regex >= 2022
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 formats = gztar
```

### Comparing `cutlery-0.0.2/setup.py` & `cutlery-0.0.3/setup.py`

 * *Files identical despite different names*

