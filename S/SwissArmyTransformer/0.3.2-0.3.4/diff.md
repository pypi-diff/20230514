# Comparing `tmp/SwissArmyTransformer-0.3.2.tar.gz` & `tmp/SwissArmyTransformer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-gyh69qc3/SwissArmyTransformer-0.3.2.tar", last modified: Fri Apr 21 14:13:42 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-zb_scopx/SwissArmyTransformer-0.3.4.tar", last modified: Sun May 14 16:50:57 2023, max compression
```

## Comparing `SwissArmyTransformer-0.3.2.tar` & `SwissArmyTransformer-0.3.4.tar`

### file list

```diff
@@ -1,140 +1,145 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.2/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.041410 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3990 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.2/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23473 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1852 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/samplers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5653 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2899 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4990 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3183 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3484 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11454 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5492 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/lora.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7364 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3786 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8842 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    26381 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4884 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/mappings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      582 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/local_attention_function.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1956 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3822 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.037410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.057410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23627 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3432 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9271 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4431 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7502 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-04-21 14:12:08.000000 SwissArmyTransformer-0.3.2/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/tests/test_train.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.4/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4131 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.4/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24121 2023-05-14 10:40:26.000000 SwissArmyTransformer-0.3.4/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.4/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.4/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/samplers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.4/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3156 2023-05-11 04:52:03.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6931 2023-05-11 06:00:33.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.4/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4930 2023-05-14 16:31:20.000000 SwissArmyTransformer-0.3.4/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12611 2023-05-14 16:36:25.000000 SwissArmyTransformer-0.3.4/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5522 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7648 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/lora_mixin.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12364 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.4/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.4/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13873 2023-05-14 16:02:55.000000 SwissArmyTransformer-0.3.4/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8013 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27225 2023-05-14 14:59:24.000000 SwissArmyTransformer-0.3.4/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-14 16:30:23.000000 SwissArmyTransformer-0.3.4/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/mappings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.4/sat/ops/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      643 2023-05-14 16:08:00.000000 SwissArmyTransformer-0.3.4/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.4/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.4/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.4/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.986356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24229 2023-05-14 16:26:37.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.4/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.4/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.4/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7498 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-05-14 16:48:32.000000 SwissArmyTransformer-0.3.4/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.4/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.4/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-14 10:56:24.000000 SwissArmyTransformer-0.3.4/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.2/LICENSE` & `SwissArmyTransformer-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/PKG-INFO` & `SwissArmyTransformer-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.2
+Version: 0.3.4
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.2/README.md` & `SwissArmyTransformer-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.2
+Version: 0.3.4
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 sat/model/mixins.py
 sat/model/registry.py
 sat/model/transformer.py
 sat/model/finetune/__init__.py
 sat/model/finetune/adapter.py
 sat/model/finetune/ffadd.py
 sat/model/finetune/lora.py
+sat/model/finetune/lora_mixin.py
 sat/model/finetune/mlp_head.py
 sat/model/finetune/prompt_tuning.py
 sat/model/official/__init__.py
 sat/model/official/bert_model.py
 sat/model/official/cait_model.py
 sat/model/official/chatglm_model.py
 sat/model/official/clip_model.py
@@ -67,14 +68,15 @@
 sat/mpu/initialize.py
 sat/mpu/layers.py
 sat/mpu/mappings.py
 sat/mpu/utils.py
 sat/ops/__init__.py
 sat/ops/layernorm.py
 sat/ops/local_attention_function.py
+sat/ops/scaled_mask_softmax.py
 sat/resources/__init__.py
 sat/resources/download.py
 sat/resources/urls.py
 sat/tokenization/__init__.py
 sat/tokenization/hf_tokenizer.py
 sat/tokenization/cogview/__init__.py
 sat/tokenization/cogview/sp_tokenizer.py
@@ -108,8 +110,11 @@
 sat/training/deepspeed_zero2.json
 sat/training/learning_rates.py
 sat/training/model_io.py
 sat/training/utils.py
 tests/test_base_model.py
 tests/test_inference.py
 tests/test_list_info.py
-tests/test_train.py
+tests/test_nested_model.py
+tests/test_train.py
+tests/test_train_dp.py
+tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.2/sat/arguments.py` & `SwissArmyTransformer-0.3.4/sat/arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import deepspeed
 import json
 import random
 import numpy as np
 import warnings
 from sat import mpu
 
+import logging
+from sat.helpers import print_all, print_rank0
 
 def add_model_config_args(parser):
     """Model arguments"""
 
     group = parser.add_argument_group('model', 'model configuration')
 
     # --------------- Core hyper-parameters --------------- 
@@ -271,15 +273,15 @@
     after = before
     multiple = args.make_vocab_size_divisible_by
     # you should control args to let it divided by 
     # mpu.get_model_parallel_world_size()
     while (after % multiple) != 0:
         after += 1
     if args.rank == 0:
