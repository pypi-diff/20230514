# Comparing `tmp/brocolli-3.0.0.tar.gz` & `tmp/brocolli-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brocolli-3.0.0.tar", last modified: Tue Feb 14 08:57:07 2023, max compression
+gzip compressed data, was "brocolli-4.0.1.tar", last modified: Sun May 14 09:53:51 2023, max compression
```

## Comparing `brocolli-3.0.0.tar` & `brocolli-4.0.1.tar`

### file list

```diff
@@ -1,139 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.140724 brocolli-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-14 08:56:50.000000 brocolli-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-14 08:57:07.140724 brocolli-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-02-14 08:56:50.000000 brocolli-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.116723 brocolli-3.0.0/brocolli/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.120724 brocolli-3.0.0/brocolli/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.136724 brocolli-3.0.0/brocolli/converter/onnx_layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/abs_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/add_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/avgpool_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/avgpool_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/batchnorm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/bnll_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/cast_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/celu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/chunk_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/clip_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/concat_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/conv_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/conv_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/conv_transpose_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/cosine_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/custom_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/div_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/dropout_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/elu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/elu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/embedding_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/exp_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/exp_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/flatten_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/flatten_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/gelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/gemm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/gemm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/getattr_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/getitem_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/gru_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/hardsigmoid_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/hardsigmoid_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/hardswish_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/hardswish_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/identity_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/layernorm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/leakyrelu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/leakyrelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/linear_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/linear_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/log_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/log_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/lstm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/matmul_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/max_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/mean_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/min_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/mul_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/neg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/normalize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/pad_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/pad_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/permute_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/pooling_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/pooling_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/power_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/prelu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/prelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/reduction_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/relu6_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/relu6_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/relu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/relu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/reshape_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/rnn_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/selu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/selu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sigmoid_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sigmoid_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sine_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/slice_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/softmax_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/softmax_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/softplus_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/softplus_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/split_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sqrt_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/squeeze_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/stack_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sub_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/sum_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/swish_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/tanh_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/tanh_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/tile_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/transpose_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/unbind_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/unsqueeze_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/upsample_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/onnx_layers/upsample_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56907 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/pytorch_caffe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/pytorch_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/pytorch_onnx_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.140724 brocolli-3.0.0/brocolli/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/graph_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/qconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.140724 brocolli-3.0.0/brocolli/quantization/quantization_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantization_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-14 08:56:50.000000 brocolli-3.0.0/brocolli/quantization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:57:07.116723 brocolli-3.0.0/brocolli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-14 08:57:07.000000 brocolli-3.0.0/brocolli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-14 08:57:07.000000 brocolli-3.0.0/brocolli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 08:57:07.000000 brocolli-3.0.0/brocolli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-14 08:57:07.000000 brocolli-3.0.0/brocolli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-14 08:57:07.000000 brocolli-3.0.0/brocolli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 08:56:50.000000 brocolli-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 08:57:07.140724 brocolli-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-14 08:56:50.000000 brocolli-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.928557 brocolli-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-14 09:53:41.000000 brocolli-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-14 09:53:51.928557 brocolli-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-14 09:53:41.000000 brocolli-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/converter/onnx_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/abs_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/add_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/baddbmm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/batchnorm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/bnll_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/cast_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/celu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/chunk_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/clip_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/concat_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_transpose_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/cosine_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/custom_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/div_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/dropout_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/elu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/elu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/embedding_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/exp_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/exp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/getattr_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/getitem_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/glu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gru_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/identity_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/layernorm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/linear_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/linear_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/log_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/log_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/lstm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/matmul_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/max_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/mean_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/min_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/mul_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/neg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/normalize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pad_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pad_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/permute_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/power_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/reduction_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/reshape_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/rnn_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/selu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/selu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sine_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/slice_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/split_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sqrt_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/squeeze_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/stack_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sub_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sum_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/swish_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tanh_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tanh_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tile_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/transpose_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/unbind_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/unsqueeze_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57317 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_caffe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/converter/pytorch_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/glu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_onnx_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/graph_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/qconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.928557 brocolli-4.0.1/brocolli/quantization/quantization_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-14 09:53:41.000000 brocolli-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:53:51.928557 brocolli-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-14 09:53:41.000000 brocolli-4.0.1/setup.py
```

### Comparing `brocolli-3.0.0/LICENSE` & `brocolli-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/PKG-INFO` & `brocolli-4.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brocolli
-Version: 3.0.0
+Version: 4.0.1
 Summary: everything in pytorch
 Home-page: https://github.com/inisis/brocolli
 Author: desmond
 Author-email: desmond.yao@buaa.edu.cn
 Project-URL: Bug Tracker, https://github.com/inisis/brocolli/issues
 Keywords: machine-learning,pytorch,caffe,torchfx
 Classifier: Programming Language :: Python :: 3
@@ -47,17 +47,20 @@
 * torch2onnx
     ```
     import torchvision.models as models
     from brocolli.converter.pytorch_onnx_parser import PytorchOnnxParser
 
     net = models.alexnet(pretrained=False)
     x = torch.rand(1, 3, 224, 224)
-    pytorch_parser = PytorchCaffeParser(net, x)
+    pytorch_parser = PytorchOnnxParser(net, x)
     pytorch_parser.convert()
     pytorch_parser.save('alexnet.onnx')
     ```
     run this script until you see "accuracy test passed" on screen, then you can get alexnet.onnx under current folder.
 
 # Contact
  QQ Group: 597059928
  
  ![image](https://raw.githubusercontent.com/inisis/brocolli/master/imgs/QGRPOUP.png)
+ 
+# Show your support
+  Give a 🌟 if this project helpes~
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `brocolli-3.0.0/README.md` & `brocolli-4.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -30,17 +30,20 @@
 * torch2onnx
     ```
     import torchvision.models as models
     from brocolli.converter.pytorch_onnx_parser import PytorchOnnxParser
 
     net = models.alexnet(pretrained=False)
     x = torch.rand(1, 3, 224, 224)
-    pytorch_parser = PytorchCaffeParser(net, x)
+    pytorch_parser = PytorchOnnxParser(net, x)
     pytorch_parser.convert()
     pytorch_parser.save('alexnet.onnx')
     ```
     run this script until you see "accuracy test passed" on screen, then you can get alexnet.onnx under current folder.
 
 # Contact
  QQ Group: 597059928
  
  ![image](https://raw.githubusercontent.com/inisis/brocolli/master/imgs/QGRPOUP.png)
+ 
+# Show your support
+  Give a 🌟 if this project helpes~
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/__init__.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,7 +88,9 @@
 from .avgpool_func import AvgPoolFunc
 from .normalize_func import NormalizeFunc
 from .getitem_func import GetItemFunc
 from .getattr_func import GetAttrFunc
 from .linear_func import LinearFunc
 from .unbind_func import UnbindFunc
 from .stack_func import StackFunc
+from .glu_func import GLUFunc
+from .baddbmm_func import BADDBMMFunc
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/add_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/add_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numbers
 import numpy as np
 import torch
 
 from .base_layer import BaseLayer
 from .cast_layer import CastLayer
-from ..utils import torch_dtype_to_numpy
+from ..onnx_utils import torch_dtype_to_numpy
 
 
 class AddLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(AddLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
@@ -107,12 +107,12 @@
                         self.generate_params(
                             np.array(self._source_node.args[0], dtype=numpy_dtype)
                         )
                     else:
                         self.generate_params(np.array(self._source_node.args[0]))
 
         node = helper.make_node("Add", self._in_names, self._out_names, self._name)
-        logger.info("add_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params, dtype=None):
         self.create_params(self._name + "_add_constant", params, dtype)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/avgpool_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/avgpool_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/base_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/base_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from onnx import helper
 from onnx.mapping import NP_TYPE_TO_TENSOR_TYPE
 from torch.fx.node import Node
-from ..utils import (
+from ..common_utils import (
     get_function_name,
     get_shape,
     map_reduce,
     get_dtype,
-    pytorch_dtype_to_onnx,
 )
+from ..onnx_utils import pytorch_dtype_to_onnx
 
 
 class BaseLayer(object):
     def __init__(self, source_node, module=None, auto_gen=True):
         self._source_node = source_node
         self._module = module
         self._auto_gen = auto_gen
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/batchnorm_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/batchnorm_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,19 @@
             self._name + "_mean", self._module.running_mean.detach().numpy()
         )
         self.create_params(
             self._name + "_var", self._module.running_var.detach().numpy()
         )
 
         attr_dict = self.get_batchnorm_attr()
-        logger.debug(attr_dict)
+        logger.debug(f"batchnorm_layer {self._name} attr_dict: {attr_dict}")
 
         node = helper.make_node(
             "BatchNormalization",
             self._in_names,
             self._out_names,
             self._name,
-            **attr_dict
+            **attr_dict,
         )
-        logger.info("batchnorm_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
 
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/bnll_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/exp_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class BnllLayer(BaseLayer):
+class ExpLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(BnllLayer, self).__init__(source_node, module, auto_gen)
+        super(ExpLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Softplus", self._in_names, self._out_names, self._name)
-        logging.info("Bnll_layer: " + self._name + " created")
+        node = helper.make_node("Exp", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/cast_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/elu_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class CastLayer(BaseLayer):
+class EluFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(CastLayer, self).__init__(source_node, module, auto_gen)
+        super(EluFunc, self).__init__(source_node, module, auto_gen)
 
-    def get_cast_attr(self):
-        attr_dict = {"to": 1}
+    def get_relu_attr(self):
+        attr_dict = {"alpha": 1.0}
+
+        attr_dict["alpha"] = self._source_node.kwargs["alpha"]
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
-
-        if attr_dict is None:
-            attr_dict = self.get_cast_attr()
-
+        attr_dict = self.get_relu_attr()
         node = helper.make_node(
-            "Cast", self._in_names, self._out_names, self._name, **attr_dict
+            "Elu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("cast_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/celu_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/elu_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class CeluFunc(BaseLayer):
+class EluLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(CeluFunc, self).__init__(source_node, module, auto_gen)
+        super(EluLayer, self).__init__(source_node, module, auto_gen)
 
-    def get_celu_attr(self):
+    def get_relu_attr(self):
         attr_dict = {"alpha": 0}
 
-        attr_dict["alpha"] = self._source_node.kwargs["alpha"]
+        attr_dict["alpha"] = self._module.alpha
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_celu_attr()
+        attr_dict = self.get_relu_attr()
         node = helper.make_node(
-            "Celu", self._in_names, self._out_names, self._name, **attr_dict
+            "Elu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("celu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/chunk_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/chunk_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,15 @@
     def __init__(self, source_node, module=None, auto_gen=True):
         super(ChunkFunc, self).__init__(source_node, module, auto_gen)
 
     def add_bottom_top(self, in_names=None, out_names=None):
         pass
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if "dim" in self._source_node.kwargs:
-            axis = self._source_node.kwargs["dim"]
-        else:
-            axis = self._source_node.args[2]
+        axis = self.get_value_by_key_or_index("dim", 2)
 
         if len(self._output_shape) == 1:
             slice_shape = self._output_shape[0][axis]
             slice_layer = SliceFunc(self._source_node, auto_gen=False)
             slice_layer.add_bottom_top(out_names=[self._source_node.name])
             params_slice = [
                 np.array([0]),
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/clip_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 from onnx import TensorProto as tp
 
 import numpy as np
 
 from .base_layer import BaseLayer
 
 
-class ClipFunc(BaseLayer):
+class Relu6Layer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(ClipFunc, self).__init__(source_node, module, auto_gen)
+        super(Relu6Layer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        params_clip = [
-            np.array(self._source_node.kwargs["min_val"]),
-            np.array(self._source_node.kwargs["max_val"]),
-        ]
-        self.generate_params(params_clip)
+        self.create_params(self._name + "_min", np.array(0, dtype=np.float32))
+        self.create_params(self._name + "_max", np.array(6, dtype=np.float32))
+
         node = helper.make_node("Clip", self._in_names, self._out_names, (self._name))
-        logger.info("relu6_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
-
-    def generate_params(self, params):
-        self.create_params(self._name + "_min", params[0])
-        self.create_params(self._name + "_max", params[1])
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/concat_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/mean_func.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from loguru import logger
 from onnx import helper
 from onnx import TensorProto as tp
-
+import numpy as np
 
 from .base_layer import BaseLayer
 
 
-class ConcatFunc(BaseLayer):
+class MeanFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(ConcatFunc, self).__init__(source_node, module, auto_gen)
+        super(MeanFunc, self).__init__(source_node, module, auto_gen)
+
+    def get_mean_attr(self):
+        attr_dict = {"keepdims": 1}
+
+        attr_dict["keepdims"] = self.get_value_by_key_or_index("keepdim", 2, False)
 
-    def get_concat_attr(self):
-        attr_dict = {"axis": []}
-        dim = self.get_value_by_key_or_index("dim", 1, 0)
+        dim = self.get_value_by_key_or_index("dim", 1, [1])
 
-        attr_dict["axis"] = dim
+        if isinstance(dim, int):
+            dim = [dim]
+
+        attr_dict["axes"] = dim
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
-
-        if attr_dict is None:
-            attr_dict = self.get_concat_attr()
+        attr_dict = self.get_mean_attr()
         node = helper.make_node(
-            "Concat", self._in_names, self._out_names, self._name, **attr_dict
+            "ReduceMean", self._in_names, self._out_names, self._name, **attr_dict
         )
 
-        logger.info("concat_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/conv_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,13 +61,13 @@
 
         attr_dict["group"] = groups
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_conv_attr()
-        logger.debug(attr_dict)
+        logger.debug(f"conv_layer: {self._name} attr_dict: {attr_dict}")
         node = helper.make_node(
             "Conv", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("conv_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/conv_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,13 +70,13 @@
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         self.create_params(self._name + "_weight", self._module.weight.detach().numpy())
         if self._module.bias is not None:
             self.create_params(self._name + "_bias", self._module.bias.detach().numpy())
 
         attr_dict = self.get_conv_attr()
-        logger.debug(attr_dict)
+        logger.debug(f"conv_layer: {self._name} attr_dict: {attr_dict}")
         node = helper.make_node(
             "Conv", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("conv_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/conv_transpose_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_transpose_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         self.create_params(self._name + "_weight", self._module.weight.detach().numpy())
         if self._module.bias is not None:
             self.create_params(self._name + "_bias", self._module.bias.detach().numpy())
 
         attr_dict = self.get_conv_attr()
-        logger.debug(attr_dict)
+        logger.debug(f"deconv_layer: {self._name} attr_dict: {attr_dict}")
         node = helper.make_node(
             "ConvTranspose", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("deconv_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/cosine_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/sqrt_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class CosineFunc(BaseLayer):
+class SqrtFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(CosineFunc, self).__init__(source_node, module, auto_gen)
+        super(SqrtFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Cos", self._in_names, self._out_names, self._name)
-        logger.info("cos_layer: " + self._name + " created")
+        node = helper.make_node("Sqrt", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/custom_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/custom_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/div_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/div_func.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,33 @@
 
 
 class DivFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(DivFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-
         assert len(self._source_node.args) == 2
         if len(self._source_node.all_input_nodes) == 1:
             if isinstance(self._source_node.args[0], Node):
                 assert isinstance(self._source_node.args[1], numbers.Number)
-                self.generate_params(np.array([self._source_node.args[1]]))
+                if isinstance(self._source_node.args[1], float):
+                    self.generate_params(
+                        np.array([self._source_node.args[1]]).astype(np.float32)
+                    )
+                else:
+                    self.generate_params(np.array([self._source_node.args[1]]))
             else:
                 assert isinstance(self._source_node.args[0], numbers.Number)
-                self.generate_params(np.array([self._source_node.args[0]]))
+                if isinstance(self._source_node.args[0], float):
+                    self.generate_params(
+                        np.array([self._source_node.args[0]]).astype(np.float32)
+                    )
+                else:
+                    self.generate_params(np.array([self._source_node.args[0]]))
 
         node = helper.make_node("Div", self._in_names, self._out_names, self._name)
 
-        logger.info("div_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params):
         self.create_params(self._name + "_add_constant", params)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/dropout_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/dropout_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 
 class DropoutLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(DropoutLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         node = helper.make_node("Dropout", self._in_names, self._out_names, self._name)
-        logger.info("dropout_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/elu_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/concat_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from loguru import logger
 from onnx import helper
+from onnx import TensorProto as tp
+
 
 from .base_layer import BaseLayer
 
 
-class EluFunc(BaseLayer):
+class ConcatFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(EluFunc, self).__init__(source_node, module, auto_gen)
+        super(ConcatFunc, self).__init__(source_node, module, auto_gen)
 
-    def get_relu_attr(self):
-        attr_dict = {"alpha": 1.0}
+    def get_concat_attr(self):
+        attr_dict = {"axis": []}
+        dim = self.get_value_by_key_or_index("dim", 1, 0)
 
-        attr_dict["alpha"] = self._source_node.kwargs["alpha"]
+        attr_dict["axis"] = dim
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_relu_attr()
+        if name is not None:
+            self._name = name
+
+        if attr_dict is None:
+            attr_dict = self.get_concat_attr()
         node = helper.make_node(
-            "Elu", self._in_names, self._out_names, self._name, **attr_dict
+            "Concat", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("elu_layer: " + self._name + " created")
+
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/elu_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class EluLayer(BaseLayer):
+class LeakyReluFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(EluLayer, self).__init__(source_node, module, auto_gen)
+        super(LeakyReluFunc, self).__init__(source_node, module, auto_gen)
 
     def get_relu_attr(self):
         attr_dict = {"alpha": 0}
 
-        attr_dict["alpha"] = self._module.alpha
+        attr_dict["alpha"] = float(self._source_node.kwargs["negative_slope"])
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_relu_attr()
         node = helper.make_node(
-            "Elu", self._in_names, self._out_names, self._name, **attr_dict
+            "LeakyRelu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("elu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/embedding_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/embedding_layer.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
         self._in_names.reverse()  # weight & input
 
         node = helper.make_node(
             "Gather", self._in_names, self._out_names, self._name, **attr_dict
         )
 
-        logger.info("gather_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/exp_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/identity_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
-
 
 from .base_layer import BaseLayer
 
 
-class ExpLayer(BaseLayer):
+class IdentityLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(ExpLayer, self).__init__(source_node, module, auto_gen)
+        super(IdentityLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Exp", self._in_names, self._out_names, self._name)
-        logger.info("exp_layer: " + self._name + " created")
+        node = helper.make_node("Identity", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/flatten_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/squeeze_func.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from loguru import logger
 import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
-
 from .base_layer import BaseLayer
 
 
-class FlattenFunc(BaseLayer):
+class SqueezeFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(FlattenFunc, self).__init__(source_node, module, auto_gen)
+        super(SqueezeFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        params = np.array(self._output_shape[0], dtype=np.int64)
+        if name is not None:
+            self._name = name
+
+        if params is None:
+            axes = self._source_node.args[1]
+            params = np.array([axes])
 
-        self.create_params(self._name + "_flatten", params)
+        self.create_params(self._name + "_squeeze", params)
 
-        node = helper.make_node("Reshape", self._in_names, self._out_names, self._name)
+        node = helper.make_node("Squeeze", self._in_names, self._out_names, self._name)
 
-        logger.info("flatten_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/flatten_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         if params is None:
             params = np.array(self._output_shape[0], dtype=np.int64)
 
         self.create_params(self._name + "_flatten", params)
 
         node = helper.make_node("Reshape", self._in_names, self._out_names, self._name)
 
-        logger.info("flatten_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/gelu_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/gelu_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 
 
 class GELULayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(GELULayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-
         node = helper.make_node(
             "GELU",
             self._in_names,
             self._out_names,
             self._name,
             domain="ai.onnx.contrib",
         )
-        logger.info("gelu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
 
 @onnx_op(
     op_type="GELU",
     inputs=[PyOp.dt_float],
     outputs=[PyOp.dt_float],
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/gemm_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_layer.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
 from .base_layer import BaseLayer
 
 
-class GemmFunc(BaseLayer):
+class GemmLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(GemmFunc, self).__init__(source_node, module, auto_gen)
+        super(GemmLayer, self).__init__(source_node, module, auto_gen)
 
     def get_gemm_attr(self):
         attr_dict = {"alpha": 1.0, "beta": 1.0, "transA": 0, "transB": 1}
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         if name is not None:
             self._name = name
 
-        attr_dict = self.get_gemm_attr()
+        self.create_params(self._name + "_weight", self._module.weight.detach().numpy())
+        if self._module.bias is not None:
+            self.create_params(self._name + "_bias", self._module.bias.detach().numpy())
 
+        attr_dict = self.get_gemm_attr()
         logger.debug(attr_dict)
         node = helper.make_node(
             "Gemm", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("gemm_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
+
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/gemm_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/sum_func.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from loguru import logger
 import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
+
 from .base_layer import BaseLayer
 
 
-class GemmLayer(BaseLayer):
+class SumFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(GemmLayer, self).__init__(source_node, module, auto_gen)
+        super(SumFunc, self).__init__(source_node, module, auto_gen)
+
+    def get_sum_attr(self):
+        attr_dict = {"keepdims": 1}
 
-    def get_gemm_attr(self):
-        attr_dict = {"alpha": 1.0, "beta": 1.0, "transA": 0, "transB": 1}
+        attr_dict["keepdims"] = self.get_value_by_key_or_index("keepdims", 2, False)
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
+        axes = self._source_node.args[1]
+        if isinstance(axes, int):
+            axes = [axes]
 
-        self.create_params(self._name + "_weight", self._module.weight.detach().numpy())
-        if self._module.bias is not None:
-            self.create_params(self._name + "_bias", self._module.bias.detach().numpy())
+        params = np.array(axes)
 
-        attr_dict = self.get_gemm_attr()
-        logger.debug(attr_dict)
+        self.create_params(self._name + "_sum", params)
+        attr_dict = self.get_sum_attr()
         node = helper.make_node(
-            "Gemm", self._in_names, self._out_names, self._name, **attr_dict
+            "ReduceSum", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("gemm_layer: " + self._name + " created")
 
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/getattr_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/getattr_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import torch
 from loguru import logger
 
 
 from .base_layer import BaseLayer
 
 
 class GetAttrFunc(BaseLayer):
@@ -16,11 +17,15 @@
         attr_itr = self._module
         for i, atom in enumerate(target_atoms):
             if not hasattr(attr_itr, atom):
                 raise RuntimeError(
                     f"Node referenced nonexistent target {'.'.join(target_atoms[:i])}"
                 )
             attr_itr = getattr(attr_itr, atom)
+        if not isinstance(attr_itr, torch.Tensor):
+            logger.warning(
+                "getattr_layer: " + self._name + " not created, because it's not Tensor"
+            )
+        else:
+            self.create_params(self._name, attr_itr.detach().numpy())
 
-        self.create_params(self._name, attr_itr.detach().numpy())
-
-        logger.info("getattr_layer: " + self._name + " created")
+            logger.info(f"{self.__class__.__name__}: {self._name} created")
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/getitem_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/getitem_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 import sys
+import torch
 from loguru import logger
 import numpy as np
 
 from .base_layer import BaseLayer
 from .slice_func import SliceFunc
 
 
+def gen_slice_params(args):
+    params_slices = []
+    for idx, function in enumerate(args):
+        if function.start is None and function.stop is None and function.step is None:
+            continue
+        else:
+            start_ = function.start if function.start is not None else 0
+            end_ = (
+                function.stop if function.stop is not None else sys.maxsize
+            )  # maybe a bug
+            axes_ = idx
+            step_ = function.step if function.step is not None else 1
+            if isinstance(end_, torch.fx.node.Node):
+                end_ = end_.meta["tensor_meta"]["value"]
+
+            params_slice = [
+                np.array([start_]),
+                np.array([end_]),
+                np.array([axes_]),
+                np.array([step_]),
+            ]
+            params_slices.append(params_slice)
+
+    return params_slices
+
+
 class GetItemFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(GetItemFunc, self).__init__(source_node, module, auto_gen)
 
     def add_bottom_top(self, in_names=None, out_names=None):
         pass
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if isinstance(self._source_node.args[1], tuple):
+        if isinstance(self._source_node.args[1], slice):
+            params_slices = gen_slice_params([self._source_node.args[1]])
+            slice_layer = SliceFunc(self._source_node, auto_gen=False)
+            slice_layer.add_bottom_top()
+            slice_layer.generate_node(params=params_slices[0])
+            self.node_post_process(slice_layer)
+        elif isinstance(self._source_node.args[1], tuple):
             if all(
                 isinstance(function, slice) for function in self._source_node.args[1]
             ):
-                params_slices = []
-                for idx, function in enumerate(self._source_node.args[1]):
-                    if (
-                        function.start is None
-                        and function.stop is None
-                        and function.step is None
-                    ):
-                        continue
-                    else:
-                        start_ = function.start if function.start is not None else 0
-                        end_ = (
-                            function.stop if function.stop is not None else sys.maxsize
-                        )  # maybe a bug
-                        axes_ = idx
-                        step_ = function.step if function.step is not None else 1
-
-                        params_slice = [
-                            np.array([start_]),
-                            np.array([end_]),
-                            np.array([axes_]),
-                            np.array([step_]),
-                        ]
-                        params_slices.append(params_slice)
+                params_slices = gen_slice_params(self._source_node.args[1])
                 if len(params_slices) == 1:
                     slice_layer = SliceFunc(self._source_node, auto_gen=False)
                     slice_layer.add_bottom_top()
                     slice_layer.generate_node(params=params_slices[0])
                     self.node_post_process(slice_layer)
                 else:
                     slice_layer = SliceFunc(self._source_node, auto_gen=False)
@@ -74,8 +85,8 @@
                         name=self._name + "_slice_" + str(len(params_slices) - 1),
                         params=params_slices[len(params_slices) - 1],
                     )
                     self.node_post_process(slice_layer)
             else:
                 raise
         else:
-            logger.info("getitem_layer: " + self._name + " not supported")
+            logger.info(f"{self.__class__.__name__}: {self._name} created")
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/gru_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/gru_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,14 @@
 
 
 class GRUCell(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(GRUCell, self).__init__(source_node, module, auto_gen)
 
     def get_gru_attr(self):
-
         attr_dict = {
             "hidden_size": [1],  # list of ints defaults is 1
         }
 
         attr_dict["hidden_size"] = self._module.hidden_size
         attr_dict["layout"] = 0  # 1 cannot infer
         if self._module.bidirectional is not False:
@@ -340,15 +339,15 @@
             self._name = name
 
         attr_dict = self.get_gru_attr()
         logger.debug(attr_dict)
         node = helper.make_node(
             "GRU", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("gru_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params, name=None):
         if name is not None:
             self._name = name
 
         self.create_params(self._name + "_weight", params[0])
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/hardsigmoid_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,9 @@
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_hardsigmoid_attr()
         node = helper.make_node(
             "HardSigmoid", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("hardsigmoid_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/hardsigmoid_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     def __init__(self, source_node, module=None, auto_gen=True):
         super(HardsigmoidLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         node = helper.make_node(
             "HardSigmoid", self._in_names, self._out_names, self._name
         )
-        logger.info("hardsigmoid_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/hardswish_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class HardswishFunc(BaseLayer):
+class HardswishLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(HardswishFunc, self).__init__(source_node, module, auto_gen)
+        super(HardswishLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         node = helper.make_node(
             "HardSwish", self._in_names, self._out_names, self._name
         )
-        logger.info("hardswish_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/hardswish_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_func.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from loguru import logger
+import numpy as np
 from onnx import helper
+from onnx import TensorProto as tp
+
 
 from .base_layer import BaseLayer
 
 
-class HardswishLayer(BaseLayer):
+class FlattenFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(HardswishLayer, self).__init__(source_node, module, auto_gen)
+        super(FlattenFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node(
-            "HardSwish", self._in_names, self._out_names, self._name
-        )
-        logger.info("hardswish_layer: " + self._name + " created")
+        params = np.array(self._output_shape[0], dtype=np.int64)
+
+        self.create_params(self._name + "_flatten", params)
+
+        node = helper.make_node("Reshape", self._in_names, self._out_names, self._name)
+
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/identity_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from loguru import logger
 from onnx import helper
+from onnx import TensorProto as tp
+import torch.nn as nn
 
 from .base_layer import BaseLayer
 
 
-class IdentityLayer(BaseLayer):
+class SoftmaxLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(IdentityLayer, self).__init__(source_node, module, auto_gen)
+        super(SoftmaxLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Identity", self._in_names, self._out_names, self._name)
-        logger.info("identity_layer: " + self._name + " created")
+        dim = self._module.dim
+        if dim is None:
+            stacklevel = 3
+            dim = nn.functional._get_softmax_dim(
+                "softmax",
+                len(self._input_shape[0]),
+                stacklevel,
+            )
+
+        node = helper.make_node(
+            "Softmax", self._in_names, self._out_names, self._name, axis=dim
+        )
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/input_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/input_layer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from loguru import logger
 from onnx import helper
 import torch
 from .base_layer import BaseLayer
-from ..utils import pytorch_dtype_to_onnx
+from ..onnx_utils import pytorch_dtype_to_onnx
 
 
 class InputLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(InputLayer, self).__init__(source_node, module, auto_gen)
         self._generate_input()
 
     def _generate_input(self):
         if self._output_type is not torch.Tensor:
             for idx in range(len(self._output_shape)):
                 onnx_type = pytorch_dtype_to_onnx(self._output_dtype[idx])
                 input_tvi = helper.make_tensor_value_info(
                     self._name + "_" + str(idx), onnx_type, self._output_shape[idx]
                 )
-                logger.info("input_layer: " + self._name + "_" + str(idx) + " created")
+                logger.info(f"{self.__class__.__name__}: {self._name} created")
                 self._in_tensor_value_info.append(input_tvi)
         else:
             onnx_type = pytorch_dtype_to_onnx(self._output_dtype[0])
             input_tvi = helper.make_tensor_value_info(
                 self._name, onnx_type, self._output_shape[0]
             )
-            logger.info("input_layer: " + self._name + " created")
+            logger.info(f"{self.__class__.__name__}: {self._name} created")
             self._in_tensor_value_info.append(input_tvi)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/layernorm_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/layernorm_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,27 +14,26 @@
         attr_dict = {"axis": "1", "eps": "1e-5"}
         attr_dict["axis"] = str(-len(self._module.normalized_shape))
         attr_dict["eps"] = str(self._module.eps)
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-
         self.create_params(self._name + "_weight", self._module.weight.detach().numpy())
         self.create_params(self._name + "_bias", self._module.bias.detach().numpy())
         attr_dict = self.get_layernorm_attr()
         node = helper.make_node(
             "LayerNormalization",
             self._in_names,
             self._out_names,
             self._name,
             domain="ai.onnx.contrib",
             attrs=str(attr_dict),
         )
-        logger.info("layernorm_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
 
 @onnx_op(
     op_type="LayerNormalization",
     inputs=[PyOp.dt_float, PyOp.dt_float, PyOp.dt_float],
     outputs=[PyOp.dt_float],
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/leakyrelu_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class LeakyReluFunc(BaseLayer):
+class LeakyReluLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(LeakyReluFunc, self).__init__(source_node, module, auto_gen)
+        super(LeakyReluLayer, self).__init__(source_node, module, auto_gen)
 
-    def get_relu_attr(self):
+    def get_leakyrelu_attr(self):
         attr_dict = {"alpha": 0}
 
-        attr_dict["alpha"] = float(self._source_node.kwargs["negative_slope"])
+        attr_dict["alpha"] = float(self._module.negative_slope)
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_relu_attr()
+        attr_dict = self.get_leakyrelu_attr()
         node = helper.make_node(
             "LeakyRelu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("leakyrelu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/leakyrelu_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/celu_func.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class LeakyReluLayer(BaseLayer):
+class CeluFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(LeakyReluLayer, self).__init__(source_node, module, auto_gen)
+        super(CeluFunc, self).__init__(source_node, module, auto_gen)
 
-    def get_leakyrelu_attr(self):
+    def get_celu_attr(self):
         attr_dict = {"alpha": 0}
 
-        attr_dict["alpha"] = float(self._module.negative_slope)
+        attr_dict["alpha"] = self._source_node.kwargs["alpha"]
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_leakyrelu_attr()
+        attr_dict = self.get_celu_attr()
         node = helper.make_node(
-            "LeakyRelu", self._in_names, self._out_names, self._name, **attr_dict
+            "Celu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("leakyrelu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/linear_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/linear_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/linear_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/linear_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/log_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/matmul_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from loguru import logger
 from onnx import helper
 from onnx import TensorProto as tp
 
-
 from .base_layer import BaseLayer
 
 
-class LogLayer(BaseLayer):
+class MatmulFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(LogLayer, self).__init__(source_node, module, auto_gen)
+        super(MatmulFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Log", self._in_names, self._out_names, self._name)
-        logging.info("log_layer: " + self._name + " created")
+        if name is not None:
+            self._name = name
+
+        node = helper.make_node("MatMul", self._in_names, self._out_names, self._name)
+
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
+
+    def generate_params(self, params):
+        self.create_params(self._name + "_matmul_constant", params)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/lstm_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/lstm_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,14 @@
 
 
 class LSTMCell(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(LSTMCell, self).__init__(source_node, module, auto_gen)
 
     def get_lstm_attr(self):
-
         attr_dict = {
             "hidden_size": [1],  # list of ints defaults is 1
         }
 
         attr_dict["hidden_size"] = self._module.hidden_size
         attr_dict["layout"] = 0  # 1 cannot infer
         if self._module.bidirectional is not False:
@@ -402,15 +401,15 @@
             self._name = name
 
         attr_dict = self.get_lstm_attr()
         logger.debug(attr_dict)
         node = helper.make_node(
             "LSTM", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("lstm_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params, name=None):
         if name is not None:
             self._name = name
 
         self.create_params(self._name + "_weight", params[0])
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/matmul_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/power_func.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from loguru import logger
+import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
+
 from .base_layer import BaseLayer
 
 
-class MatmulFunc(BaseLayer):
+class PowerFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(MatmulFunc, self).__init__(source_node, module, auto_gen)
+        super(PowerFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
-
-        node = helper.make_node("MatMul", self._in_names, self._out_names, self._name)
-
-        logger.info("matmul_layer: " + self._name + " created")
+        params = np.array([self._source_node.args[1]])
+        self.create_params(self._name + "_weight", params)
+        node = helper.make_node("Pow", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params):
-        self.create_params(self._name + "_matmul_constant", params)
+        self.create_params(self._name + "_weight", params)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/max_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/max_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_mean_attr()
         self._out_names[0] = self._name + "_0"
         node = helper.make_node(
             "ReduceMax", self._in_names, self._out_names, self._name, **attr_dict
         )
 
-        logger.info("max_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/mean_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/permute_func.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
-import numpy as np
 
 from .base_layer import BaseLayer
 
 
-class MeanFunc(BaseLayer):
+class PermuteFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(MeanFunc, self).__init__(source_node, module, auto_gen)
+        super(PermuteFunc, self).__init__(source_node, module, auto_gen)
 
-    def get_mean_attr(self):
-        attr_dict = {"keepdims": 1}
+    def gen_transpose_attr(self):
+        attr_dict = {"perm": []}
+        order = []
+        for arg in self._source_node.args:
+            if isinstance(arg, int):
+                order.append(arg)
+            elif isinstance(arg, (list, tuple)):
+                order.extend(arg)
 
-        attr_dict["keepdims"] = self.get_value_by_key_or_index("keepdim", 2, False)
-
-        dim = self.get_value_by_key_or_index("dim", 1, [1])
-
-        if isinstance(dim, int):
-            dim = [dim]
-
-        attr_dict["axes"] = dim
+        attr_dict["perm"] = order
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_mean_attr()
+        if name is not None:
+            self._name = name
+
+        if attr_dict is None:
+            attr_dict = self.gen_transpose_attr()
+
         node = helper.make_node(
-            "ReduceMean", self._in_names, self._out_names, self._name, **attr_dict
+            "Transpose", self._in_names, self._out_names, self._name, **attr_dict
         )
-
-        logger.info("mean_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/mul_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/mul_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from loguru import logger
 from onnx import helper
 from torch.fx.node import Node
 import numbers
 import numpy as np
 
 from .base_layer import BaseLayer
-from ..utils import torch_dtype_to_numpy
+from ..onnx_utils import torch_dtype_to_numpy
 
 
 class MulLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(MulLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
@@ -33,15 +33,15 @@
                             np.array([self._source_node.args[0]], dtype=numpy_dtype)
                         )
                     else:
                         self.generate_params(np.array([self._source_node.args[0]]))
 
             node = helper.make_node("Mul", self._in_names, self._out_names, self._name)
 
-            logger.info("mul_layer: " + self._name + " created")
+            logger.info(f"{self.__class__.__name__}: {self._name} created")
             self._node.append(node)
         else:
             mul_layer = MulFunc(self._source_node, self._module, auto_gen=False)
             mul_layer.add_bottom_top(in_names=self._in_names)
             mul_layer.generate_node(self._name)
             self.node_post_process(mul_layer)
 
@@ -50,14 +50,16 @@
 
 
 class MulFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(MulFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
+        if name is not None:
+            self._name = name
         node = helper.make_node("Mul", self._in_names, self._out_names, self._name)
 
-        logger.info("mul_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params, dtype=None):
         self.create_params(self._name + "_mul_constant", params, dtype)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/neg_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from loguru import logger
 from onnx import helper
 from onnx import TensorProto as tp
 
+import numpy as np
 
 from .base_layer import BaseLayer
 
 
-class NegFunc(BaseLayer):
+class Relu6Func(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(NegFunc, self).__init__(source_node, module, auto_gen)
+        super(Relu6Func, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Neg", self._in_names, self._out_names, self._name)
-        logger.info("neg_layer: " + self._name + " created")
+        self.create_params(self._name + "_min", np.array(0, dtype=np.float32))
+        self.create_params(self._name + "_max", np.array(6, dtype=np.float32))
+        node = helper.make_node("Clip", self._in_names, self._out_names, (self._name))
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/normalize_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/normalize_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,9 +17,9 @@
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_relu_attr()
         node = helper.make_node(
             "LpNormalization", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("lpnormalization_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/output_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/output_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from loguru import logger
 from onnx import helper
 from onnx import TensorProto as tp
 import torch
 
 from .base_layer import BaseLayer
-from ..utils import pytorch_dtype_to_onnx
+from ..onnx_utils import pytorch_dtype_to_onnx
 
 
 class OutputLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(OutputLayer, self).__init__(source_node, module, auto_gen)
         self.generate_output()
 
@@ -18,22 +18,22 @@
     def generate_output(self):
         if self._output_type is torch.Tensor or len(self._output_shape) == 1:
             name = self.recursive_find_name(self._source_node.all_input_nodes[0])
             onnx_type = pytorch_dtype_to_onnx(self._output_dtype[0])
             output_tvi = helper.make_tensor_value_info(
                 name, onnx_type, self._output_shape[0]
             )
-            logger.info("output_layer: " + name + " created")
+            logger.info(f"{self.__class__.__name__}: {self._name} created")
             self._out_tensor_value_info.append(output_tvi)
         elif len(self._output_shape) == len(self._source_node.all_input_nodes):
             for idx, shape in enumerate(self._output_shape):
                 name = self.recursive_find_name(self._source_node.all_input_nodes[idx])
                 onnx_type = pytorch_dtype_to_onnx(self._output_dtype[idx])
                 output_tvi = helper.make_tensor_value_info(name, onnx_type, shape)
-                logger.info("output_layer: " + name + " created")
+                logger.info(f"{self.__class__.__name__}: {self._name} created")
                 self._out_tensor_value_info.append(output_tvi)
         else:
             for idx, shape in enumerate(self._output_shape):
                 name = self.recursive_find_name(self._source_node.all_input_nodes[0])
                 onnx_type = pytorch_dtype_to_onnx(self._output_dtype[idx])
                 output_tvi = helper.make_tensor_value_info(
                     name + "_" + str(idx), onnx_type, shape
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/pad_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/pad_func.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class PadFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(PadFunc, self).__init__(source_node, module, auto_gen)
 
     def gen_pad_attr(self):
         attr_dict = {"mode": "constant"}
 
-        mode = self._source_node.kwargs["mode"]
+        mode = self.get_value_by_key_or_index("mode", 2, "constant")
 
         if mode == "replicate":
             attr_dict["mode"] = "edge"
         elif mode == "reflection":
             attr_dict["mode"] = "reflect"
 
         return attr_dict
@@ -35,24 +35,23 @@
             padding = self._source_node.args[1]
 
             for idx in range(len(padding) // 2):
                 pads[output_dim - idx - 1] = padding[idx * 2]
                 pads[output_dim * 2 - idx - 1] = padding[idx * 2 + 1]
 
             params = np.array(pads)
+            value = self.get_value_by_key_or_index("value", 3, 0.0)
 
-            value = self._source_node.kwargs["value"]
-
-            params = [np.array(pads), np.array(value)]
+            params = [np.array(pads), np.array(value).astype(np.float32)]
 
         if attr_dict is None:
             attr_dict = self.gen_pad_attr()
 
         self.create_params(self._name + "_pad", params[0])
         self.create_params(self._name + "_value", params[1])
 
         node = helper.make_node(
             "Pad", self._in_names, self._out_names, self._name, **attr_dict
         )
 
-        logger.info("pad_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/pad_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/pad_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,21 +37,21 @@
                 pads[output_dim - idx - 1] = padding[idx * 2]
                 pads[output_dim * 2 - idx - 1] = padding[idx * 2 + 1]
 
             if hasattr(self._module, "value"):
                 value = self._module.value
             else:
                 value = 0.0
-            params = [np.array(pads), np.array(value)]
+            params = [np.array(pads), np.array(value).astype(np.float32)]
 
         self.create_params(self._name + "_pad", params[0])
         self.create_params(self._name + "_value", params[1])
 
         if attr_dict is None:
             attr_dict = self.gen_pad_attr()
 
         node = helper.make_node(
             "Pad", self._in_names, self._out_names, self._name, **attr_dict
         )
 
-        logger.info("pad_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/permute_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/transpose_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class PermuteFunc(BaseLayer):
+class TransposeFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(PermuteFunc, self).__init__(source_node, module, auto_gen)
+        super(TransposeFunc, self).__init__(source_node, module, auto_gen)
 
     def gen_transpose_attr(self):
         attr_dict = {"perm": []}
-        order = []
-        for arg in self._source_node.args:
-            if isinstance(arg, int):
-                order.append(arg)
-            elif isinstance(arg, (list, tuple)):
-                order.extend(arg)
+        input_dim = len(self._output_shape[0])
+        axes = list(range(input_dim))
+        axes[self._source_node.args[1]], axes[self._source_node.args[2]] = (
+            axes[self._source_node.args[2]],
+            axes[self._source_node.args[1]],
+        )
 
-        attr_dict["perm"] = order
+        attr_dict["perm"] = axes
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         if name is not None:
             self._name = name
 
         if attr_dict is None:
             attr_dict = self.gen_transpose_attr()
 
         node = helper.make_node(
             "Transpose", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("transpose_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/pooling_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 class PoolingFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(PoolingFunc, self).__init__(source_node, module, auto_gen)
 
     def get_pooling_attr(self, function_name):
-
         pool_dim = int(re.findall(r"(?:pool)([0-9]d*?)", str(function_name))[0])
 
         attr_dict = {
             "kernel_shape": [],
             "strides": [1, 1],
             "pads": [0, 0, 0, 0],
             "ceil_mode": False,
@@ -46,16 +45,15 @@
             else:
                 attr_dict["strides"] = attr_dict["kernel_shape"] = k
 
             attr_dict["pads"] = [0] * (pool_dim * 2)
 
             return attr_dict
 
-        kernel_size = self._source_node.args[1]
-
+        kernel_size = self.get_value_by_key_or_index("kernel_size", 1, None)
         stride = self.get_value_by_key_or_index("stride", 2, kernel_size)
         padding = self.get_value_by_key_or_index("padding", 3, 0)
         ceil_mode = self.get_value_by_key_or_index("ceil_mode", 4, False)
 
         if isinstance(kernel_size, tuple):
             if len(kernel_size) == 1:
                 attr_dict["kernel_shape"] = kernel_size * pool_dim
@@ -124,16 +122,16 @@
             else:
                 attr_dict = self.get_pooling_attr(function_name)
                 node = helper.make_node(
                     "AveragePool",
                     self._in_names,
                     self._out_names,
                     self._name,
-                    **attr_dict
+                    **attr_dict,
                 )
         elif function_name == "avg_pool2d" or function_name == "avg_pool1d":
             attr_dict = self.get_pooling_attr(function_name)
             node = helper.make_node(
                 "AveragePool", self._in_names, self._out_names, self._name, **attr_dict
             )
-        logger.info("pooling_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/pooling_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,23 @@
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         if name is not None:
             self._name = name
 
-        if isinstance(self._module, (nn.MaxPool1d, nn.MaxPool2d)):
+        if isinstance(self._module, (nn.MaxPool1d, nn.MaxPool2d, nn.MaxPool3d)):
             attr_dict = self.get_pooling_attr()
             node = helper.make_node(
                 "MaxPool", self._in_names, self._out_names, self._name, **attr_dict
             )
-        elif isinstance(self._module, (nn.AdaptiveAvgPool1d, nn.AdaptiveAvgPool2d)):
+        elif isinstance(
+            self._module,
+            (nn.AdaptiveAvgPool1d, nn.AdaptiveAvgPool2d, nn.AdaptiveAvgPool3d),
+        ):
             if isinstance(self._module.output_size, int):
                 output_size = [self._module.output_size]
                 output_size_len = 1
             else:
                 output_size = [int(v) for v in self._module.output_size]
                 output_size_len = len(self._module.output_size)
             if output_size == [1] * output_size_len:
@@ -107,16 +110,20 @@
             else:
                 attr_dict = self.get_pooling_attr()
                 node = helper.make_node(
                     "AveragePool",
                     self._in_names,
                     self._out_names,
                     self._name,
-                    **attr_dict
+                    **attr_dict,
                 )
         elif isinstance(self._module, (nn.AvgPool1d, nn.AvgPool2d)):
             attr_dict = self.get_pooling_attr()
             node = helper.make_node(
                 "AveragePool", self._in_names, self._out_names, self._name, **attr_dict
             )
-        logger.info("pooling_layer: " + self._name + " created")
+        else:
+            raise NotImplementedError(
+                "module %s is not implemented" % (self._module.__class__.__name__)
+            )
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/power_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/neg_func.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from loguru import logger
-import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class PowerFunc(BaseLayer):
+class NegFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(PowerFunc, self).__init__(source_node, module, auto_gen)
+        super(NegFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        params = np.array([self._source_node.args[1]])
-        self.create_params(self._name + "_weight", params)
-        node = helper.make_node("Pow", self._in_names, self._out_names, self._name)
-        logger.info("power_layer: " + self._name + " created")
+        node = helper.make_node("Neg", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
-
-    def generate_params(self, params):
-        self.create_params(self._name + "_weight", params)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/prelu_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_func.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         if out_names is None:
             out_names = [self._name]
 
         self._in_names.extend(in_names)
         self._out_names.extend(out_names)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-
         target_atoms = self._source_node.args[1].target.split(".")
         attr_itr = self._module
         for i, atom in enumerate(target_atoms):
             if not hasattr(attr_itr, atom):
                 raise RuntimeError(
                     f"Node referenced nonexistent target {'.'.join(target_atoms[:i])}"
                 )
@@ -36,9 +35,9 @@
             param_shape = [1] * len(shape)
             param_shape[1] = params.shape[0]
             params = params.reshape(param_shape)
             self.create_params(self._name + "_prelu", params)
 
         node = helper.make_node("PRelu", self._in_names, self._out_names, self._name)
 
-        logger.info("prelu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/prelu_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,9 +26,9 @@
             param_shape = [1] * len(shape)
             param_shape[1] = weight.shape[0]
             params = weight.reshape(param_shape)
 
         self.create_params(self._name + "_prelu", params)
         node = helper.make_node("PRelu", self._in_names, self._out_names, self._name)
 
-        logger.info("prelu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/reduction_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/reduction_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/relu6_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_func.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from loguru import logger
+import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
-import numpy as np
-
 from .base_layer import BaseLayer
 
 
-class Relu6Func(BaseLayer):
+class GemmFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(Relu6Func, self).__init__(source_node, module, auto_gen)
+        super(GemmFunc, self).__init__(source_node, module, auto_gen)
+
+    def get_gemm_attr(self):
+        attr_dict = {"alpha": 1.0, "beta": 1.0, "transA": 0, "transB": 1}
+
+        return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        self.create_params(self._name + "_min", np.array(0, dtype=np.float32))
-        self.create_params(self._name + "_max", np.array(6, dtype=np.float32))
-        node = helper.make_node("Clip", self._in_names, self._out_names, (self._name))
-        logger.info("relu6_layer: " + self._name + " created")
+        if name is not None:
+            self._name = name
+
+        attr_dict = self.get_gemm_attr()
+
+        logger.debug(attr_dict)
+        node = helper.make_node(
+            "Gemm", self._in_names, self._out_names, self._name, **attr_dict
+        )
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/relu6_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_layer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from loguru import logger
 from onnx import helper
 from onnx import TensorProto as tp
 
-import numpy as np
 
 from .base_layer import BaseLayer
 
 
-class Relu6Layer(BaseLayer):
+class SigmoidLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(Relu6Layer, self).__init__(source_node, module, auto_gen)
+        super(SigmoidLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        self.create_params(self._name + "_min", np.array(0, dtype=np.float32))
-        self.create_params(self._name + "_max", np.array(6, dtype=np.float32))
+        if name is not None:
+            self._name = name
 
-        node = helper.make_node("Clip", self._in_names, self._out_names, (self._name))
-        logger.info("relu6_layer: " + self._name + " created")
+        node = helper.make_node("Sigmoid", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/reshape_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/reshape_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,9 +27,9 @@
         if params is None:
             params = np.array(self._output_shape[0], dtype=np.int64)
 
         self.create_params(self._name + "_reshape", params)
 
         node = helper.make_node("Reshape", self._in_names, self._out_names, self._name)
 
-        logger.info("reshape_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/rnn_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/rnn_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,14 @@
 
 
 class RNNCell(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
         super(RNNCell, self).__init__(source_node, module, auto_gen)
 
     def get_rnn_attr(self):
-
         attr_dict = {
             "hidden_size": [1],  # list of ints defaults is 1
         }
 
         attr_dict["hidden_size"] = self._module.hidden_size
         attr_dict["layout"] = 0  # 1 cannot infer
         if self._module.bidirectional is not False:
@@ -351,15 +350,15 @@
             self._name = name
 
         attr_dict = self.get_rnn_attr()
         logger.debug(attr_dict)
         node = helper.make_node(
             "RNN", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("rnn_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
 
     def generate_params(self, params, name=None):
         if name is not None:
             self._name = name
 
         self.create_params(self._name + "_weight", params[0])
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/selu_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_func.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from loguru import logger
 from onnx import helper
+from onnx import TensorProto as tp
+
 
 from .base_layer import BaseLayer
 
 
-class SeluFunc(BaseLayer):
+class SigmoidFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SeluFunc, self).__init__(source_node, module, auto_gen)
-
-    def get_relu_attr(self):
-        attr_dict = {"alpha": 1.67326, "beta": 1.0507}
-
-        return attr_dict
+        super(SigmoidFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        attr_dict = self.get_relu_attr()
-        node = helper.make_node("Selu", self._in_names, self._out_names, self._name)
-        logger.info("selu_layer: " + self._name + " created")
+        if name is not None:
+            self._name = name
+        node = helper.make_node("Sigmoid", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/selu_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/selu_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         attr_dict = self.get_selu_attr()
         logger.debug(attr_dict)
         node = helper.make_node(
             "Selu", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("selu_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/sigmoid_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_layer.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class SigmoidFunc(BaseLayer):
+class SoftplusLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SigmoidFunc, self).__init__(source_node, module, auto_gen)
+        super(SoftplusLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Sigmoid", self._in_names, self._out_names, self._name)
-        logger.info("sigmoid_layer: " + self._name + " created")
+        node = helper.make_node("Softplus", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/sigmoid_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/sine_func.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class SigmoidLayer(BaseLayer):
+class SineFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SigmoidLayer, self).__init__(source_node, module, auto_gen)
+        super(SineFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
-
-        node = helper.make_node("Sigmoid", self._in_names, self._out_names, self._name)
-        logger.info("sigmoid_layer: " + self._name + " created")
+        node = helper.make_node("Sin", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/sine_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/unsqueeze_func.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 from loguru import logger
+import numpy as np
 from onnx import helper
-from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class SineFunc(BaseLayer):
+class UnsqueezeFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SineFunc, self).__init__(source_node, module, auto_gen)
+        super(UnsqueezeFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Sin", self._in_names, self._out_names, self._name)
-        logger.info("sine_layer: " + self._name + " created")
+        if name is not None:
+            self._name = name
+
+        if params is None:
+            axes = self._source_node.args[1]
+            params = np.array([axes])
+
+        self.create_params(self._name + "_unsqueeze", params)
+        node = helper.make_node(
+            "Unsqueeze", self._in_names, self._out_names, self._name
+        )
+
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/slice_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/slice_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
 class SliceFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
@@ -16,9 +15,9 @@
 
         self.create_params(self._name + "_start", params[0])
         self.create_params(self._name + "_end", params[1])
         self.create_params(self._name + "_axes", params[2])
         self.create_params(self._name + "_steps", params[3])
 
         node = helper.make_node("Slice", self._in_names, self._out_names, self._name)
-        logger.info("slice_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/softmax_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_func.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,9 +19,9 @@
                 len(self._input_shape[0]),
                 stacklevel,
             )
 
         node = helper.make_node(
             "Softmax", self._in_names, self._out_names, self._name, axis=dim
         )
-        logger.info("softmax_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/softplus_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_func.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class SoftplusFunc(BaseLayer):
+class HardswishFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SoftplusFunc, self).__init__(source_node, module, auto_gen)
+        super(HardswishFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Softplus", self._in_names, self._out_names, self._name)
-        logger.info("softplus_layer: " + self._name + " created")
+        node = helper.make_node(
+            "HardSwish", self._in_names, self._out_names, self._name
+        )
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/softplus_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_func.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
-
 
 from .base_layer import BaseLayer
 
 
-class SoftplusLayer(BaseLayer):
+class SoftplusFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SoftplusLayer, self).__init__(source_node, module, auto_gen)
+        super(SoftplusFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         node = helper.make_node("Softplus", self._in_names, self._out_names, self._name)
-        logger.info("softplus_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/split_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/split_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,17 @@
                 for idx in range(len(self._output_shape)):
                     out_names.append(self._name + "_" + str(idx))
 
         self._in_names.extend(in_names)
         self._out_names.extend(out_names)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
+        if name is not None:
+            self._name = name
+
         if params is None:
             if "dim" in self._source_node.kwargs:
                 axis = self._source_node.kwargs["dim"]
             else:
                 axis = self._source_node.args[2]
 
             shape = []
@@ -52,9 +55,9 @@
             attr_dict = self.get_split_attr()
 
         self.create_params(self._name + "_split", params)
 
         node = helper.make_node(
             "Split", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("split_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/sqrt_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/bnll_layer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
-
+from loguru import logger
 
 from .base_layer import BaseLayer
 
 
-class SqrtFunc(BaseLayer):
+class BnllLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(SqrtFunc, self).__init__(source_node, module, auto_gen)
+        super(BnllLayer, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        node = helper.make_node("Sqrt", self._in_names, self._out_names, self._name)
-        logger.info("sqrt_layer: " + self._name + " created")
+        node = helper.make_node("Softplus", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/stack_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/stack_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/swish_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/swish_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/template.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,9 +28,9 @@
             # handle non user-defined situation optional
             attr_dict = self.get_template_attr()
 
         self.create_params(self._name, params)
         node = helper.make_node(
             "template", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("template_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/tile_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/tile_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         if params is None:
             repeats = np.array(self._output_shape[0]) // np.array(self._input_shape[0])
             params = np.array(repeats, dtype=np.int64)
 
         self.create_params(self._name + "_tile", params)
 
         node = helper.make_node("Tile", self._in_names, self._out_names, self._name)
-        logger.info("tile_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/transpose_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/cast_layer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 from loguru import logger
 from onnx import helper
 
 from .base_layer import BaseLayer
 
 
-class TransposeFunc(BaseLayer):
+class CastLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(TransposeFunc, self).__init__(source_node, module, auto_gen)
+        super(CastLayer, self).__init__(source_node, module, auto_gen)
 
-    def gen_transpose_attr(self):
-        attr_dict = {"perm": []}
-        input_dim = len(self._output_shape[0])
-        axes = list(range(input_dim))
-        axes[self._source_node.args[1]], axes[self._source_node.args[2]] = (
-            axes[self._source_node.args[2]],
-            axes[self._source_node.args[1]],
-        )
-
-        attr_dict["perm"] = axes
+    def get_cast_attr(self):
+        attr_dict = {"to": 1}
 
         return attr_dict
 
     def generate_node(self, name=None, params=None, attr_dict=None):
         if name is not None:
             self._name = name
 
         if attr_dict is None:
-            attr_dict = self.gen_transpose_attr()
+            attr_dict = self.get_cast_attr()
 
         node = helper.make_node(
-            "Transpose", self._in_names, self._out_names, self._name, **attr_dict
+            "Cast", self._in_names, self._out_names, self._name, **attr_dict
         )
-        logger.info("transpose_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/unbind_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/unbind_func.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from loguru import logger
-from onnx import helper
-from onnx import TensorProto as tp
 import numpy as np
 
 from .base_layer import BaseLayer
 from .split_func import SplitFunc
 from .squeeze_func import SqueezeFunc
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/unsqueeze_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/cosine_func.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 from loguru import logger
-import numpy as np
 from onnx import helper
 from onnx import TensorProto as tp
 
 
 from .base_layer import BaseLayer
 
 
-class UnsqueezeFunc(BaseLayer):
+class CosineFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
-        super(UnsqueezeFunc, self).__init__(source_node, module, auto_gen)
+        super(CosineFunc, self).__init__(source_node, module, auto_gen)
 
     def generate_node(self, name=None, params=None, attr_dict=None):
-        if name is not None:
-            self._name = name
-
-        if params is None:
-            axes = self._source_node.args[1]
-            params = np.array([axes])
-
-        self.create_params(self._name + "_unsqueeze", params)
-        node = helper.make_node(
-            "Unsqueeze", self._in_names, self._out_names, self._name
-        )
-
-        logger.info("unsqueeze_layer: " + self._name + " created")
+        node = helper.make_node("Cos", self._in_names, self._out_names, self._name)
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/upsample_func.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
 import numpy as np
 
 from .base_layer import BaseLayer
 
 
 class UpsampleFunc(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
@@ -33,9 +32,9 @@
 
         scales = np.array(scales, dtype="float32")
         self.create_params(self._name + "_roi", np.array([], dtype=np.float32))
         self.create_params(self._name + "_scale", scales)
         node = helper.make_node(
             "Resize", self._in_names, self._out_names, self._name, mode="nearest"
         )
-        logger.info("upsample_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/onnx_layers/upsample_layer.py` & `brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from loguru import logger
 from onnx import helper
-from onnx import TensorProto as tp
 import numpy as np
 
 from .base_layer import BaseLayer
 
 
 class UpsampleLayer(BaseLayer):
     def __init__(self, source_node, module=None, auto_gen=True):
@@ -35,9 +34,9 @@
 
         scales = np.array(scales, dtype="float32")
         self.create_params(self._name + "_roi", np.array([]))
         self.create_params(self._name + "_scale", scales)
         node = helper.make_node(
             "Resize", self._in_names, self._out_names, self._name, mode="nearest"
         )
-        logger.info("upsample_layer: " + self._name + " created")
+        logger.info(f"{self.__class__.__name__}: {self._name} created")
         self._node.append(node)
```

### Comparing `brocolli-3.0.0/brocolli/converter/optimizer.py` & `brocolli-4.0.1/brocolli/converter/optimizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 def get_default_fusion_patterns():
     return DEFAULT_FUSION_PATTERNS
 
 
 def graph_constant_fold_inplace(graph):
     for node in graph.nodes:
         if node.op == "Identity" or node.op == "Dropout":
-            inp_node = node.i()
-            inp_node.outputs = node.outputs
+            input_node = node.i()
+            input_node.outputs.remove(node.inputs[0])
+            input_node.outputs.append(node.outputs[0])
             node.outputs.clear()
 
 
 @register_fusion_pattern("GELU")
 def find_gelu_nodes(node):
     # fmt: off
     '''
@@ -82,29 +83,29 @@
          \      /
             Mul
     '''
     # fmt: on
     match = {}
     if node.op == "Mul":
         if node.i(1).op == "Sigmoid":
-            input_variable = node.i(1).inputs[0]
-            mul_node = node.i(1)
-            sigmoid_node = node
-
-            input_variable.outputs.remove(mul_node)
-            input_variable.outputs.remove(sigmoid_node)
-
-            output_variable = node.outputs[0]
-            output_variable.inputs.clear()
-            match.update(
-                {
-                    "inputs": [input_variable],
-                    "outputs": [output_variable],
-                }
-            )
+            sigmoid_node = node.i(1)
+            mul_node = node
+            if sigmoid_node.inputs[0] in mul_node.inputs:
+                input_variable = node.i(1).inputs[0]
+                input_variable.outputs.remove(sigmoid_node)
+                input_variable.outputs.remove(mul_node)
+
+                output_variable = node.outputs[0]
+                output_variable.inputs.clear()
+                match.update(
+                    {
+                        "inputs": [input_variable],
+                        "outputs": [output_variable],
+                    }
+                )
 
     return match
 
 
 @register_fusion_pattern("LayerNormalization")
 def find_layernorm_nodes(node):
     # fmt: off
@@ -172,14 +173,49 @@
                         )
                     },
                 }
             )
     return match
 
 