-        print('> padded vocab (size: {}) with {} dummy '
+        print_rank0('> padded vocab (size: {}) with {} dummy '
                  'tokens (new size: {})'.format(
         before, after - before, after))
 
 def _simple_init(model_parallel_size=1):
     '''Necessary initialization for torch.distributed for model-only mode'''
     args = argparse.Namespace(
         distributed_backend='nccl',
@@ -287,17 +289,17 @@
     )
     args.rank = int(os.getenv('RANK', '0'))
     args.world_size = int(os.getenv("WORLD_SIZE", '1'))
     args.local_rank = int(os.getenv("LOCAL_RANK", '0')) # torchrun
     args.device = args.local_rank
     args.deepspeed = False
     if initialize_distributed(args): # first time init model parallel, print warning
-        warnings.warn(
+        print_rank0(
                   'You are using model-only mode.\n\
-                  For torch.distributed users or loading model parallel models, set environment variables RANK, WORLD_SIZE and LOCAL_RANK.'
+For torch.distributed users or loading model parallel models, set environment variables RANK, WORLD_SIZE and LOCAL_RANK.'
                   )
         return True
     return False
 
 def get_args(args_list=None, parser=None):
     """Parse all the args."""
     if parser is None:
@@ -313,15 +315,15 @@
 
     # Include DeepSpeed configuration arguments
     parser = deepspeed.add_config_arguments(parser)
 
     args = parser.parse_args(args_list)
 
     if not args.train_data:
-        print('WARNING: No training data specified')
+        print_rank0('WARNING: No training data specified')
 
     assert (args.train_iters is None)^(args.epochs is None)
 
     args.cuda = torch.cuda.is_available()
 
     args.rank = int(os.getenv('RANK', '0'))
     args.world_size = int(os.getenv("WORLD_SIZE", '1'))
@@ -339,15 +341,15 @@
             'LOCAL_RANK (default 0) and args.device inconsistent. '
             'This can only happens in inference mode. '
             'Please use CUDA_VISIBLE_DEVICES=x for single-GPU training. '
             )
 
     # args.model_parallel_size = min(args.model_parallel_size, args.world_size)
     if args.rank == 0:
-        print('using world size: {} and model-parallel size: {} '.format(
+        print_rank0('using world size: {} and model-parallel size: {} '.format(
             args.world_size, args.model_parallel_size))
     if args.vocab_size > 0:
         _adjust_vocab_size(args)
     
     if args.train_data_weights is not None:
         assert len(args.train_data_weights) == len(args.train_data)
     
@@ -356,15 +358,15 @@
         if args.deepspeed_config is None: # not specified
             args.deepspeed_config = os.path.join(os.path.dirname(__file__), 'training', f'deepspeed_zero{args.zero_stage}.json')
             override_deepspeed_config = True
         else:
             override_deepspeed_config = False
     if args.zero_stage > 0:
         if args.rank == 0 and not args.fp16:
-            print('Automatically set fp16=True to use ZeRO.')     
+            print_rank0('Automatically set fp16=True to use ZeRO.')     
         args.fp16 = True
         args.bf16 = False
 
     if args.deepspeed:
         if args.checkpoint_activations:
             args.deepspeed_activation_checkpointing = True
         else:
@@ -381,15 +383,15 @@
             deepspeed_config["train_micro_batch_size_per_gpu"] = args.batch_size
             deepspeed_config["gradient_accumulation_steps"] = args.gradient_accumulation_steps
             optimizer_params_config = deepspeed_config["optimizer"]["params"]
             optimizer_params_config["lr"] = args.lr
             optimizer_params_config["weight_decay"] = args.weight_decay
         else: # override args with values in deepspeed_config
             if args.rank == 0:
-                print('Will override arguments with manually specified deepspeed_config!')
+                print_rank0('Will override arguments with manually specified deepspeed_config!')
             if "fp16" in deepspeed_config and deepspeed_config["fp16"]["enabled"]:
                 args.fp16 = True
             else:
                 args.fp16 = False
             if "train_micro_batch_size_per_gpu" in deepspeed_config:
                 args.batch_size = deepspeed_config["train_micro_batch_size_per_gpu"]
             if "gradient_accumulation_steps" in deepspeed_config:
@@ -417,23 +419,41 @@
     # expand relative path
     folder = os.path.dirname(path)
     for k in config:
         # all the relative paths in config are based on the folder
         if k.endswith('_path'): 
             config[k] = os.path.join(folder, config[k])
             if args.rank == 0:
-                print(f'> parsing relative path {k} in model_config as {config[k]}.')
+                print_rank0(f'> parsing relative path {k} in model_config as {config[k]}.')
     args = vars(args)
     for k in list(args.keys()):
         if k in config:
             del args[k]
     args = argparse.Namespace(**config, **args)
     return args
 
 
+def overwrite_args_by_dict(args, overwrite_args={}):
+    if 'decoder_freq' in overwrite_args:
+        decoder_freq = overwrite_args['decoder_freq']
+        del overwrite_args['decoder_freq']
+    else:
+        decoder_freq = None
+    for k in overwrite_args:
+        setattr(args, k, overwrite_args[k])
+    if decoder_freq is not None:
+        args.is_decoder = []
+        for i in range(args.num_layers):
+            if i % decoder_freq == 0:
+                args.is_decoder.append(True)
+            else:
+                args.is_decoder.append(False)
+    return args
+
+
 def initialize_distributed(args):
     """Initialize torch.distributed."""
     if torch.distributed.is_initialized():
         if mpu.model_parallel_is_initialized():
             if args.model_parallel_size != mpu.get_model_parallel_world_size():
                 raise ValueError('model_parallel_size is inconsistent with prior configuration.'
                                  'We currently do not support changing model_parallel_size.')
```

### Comparing `SwissArmyTransformer-0.3.2/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.3.4/sat/data_utils/configure_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from functools import partial
 
 from torch.utils import data
 from .samplers import DistributedBatchSampler
 from torch.utils.data import ChainDataset, IterableDataset
 
 from sat import mpu
-    
+from sat.helpers import print_all, print_rank0
 
 def make_data_loader(dataset, batch_size, args, split, collate_fn=None):
 
     world_size = torch.distributed.get_world_size(
         group=mpu.get_data_parallel_group())
     rank = torch.distributed.get_rank(group=mpu.get_data_parallel_group())
     distributed = world_size > 1
@@ -92,15 +92,15 @@
                                               collate_fn=collate_fn)
     return data_loader
 
 
 def make_dataset_full(path, split, args, create_dataset_function, 
         dataset_weights=None, random_mapping=True, is_train_data=False, **kwargs):
     """function to create datasets+tokenizers for common options"""
-    print('make dataset ...', path)
+    print_all('make dataset ' + str(path), level='DEBUG')
     assert isinstance(path, list)
 
     if args.iterable_dataset: # cannot indexed
         # the random mapping is flexible and efficient, but sometimes we have pratical issue
         # For instance, someone just gives you a iterable dataset, e.g. webdataset
         from .datasets import ConfiguredResampledShards, DataPipeline
         valid_types = (ConfiguredResampledShards, DataPipeline)
```

### Comparing `SwissArmyTransformer-0.3.2/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.3.4/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.3.4/sat/data_utils/hf_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Time    :   2021/12/14
 # @Author  :   Zhuoyi Yang
 # @Contact :   yangzhuo18@mails.tsinghua.edu.cn
 
 import os
 import datasets
 from datasets import load_dataset
+from sat.helpers import print_rank0
 
 def parse_huggingface_path(path):
     if path.startswith('hf://'):
         path = path[5:]
     names = path.split('/')
     first_name = names[0]
     second_name = names[1] if len(names) >= 2 and names[1] != '*' else None
@@ -27,13 +28,13 @@
 
     if dataset_path and os.path.exists(dataset_path) and not rebuild:
         dataset = datasets.load_from_disk(dataset_path)
     else:
         dataset = load_dataset(dataset_name, sub_name, cache_dir=cache_dir, split=split,
         download_config=datasets.utils.DownloadConfig(max_retries=20)) # TODO
         # dataset = dataset.filter(lambda example, indice: indice % 100 == 0, with_indices=True)
-        print(f'> Preprocessing the {dataset_name} by process_fn... Next time will return cached files.\n> Pass "rebuild=True" to load_hf_dataset if change process_fn. Change "transformer_name" for different tokenizers or models.')
+        print_rank0(f'> Preprocessing the {dataset_name} by process_fn... Next time will return cached files.\n> Pass "rebuild=True" to load_hf_dataset if change process_fn. Change "transformer_name" for different tokenizers or models.')
         dataset = dataset.map(process_fn, batched=False, load_from_cache_file=True)
         if dataset_path:
             dataset.save_to_disk(dataset_path)
     dataset.set_format(type='torch', columns=columns)
     return dataset
```

### Comparing `SwissArmyTransformer-0.3.2/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.3.4/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.3.4/sat/generation/autoregressive_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 from .sampling_strategies import BaseStrategy
+from sat.helpers import print_rank0
 
 def get_masks_and_position_ids_default(seq):
     tokens = seq.unsqueeze(0)
 
     attention_mask = torch.ones((1, len(seq), len(seq)), device=tokens.device)
     attention_mask.tril_()
     attention_mask.unsqueeze_(1)
@@ -63,14 +64,17 @@
         seq: [2, 3, 5, ..., -1(to be generated), -1, ...]
         mems: [num_layers, batch_size, len_mems(index), mem_hidden_size]
             cache, should be first mems.shape[1] parts of context_tokens.
             mems are the first-level citizens here, but we don't assume what is memorized.
             input mems are used when multi-phase generation.
     '''
     assert len(seq.shape) == 1
+    if hasattr(strategy, 'num_beams') and batch_size < strategy.num_beams:
+        batch_size = strategy.num_beams
+        print_rank0(f'Adjust batch_size to {batch_size} due to num_beams. Mute this warning by setting batch_size == num_beams.', level='DEBUG')
 
     # building the initial tokens, attention_mask, and position_ids
     context_length = 0
     while seq[context_length] >= 0:
         context_length += 1 # [0, context_length-1] are given
     assert context_length > 0
     tokens, attention_mask, position_ids = get_masks_and_position_ids(seq)
@@ -99,16 +103,16 @@
         if log_attention_weights is not None:
             log_attention_weights_part = log_attention_weights[..., index: counter+1, :counter+1] # TODO memlen
         else:
             log_attention_weights_part = None
 
         logits, *output_per_layers = model(
             tokens[:, index:], 
-            position_ids[..., index: counter+1],
-            attention_mask[..., index: counter+1, :counter+1], # TODO memlen
+            position_ids=position_ids[..., index: counter+1],
+            attention_mask=attention_mask[..., index: counter+1, :counter+1], # TODO memlen
             mems=mems,
             log_attention_weights=log_attention_weights_part,
             **kw_args
         )
         mem_kv = [o['mem_kv'] for o in output_per_layers]
         mems = update_mems(mem_kv, mems, max_memory_length=max_memory_length)
         counter += 1
@@ -128,15 +132,15 @@
     assert len(tokens.shape) <= 2 and len(loss_mask.shape)
     if len(tokens.shape) == 1:
         tokens = tokens.unsqueeze(0)
     if len(loss_mask.shape) == 1:
         loss_mask = loss_mask.unsqueeze(0).expand(tokens.shape)
     pad_pos = tokens < 0
     if pad_pos.any():
-        print('Find -1 in tokens, automatically ignore them.')
+        print_rank0('Find -1 in tokens, automatically ignore them.', level='DEBUG')
         tokens[pad_pos] = 0
         loss_mask[pad_pos] = 0
 
     attention_mask = attention_mask.type_as(next(model.parameters()))
     logits = model(tokens, position_ids, attention_mask)[0]
     logits = logits.float()
     for slc in invalid_slices:
```

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.3.4/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/magnify.py` & `SwissArmyTransformer-0.3.4/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/base_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,34 @@
     if top_k > 0:
         # Remove all tokens with a probability less than the last token of the top-k
         indices_to_remove = logits < torch.topk(logits, top_k)[0][..., -1, None]
         logits[indices_to_remove] = filter_value
 
     if top_p > 0.0:
         # convert to 1D
-        logits = logits.view(logits.size()[1]).contiguous()
+        # logits = logits.view(logits.size()[1])
+        logits = logits.contiguous()
         sorted_logits, sorted_indices = torch.sort(logits, descending=True)
         cumulative_probs = torch.cumsum(F.softmax(sorted_logits, dim=-1), dim=-1)
 
         # Remove tokens with cumulative probability above the threshold
         sorted_indices_to_remove = cumulative_probs > top_p
         # Shift the indices to the right to keep also the first token above the threshold
         sorted_indices_to_remove[..., 1:] = sorted_indices_to_remove[..., :-1].clone()
         sorted_indices_to_remove[..., 0] = 0
-        indices_to_remove = sorted_indices[sorted_indices_to_remove]
-        logits[indices_to_remove] = filter_value
-        # going back to 2D
-        logits = logits.view(1, -1).contiguous()
+
+        # indices_to_remove = sorted_indices[sorted_indices_to_remove]
+        # logits[indices_to_remove] = filter_value
+        # # going back to 2D
+        # logits = logits.view(1, -1).contiguous()
+
+        batch_size, vocab_size = logits.shape[:2]
+        for i in range(batch_size):
+            indices_to_remove = sorted_indices[i][sorted_indices_to_remove[i]]
+            logits[i][indices_to_remove] = filter_value
 
     return logits
 
 
 class BaseStrategy:
     def __init__(self, invalid_slices=[], temperature=1., top_k=200, eps=1e-4, top_p=0.0, end_tokens=None):
         self.invalid_slices = invalid_slices
```

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,107 @@
 # -*- encoding: utf-8 -*-
 '''
-@File    :   base_strategy.py
+@File    :   beam_search_strategy.py
 @Time    :   2021/10/08 22:22:42
 @Author  :   Ming Ding
 @Contact :   dm18@mails.tsinghua.edu.cn
 '''
 
 # here put the import lib
 import torch
 import torch.nn.functional as F
+from .base_strategy import top_k_logits
 
 class BeamSearchStrategy:
-    def __init__(self, num_beams, length_penalty=1., consider_end=False,
-                end_tokens=[], invalid_slices=[], no_repeat_ngram_size=0, min_tgt_length=0):
+    def __init__(self, num_beams, length_penalty=1., 
+                temperature=1., top_k=0., top_p=0.0,
+                consider_end=True,
+                end_tokens=[], invalid_slices=[], no_repeat_ngram_size=0, 
+                min_tgt_length=0,
+                prefer_min_length=5,
+                prefer_max_length=100,
+                stop_n_iter_unchanged=10):
         self.num_beams = num_beams
         self.length_penalty = length_penalty
         self.end_tokens = end_tokens
         self.ngram = no_repeat_ngram_size
         self.min_tgt_length = min_tgt_length
         self.invalid_slices = invalid_slices
         self.consider_end = consider_end
+        self.stop_n_iter_unchanged = stop_n_iter_unchanged
+        self.prefer_min_length = prefer_min_length
+        self.prefer_max_length = prefer_max_length
+        self.temperature = temperature
+        self.top_k = top_k
+        self.top_p = top_p
         self._init_cache()
 
     def _init_cache(self):
         self.end_beams = [] # list of LongTensors
         self.end_beams_penalized_scores = [] # list of LongTensors
         self.cached_beam_scores = 0 # [batch_size]
         self.cached_beam_ngram_bans = [{} for i in range(self.num_beams)]
         self.is_done = False
+        self.end_beams_unchanged = 0
+        self.context_length = None
     
     def _add_end_beams(self, score, beam):
-        score = score / ((5. + len(beam)) / 6) ** self.length_penalty # Magic number for OpenNMT 
+        gen_length = len(beam) - self.context_length # we usually care about generated length, instead of total length
+        # score = score / ((5. + gen_length) / 6) ** self.length_penalty # Magic number for OpenNMT 
+        # ----
+        trunc_length = min(self.prefer_max_length, gen_length) + 1
+        if gen_length >= self.prefer_min_length:
+            adjust_penalty = self.length_penalty
+        else:
+            t = gen_length / self.prefer_min_length
+            min_penalty = min(0.5, self.length_penalty / 2)
+            adjust_penalty = t * self.length_penalty + (1-t) * min_penalty
+        # print(float(score), trunc_length, adjust_penalty)
+        score = float(score) / trunc_length ** adjust_penalty
+        # ----
+        
         for i in range(len(self.end_beams), -1, -1):
             if i == 0 or score < self.end_beams_penalized_scores[i-1]:
                 break
         self.end_beams.insert(i, beam)
         self.end_beams_penalized_scores.insert(i, score)
-
         self.end_beams = self.end_beams[:self.num_beams]
         self.end_beams_penalized_scores = self.end_beams_penalized_scores[:self.num_beams]
+        # print('add end beam', score, i)
+        return (i == 0)
 
     def forward(self, logits, tokens, mems):
         batch_size, vocab_size = logits.shape
         seq_len = tokens.shape[-1]
+        if self.context_length is None:
+            self.context_length = seq_len
         logits = logits.float()
         for invalid_slice in self.invalid_slices:
             logits[..., invalid_slice] = -65504
         if self.min_tgt_length > seq_len:
             for end_token in self.end_tokens:
                 logits[..., end_token] = -65504
         if self.ngram > 0 and seq_len > self.ngram:
             for i in range(batch_size):
                 ngram_prefix = tokens[i, -(self.ngram-1):].tolist() # TODO ngram=1
                 for banned_index in self.cached_beam_ngram_bans[i].get(tuple(ngram_prefix), []):
                     logits[i, banned_index] = -65504
         
+        logits = logits / self.temperature
+        logits = top_k_logits(logits, self.top_k, self.top_p)
+
         next_token_scores = F.log_softmax(logits, dim=-1) # [batch_size, vocab_size]
         prev_scores = self.cached_beam_scores
         if isinstance(self.cached_beam_scores, torch.Tensor):
             prev_scores = prev_scores[:, None].expand_as(next_token_scores)
         next_token_scores = next_token_scores + prev_scores
         
         next_token_scores = next_token_scores.view(batch_size * vocab_size)
 
-        probs = F.softmax(next_token_scores, dim=0)
+        probs = F.softmax(logits.view(batch_size * vocab_size), dim=0)
         next_tokens = torch.multinomial(probs, 
             num_samples=(max(1,len(self.end_tokens))+1) * self.num_beams) # [2*nb]
         next_token_scores = next_token_scores[next_tokens]
         next_token_scores, _indices = torch.sort(next_token_scores, descending=True, dim=0)
         next_tokens = next_tokens[_indices]
 
         next_indices = torch.div(next_tokens, vocab_size, rounding_mode='trunc')
@@ -76,18 +110,20 @@
         # select out end beams or continue beams
         if mems.shape[1] < batch_size:
             mems = mems.expand(-1, batch_size, -1, -1)
         beam_continue = []
         scores_continue = []
         bans_continue = []
         mems_contiue = []
+        end_beams_changed = False
         for i in range(len(next_tokens)):
             beam = torch.cat((tokens[next_indices[i]], next_tokens[i:i+1]))
             if int(next_tokens[i]) in self.end_tokens:
-                self._add_end_beams(next_token_scores[i], beam)
+                changed = self._add_end_beams(next_token_scores[i], beam)
+                end_beams_changed = end_beams_changed or changed
             elif len(beam_continue) < self.num_beams:
                 beam_continue.append(beam)
                 mems_contiue.append(mems[:, next_indices[i]])
                 # update caches
                 scores_continue.append(next_token_scores[i])
                 if self.ngram > 0:
                     bans = self.cached_beam_ngram_bans[next_indices[i]].copy()
@@ -97,20 +133,28 @@
             else:
                 break
         tokens = torch.stack(beam_continue)
         mems = torch.stack(mems_contiue, dim=1)
         self.cached_beam_scores = torch.tensor(scores_continue, device=logits.device)
         self.cached_beam_ngram_bans = bans_continue
 
-        # TODO is_done
+        # check if done, this is not a official solution
+        if end_beams_changed:
+            self.end_beams_unchanged = 0
+        elif len(self.end_beams) > 0:
+            self.end_beams_unchanged += 1
+            if self.end_beams_unchanged >= self.stop_n_iter_unchanged:
+                self.is_done = True
+
         return tokens, mems
 
     def finalize(self, tokens, mems):
         if self.consider_end:
-            for i in range(tokens.shape[0]):
-                self._add_end_beams(self.cached_beam_scores[i], tokens[i])
+            if not self.is_done:
+                for i in range(tokens.shape[0]):
+                    self._add_end_beams(self.cached_beam_scores[i], tokens[i])
             mems = None
             ret = self.end_beams
         else:
             ret = tokens
         self._init_cache()
         return ret, mems
```

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/generation/utils.py` & `SwissArmyTransformer-0.3.4/sat/generation/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 func(raw_text)
                 if torch.distributed.get_rank() == 0:
                     print("\nTaken time {:.2f}\n".format(time.time() - start_time), flush=True)
             except (ValueError, FileNotFoundError) as e:
                 print(e)
                 continue
     else:
-        with open(input_source, 'r') as fin:
+        with open(input_source, 'r', encoding="utf-8") as fin:
             inputs = fin.readlines()
         for line_no, raw_text in enumerate(inputs):
             if line_no % get_data_parallel_world_size() != get_data_parallel_rank():
                 continue
             rk = dist.get_rank()
             if get_model_parallel_rank() == 0:
                 print(f'Working on No. {line_no} on model group {rk}... ')
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/base_model.py` & `SwissArmyTransformer-0.3.4/sat/model/base_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 import torch
 import inspect
 import warnings
 import argparse
 from sat.model.registry import model_registry, MetaModel
 
 from sat.model.transformer import BaseTransformer, standard_attention
-from sat import update_args_with_file
+from sat.arguments import update_args_with_file, overwrite_args_by_dict
 from sat.training.deepspeed_training import load_checkpoint, get_model
+from sat.helpers import print_rank0
 
 from sat.transformer_defaults import HOOKS_DEFAULT
 from sat.resources import auto_create
 
 def non_conflict(func):
     '''mark a hook function as non-conflict,
     so that it can be compatible with any already defined hooks.
@@ -86,33 +87,38 @@
 
             self.transformer = BaseTransformer(
                 num_layers=args.num_layers,
                 vocab_size=args.vocab_size,
                 hidden_size=args.hidden_size,
                 num_attention_heads=args.num_attention_heads,
                 max_sequence_length=args.max_sequence_length,
-                embedding_dropout_prob=args.hidden_dropout,
-                attention_dropout_prob=args.attention_dropout,
-                output_dropout_prob=args.hidden_dropout,
-                inner_hidden_size=args.inner_hidden_size,
-                hidden_size_per_attention_head=args.hidden_size_per_attention_head,
+                layernorm_order=args.layernorm_order,
+                embedding_dropout_prob=args.hidden_dropout if hasattr(args, 'hidden_dropout') else 0,
+                attention_dropout_prob=args.attention_dropout if hasattr(args, 'attention_dropout') else 0,
+                output_dropout_prob=args.hidden_dropout if hasattr(args, 'hidden_dropout') else 0,
+                inner_hidden_size=args.inner_hidden_size if hasattr(args, 'inner_hidden_size') else None,
+                hidden_size_per_attention_head=args.hidden_size_per_attention_head if hasattr(args, 'hidden_size_per_attention_head') else None,
                 checkpoint_activations=args.checkpoint_activations if hasattr(args, 'checkpoint_activations') else False,
                 checkpoint_num_layers=args.checkpoint_num_layers if hasattr(args, 'checkpoint_num_layers') else 1,
-                layernorm_order=args.layernorm_order,
+                is_decoder=args.is_decoder if hasattr(args, 'is_decoder') else False,
+                cross_attn_hidden_size=args.cross_attn_hidden_size if hasattr(args, 'cross_attn_hidden_size') else None,
+                use_final_layernorm=args.use_final_layernorm if hasattr(args, 'use_final_layernorm') else True,
+                layernorm_epsilon=args.layernorm_epsilon if hasattr(args, 'layernorm_epsilon') else 1e-5,
+                use_bias=args.use_bias if hasattr(args, 'use_bias') else True,
                 hooks=self.hooks,
                 params_dtype=params_dtype,
                 skip_init=args.skip_init,
-                device=torch.cuda.current_device() if args.use_gpu_initialization else torch.device('cpu'),
+                device=torch.cuda.current_device() if hasattr(args, 'use_gpu_initialization') and args.use_gpu_initialization else torch.device('cpu'),
                 **kwargs
             )
 
     def reinit(self, mixin_names=None):  # will be called when loading model, None means all
         # if some mixins are loaded, overrides this function
         for k, m in self.mixins.items():
-            if k in mixin_names or mixin_names is None:
+            if mixin_names is None or k in mixin_names:
                 m.reinit(self)
 
     def add_mixin(self, name, new_mixin, reinit=False):
         assert name not in self.mixins
         assert isinstance(new_mixin, BaseMixin)
 
         self.mixins[name] = new_mixin  # will auto-register parameters
@@ -180,15 +186,15 @@
 
     @classmethod
     def add_model_specific_args(cls, parser):
         # recorded in arguments.py: add_model_config_args
         return parser
 
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, **kwargs):
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
         '''Load a pretrained checkpoint of the current model.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it. None will create a new model-only one with defaults.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: the url of the model. Default: SAT_URL.
                 prefix: the prefix of the checkpoint. Default: ''.
@@ -200,14 +206,15 @@
             model_path = name
         else:
             model_path = auto_create(name, path=home_path, url=url)
         # create a new args if not provided
         if args is None:
             args = cls.get_args()
         args = update_args_with_file(args, path=os.path.join(model_path, 'model_config.json'))
+        args = overwrite_args_by_dict(args, overwrite_args=overwrite_args)
         model = get_model(args, cls, **kwargs)
         if not build_only:
             load_checkpoint(model, args, load_path=model_path, prefix=prefix)
         return model, args
     
     @classmethod
     def list_avail_args(cls, print=True):
@@ -231,23 +238,24 @@
             Returns:
                 args: the parsed args.
         '''
         parser = cls.list_avail_args(print=False)
         # use parser to parse kwargs
         args = parser.parse_args([])
         for k, v in kwargs.items():
-            if hasattr(args, k):
+            if hasattr(args, k) or k in ['fp16']: # optional args
                 setattr(args, k, v)
             else:
-                raise ValueError(f'Unknown arg {k}.')
+                print_rank0(f'warning: Unknown arg {k} for class {cls.__name__}.', level='DEBUG')
+                setattr(args, k, v)
         return args
 
 class AutoModel():
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, **kwargs):
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
         '''Automatically find the class and instantiate it. Auto-download.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: manually specified url for the `name` model.
         '''
@@ -257,14 +265,15 @@
             model_path = auto_create(name, path=home_path, url=url)
         if args is None:
             args = argparse.Namespace() # null, fill later
             null_args = True
         else:
             null_args = False
         args = update_args_with_file(args, path=os.path.join(model_path, 'model_config.json'))
+        args = overwrite_args_by_dict(args, overwrite_args=overwrite_args)
         if not hasattr(args, 'model_class'):
             raise ValueError('model_config.json must have key "model_class" for AutoModel.from_pretrained.')
         model_cls = model_registry.get(args.model_class)
         if null_args:
             # fill args with default values, if not provided
             model_default_args = model_cls.get_args()
             for k, v in model_default_args.__dict__.items():
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.3.4/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.3.4/sat/model/encoder_decoder_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,13 +95,13 @@
         group.add_argument("--dec-max-sequence-length", type=int, default=None)
         group.add_argument("--dec-inner-hidden-size", type=int, default=None)
         group.add_argument("--dec-hidden-size-per-attention-head", type=int, default=None)
         group.add_argument("--dec-layernorm-order", type=str, default=None)
         return parser
 
     @classmethod
-    def from_pretrained(cls, args, name, *, home_path=None, url=None):
+    def from_pretrained(cls, args, name, *, home_path=None, url=None): # TODO update model-only mode
         model_path = auto_create(name, path=home_path, url=url)
         args = update_args_with_file(args, path=os.path.join(model_path, 'model_config.json'))
         model = get_model(args, cls)
         load_checkpoint(model, args, load_path=model_path)
         return model, args
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.3.4/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.3.4/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.3.4/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.3.4/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.3.4/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/__init__.py` & `SwissArmyTransformer-0.3.4/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/chatglm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,19 @@
         self.mask_token_id = args.mask_token_id
         self.gmask_token_id = args.gmask_token_id
         self.pad_token_id = 3
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return None
     