+# @register_fusion_pattern("GLU")
+def find_glu_nodes(node):
+    # fmt: off
+    '''
+             x
+             |
+           Split
+         /      \
+         |    Sigmoid
+         \      /
+            Mul
+    '''
+    # fmt: on
+    match = {}
+    if node.op == "Mul":
+        if node.i(1).op == "Sigmoid":
+            sigmoid_node = node.i(1)
+            mul_node = node
+            if sigmoid_node.inputs[0] in mul_node.inputs:
+                input_variable = node.i(1).inputs[0]
+                input_variable.outputs.remove(sigmoid_node)
+                input_variable.outputs.remove(mul_node)
+
+                output_variable = node.outputs[0]
+                output_variable.inputs.clear()
+                match.update(
+                    {
+                        "inputs": [input_variable],
+                        "outputs": [output_variable],
+                    }
+                )
+
+    return match
+
+
 @gs.Graph.register()
 def replace_custom_layer(
     self, op, inputs, outputs, name, attrs=None, domain="ai.onnx.contrib"
 ):
     return self.layer(
         op=op,
         inputs=inputs,
@@ -195,15 +231,15 @@
     counter = Counter()
     for node in reversed(graph.nodes):
         if node.name not in match_map:
             for layer_type, func in fusion_patterns.items():
                 with contextlib.suppress(IndexError):
                     match = func(node)
                     if match:
-                        logger.debug("matched patter {}", layer_type)
+                        logger.debug(f"matched pattern {layer_type}")
                         match.update({"op": layer_type})
                         match.update(
                             {
                                 "name": "{}_{}".format(
                                     layer_type.lower(), counter[layer_type]
                                 )
                             }
@@ -220,11 +256,13 @@
     graph = gs.import_onnx(model)
     graph.fold_constants().cleanup()
     fusion_patterns = get_default_fusion_patterns()
     fusion_pairs = find_matches(graph, fusion_patterns)
     for _, match in fusion_pairs.items():
         graph.replace_custom_layer(**match)
     graph_constant_fold_inplace(graph)
-    graph.cleanup(remove_unused_graph_inputs=True).toposort()
+    graph.cleanup(
+        remove_unused_node_outputs=True, remove_unused_graph_inputs=True
+    ).toposort()
     model = gs.export_onnx(graph)
 
     return model
```

### Comparing `brocolli-3.0.0/brocolli/converter/pytorch_caffe_parser.py` & `brocolli-4.0.1/brocolli/converter/pytorch_caffe_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from builtins import isinstance
 import numpy as np
 from loguru import logger
 from brocolli.converter.pytorch_graph import PytorchGraph
 import caffe.proto.caffe_pb2 as pb2
 
 import caffe
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.utils.fusion import fuse_conv_bn_eval, fuse_linear_bn_eval
 from torch.fx.node import Node
 from torch.fx.graph_module import GraphModule
 import google.protobuf.text_format
-from .utils import get_function_name
+from .common_utils import get_function_name
 
 
 def as_blob(array):
     blob = pb2.BlobProto()
     blob.shape.dim.extend(array.shape)
     blob.data.extend(array.astype(float).flat)
     return blob
@@ -51,16 +50,16 @@
     def convert(self):
         self.text_net, self.binary_weights = self.gen_ir()
 
     def save(self, dest_path):
         self.dest_path = dest_path
         self.save_to_proto(self.text_net, dest_path + ".prototxt")
         self.save_weights(self.binary_weights, dest_path + ".caffemodel")
-        logger.info("prototxt saved to {}.prototxt".format(dest_path))
-        logger.info("caffemodel saved to {}.caffemodel".format(dest_path))
+        logger.info(f"prototxt saved to {dest_path}.prototxt")
+        logger.info(f"caffemodel saved to {dest_path}.caffemodel")
 
     def save_to_proto(self, net, filename):
         with open(filename, "wb") as f:
             f.write(google.protobuf.text_format.MessageToString(net).encode())
 
     def save_weights(self, weights, filename):
         with open(filename, "wb") as f:
@@ -350,14 +349,17 @@
                     layer_data = self.rename_sub(node)
                     self.layers.append(layer_data)
                 elif function_name == "abs":
                     layer_data = self.rename_abs(node)
                     self.layers.append(layer_data)
                 elif function_name == "getattr":
                     pass
+                elif function_name == "interpolate":
+                    layer_data = self.rename_interpolate(node)
+                    self.layers.append(layer_data)
                 else:
                     raise NotImplementedError(
                         "function %s is not implemented" % (function_name)
                     )
             elif node.op == "call_method":
                 if str(node.target) == "size":
                     pass
@@ -764,24 +766,34 @@
             if isinstance(arg, int):
                 layer.permute_param.order.extend([arg])
 
         self.add_bottom_top(layer, source_node)
 
         return layer
 
-    def rename_Upsample(self, source_node, module):
+    def rename_Upsample(self, source_node, module=None):
         layer = pb2.LayerParameter()
         layer.type = "Upsample"
 
         layer.upsample_param.scale = int(module.scale_factor)
 
         self.add_bottom_top(layer, source_node)
 
         return layer
 
+    def rename_interpolate(self, source_node, module=None):
+        layer = pb2.LayerParameter()
+        layer.type = "Upsample"
+
+        layer.upsample_param.scale = int(source_node.kwargs["scale_factor"])
+
+        self.add_bottom_top(layer, source_node)
+
+        return layer
+
     def rename_Cat(self, source_node):
         layer = pb2.LayerParameter()
         layer.type = "Concat"
 
         if "dim" in source_node.kwargs:
             layer.concat_param.axis = source_node.kwargs["dim"]
         else:
```

### Comparing `brocolli-3.0.0/brocolli/converter/pytorch_graph.py` & `brocolli-4.0.1/brocolli/converter/pytorch_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 import torch.nn as nn
 
 import torch.fx
 from torch.fx import Tracer, Interpreter
 from torch.fx.graph_module import GraphModule
 from torch.fx.node import map_aggregate
 
-from .utils import get_function_name, map_replace, gen_torch_tensor
+import numbers
+from loguru import logger
+from tabulate import tabulate
+
+from .common_utils import get_function_name
 from .pytorch_layer.transformer import (
     Transformer,
     TransformerEncoder,
     TransformerDecoder,
     TransformerEncoderLayer,
     TransformerDecoderLayer,
 )
 from .pytorch_layer.mha import MultiheadAttention
-
 from .pytorch_layer.layernorm import LayerNorm
+from .pytorch_layer.glu import GLU
 
 
 class BrocolliTracer(Tracer):
     def __init__(self, *args, customed_leaf_module=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.customed_leaf_module = customed_leaf_module
 
     def is_leaf_module(self, m: torch.nn.Module, module_qualified_name: str):
         if self.customed_leaf_module and isinstance(m, self.customed_leaf_module):
-
             return True
 
         if hasattr(m, "_is_leaf_module") and m._is_leaf_module:
             return True
 
         return m.__module__.startswith("torch.nn") and not isinstance(
             m, torch.nn.Sequential
@@ -40,22 +43,26 @@
 class BrocolliShapeRunner(Interpreter):
     def __init__(self, module, dynamic_batch=False):
         super(BrocolliShapeRunner, self).__init__(module)
         self.dynamic_batch = dynamic_batch
 
     def run_node(self, n):
         result = super().run_node(n)
+        if isinstance(result, numbers.Number):
+            result = torch.tensor(result)
 
         found_tensor = False
 
         def extract_tensor_metadata(result: torch.Tensor):
             meta_info = {}
             shape = list(result.shape)
             if self.dynamic_batch:
                 shape[0] = -1
+
+            meta_info["value"] = result
             meta_info["shape"] = torch.Size(shape)
             meta_info["dtype"] = result.dtype
 
             return meta_info
 
         def extract_tensor_meta(obj):
             if isinstance(obj, torch.Tensor):
@@ -87,24 +94,35 @@
         elif isinstance(self.model, nn.Module):
             self.replace(self.model)
             self.tracer = BrocolliTracer()
             self.graph = self.tracer.trace(self.model, concrete_args)
             self.graph_module = GraphModule(self.tracer.root, self.graph)
             if concrete_args is not None:
                 self.trace_prune(self.graph_module)
-            self.shape_inference()
+            with torch.no_grad():
+                self.shape_inference()
         else:
             raise Exception(
                 "model must be a torch.nn.Module \
                             or a torch.fx.GraphModule"
             )
 
         self.graph = self.graph_module.graph
         self.nodes = list(self.graph_module.graph.nodes)
-        self.graph.print_tabular()
+        self.print_tabular(self.graph_module)
+
+    def print_tabular(self, graph_module):
+        nodes = list(graph_module.graph.nodes)
+        node_specs = [[n.op, n.name, n.target, n.args, n.kwargs] for n in nodes]
+        logger.debug(
+            tabulate(
+                node_specs,
+                headers=["\nopcode", "\nname", "\ntarget", "\nargs", "\nkwargs"],
+            )
+        )
 
     def replace(self, model):
         for name, module in model.named_children():
             if isinstance(module, nn.Transformer):
                 converted_module = Transformer.from_torch(module)
                 setattr(model, name, converted_module)
             elif isinstance(module, nn.TransformerEncoder):
@@ -118,14 +136,20 @@
                 setattr(model, name, converted_module)
             elif isinstance(module, nn.TransformerDecoderLayer):
                 converted_module = TransformerDecoderLayer.from_torch(module)
                 setattr(model, name, converted_module)
             elif isinstance(module, nn.MultiheadAttention):
                 converted_module = MultiheadAttention.from_torch(module)
                 setattr(model, name, converted_module)
+            elif isinstance(module, nn.LayerNorm):
+                converted_module = LayerNorm.from_torch(module)
+                setattr(model, name, converted_module)
+            elif isinstance(module, nn.GLU):
+                converted_module = GLU(dim=module.dim)
+                setattr(model, name, converted_module)
             elif list(module.named_children()):
                 self.replace(module)
 
     def placeholder_prune(self, graph_module):
         for node in list(graph_module.graph.nodes):
             if node.op == "placeholder" and node.next.op == "call_function":
                 function_name = get_function_name(node.next.target)
```

### Comparing `brocolli-3.0.0/brocolli/converter/pytorch_onnx_parser.py` & `brocolli-4.0.1/brocolli/converter/pytorch_onnx_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,63 @@
+import sys
 import time
 import numpy as np
 from loguru import logger
 import torch
 import torch.nn as nn
 from torch.fx.graph_module import GraphModule
 from onnx import save, helper, checker, defs, load
-from tabulate import tabulate
 
 torch.manual_seed(0)
 np.random.seed(0)
 
 from .onnx_layers import *
 from .pytorch_graph import PytorchGraph
-from .utils import (
+from .common_utils import (
     fuse_all_conv_bn,
     get_function_name,
     map_reduce,
     gen_numpy_data,
 )
 from .optimizer import optimize_model
 
 
 class PytorchOnnxParser:
     def __init__(
-        self, model, inputs, fuse=False, concrete_args=None, dynamic_batch=False
+        self,
+        model,
+        inputs,
+        fuse=False,
+        concrete_args=None,
+        dynamic_batch=False,
+        level=1,
     ):
         super(PytorchOnnxParser, self).__init__()
         self.model = model.eval()
         self.inputs = inputs
         if isinstance(self.inputs, torch.Tensor):
             self.inputs = [self.inputs]
         self.fuse = fuse
         self.concrete_args = concrete_args
         self.dynamic_batch = dynamic_batch
+        self.init_logging(level)
+        self.pyotrch_inference()
 
-    def print_tabular(self, graph_module):
-        nodes = list(graph_module.graph.nodes)
-        node_specs = [[n.op, n.name, n.target, n.args, n.kwargs] for n in nodes]
-        logger.debug(
-            tabulate(
-                node_specs,
-                headers=["\nopcode", "\nname", "\ntarget", "\nargs", "\nkwargs"],
-            )
-        )
+    def init_logging(self, level):
+        logger.remove()
+        if level == 0:
+            logger.add(sys.stderr, level="DEBUG")
+        elif level == 1:
+            logger.add(sys.stderr, level="INFO")
+        elif level == 2:
+            logger.add(sys.stderr, level="WARNING")
+        elif level == 3:
+            logger.add(sys.stderr, level="ERROR")
+        else:
+            raise Exception("level must be 0, 1, 2 or 3")
 
     def convert(self):
         if isinstance(self.model, GraphModule):
             pass
         elif isinstance(self.model, nn.Module):
             if self.fuse:
                 fuse_all_conv_bn(self.model)
@@ -68,27 +79,32 @@
     def gen_onnx_graph(self):
         for node in self.pytorch_graph.nodes:
             if node.op == "placeholder":
                 input_layer = InputLayer(node)
                 self.node_post_process(input_layer)
             elif node.op == "call_module":
                 module = self.modules[node.target]
-                if isinstance(module, (nn.Conv2d, nn.Conv1d)):
+                if isinstance(module, (nn.Conv1d, nn.Conv2d, nn.Conv3d)):
                     conv_layer = ConvLayer(node, module)
                     self.node_post_process(conv_layer)
-                elif isinstance(module, nn.BatchNorm2d):
+                elif isinstance(
+                    module, (nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d)
+                ):
                     batchnorm_layer = BatchNormLayer(node, module)
                     self.node_post_process(batchnorm_layer)
                 elif isinstance(module, nn.ReLU):
                     relu_layer = ReluLayer(node, module)
                     self.node_post_process(relu_layer)
-                elif isinstance(module, (nn.MaxPool1d, nn.MaxPool2d)):
+                elif isinstance(module, (nn.MaxPool1d, nn.MaxPool2d, nn.MaxPool3d)):
                     pooling_layer = PoolingLayer(node, module)
                     self.node_post_process(pooling_layer)
-                elif isinstance(module, (nn.AdaptiveAvgPool1d, nn.AdaptiveAvgPool2d)):
+                elif isinstance(
+                    module,
+                    (nn.AdaptiveAvgPool1d, nn.AdaptiveAvgPool2d, nn.AdaptiveAvgPool3d),
+                ):
                     pooling_layer = PoolingLayer(node, module)
                     self.node_post_process(pooling_layer)
                 elif isinstance(module, nn.Linear):
                     linear_layer = LinearLayer(node, module)
                     self.node_post_process(linear_layer)
                 elif isinstance(module, nn.Dropout):
                     dropout_layer = DropoutLayer(node, module)
@@ -154,17 +170,14 @@
                     self.node_post_process(sigmoid_layer)
                 elif isinstance(module, nn.Softmax):
                     softmax_layer = SoftmaxLayer(node, module)
                     self.node_post_process(softmax_layer)
                 elif isinstance(module, nn.Softplus):
                     layer = SoftplusLayer(node, module)
                     self.node_post_process(layer)
-                elif isinstance(module, nn.LayerNorm):
-                    layer = LayerNormLayer(node, module)
-                    self.node_post_process(layer)
                 elif isinstance(module, nn.Embedding):
                     layer = EmbeddingLayer(node, module)
                     self.node_post_process(layer)
                 elif isinstance(module, nn.Tanh):
                     layer = TanhLayer(node, module)
                     self.node_post_process(layer)
                 elif isinstance(module, nn.SiLU):
@@ -316,35 +329,41 @@
                     self.node_post_process(matmul_layer)
                 elif function_name == "softplus":
                     softplus_layer = SoftplusFunc(node)
                     self.node_post_process(softplus_layer)
                 elif function_name == "interpolate":
                     upsample_layer = UpsampleFunc(node)
                     self.node_post_process(upsample_layer)
-                elif function_name == "_pad":
+                elif function_name == "_pad" or function_name == "pad":
                     pad_layer = PadFunc(node)
                     self.node_post_process(pad_layer)
                 elif function_name == "tile":
                     tile_layer = TileFunc(node)
                     self.node_post_process(tile_layer)
                 elif function_name == "normalize":
                     normalize_layer = NormalizeFunc(node)
                     self.node_post_process(normalize_layer)
                 elif function_name == "clamp":
-                    clip_layer = ClipFunc(node, auto_gen=False)
+                    clip_layer = ClipFunc(node)
                     self.node_post_process(clip_layer)
                 elif function_name == "reshape":
                     reshape_layer = ReshapeFunc(node)
                     self.node_post_process(reshape_layer)
                 elif function_name == "dropout":
                     reshape_layer = DropoutLayer(node)
                     self.node_post_process(reshape_layer)
                 elif function_name == "stack":
                     stack_layer = StackFunc(node)
                     self.node_post_process(stack_layer)
+                elif function_name == "glu":
+                    glu_layer = GLUFunc(node)
+                    self.node_post_process(glu_layer)
+                elif function_name == "baddbmm":
+                    baddbmm_layer = BADDBMMFunc(node)
+                    self.node_post_process(baddbmm_layer)
                 else:
                     raise NotImplementedError(
                         "function %s is not implemented" % (function_name)
                     )
             elif node.op == "call_method":
                 if str(node.target) == "size":
                     pass
@@ -403,14 +422,20 @@
                     self.node_post_process(split_layer)
                 elif str(node.target) == "flatten":
                     flatten_layer = FlattenFunc(node)
                     self.node_post_process(flatten_layer)
                 elif str(node.target) == "unbind":
                     unbind_layer = UnbindFunc(node)
                     self.node_post_process(unbind_layer)
+                elif str(node.target) == "exp":
+                    exp_layer = ExpFunc(node)
+                    self.node_post_process(exp_layer)
+                elif str(node.target) == "__getitem__":
+                    getitem_layer = GetItemFunc(node)
+                    self.node_post_process(getitem_layer)
                 else:
                     raise NotImplementedError(
                         "method %s is not implemented" % (str(node.target))
                     )
             elif node.op == "output":
                 output_layer = OutputLayer(node)
                 self.node_post_process(output_layer)
@@ -445,18 +470,17 @@
             graph_def, producer_name="pytorch", opset_imports=opset_imports
         )
         self.freeze()
         self.model_def = optimize_model(self.model_def)
         checker.check_model(self.model_def)
         logger.info("onnx model conversion completed")
         save(self.model_def, dest_path)
-        logger.info("onnx model saved to {}".format(dest_path))
+        logger.info(f"onnx model saved to {dest_path}")
 
     def check_result(self):
-        self.pyotrch_inference()
         self.onnx_inference()
         pytorch_output_list = map_reduce(self.pytorch_output, gen_numpy_data)
         assert len(pytorch_output_list) == len(
             self.onnx_output
         ), "pytorch_output: %d vs onnx_output %d" % (
             len(pytorch_output_list),
             len(self.onnx_output),
@@ -500,15 +524,15 @@
         sess_options.register_custom_ops_library(get_library_path())
         sess = rt.InferenceSession(self.dest_path, sess_options)
         onnx_rt_dict = self.get_onnx_input(sess, self.inputs)
         onnx_outname = [output.name for output in sess.get_outputs()]
         start = time.time()
         self.onnx_output = sess.run(onnx_outname, onnx_rt_dict)
         end = time.time()
-        logger.info("onnx ran in {:0.4f}s".format(end - start))
+        logger.info(f"onnx ran in {(end - start):0.4f}s")
         if isinstance(self.onnx_output, np.ndarray):
             self.onnx_output = [self.onnx_output]
 
     def export_onnx(self, name, opset_version=13, optimize=False):
         torch.onnx.export(
             self.model, tuple(self.inputs), name, opset_version=opset_version
         )
@@ -539,14 +563,14 @@
 
     def freeze(self):
         logger.info("removing not constant initializers from model")
         inputs = self.model_def.graph.input
         name_to_input = {}
         for input in inputs:
             if input.name in name_to_input.keys():
-                logger.warning("Duplicate input name: {}".format(input.name))
+                logger.warning(f"Duplicate input name: {input.name}")
             name_to_input[input.name] = input
 
         for initializer in self.model_def.graph.initializer:
             if initializer.name in name_to_input:
                 inputs.remove(name_to_input[initializer.name])
                 name_to_input.pop(initializer.name)
```

### Comparing `brocolli-3.0.0/brocolli/quantization/fuser.py` & `brocolli-4.0.1/brocolli/quantization/fuser.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         self.conv = quantizer.modules[self.conv_node.target]
 
     def fuse(self, fused_graph, modules):
         op_list = []
         assert self.bn_node is not None
         op_list.append(self.conv)
         op_list.append(self.bn)
-
         fused_conv = fuse_conv_bn_eval(self.conv, self.bn)
         replace_node_module(self.conv_node, modules, fused_conv)
 
         if self.bn_node is not None:
             replace_node_module(self.bn_node, modules, torch.nn.Identity())
 
         self.bn_node.replace_all_uses_with(self.conv_node)
```

### Comparing `brocolli-3.0.0/brocolli/quantization/graph_modules.py` & `brocolli-4.0.1/brocolli/quantization/graph_modules.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import torch
 import copy
 from torch.fx import GraphModule
 
 
 class BrocolliGraphModule(GraphModule):
     def __init__(self, root, graph, class_name="GraphModule"):
-        super().__init__(root, graph, class_name)
+        graph_copy = copy.deepcopy(graph)
+        super().__init__(root, graph_copy, class_name)
         self.class_name = class_name
 
     def __deepcopy__(self, memo):
         fake_mod = torch.nn.Module()
         fake_mod.__dict__ = copy.deepcopy(self.__dict__)
-        graph_copy = copy.deepcopy(self.graph)
-        graph_module = BrocolliGraphModule(fake_mod, graph_copy, self.class_name)
-        graph_module.__dict__.update(fake_mod.__dict__)
+        graph_module = BrocolliGraphModule(fake_mod, self.graph, self.class_name)
+        for key, value in fake_mod.__dict__.items():
+            if (
+                key not in graph_module.__dict__.keys()
+            ):  # to handle those user-defined attr
+                graph_module.__dict__[key] = value
 
         return graph_module
```

### Comparing `brocolli-3.0.0/brocolli/quantization/observer.py` & `brocolli-4.0.1/brocolli/quantization/observer.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 ABC: Any = ABCMeta(str("ABC"), (object,), {})
 
 AVIAIABLE_OBSERVERS = []
 
 
 def register_observer(cls):
-
     AVIAIABLE_OBSERVERS.append(cls)
 
     return cls
 
 
 def get_available_observers():
     return AVIAIABLE_OBSERVERS
@@ -122,28 +121,29 @@
             torch.quint4x2,
         ), "Default Observer only works for qint8, quint8 and quint4x2 data type"
         self.has_customized_qrange = (quant_min is not None) and (quant_max is not None)
         if self.has_customized_qrange:
             self._validate_qmin_qmax(quant_min, quant_max)
         self.quant_min = quant_min
         self.quant_max = quant_max
+        self.input_shape = None
 
     @torch.jit.export
     def _validate_qmin_qmax(self, quant_min: int, quant_max: int):
         assert (
             quant_min <= 0 <= quant_max
         ), "Used-specified quantization range must include 0."
         assert (
             quant_min < quant_max
         ), "qmin must be strictly less than qmax for user-specified quantization range."
 
     @torch.jit.export
     def _calculate_qmin_qmax(self):
         if self.dtype == torch.qint8:
-            quant_min, quant_max = -128, 127
+            quant_min, quant_max = -127, 127
         elif self.dtype == torch.quint8:
             quant_min, quant_max = 0, 255
 
         return quant_min, quant_max
 
     @torch.jit.export
     def _calculate_qparams(self, min_val: torch.Tensor, max_val: torch.Tensor):
@@ -238,14 +238,15 @@
         ):
             raise NotImplementedError(
                 "Cannot reduce range for symmetric \
                                        quantization for quint8"
             )
 
     def forward(self, x_orig):
+        self.input_shape = x_orig.shape
         if x_orig.numel() == 0:
             return x_orig
         x = x_orig.detach()  # avoid keeping autograd tape
         x = x.to(self.min_val.dtype)
         min_val_cur, max_val_cur = torch._aminmax(x)
         min_val = torch.min(min_val_cur, self.min_val)
         max_val = torch.max(max_val_cur, self.max_val)
@@ -296,14 +297,15 @@
             and self.dtype == torch.quint8
         ):
             raise NotImplementedError(
                 "Cannot reduce range for symmetric quantization for quint8"
             )
 
     def forward(self, x_orig):
+        self.input_shape = x_orig.shape
         return self._forward(x_orig)
 
     def _forward(self, x_orig):
         if x_orig.numel() == 0:
             return x_orig
         x = x_orig.detach()  # avoid keeping autograd tape
         min_vals = self.min_vals
@@ -334,11 +336,77 @@
     def calculate_qparams(self):
         return self._calculate_qparams(self.min_vals, self.max_vals)
 
     def extra_repr(self):
         return "min_val={}, max_val={}".format(self.min_vals, self.max_vals)
 
 
-default_observer = MinMaxObserver.with_args()
+def grad_scale(x, scale):
+    y = x
+    y_grad = x * scale
+    return (y - y_grad).detach() + y_grad
+
+
+def round_pass(x):
+    y = x.round()
+    y_grad = x
+    return (y - y_grad).detach() + y_grad
+
+
+class LSQObserver(_ObserverBase):
+    def __init__(
+        self, dtype=torch.qint8, all_positive=False, symmetric=False, per_channel=True
+    ):
+        super(LSQObserver, self).__init__(dtype)
+        bit = 8 if (dtype == torch.qint8 or dtype == torch.quint8) else 16
+        if all_positive:
+            assert not symmetric, "Positive quantization cannot be symmetric"
+            # unsigned activation is quantized to [0, 2^b-1]
+            self.thd_neg = 0
+            self.thd_pos = 2**bit - 1
+        else:
+            if symmetric:
+                # signed weight/activation is quantized to [-2^(b-1)+1, 2^(b-1)-1]
+                self.thd_neg = -(2 ** (bit - 1)) + 1
+                self.thd_pos = 2 ** (bit - 1) - 1
+            else:
+                # signed weight/activation is quantized to [-2^(b-1), 2^(b-1)-1]
+                self.thd_neg = -(2 ** (bit - 1))
+                self.thd_pos = 2 ** (bit - 1) - 1
+
+        self.per_channel = per_channel
+        self.s = torch.nn.Parameter(torch.ones(1))
+
+    def init_from(self, x, *args, **kwargs):
+        if self.per_channel:
+            self.s = torch.nn.Parameter(
+                x.detach().abs().mean(dim=list(range(1, x.dim())), keepdim=True)
+                * 2
+                / (self.thd_pos**0.5)
+            )
+        else:
+            self.s = torch.nn.Parameter(
+                x.detach().abs().mean() * 2 / (self.thd_pos**0.5)
+            )
+
+    def forward(self, x):
+        print(self.s)
+        if self.per_channel:
+            s_grad_scale = 1.0 / ((self.thd_pos * x.numel()) ** 0.5)
+        else:
+            s_grad_scale = 1.0 / ((self.thd_pos * x.numel()) ** 0.5)
+        s_scale = grad_scale(self.s, s_grad_scale)
+
+        x = x / s_scale
+        x = torch.clamp(x, self.thd_neg, self.thd_pos)
+        x = round_pass(x)
+        x = x * s_scale
+        return x
+
+    def calculate_qparams(self):
+        return self.s
+
+
+default_observer = MinMaxObserver.with_args(qscheme=torch.per_tensor_symmetric)
 default_weight_observer = PerChannelMinMaxObserver.with_args(
     dtype=torch.qint8, qscheme=torch.per_channel_symmetric
 )
```

### Comparing `brocolli-3.0.0/brocolli/quantization/profiler.py` & `brocolli-4.0.1/brocolli/quantization/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import time
 import numpy as np
-import pandas as pd
 from tabulate import tabulate
 from loguru import logger
 
 from torch.fx.interpreter import Interpreter
 
 
 class ProfileStats(object):
```

### Comparing `brocolli-3.0.0/brocolli/quantization/qconfig.py` & `brocolli-4.0.1/brocolli/quantization/qconfig.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 import torch
 import torch.nn as nn
 from collections import namedtuple
 
-from .observer import MinMaxObserver, PerChannelMinMaxObserver
+from .observer import MinMaxObserver, PerChannelMinMaxObserver, LSQObserver
 
 
-class QConfig(namedtuple("QConfig", ["activation", "weight", "output"])):
-    def __new__(cls, activation, weight, output):
+class QConfig(namedtuple("QConfig", ["activation", "weight"])):
+    def __new__(cls, activation, weight):
         if isinstance(activation, nn.Module) or isinstance(weight, nn.Module):
             raise ValueError(
                 "QConfig received observer instance, please pass observer class instead. "
                 + "Use MyObserver.with_args(x=1) to override arguments to constructor if needed"
             )
-        return super(QConfig, cls).__new__(cls, activation, weight, output)
+        return super(QConfig, cls).__new__(cls, activation, weight)
 
 
-def get_qconfig(bit, input_dtype=torch.qint8, output_dtype=torch.qint8):
-    if bit == 8:
+def get_qconfig(bit, input_dtype=torch.qint8, lsq=False):
+    if lsq:
         return QConfig(
-            activation=MinMaxObserver.with_args(dtype=input_dtype),
+            activation=LSQObserver.with_args(
+                dtype=input_dtype, all_positive=True, symmetric=False, per_channel=False
+            ),
+            weight=LSQObserver.with_args(
+                dtype=input_dtype, all_positive=True, symmetric=False, per_channel=True
+            ),
+        )
+    elif bit == 8:
+        return QConfig(
+            activation=MinMaxObserver.with_args(
+                dtype=input_dtype, qscheme=torch.per_tensor_symmetric
+            ),
             weight=PerChannelMinMaxObserver.with_args(
                 dtype=torch.qint8, qscheme=torch.per_channel_symmetric
             ),
-            output=MinMaxObserver.with_args(dtype=output_dtype),
         )
     elif bit == 16:
         return QConfig(
-            activation=MinMaxObserver.with_args(dtype=input_dtype),
+            activation=MinMaxObserver.with_args(
+                dtype=input_dtype, qscheme=torch.per_tensor_symmetric
+            ),
             weight=PerChannelMinMaxObserver.with_args(
                 dtype=torch.qint8, qscheme=torch.per_channel_symmetric
             ),
-            output=MinMaxObserver.with_args(dtype=output_dtype),
         )
     else:
         raise ValueError("Quantization bit {} is not supported".format(bit))
```

### Comparing `brocolli-3.0.0/brocolli/quantization/quantization_layers/conv.py` & `brocolli-4.0.1/brocolli/quantization/quantization_layers/conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .base import BaseOperator
 from .utils import _pair, _quantize_weight, _quantize_bias
-
+from .registry import register_quant_op
 
 _SUPPORTED_PADDING = {"zeros", "reflect"}
 
 
 class _ConvNd(nn.Module):
     def __init__(
         self,
@@ -150,20 +150,21 @@
             mod.padding,
             mod.dilation,
             mod.groups,
             mod.bias is not None,
             mod.padding_mode,
         )
 
-        qconv.qbit = mod.qbit
+        qconv.qbit = mod.activation_pre_process.qbit
         qconv.weight = torch.nn.Parameter(qweight, requires_grad=False)
-        qconv.bias = torch.nn.Parameter(qbias, requires_grad=False)
-        qconv.act_scale = float(act_scale)
-        qconv.wt_scale = wt_scale.reshape(1, -1, 1, 1)
-        qconv.output_scale = float(output_scale)
+        if mod.bias is not None:
+            qconv.bias = torch.nn.Parameter(qbias, requires_grad=False)
+        qconv.act_scale = torch.Tensor(act_scale).to(qweight.device)
+        qconv.wt_scale = torch.Tensor(wt_scale).reshape(1, -1, 1, 1).to(qweight.device)
+        qconv.output_scale = torch.Tensor(output_scale).to(qweight.device)
         qconv.output_min_value = activation_post_process.min_val
         qconv.output_max_value = activation_post_process.max_val
 
         return qconv
 
     @staticmethod
     def from_float(cls, mod):
@@ -171,23 +172,26 @@
             " brocolli."
             + cls.__name__
             + ".from_float only works for "
             + cls._FLOAT_MODULE.__name__
             + " but got:"
             + str(type(mod))
         )
-        assert hasattr(mod, "qconfig"), "Input float module must have qconfig defined."
+        assert hasattr(
+            mod.activation_pre_process, "qconfig"
+        ), "Conv float module must have qconfig defined."
         activation_pre_process = mod.activation_pre_process
-        weight_post_process = mod.qconfig.weight()
+        weight_post_process = activation_pre_process.qconfig.weight()
         activation_post_process = mod.activation_post_process
         return cls.get_qconv(
             mod, activation_pre_process, weight_post_process, activation_post_process
         )
 
 
+@register_quant_op(torch.nn.Conv2d)
 class Conv2d(_ConvNd, BaseOperator):
     _FLOAT_MODULE = nn.Conv2d
 
     def __init__(
         self,
         in_channels,
         out_channels,
@@ -225,23 +229,22 @@
         return "QuantizedConv2d"
 
     def forward(self, input):
         if len(input.shape) != 4:
             raise ValueError("Input shape must be `(N, C, H, W)`!")
 
         out = F.conv2d(
-            input.to(torch.int64),
-            self.weight.to(torch.int64),
-            self.bias.to(torch.int64),
+            input.to(torch.double),
+            self.weight.to(torch.double),
+            self.bias.to(torch.double) if self.bias is not None else None,
             self.stride,
             self.padding,
             self.dilation,
             self.groups,
         )
-
         out = out * self.act_scale * self.wt_scale / self.output_scale
         out = self.clamp(out)
 
         return out
 
     @classmethod
     def from_float(cls, mod):
```

### Comparing `brocolli-3.0.0/brocolli/quantization/quantization_layers/linear.py` & `brocolli-4.0.1/brocolli/quantization/quantization_layers/linear.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .base import BaseOperator
 from .utils import _quantize_weight, _quantize_bias
+from .registry import register_quant_op
 
 
+@register_quant_op(torch.nn.Linear)
 class Linear(nn.Module, BaseOperator):
     def __init__(self, in_features, out_features, bias=True):
         super(Linear, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
         self.bias = bias
 
@@ -20,41 +22,44 @@
         return s.format(**self.__dict__)
 
     def _get_name(self):
         return "QuantizedLinear"
 
     @classmethod
     def from_float(cls, mod):
-        weight_post_process = mod.qconfig.weight()
+        assert hasattr(
+            mod.activation_pre_process, "qconfig"
+        ), "Conv float module must have qconfig defined."
+        weight_post_process = mod.activation_pre_process.qconfig.weight()
         weight_post_process(mod.weight)
         qweight, wt_scale = _quantize_weight(mod.weight.float(), weight_post_process)
         act_scale = mod.activation_pre_process.calculate_qparams()
         qbias = (
             _quantize_bias(mod.bias.float(), wt_scale * act_scale)
             if mod.bias is not None
             else None
         )
         output_scale = mod.activation_post_process.calculate_qparams()
         qlinear = cls(mod.in_features, mod.out_features, mod.bias)
 
-        qlinear.qbit = mod.qbit
+        qlinear.qbit = mod.activation_pre_process.qbit
         qlinear.weight = torch.nn.Parameter(qweight, requires_grad=False)
         qlinear.bias = torch.nn.Parameter(qbias, requires_grad=False)
-        qlinear.act_scale = float(act_scale)
-        qlinear.wt_scale = wt_scale.reshape(1, -1)
-        qlinear.output_scale = float(output_scale)
+        qlinear.act_scale = torch.Tensor(act_scale).to(qweight.device)
+        qlinear.wt_scale = torch.Tensor(wt_scale).reshape(1, -1).to(qweight.device)
+        qlinear.output_scale = torch.Tensor(output_scale).to(qweight.device)
         qlinear.output_min_value = mod.activation_post_process.min_val
         qlinear.output_max_value = mod.activation_post_process.max_val
 
         return qlinear
 
     def forward(self, input):
         out = F.linear(
-            input.to(torch.int64),
-            self.weight.to(torch.int64),
-            self.bias.to(torch.int64),
+            input.to(torch.double),
+            self.weight.to(torch.double),
+            self.bias.to(torch.double),
         )
 
         out = out * self.act_scale * self.wt_scale / self.output_scale
         out = self.clamp(out)
 
         return out
```

### Comparing `brocolli-3.0.0/brocolli/quantization/quantization_layers/output.py` & `brocolli-4.0.1/brocolli/quantization/quantization_layers/output.py`

 * *Files identical despite different names*

### Comparing `brocolli-3.0.0/brocolli/quantization/quantization_layers/relu.py` & `brocolli-4.0.1/brocolli/quantization/quantization_layers/relu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .base import BaseOperator
 from .utils import _gen_lut
+from .registry import register_quant_op
 
 
 class ReLU(nn.Module, BaseOperator):
     def __init__(self):
         super(ReLU, self).__init__()
 
     def extra_repr(self):
@@ -15,15 +16,17 @@
         return s.format(**self.__dict__)
 
     def _get_name(self):
         return "QuantizedReLU"
 
     @classmethod
     def from_float(cls, mod, lut=False):
-        assert hasattr(mod, "qconfig"), "Relu float module must have qconfig defined."
+        assert hasattr(
+            mod.activation_pre_process, "qconfig"
+        ), "ReLU float module must have qconfig defined."
         activation_pre_process = mod.activation_pre_process
         activation_post_process = mod.activation_post_process
         act_scale = activation_pre_process.calculate_qparams()
         output_scale = activation_post_process.calculate_qparams()
 
         if lut:
             if activation_pre_process.min_val >= 0:
@@ -33,35 +36,35 @@
             else:
                 lut_start = -128
                 zero_point = 128
                 lut_end = 127
             lut_weight = _gen_lut(F.relu, act_scale, output_scale, lut_start, lut_end)
             lut_weight = torch.nn.Parameter(lut_weight, requires_grad=False)
             qrelu = cls()
-            qrelu.qbit = mod.qbit
+            qrelu.qbit = mod.activation_pre_process.qbit
             qrelu.lut_weight = lut_weight
             qrelu.zero_point = zero_point
             qrelu.act_scale = float(act_scale)
             qrelu.output_scale = float(output_scale)
             qrelu.output_min_value = activation_post_process.min_val
             qrelu.output_max_value = activation_post_process.max_val
         else:
             qrelu = cls()
-            qrelu.qbit = mod.qbit
+            qrelu.qbit = mod.activation_pre_process.qbit
             qrelu.act_scale = float(act_scale)
             qrelu.output_scale = float(output_scale)
             qrelu.output_min_value = activation_post_process.min_val
             qrelu.output_max_value = activation_post_process.max_val
 
         return qrelu
 
     def forward(self, input):
         if hasattr(self, "lut_weight"):
             input = input.to(torch.int64) + self.zero_point
             out = F.embedding(input, self.lut_weight).squeeze(-1)
         else:
-            out = F.relu(input.to(torch.int64))
+            out = F.relu(input.to(torch.float64))
             out = out * self.act_scale / self.output_scale
 
         out = self.clamp(out)
 
         return out
```

### Comparing `brocolli-3.0.0/brocolli.egg-info/PKG-INFO` & `brocolli-4.0.1/brocolli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brocolli
-Version: 3.0.0
+Version: 4.0.1
 Summary: everything in pytorch
 Home-page: https://github.com/inisis/brocolli
 Author: desmond
 Author-email: desmond.yao@buaa.edu.cn
 Project-URL: Bug Tracker, https://github.com/inisis/brocolli/issues
 Keywords: machine-learning,pytorch,caffe,torchfx
 Classifier: Programming Language :: Python :: 3
@@ -47,17 +47,20 @@
 * torch2onnx
     ```
     import torchvision.models as models
     from brocolli.converter.pytorch_onnx_parser import PytorchOnnxParser
 
     net = models.alexnet(pretrained=False)
     x = torch.rand(1, 3, 224, 224)
-    pytorch_parser = PytorchCaffeParser(net, x)
+    pytorch_parser = PytorchOnnxParser(net, x)
     pytorch_parser.convert()
     pytorch_parser.save('alexnet.onnx')
     ```
     run this script until you see "accuracy test passed" on screen, then you can get alexnet.onnx under current folder.
 
 # Contact
  QQ Group: 597059928
  
  ![image](https://raw.githubusercontent.com/inisis/brocolli/master/imgs/QGRPOUP.png)
+ 
+# Show your support
+  Give a 🌟 if this project helpes~
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `brocolli-3.0.0/brocolli.egg-info/SOURCES.txt` & `brocolli-4.0.1/brocolli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 brocolli/__init__.py
 brocolli.egg-info/PKG-INFO
 brocolli.egg-info/SOURCES.txt
 brocolli.egg-info/dependency_links.txt
 brocolli.egg-info/requires.txt
 brocolli.egg-info/top_level.txt
 brocolli/converter/__init__.py
+brocolli/converter/common_utils.py
+brocolli/converter/onnx_utils.py
 brocolli/converter/optimizer.py
 brocolli/converter/pytorch_caffe_parser.py
 brocolli/converter/pytorch_graph.py
 brocolli/converter/pytorch_onnx_parser.py
-brocolli/converter/utils.py
 brocolli/converter/onnx_layers/__init__.py
 brocolli/converter/onnx_layers/abs_func.py
 brocolli/converter/onnx_layers/add_layer.py
 brocolli/converter/onnx_layers/avgpool_func.py
 brocolli/converter/onnx_layers/avgpool_layer.py
+brocolli/converter/onnx_layers/baddbmm_func.py
 brocolli/converter/onnx_layers/base_layer.py
 brocolli/converter/onnx_layers/batchnorm_layer.py
 brocolli/converter/onnx_layers/bnll_layer.py
 brocolli/converter/onnx_layers/cast_layer.py
 brocolli/converter/onnx_layers/celu_func.py
 brocolli/converter/onnx_layers/chunk_func.py
 brocolli/converter/onnx_layers/clip_func.py
@@ -42,14 +44,15 @@
 brocolli/converter/onnx_layers/flatten_func.py
 brocolli/converter/onnx_layers/flatten_layer.py
 brocolli/converter/onnx_layers/gelu_layer.py
 brocolli/converter/onnx_layers/gemm_func.py
 brocolli/converter/onnx_layers/gemm_layer.py
 brocolli/converter/onnx_layers/getattr_func.py
 brocolli/converter/onnx_layers/getitem_func.py
+brocolli/converter/onnx_layers/glu_func.py
 brocolli/converter/onnx_layers/gru_layer.py
 brocolli/converter/onnx_layers/hardsigmoid_func.py
 brocolli/converter/onnx_layers/hardsigmoid_layer.py
 brocolli/converter/onnx_layers/hardswish_func.py
 brocolli/converter/onnx_layers/hardswish_layer.py
 brocolli/converter/onnx_layers/identity_layer.py
 brocolli/converter/onnx_layers/input_layer.py
@@ -106,25 +109,34 @@
 brocolli/converter/onnx_layers/template.py
 brocolli/converter/onnx_layers/tile_func.py
 brocolli/converter/onnx_layers/transpose_func.py
 brocolli/converter/onnx_layers/unbind_func.py
 brocolli/converter/onnx_layers/unsqueeze_func.py
 brocolli/converter/onnx_layers/upsample_func.py
 brocolli/converter/onnx_layers/upsample_layer.py
+brocolli/converter/pytorch_layer/__init__.py
+brocolli/converter/pytorch_layer/glu.py
+brocolli/converter/pytorch_layer/layernorm.py
+brocolli/converter/pytorch_layer/mha.py
+brocolli/converter/pytorch_layer/transformer.py
+brocolli/converter/pytorch_layer/utils.py
 brocolli/quantization/__init__.py
+brocolli/quantization/comparator.py
 brocolli/quantization/fuser.py
 brocolli/quantization/graph_modules.py
 brocolli/quantization/observer.py
 brocolli/quantization/pattern.py
 brocolli/quantization/profiler.py
 brocolli/quantization/qconfig.py
 brocolli/quantization/quantizer.py
 brocolli/quantization/utils.py
 brocolli/quantization/quantization_layers/__init__.py
+brocolli/quantization/quantization_layers/arithmetic.py
 brocolli/quantization/quantization_layers/base.py
 brocolli/quantization/quantization_layers/conv.py
 brocolli/quantization/quantization_layers/input.py
 brocolli/quantization/quantization_layers/linear.py
 brocolli/quantization/quantization_layers/output.py
 brocolli/quantization/quantization_layers/pooling.py
+brocolli/quantization/quantization_layers/registry.py
 brocolli/quantization/quantization_layers/relu.py
 brocolli/quantization/quantization_layers/utils.py
```

### Comparing `brocolli-3.0.0/setup.py` & `brocolli-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="brocolli",
-    version="3.0.0",
+    version="4.0.1",
     author="desmond",
     author_email="desmond.yao@buaa.edu.cn",
     description="everything in pytorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/inisis/brocolli",
     install_requires=["loguru", "onnx==1.9.0", "onnxruntime==1.8.0", "tabulate"],
```