-    def forward(self, input_ids, attention_mask=None, position_ids=None, past_key_values=None, **kwargs):
-        attention_mask, position_ids = self.get_inputs(input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
+    def forward(self, input_ids, position_ids=None, attention_mask=None, past_key_values=None, **kwargs):
+        if attention_mask is None and position_ids is None:
+            attention_mask, position_ids = self.get_inputs(input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
+        if attention_mask is not None and attention_mask.dtype is torch.bool:
+            attention_mask = (~attention_mask).long()
         if past_key_values is not None:
             input_ids = input_ids[:, -1:]
             position_ids = position_ids[..., -1:]
             if input_ids.size(0) != 1:
                 attention_mask = attention_mask[:, :, -1:]
         return super().forward(input_ids=input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
     
@@ -193,16 +196,14 @@
             if past_key_values is not None and input_ids.size(0) == 1:
                 attention_mask = torch.tensor([[1]], dtype=torch.long, device=input_ids.device)
             else:
                 attention_mask = self.get_masks(
                     input_ids=input_ids,
                     device=input_ids.device, **kwargs
                 )
-        elif attention_mask.dtype is torch.bool:
-            attention_mask = (~attention_mask).long()
         if position_ids is None:
             MASK, gMASK = self.mask_token_id, self.gmask_token_id
             mask_token = gMASK if gMASK in input_ids else MASK
             use_gmask = True if gMASK in input_ids else False
 
             mask_positions = [seq.tolist().index(mask_token) for seq in input_ids]
             position_ids = self.get_position_ids(
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/eva2_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from sat.model.base_model import BaseModel
 from sat.model.mixins import BaseMixin
 import torch.nn as nn
 from .vit_model import ViTProperty
-from sat.ops import LayerNorm
+from sat.ops.layernorm import LayerNorm
 
 class MaskedPatchEmbedMixin(BaseMixin):
     def __init__(self, in_channels, hidden_size, property):
         super(MaskedPatchEmbedMixin, self).__init__()
         self.property = property
         self.mask_token = nn.Parameter(torch.zeros(1, 1, hidden_size))
         self.proj = nn.Conv2d(in_channels, hidden_size, kernel_size=property.patch_size, stride=property.patch_size)
@@ -127,15 +127,15 @@
         self.property = ViTProperty(args.image_size, args.patch_size, args.pre_len, args.post_len)
         args.max_sequence_length = self.property.seq_len
         super().__init__(args, transformer=transformer, parallel_output=parallel_output, **kwargs)
         self.add_mixin("patch_embedding", MaskedPatchEmbedMixin(args.in_channels, args.hidden_size, self.property))
         # The old_property of ViTModel is not elegent. However, I don't have time to fix them (including vit, cait, deit, yolos). I can only discard it since eva model for now.
         # self.add_mixin("pos_embedding", InterpolatedPositionEmbeddingMixin(args.hidden_size, self.old_property, self.property))
         self.add_mixin("eva2-final", EVA2FinalMixin(args.predict_feature_dim, args.hidden_size))
-        self.add_mixin("eva2-mlp", SwiGLUMixin(args.num_layers, args.hidden_size, args.inner_hidden_size, eps=kwargs["layernorm_epsilon"]))
+        self.add_mixin("eva2-mlp", SwiGLUMixin(args.num_layers, args.hidden_size, args.inner_hidden_size, eps=args.layernorm_epsilon))
         self.add_mixin("eva2-attn", EVA2AttnMixin(args.hidden_size, args.num_attention_heads, self.property))
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return self.transformer.position_embeddings.weight.unsqueeze(0)
 
     @classmethod
     def add_model_specific_args(cls, parser):
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/glm130B_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,14 @@
 
 # flags required to enable jit fusion kernels
 torch._C._jit_set_profiling_mode(False)
 torch._C._jit_set_profiling_executor(False)
 torch._C._jit_override_can_fuse_on_cpu(True)
 torch._C._jit_override_can_fuse_on_gpu(True)
 
-try:
-    from apex.transformer.functional import FusedScaleMaskSoftmax
-    from apex.transformer.enums import AttnMaskType
-except ModuleNotFoundError:
-    print(
-        "Please install apex to use FusedScaleMaskSoftmax, otherwise the inference efficiency will be greatly reduced"
-    )
-    FusedScaleMaskSoftmax = None
-
-
 class RotaryEmbeddingMixin(BaseMixin):
     def __init__(
         self,
         fp16: bool,
         hidden_size: int,
         num_attention_heads: int,
         model_parallel_size: int,
@@ -163,14 +153,17 @@
 
 class SelfAttentionWithFP32SoftmaxMixin(BaseMixin):
     def __init__(self, hidden_size, num_attention_heads, model_parallel_size):
         super().__init__()
         self.hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
         self.hidden_size_per_partition = divide(hidden_size, model_parallel_size)
         self.scale_mask_softmax = None
+
+        from sat.ops.scaled_mask_softmax import FusedScaleMaskSoftmax, AttnMaskType
+
         if FusedScaleMaskSoftmax is not None:
             self.scale_mask_softmax = FusedScaleMaskSoftmax(
                 input_in_fp16=True,
                 input_in_bf16=False,
                 attn_mask_type=AttnMaskType.padding,
                 scaled_masked_softmax_fusion=True,
                 mask_func=self.attention_mask_func,
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/glm_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     def position_embedding_forward(self, position_ids, **kwargs):
         position_ids, block_position_ids = position_ids[:, 0], position_ids[:, 1]
         position_embeddings = self.transformer.position_embeddings(position_ids)
         block_position_embeddings = self.block_position_embeddings(block_position_ids)
         return position_embeddings + block_position_embeddings
 
 class GLMModel(BaseModel):
-    def __init__(self, args, transformer=None, parallel_output=True):
-        super().__init__(args, transformer=transformer, parallel_output=parallel_output)
+    def __init__(self, args, transformer=None, **kwargs):
+        super().__init__(args, transformer=transformer, **kwargs)
         self.add_mixin('block_position_embedding', 
             BlockPositionEmbeddingMixin(args.max_sequence_length, args.hidden_size)
         )
     
     @classmethod
     def add_model_specific_args(cls, parser):
         """Arguments for GLM"""
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/vit_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,16 @@
         pre_word_embeddings = self.transformer.word_embeddings(input_ids[:,:self.property.pre_len])
         post_word_embeddings = self.transformer.word_embeddings(input_ids[:,self.property.pre_len:self.property.pre_len+self.property.post_len])
         embeddings = torch.cat([pre_word_embeddings, embeddings, post_word_embeddings], dim=1)
         return embeddings
 
 
 class InterpolatedPositionEmbeddingMixin(BaseMixin):
-    def __init__(self, hidden_size, old_property, property, init_method_std=0.02):
+    def __init__(self, property, init_method_std=0.02):
         super(InterpolatedPositionEmbeddingMixin, self).__init__()
-        self.old_property = old_property
         self.property = property
         self.init_method_std = init_method_std
 
     def interpolate_pos_encoding(self, height, width):
         """
         Adapted from https://github.com/huggingface/transformers/blob/master/src/transformers/models/vit/modeling_vit.py#L79
         This method allows to interpolate the pre-trained position encodings, to be able to use the model on higher
@@ -101,68 +100,60 @@
         * online mode: You need to interpolate position_embeddings for every forward pass.
 
         Input:
         * position_ids: (batch_size, seq_len)
         * kwargs["offline"]: boolean to identify offline or not
         * kwargs["height"], kwargs["width"]: specified image height and width for online mode
         """
-        if kwargs["offline"]:
-            return self.transformer.position_embeddings(position_ids)
-        else:
-            new_height, new_width = kwargs['height'], kwargs['width']
-            new_pos = self.interpolate_pos_encoding(new_height, new_width)
-            return new_pos[position_ids]
+        return self.transformer.position_embeddings.weight.unsqueeze(0)
 
-    def reinit(self, parent_model=None):
+    def reinit(self, parent_model=None, property=None):
         """
         new pre_len, new num_patches and new post_len should all be larger or equal than the old ones.
         """
+        assert property is not None
         old_weight = self.transformer.position_embeddings.weight.data
-        pre_weight = old_weight[:self.old_property.pre_len]
-        post_weight = old_weight[self.old_property.pre_len+self.old_property.num_patches:]
-        image_weight = old_weight[self.old_property.pre_len:self.old_property.pre_len+self.old_property.num_patches].reshape(1, self.old_property.grid_size[0], self.old_property.grid_size[1], -1).permute(0, 3, 1, 2)
-        image_weight = F.interpolate(image_weight, size=self.property.grid_size, mode='bicubic', align_corners=False).permute(0, 2, 3, 1).reshape(self.property.num_patches, -1)
-        self.transformer.position_embeddings = torch.nn.Embedding(self.property.seq_len, old_weight.shape[1]).type(old_weight.dtype).to(old_weight.device)
+        pre_weight = old_weight[:self.property.pre_len]
+        post_weight = old_weight[self.property.pre_len+self.property.num_patches:]
+        image_weight = old_weight[self.property.pre_len:self.property.pre_len+self.property.num_patches].reshape(1, self.property.grid_size[0], self.property.grid_size[1], -1).permute(0, 3, 1, 2)
+        image_weight = F.interpolate(image_weight, size=property.grid_size, mode='bicubic', align_corners=False).permute(0, 2, 3, 1).reshape(property.num_patches, -1)
+        self.transformer.position_embeddings = torch.nn.Embedding(property.seq_len, old_weight.shape[1]).type(old_weight.dtype).to(old_weight.device)
         torch.nn.init.normal_(self.transformer.position_embeddings.weight, mean=0.0, std=self.init_method_std)
-        self.transformer.position_embeddings.weight.data[:self.old_property.pre_len] = pre_weight
-        self.transformer.position_embeddings.weight.data[self.property.pre_len:self.property.pre_len+self.property.num_patches] = image_weight
-        self.transformer.position_embeddings.weight.data[self.property.pre_len+self.property.num_patches:self.property.pre_len+self.property.num_patches+self.old_property.post_len] = post_weight
+        self.transformer.position_embeddings.weight.data[:self.property.pre_len] = pre_weight
+        self.transformer.position_embeddings.weight.data[property.pre_len:property.pre_len+property.num_patches] = image_weight
+        self.transformer.position_embeddings.weight.data[property.pre_len+property.num_patches:property.pre_len+property.num_patches+self.property.post_len] = post_weight
+        self.property = property
 
 
 class ClsMixin(BaseMixin):
     def __init__(self, hidden_size, num_classes):
         super().__init__()
         self.classifier = nn.Linear(hidden_size, num_classes)
 
     def final_forward(self, logits, **kw_args):
         logits = self.classifier(logits[:, 0])
         return logits
 
 
 class ViTModel(BaseModel):
     def __init__(self, args, transformer=None, parallel_output=True, **kwargs):
-        self.property = ViTProperty(args.image_size, args.patch_size, args.pre_len, args.post_len)
-        assert args.old_image_size is not None and args.old_pre_len is not None and args.old_post_len is not None
-        self.old_property = ViTProperty(args.old_image_size, args.patch_size, args.old_pre_len, args.old_post_len)
-        args.max_sequence_length = self.old_property.pre_len + self.old_property.num_patches + self.old_property.post_len
+        property = ViTProperty(args.image_size, args.patch_size, args.pre_len, args.post_len)
+        args.max_sequence_length = property.pre_len + property.num_patches + property.post_len
         if 'activation_func' not in kwargs:
             kwargs['activation_func'] = gelu
         super().__init__(args, transformer=transformer, parallel_output=parallel_output, **kwargs)
-        self.add_mixin("patch_embedding", ImagePatchEmbeddingMixin(args.in_channels, args.hidden_size, self.property))
-        self.add_mixin("pos_embedding", InterpolatedPositionEmbeddingMixin(args.hidden_size, self.old_property, self.property))
+        self.add_mixin("patch_embedding", ImagePatchEmbeddingMixin(args.in_channels, args.hidden_size, property))
+        self.add_mixin("pos_embedding", InterpolatedPositionEmbeddingMixin(property))
         self.add_mixin("cls", ClsMixin(args.hidden_size, args.num_classes))
 
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('ViT', 'ViT Configurations')
         group.add_argument('--image-size', nargs='+', type=int, default=[224, 224])
         group.add_argument('--pre-len', type=int, default=1) # [cls] by default
         group.add_argument('--post-len', type=int, default=0) # empty by default, but sometimes with special tokens, such as [det] in yolos.
         group.add_argument('--in-channels', type=int, default=3)
         group.add_argument('--num-classes', type=int, default=21843)
         group.add_argument('--patch-size', type=int, default=16)
-        group.add_argument('--old-image-size', nargs='+', type=int, default=None)
-        group.add_argument('--old-pre-len', type=int, default=None)
-        group.add_argument('--old-post-len', type=int, default=None)
         return parser
```

### Comparing `SwissArmyTransformer-0.3.2/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.3.4/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.3.4/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.3.4/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.3.4/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/registry.py` & `SwissArmyTransformer-0.3.4/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/model/transformer.py` & `SwissArmyTransformer-0.3.4/sat/model/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from sat.mpu.layers import ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding
 from sat.mpu.mappings import gather_from_model_parallel_region, copy_to_model_parallel_region
 
 from deepspeed.runtime.activation_checkpointing.checkpointing import checkpoint
 
 from sat.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
 from sat.mpu.utils import split_tensor_along_last_dim
-from sat.ops import LayerNorm
+from sat.ops.layernorm import LayerNorm
 
 from sat.transformer_defaults import HOOKS_DEFAULT, standard_attention
 
 
 class SelfAttention(torch.nn.Module):
     def __init__(self, hidden_size, num_attention_heads,
                  attention_dropout_prob, output_dropout_prob,
@@ -108,15 +108,15 @@
 
 
 class CrossAttention(torch.nn.Module):
     """Parallel cross-attention layer for Transformer"""
 
     def __init__(self, hidden_size, num_attention_heads, attention_dropout_prob, output_dropout_prob, init_method,
                  layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True, hooks={},
-                 transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
+                 cross_attn_hidden_size=None, transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
         super().__init__()
         # Set output layer initialization if not provided.
         if output_layer_init_method is None:
             output_layer_init_method = init_method
         self.hooks = hooks
         self.layer_id = layer_id
         # Per attention head and per partition values.
@@ -129,15 +129,17 @@
         self.num_attention_heads_per_partition = divide(num_attention_heads, world_size)
         self.inner_hidden_size = num_attention_heads * self.hidden_size_per_attention_head
         self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
         # Strided linear layer.
         self.query = ColumnParallelLinear(hidden_size, self.inner_hidden_size,
                                           gather_output=False,
                                           init_method=init_method, bias=bias, params_dtype=params_dtype, module=self, name="query", skip_init=skip_init, device=device)
-        self.key_value = ColumnParallelLinear(hidden_size, 2 * self.inner_hidden_size,
+        if cross_attn_hidden_size is None:
+            cross_attn_hidden_size = hidden_size
+        self.key_value = ColumnParallelLinear(cross_attn_hidden_size, 2 * self.inner_hidden_size,
                                               stride=2,
                                               gather_output=False,
                                               init_method=init_method, bias=bias, params_dtype=params_dtype, module=self, name="key_value",
                                               skip_init=skip_init, device=device)
         # Dropout. Note that for a single iteration, this layer will generate
         # different outputs on different number of parallel partitions but
         # on average it should not be partition dependent.
@@ -241,28 +243,29 @@
             layer_id,
             inner_hidden_size=None,
             hidden_size_per_attention_head=None,
             output_layer_init_method=None,
             layernorm_order='pre',
             layernorm=LayerNorm,
             is_decoder=False,
+            cross_attn_hidden_size=None,
             use_bias=True,
             activation_func=gelu,
             hooks={},
             transformer_pointer=None,
             params_dtype=torch.float,
             skip_init=False,
             device=torch.device('cpu')
     ):
         super(BaseTransformerLayer, self).__init__()
         # Set output layer initialization if not provided.
         if output_layer_init_method is None:
             output_layer_init_method = init_method
         self.layer_id = layer_id
-        self.is_decoder = is_decoder
+        self.is_decoder = is_decoder[layer_id] if type(is_decoder) is list else is_decoder
         self.layernorm_order = layernorm_order
         self.hooks = hooks
         object.__setattr__(self, 'transformer', transformer_pointer)
         assert transformer_pointer is not None
 
         # Layernorm on the input data.
         self.input_layernorm = layernorm(hidden_size, eps=layernorm_epsilon)
@@ -298,14 +301,15 @@
                 num_attention_heads,
                 attention_dropout_prob,
                 output_dropout_prob,
                 init_method,
                 layer_id,
                 hidden_size_per_attention_head=hidden_size_per_attention_head,
                 output_layer_init_method=output_layer_init_method,
+                cross_attn_hidden_size=cross_attn_hidden_size,
                 bias=use_bias,
                 hooks=hooks,
                 transformer_pointer=transformer_pointer,
                 params_dtype=params_dtype
             )
             self.post_cross_attention_layernorm = layernorm(hidden_size, eps=layernorm_epsilon)
 
@@ -333,40 +337,49 @@
 class BaseTransformer(torch.nn.Module):
     def __init__(self,
                  num_layers,
                  vocab_size,
                  hidden_size,
                  num_attention_heads,
                  max_sequence_length,
-                 embedding_dropout_prob,
-                 attention_dropout_prob,
-                 output_dropout_prob,
-                 checkpoint_activations,
+                 embedding_dropout_prob=0,
+                 attention_dropout_prob=0,
+                 output_dropout_prob=0,
+                 checkpoint_activations=False,
                  checkpoint_num_layers=1,
                  layernorm_epsilon=1.0e-5,
                  init_method_std=0.02,
                  inner_hidden_size=None,
                  hidden_size_per_attention_head=None,
                  layernorm_order='pre',
                  parallel_output=True,
                  is_decoder=False,
+                 cross_attn_hidden_size=None,
                  use_bias=True,
                  activation_func=gelu,
                  layernorm=LayerNorm,
                  init_method=None,
                  use_final_layernorm=True,
                  hooks={},
                  params_dtype=torch.float,
                  skip_init=False,
                  device=torch.device('cpu')
                  ):
         super(BaseTransformer, self).__init__()
 
         # recording parameters
+        self.inner_hidden_size = inner_hidden_size
+        self.hidden_size_per_attention_head = hidden_size_per_attention_head
         self.is_decoder = is_decoder
+        self.cross_attn_hidden_size = cross_attn_hidden_size
+        if not is_decoder and cross_attn_hidden_size is not None:
+            print('warning: cross_attn_hidden_size is set but is_decoder is False')
+        self.use_bias = use_bias
+        self.use_final_layernorm = use_final_layernorm
+        self.layernorm_epsilon = layernorm_epsilon
         self.parallel_output = parallel_output
         self.checkpoint_activations = checkpoint_activations
         self.checkpoint_num_layers = checkpoint_num_layers
         self.max_sequence_length = max_sequence_length
         self.layernorm_order = layernorm_order
         self.hooks = copy.copy(hooks)  # hooks will be updated each forward
         object.__setattr__(self, 'transformer', self) # to give the default hooks the same api as outer hooks
@@ -398,14 +411,15 @@
                 layernorm_epsilon,
                 self.init_method,
                 layer_id,
                 inner_hidden_size=inner_hidden_size,
                 hidden_size_per_attention_head=hidden_size_per_attention_head,
                 output_layer_init_method=self.output_layer_init_method,
                 is_decoder=self.is_decoder,
+                cross_attn_hidden_size=cross_attn_hidden_size,
                 layernorm_order=layernorm_order,
                 layernorm=layernorm,
                 use_bias=use_bias,
                 activation_func=activation_func,
                 hooks=self.hooks,
                 transformer_pointer=self,
                 params_dtype=params_dtype,
@@ -413,15 +427,14 @@
                 device=device
             )
 
         self.layers = torch.nn.ModuleList(
             [get_layer(layer_id) for layer_id in range(num_layers)])
 
         # Final layer norm before output.
-        self.use_final_layernorm = use_final_layernorm
         if use_final_layernorm:
             self.final_layernorm = layernorm(hidden_size, eps=layernorm_epsilon)
 
     def forward(self, input_ids, position_ids, attention_mask, *,
                 output_hidden_states=False, **kw_args):
         # sanity check
         assert len(input_ids.shape) >= 2
```

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/__init__.py` & `SwissArmyTransformer-0.3.4/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.3.4/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/data.py` & `SwissArmyTransformer-0.3.4/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/initialize.py` & `SwissArmyTransformer-0.3.4/sat/mpu/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 """Model and data parallel groups."""
 
 import torch
 
 from .utils import ensure_divisibility
+from sat.helpers import print_rank0
 
 
 # Model parallel group that the current rank belongs to.
 _MODEL_PARALLEL_GROUP = None
 # Data parallel group that the current rank belongs to.
 _DATA_PARALLEL_GROUP = None
 
@@ -43,15 +44,15 @@
             [g0, g2, g4, g6], [g1, g3, g5, g7]
     Note that for efficiency, the caller should make sure adjacent ranks
     are on the same DGX box. For example if we are using 2 DGX-1 boxes
     with a total of 16 GPUs, rank 0 to 7 belong to the first box and
     ranks 8 to 15 belong to the second box.
     """
     if torch.distributed.get_rank() == 0:
-        print('> initializing model parallel with size {}'.format(
+        print_rank0('> initializing model parallel with size {}'.format(
             model_parallel_size_))
     # Get world size and rank. Ensure some consistencies.
     assert torch.distributed.is_initialized()
     world_size = torch.distributed.get_world_size()
     model_parallel_size = min(model_parallel_size_, world_size)
     ensure_divisibility(world_size, model_parallel_size)
     rank = torch.distributed.get_rank()
```

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/layers.py` & `SwissArmyTransformer-0.3.4/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/mappings.py` & `SwissArmyTransformer-0.3.4/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/mpu/utils.py` & `SwissArmyTransformer-0.3.4/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.3.4/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/resources/download.py` & `SwissArmyTransformer-0.3.4/sat/resources/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,41 +12,56 @@
 import math
 import random
 import requests
 from tqdm import tqdm
 from filelock import FileLock
 from .urls import MODEL_URLS
 
-def download_with_progress_bar(save_path, url):
-    with requests.get(url, stream=True) as r:
-        r.raise_for_status()
-        os.makedirs(os.path.dirname(save_path), exist_ok=True)
-        with open(save_path, 'wb') as f:
-            pbar = tqdm(total=int(r.headers['Content-Length']), unit_scale=True)
-            for chunk in r.iter_content(chunk_size=32 * 1024):
-                if chunk:  # filter out keep-alive new chunks
-                    f.write(chunk)
+def download_with_progress_bar(save_path, url, chunk_size=2048):
+    resume_header = None
+    file_size_downloaded = 0
+
+    os.makedirs(os.path.dirname(save_path), exist_ok=True)
+
+    if os.path.exists(save_path):
+        file_size_downloaded = os.path.getsize(save_path)
+        resume_header = {'Range': f'bytes={file_size_downloaded}-'}
+
+    response = requests.get(url, stream=True, headers=resume_header)
+    total_size = int(response.headers.get('content-length', 0)) + file_size_downloaded
+    if total_size == file_size_downloaded:
+        return
+    
+    with open(save_path, 'ab') as file:
+        with tqdm(total=total_size, unit='B', unit_scale=True, desc=save_path, initial=file_size_downloaded) as pbar:
+            for chunk in response.iter_content(chunk_size=chunk_size):
+                if chunk:
+                    file.write(chunk)
                     pbar.update(len(chunk))
 
 def auto_create(name, *, path=None, url=None):
     if path is None:
         path = os.getenv('SAT_HOME', '~/.sat_models') # TODO Rename
     path = os.path.expanduser(path)
     file_path = os.path.join(path, name + '.zip')
     model_path = os.path.join(path, name)
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     lock = FileLock(file_path + '.lock')
     with lock:
-        if os.path.exists(file_path) or os.path.isdir(model_path):
+        if os.path.isdir(model_path):
             pass
         else:
             if url is None:
                 url = MODEL_URLS[name]
             print(f'Downloading models {url} into {file_path} ...')
-            download_with_progress_bar(file_path, url)
+            try:
+                download_with_progress_bar(file_path, url)
+            except Exception as e:
+                print(f'Failed to download or check, if you already had the zip file, please unzip it manually as {model_path}!')
+                raise e
         # unzip
         if not os.path.isdir(model_path):
             import zipfile
             print(f'Unzipping {file_path}...')
             f = zipfile.ZipFile(file_path, 'r')
             f.extractall(path=path) # TODO check hierarcy of folders and name consistency
             assert os.path.isdir(model_path), f'Unzip failed, or the first-level folder in zip is not {name}.'
```

### Comparing `SwissArmyTransformer-0.3.2/sat/resources/urls.py` & `SwissArmyTransformer-0.3.4/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 
-from sat.training.utils import print_rank_0
+from sat.helpers import print_rank0
 
 
 def get_tokenizer(args=None, *, tokenizer_type=None, outer_tokenizer=None):
     '''
         If you're using outer_tokenizer, call `get_tokenizer(args, outer_tokenizer)`
         before `training_main`.
     '''
     if outer_tokenizer is not None: # set 1
         get_tokenizer.tokenizer = outer_tokenizer
         get_tokenizer.tokenizer_type = 'outer_tokenizer'
-        print_rank_0('> Set tokenizer as an outer_tokenizer! Now you can get_tokenizer() everywhere.')
+        print_rank0('> Set tokenizer as an outer_tokenizer! Now you can get_tokenizer() everywhere.')
         return outer_tokenizer
     if tokenizer_type is None:
         if args is None:
             assert hasattr(get_tokenizer, 'tokenizer'), 'Never set tokenizer.'
             return get_tokenizer.tokenizer
         tokenizer_type = args.tokenizer_type
 
@@ -65,25 +65,25 @@
         from .icetk_glm_130B import _IceTokenizer
         get_tokenizer.tokenizer = _IceTokenizer()
     # elif tokenizer_type.startswith('hf'):
     #     from .hf_tokenizer import HFT5Tokenizer
     #     if tokenizer_type == "hf_T5Tokenizer":
     #         get_tokenizer.tokenizer = HFT5Tokenizer(args.tokenizer_model_type, cache_dir=args.cache_dir)
     else:
-        print_rank_0('Try to load tokenizer from Huggingface transformers...')
+        print_rank0('Try to load tokenizer from Huggingface transformers...')
         os.environ['TOKENIZERS_PARALLELISM'] = 'true'
         from transformers import AutoTokenizer
         try:
             get_tokenizer.tokenizer = AutoTokenizer.from_pretrained(tokenizer_type, trust_remote_code=True)
         except OSError as e:
-            print_rank_0(f'Cannot find {tokenizer_type} from Huggingface or sat. Creating a fake tokenizer...')
+            print_rank0(f'Cannot find {tokenizer_type} from Huggingface or sat. Creating a fake tokenizer...')
             assert args.vocab_size > 0
             get_tokenizer.tokenizer = FakeTokenizer(args.vocab_size)
             return get_tokenizer.tokenizer
-    print_rank_0(f'> Set tokenizer as a {tokenizer_type} tokenizer! Now you can get_tokenizer() everywhere.')
+    print_rank0(f'> Set tokenizer as a {tokenizer_type} tokenizer! Now you can get_tokenizer() everywhere.')
     return get_tokenizer.tokenizer
 
 
 class FakeTokenizer(object):
     def __init__(self, num_tokens):
         self.num_tokens = num_tokens
```

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.3.4/sat/training/deepspeed_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
 from .learning_rates import AnnealingLR
 from .model_io import load_checkpoint, save_checkpoint
 
 from .utils import Timers
 from .utils import report_memory
 from .utils import print_args
-from .utils import print_rank_0
 from .utils import get_sample_writer
 
 from sat import mpu
 from sat.data_utils import make_loaders
-from sat.ops import LayerNorm
+from sat.ops.layernorm import LayerNorm
 from sat.arguments import set_random_seed, initialize_distributed
+from sat.helpers import print_rank0, print_all
 
 def training_main(args, model_cls, forward_step_function, create_dataset_function, handle_metrics_function=None, init_function=None, collate_fn=None, forward_step_eval=None):
     """Main training program."""
     hooks = {
         'forward_step': forward_step_function,
         'init_function': init_function,
         'create_dataset_function': create_dataset_function,
@@ -99,30 +99,30 @@
 
     # initialize lr scheduler
     lr_scheduler = get_learning_rate_scheduler(optimizer, args.iteration, args)
 
     summary_writer = None
     if torch.distributed.get_rank() == 0:
         if args.mode == 'pretrain':
-            print('Pretraining or Continuing training the Model...')
+            print_rank0('Pretraining or Continuing training the Model...')
         elif args.mode == 'finetune':
-            print('Finetuning Model...')
+            print_rank0('Finetuning Model...')
         print_args(args)
         summary_writer = get_sample_writer(base=args.summary_dir, name=args.experiment_name, iteration=args.iteration)
 
     # Resume data loader if necessary.
     if args.resume_dataloader:
         if not args.iterable_dataset:
             if train_data is not None:
                 train_data.batch_sampler.start_iter = args.iteration % len(train_data)
             if val_data is not None:
                 start_iter_val = (args.train_iters // args.save_interval) * args.eval_interval
                 val_data.batch_sampler.start_iter = start_iter_val % len(val_data)
         else:
-            print('Warning: we cannot resume iterable dataloader. skipping...')
+            print_rank0('Warning: we cannot resume iterable dataloader. skipping...')
 
     # training 
     iteration = 0
     if args.train_iters > 0:
         if args.do_train:
             with ExitStack() as stack:
                 def save_on_exit(args_, model_, optimizer_, lr_scheduler_):
@@ -144,27 +144,42 @@
         prefix = 'the end of training for test data'
         test_loss = evaluate_and_print_results(prefix, iter(test_data),
             model, len(test_data) if args.strict_eval else args.eval_iters, args, timers, True, split='test', hooks=hooks)
 
 def get_model(args, model_cls, **kwargs):
     """Build the model."""
 
-    print_rank_0(f'building {model_cls.__name__} model ...')
-    model = model_cls(args, **kwargs)
+    print_rank0(f'building {model_cls.__name__} model ...')
+    if 'params_dtype' not in kwargs:
+        if hasattr(args, 'fp16') and args.fp16:
+            params_dtype = torch.half
+        elif hasattr(args, 'bf16') and args.bf16:
+            params_dtype = torch.bfloat16
+        else:
+            params_dtype = torch.float32
+    else:
+        # pop params_dtype from kwargs
+        params_dtype = kwargs.pop('params_dtype')
+        
+    model = model_cls(args, params_dtype=params_dtype, **kwargs)
 
     if mpu.get_data_parallel_rank() == 0:
-        print(' > number of parameters on model parallel rank {}: {}'.format(
+        print_all(' > number of parameters on model parallel rank {}: {}'.format(
             mpu.get_model_parallel_rank(),
             sum([p.nelement() for p in model.parameters()])), flush=True)
-
-    model.cuda(torch.cuda.current_device())
+    
     if hasattr(args, 'fp16') and args.fp16:
         model.half()
     elif hasattr(args, 'bf16') and args.bf16:
         model.bfloat16()
+
+    if torch.cuda.is_available():
+        model.cuda(torch.cuda.current_device())
+    else:
+        print_rank0('No GPU detected, using CPU for inference.', level='WARNING')
     
     return model
 
 
 def setup_model_untrainable_params_and_optimizer(args, model, config_params=None):
     """Setup model and optimizer."""
 
@@ -172,15 +187,15 @@
         model.disable_untrainable_params() # mark trainable params
 
     param_groups = get_optimizer_param_groups(model)
 
     if args.train_data is not None:
         if args.deepspeed:
             from packaging import version
-            print_rank_0("DeepSpeed is enabled.")
+            print_rank0("DeepSpeed is enabled.", level='DEBUG')
             model, optimizer, _, _ = deepspeed.initialize(
                 model=model,
                 model_parameters=param_groups,
                 args=args,
                 mpu=mpu,
                 dist_init_required=False,
                 config_params=args.deepspeed_config
@@ -342,15 +357,15 @@
             evaluate_and_print_results(
                 prefix, val_data_iterator, model, eval_iters, args, timers, False, step=args.iteration, split='val', summary_writer=summary_writer, hooks=hooks)
 
         if args.exit_interval and args.iteration % args.exit_interval == 0:
             torch.distributed.barrier()
             time_str = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             rank = torch.distributed.get_rank()
-            print('rank: {} | time: {} | exiting the program at iteration {}'.
+            print_all('rank: {} | time: {} | exiting the program at iteration {}'.
                   format(rank, time_str, args.iteration), flush=True)
             exit()
 
     return args.iteration, skipped_iters
 
 
 def train_step(data_iterator, model, optimizer, lr_scheduler,
@@ -381,15 +396,15 @@
         for name in metrics:
             if not 'eval' in name:
                 metrics[name] = metrics[name].detach().clone()
                 torch.distributed.all_reduce(metrics[name].data)
                 metrics[name].data /= args.world_size
                 loss_checker = loss_checker + metrics[name]
         if loss_checker.isnan().any() or loss_checker.isinf().any():
-            print('Skipping backward and optimizer step for nan or inf in forwarding metrics/loss!')
+            print_all('Skipping backward and optimizer step for nan or inf in forwarding metrics/loss!')
             return lm_loss.detach(), 1, metrics
 
         # Accumulate the statistics
         lm_loss_total += lm_loss_reduced
         for name in metrics:
             if name not in metrics_total:
                 metrics_total[name] = 0.0
@@ -454,15 +469,15 @@
         drop_number = args.test_drop_number
     is_scalar = {}
     with torch.no_grad():
         iteration = 0
         while iteration < eval_iters:
             iteration += 1
             if verbose and iteration % args.log_interval == 0:
-                print_rank_0('Evaluating iter {}/{}'.format(iteration, eval_iters))
+                print_rank0('Evaluating iter {}/{}'.format(iteration, eval_iters))
             # Forward evaluation.
             # try:
             lm_loss, metrics = forward_step(data_iterator, model, args, timers)
             '''when contiguous memory optimizations are enabled, the buffers
             allocated by the optimizations are deallocated during backward pass
             in the absence of backward pass the buffers should be reset after each
             forward pass'''
@@ -530,15 +545,15 @@
     log_string += ' learning rate {:.3E} |'.format(lr)
     log_string += ' total loss {:.6E} |'.format(loss)
     for key in avg_metrics:
         log_string += ' {} {:.6E} |'.format(key, avg_metrics[key])
     if args.fp16:
         log_string += ' loss scale {:.1f} |'.format(
             optimizer.cur_scale if args.deepspeed else optimizer.loss_scale)
-    print_rank_0(log_string)
+    print_rank0(log_string)
     if summary_writer is not None:
         summary_writer.add_scalar(f'Train/lr', lr, step)
         summary_writer.add_scalar(f'Train/train_loss', loss, step)
         summary_writer.add_scalar(f'Train/elapsed_time', elapsed_time, step)
         for key in avg_metrics:
             summary_writer.add_scalar('Train/'+key, avg_metrics[key], step)
 
@@ -546,17 +561,17 @@
 def report_evaluate_metrics(summary_writer, prefix, loss, ppl, step, avg_metrics):
     string = ' validation loss at {} | '.format(prefix)
     string += 'loss: {:.6E} | '.format(loss)
     string += 'PPL: {:.6E}'.format(ppl)
     for key in avg_metrics:
         string += ' {} {:.6E} |'.format(key, avg_metrics[key].item())
     length = len(string) + 1
-    print_rank_0('-' * 100)
-    print_rank_0('-' * length)
-    print_rank_0(string)
-    print_rank_0('-' * length)
+    print_rank0('-' * 100)
+    print_rank0('-' * length)
+    print_rank0(string)
+    print_rank0('-' * length)
     if summary_writer is not None:
         summary_writer.add_scalar(f'Train/valid_ppl', ppl, step)
         summary_writer.add_scalar(f'Train/valid_loss', loss, step)
         for key in avg_metrics:
             summary_writer.add_scalar('Train/valid_'+key, avg_metrics[key], step)
```

### Comparing `SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/sat/training/learning_rates.py` & `SwissArmyTransformer-0.3.4/sat/training/learning_rates.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
 import math
 
+from sat.helpers import print_rank0
+
 
 class AnnealingLR(_LRScheduler):
     """Anneals the learning rate from start to zero along a cosine curve."""
 
     DECAY_STYLES = ['linear', 'cosine', 'exponential', 'constant', 'None']
 
     def __init__(self, optimizer, start_lr, warmup_iter, num_iters, decay_style=None, last_iter=-1, decay_ratio=0.5, auto_warmup_steps=50, auto_warmup_rate=0.05):
@@ -33,15 +35,15 @@
         self.end_iter = num_iters
         self.decay_style = decay_style.lower() if isinstance(decay_style, str) else None
         self.decay_ratio = 1 / decay_ratio
         self.auto_warmup_steps = auto_warmup_steps
         self.auto_warmup_rate = auto_warmup_rate
         self.step(self.num_iters)
         if not torch.distributed.is_initialized() or torch.distributed.get_rank() == 0:
-            print(f'learning rate decaying style {self.decay_style}, ratio {self.decay_ratio}')
+            print_rank0(f'learning rate decaying style {self.decay_style}, ratio {self.decay_ratio}')
 
     def get_lr(self):
         if self.num_iters <= self.init_step + self.auto_warmup_steps:
             return float(self.start_lr) * self.auto_warmup_rate
         
         if self.warmup_iter > 0 and self.num_iters <= self.warmup_iter:
             return float(self.start_lr) * self.num_iters / self.warmup_iter
```

### Comparing `SwissArmyTransformer-0.3.2/sat/training/model_io.py` & `SwissArmyTransformer-0.3.4/sat/training/model_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import random
 import torch
 import numpy as np
 import json
 import argparse
 
 from sat import mpu
-from .utils import print_rank_0
+from sat.helpers import print_rank0, print_all
 
 def get_checkpoint_name(checkpoints_path, iteration, release=False, zero=False):
     if release:
         d = 'release'
     else:
         d = '{:d}'.format(iteration)
     if zero:
@@ -50,17 +50,17 @@
         if hasattr(args, k):
             ret[k] = getattr(args, k)
     return ret
 
 def save_checkpoint(iteration, model, optimizer,
                     lr_scheduler, args):
     """Save a model checkpoint."""
-    if args.deepspeed:
+    if hasattr(args, 'deepspeed') and args.deepspeed:
         if mpu.get_data_parallel_rank() == 0:
-            print('Saving Model...')
+            print_rank0('Saving Model...')
             save_ds_checkpoint(iteration, model, lr_scheduler, args)
     elif args.mode == 'inference':
         os.makedirs(os.path.join(args.save, str(iteration)), exist_ok=True)
         torch.save({'module': model.state_dict()}, os.path.join(args.save, str(iteration), 'mp_rank_00_model_states.pt'))
     else:
         raise ValueError("training without deepspeed is not supported.")
     # Wait so everyone is done (necessary)
@@ -75,19 +75,37 @@
             module = model.module if hasattr(model, 'module') else model
             # model_class
             to_dump = {'model_class': type(module).__name__} 
             # tokenizer_type
             if args.tokenizer_type != 'fake':
                 to_dump['tokenizer_type'] = args.tokenizer_type 
             # architecture related args
-            arch_args_list = ['num_layers', 'hidden_size', 'num_attention_heads', 'vocab_size', 'hidden_dropout', 'attention_dropout',
-             'layernorm_order', 'inner_hidden_size', 'hidden_size_per_attention_head', 'model_parallel_size', 'max_sequence_length']
+            arch_args_list = ['num_layers', 'hidden_size', 'num_attention_heads', 'vocab_size',
+             'layernorm_order', 'model_parallel_size', 'max_sequence_length',
+             ]
             for name in arch_args_list: 
                 if hasattr(args, name) and getattr(args, name) is not None:
                     to_dump[name] = getattr(args, name)
+
+            # optional architecture related args, only save if not default
+            # optional means might be changed when loading 
+            optional_arch_args_list = [
+                ('is_decoder', False), 
+                ('cross_attn_hidden_size', None), 
+                ('use_bias', True),
+                ('inner_hidden_size', None),
+                ('hidden_size_per_attention_head', None),
+                ('use_final_layernorm', True),
+                ('layernorm_epsilon', 1e-5),
+            ]
+            if hasattr(module, 'transformer'):
+                for name, default in optional_arch_args_list:
+                    if module.transformer.__dict__[name] != default:
+                        to_dump[name] = module.transformer.__dict__[name]
+
             # model specific args
             model_specific_args = extract_model_specific_args_from_model(args, module)
             to_dump.update(model_specific_args)
 
             json.dump(to_dump, f, indent=4)
 
     # Wait so everyone is done (not necessary)
@@ -125,29 +143,29 @@
     return True
 
 
 def get_checkpoint_iteration(load_path):
     # Read the tracker file and set the iteration.
     tracker_filename = get_checkpoint_tracker_filename(load_path)
     if not os.path.isfile(tracker_filename):
-        print_rank_0('could not find the metadata file {} '.format(
+        print_rank0('could not find the metadata file {} '.format(
             tracker_filename))
         raise ValueError('could not find the metadata file {}, please check --load'.format(
             tracker_filename))
         return 0, False, False
     iteration = 0
     release = False
     with open(tracker_filename, 'r') as f:
         metastring = f.read().strip()
         try:
             iteration = int(metastring)
         except ValueError:
             release = metastring == 'release'
             if not release:
-                print_rank_0('ERROR: Invalid metadata file {}. Exiting'.format(
+                print_rank0('ERROR: Invalid metadata file {}. Exiting'.format(
                     tracker_filename))
                 exit()
     assert iteration > 0 or release, 'error parsing metadata file {}'.format(
         tracker_filename)
 
     return iteration, release, True
 
@@ -165,15 +183,15 @@
 
     iteration, release, success = get_checkpoint_iteration(load_path)
     if not success:
         return 0
     
     checkpoint_name = get_checkpoint_name(load_path, iteration, release)
     if mpu.get_data_parallel_rank() == 0:
-            print('global rank {} is loading checkpoint {}'.format(
+            print_all('global rank {} is loading checkpoint {}'.format(
                 torch.distributed.get_rank(), checkpoint_name))
     sd = torch.load(checkpoint_name, map_location='cpu')
     new_sd = {'module':{}}
     for k in sd:
         if k != 'module':
             new_sd[k] = sd[k]
     for k in sd['module']:
@@ -185,20 +203,20 @@
         module = model.module
     else: # inference without deepspeed
         module = model
 
     # only load module, other hyperparameters are just for recording.
     missing_keys, unexpected_keys = module.load_state_dict(sd['module'], strict=False)
     if len(unexpected_keys) > 0:
-        print_rank_0(
+        print_rank0(
             f'Will continue but found unexpected_keys! Check whether you are loading correct checkpoints: {unexpected_keys}.')
     if len(missing_keys) > 0:
         if args.mode == 'inference':
             if 'force_inference' in args and args.force_inference:
-                print(f'Warning: Missing keys for inference: {missing_keys}.')
+                print_rank0(f'Warning: Missing keys for inference: {missing_keys}.')
             else:
                 raise ValueError(f'Missing keys for inference: {missing_keys}.\nIf you still want to inference anyway, pass --force_inference to args.')
         else: # new params
             assert all(name.find('mixins')>=0 for name in missing_keys), missing_keys
             assert args.mode == 'finetune'
             # list all mixin names
             mixin_names = []
@@ -220,19 +238,19 @@
         try:
             random.setstate(sd['random_rng_state'])
             np.random.set_state(sd['np_rng_state'])
             torch.set_rng_state(sd['torch_rng_state'])
             torch.cuda.set_rng_state(sd['cuda_rng_state'])
             mpu.get_cuda_rng_tracker().set_states(sd['rng_tracker_states'])
         except KeyError:
-            print_rank_0('Unable to load optimizer from checkpoint {}, exiting. '
+            print_rank0('Unable to load optimizer from checkpoint {}, exiting. '
                          'Specify --no-load-rng or --finetune to prevent '
                          'attempting to load the random '
                          'state.'.format(checkpoint_name))
             exit()
     elif args.mode == 'inference':
         module.eval()
 
     if mpu.get_data_parallel_rank() == 0:
-        print('  successfully loaded {}'.format(checkpoint_name))
+        print_all('> successfully loaded {}'.format(checkpoint_name))
     del sd
     return iteration
```

### Comparing `SwissArmyTransformer-0.3.2/sat/training/utils.py` & `SwissArmyTransformer-0.3.4/sat/training/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,41 +16,42 @@
 """Utilities for logging and serialization"""
 
 import os
 import random
 import time
 import numpy as np
 import torch
+from sat.helpers import print_rank0
 
 from tensorboardX import SummaryWriter
 
 SUMMARY_WRITER_DIR_NAME = 'runs'
 
 def get_sample_writer(name, base="..", iteration=0):
     """Returns a tensorboard summary writer
     """
     return SummaryWriter(
         log_dir=os.path.join(base, SUMMARY_WRITER_DIR_NAME, name), purge_step=iteration)
 
 
-def print_rank_0(message):
-    if torch.distributed.is_initialized():
-        if torch.distributed.get_rank() == 0:
-            print(message, flush=True)
-    else:
-        print(message, flush=True)
+# def print_rank0(message):
+#     if torch.distributed.is_initialized():
+#         if torch.distributed.get_rank() == 0:
+#             print(message, flush=True)
+#     else:
+#         print(message, flush=True)
 
 
 def print_args(args):
     """Print arguments."""
 
-    print('arguments:', flush=True)
+    print_rank0('arguments:', flush=True)
     for arg in vars(args):
         dots = '.' * (29 - len(arg))
-        print('  {} {} {}'.format(arg, dots, getattr(args, arg)), flush=True)
+        print_rank0('  {} {} {}'.format(arg, dots, getattr(args, arg)), flush=True)
     if args.save_args:
         os.makedirs(os.path.join(args.summary_dir, SUMMARY_WRITER_DIR_NAME), exist_ok=True)
         with open(os.path.join(args.summary_dir, SUMMARY_WRITER_DIR_NAME, args.experiment_name+'.txt'), "w") as f:
             for arg in vars(args):
                 dots = '.' * (29 - len(arg))
                 f.write('  {} {} {}\n'.format(arg, dots, getattr(args, arg)))
 
@@ -116,24 +117,24 @@
         string = 'time (ms)'
         for name in names:
             if name not in self.timers:
                 continue
             elapsed_time = self.timers[name].elapsed(
                 reset=reset) * 1000.0 / normalizer
             string += ' | {}: {:.2f}'.format(name, elapsed_time)
-        print_rank_0(string)
+        print_rank0(string)
 
 
 def report_memory(name):
     """Simple GPU memory report."""
 
     mega_bytes = 1024.0 * 1024.0
     string = name + ' memory (MB)'
     string += ' | allocated: {}'.format(
         torch.cuda.memory_allocated() / mega_bytes)
     string += ' | max allocated: {}'.format(
         torch.cuda.max_memory_allocated() / mega_bytes)
     string += ' | cached: {}'.format(torch.cuda.memory_reserved() / mega_bytes)
     string += ' | max cached: {}'.format(
         torch.cuda.max_memory_reserved() / mega_bytes)
-    print_rank_0(string)
+    print_rank0(string)
```

### Comparing `SwissArmyTransformer-0.3.2/sat/transformer_defaults.py` & `SwissArmyTransformer-0.3.4/sat/transformer_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     if self.is_decoder:
         encoder_outputs = kw_args['encoder_outputs']
         if encoder_outputs is not None:
             assert 'cross_attention_mask' in kw_args
             # Cross attention
             attention_output = self.cross_attention(mlp_input, **kw_args)
             # Residual connection.
-            hidden_states = hidden_states + attention_output
+            hidden_states = mlp_input + attention_output
             # Layer norm post the cross attention
             mlp_input = self.post_cross_attention_layernorm(hidden_states)
 
     # MLP.
     mlp_output = self.mlp(mlp_input, **kw_args)
 
     # Fourth LayerNorm
```

### Comparing `SwissArmyTransformer-0.3.2/setup.py` & `SwissArmyTransformer-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.3.2',
+    version='0.3.4',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.3.2/tests/test_base_model.py` & `SwissArmyTransformer-0.3.4/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/tests/test_inference.py` & `SwissArmyTransformer-0.3.4/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.2/tests/test_train.py` & `SwissArmyTransformer-0.3.4/tests/test_train.py`

 * *Files identical despite different names*

