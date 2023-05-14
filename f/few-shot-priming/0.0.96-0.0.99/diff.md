# Comparing `tmp/few_shot_priming-0.0.96-py3-none-any.whl.zip` & `tmp/few_shot_priming-0.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 336417 bytes, number of entries: 13
+Zip file size: 336423 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-08 08:47 few_shot_priming/__init__.py
 -rw-rw-r--  2.0 unx     5889 b- defN 23-Mar-16 09:19 few_shot_priming/baseline.py
 -rw-rw-r--  2.0 unx      624 b- defN 23-Mar-17 09:19 few_shot_priming/conf.yaml
--rw-rw-r--  2.0 unx    12598 b- defN 23-Mar-17 09:16 few_shot_priming/few_shot_stance.py
+-rw-rw-r--  2.0 unx    12600 b- defN 23-Mar-17 09:43 few_shot_priming/few_shot_stance.py
 -rw-rw-r--  2.0 unx      444 b- defN 23-Mar-15 15:25 few_shot_priming/ibm_baseline.py
 -rw-rw-r--  2.0 unx  1017422 b- defN 23-Feb-23 10:49 few_shot_priming/data/claim_stance_dataset_v1.csv
 -rw-rw-r--  2.0 unx   518571 b- defN 23-Mar-10 14:56 few_shot_priming/experiment/test.csv
 -rw-rw-r--  2.0 unx   240003 b- defN 23-Mar-10 14:56 few_shot_priming/experiment/train.csv
 -rw-rw-r--  2.0 unx   178874 b- defN 23-Mar-10 14:56 few_shot_priming/experiment/validation.csv
--rw-rw-r--  2.0 unx     6860 b- defN 23-Mar-17 09:19 few_shot_priming-0.0.96.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-17 09:19 few_shot_priming-0.0.96.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Mar-17 09:19 few_shot_priming-0.0.96.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1169 b- defN 23-Mar-17 09:19 few_shot_priming-0.0.96.dist-info/RECORD
-13 files, 1982563 bytes uncompressed, 334445 bytes compressed:  83.1%
+-rw-rw-r--  2.0 unx     6860 b- defN 23-Mar-17 09:50 few_shot_priming-0.0.99.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Mar-17 09:50 few_shot_priming-0.0.99.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Mar-17 09:50 few_shot_priming-0.0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1169 b- defN 23-Mar-17 09:50 few_shot_priming-0.0.99.dist-info/RECORD
+13 files, 1982565 bytes uncompressed, 334451 bytes compressed:  83.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: few_shot_priming/experiment/train.csv
 Comment: 
 
 Filename: few_shot_priming/experiment/validation.csv
 Comment: 
 
-Filename: few_shot_priming-0.0.96.dist-info/METADATA
+Filename: few_shot_priming-0.0.99.dist-info/METADATA
 Comment: 
 
-Filename: few_shot_priming-0.0.96.dist-info/WHEEL
+Filename: few_shot_priming-0.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: few_shot_priming-0.0.96.dist-info/top_level.txt
+Filename: few_shot_priming-0.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: few_shot_priming-0.0.96.dist-info/RECORD
+Filename: few_shot_priming-0.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## few_shot_priming/few_shot_stance.py

```diff
@@ -284,17 +284,17 @@
             all_test_labels.extend(test_labels.cpu().tolist())
             all_test_preds.extend(torch.argmax(test_logits, dim = -1).cpu().tolist())
             loss = loss_func(test_logits, test_labels)
             test_loss += loss.item()
             metrics[f"{experiment_type}/loss"] = test_loss/(step+1)
             wandb.log(metrics)
         metrics[f"{experiment_type}/accuracy"] = accuracy_score(all_test_labels, all_test_preds)
-        metrics["score"] = accuracy_score(all_test_labels, all_test_preds)
         wandb.log(metrics)
-
+    metrics["score"] = [f"{experiment_type}/accuracy"]
+    wandb.log(metrics)
 if __name__ == "__main__":
     args = parse_args()
     if args.offline:
         offline = True
     else:
         offline = False
```

## Comparing `few_shot_priming-0.0.96.dist-info/METADATA` & `few_shot_priming-0.0.99.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-priming
-Version: 0.0.96
+Version: 0.0.99
 Summary: Analyzing priming effects in a few shot setting environment
 Home-page: https://gitlab.uni-hannover.de/y.ajjour/few-shot-priming
 Author: Yamen Ajjour
 Author-email: yajjour@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `few_shot_priming-0.0.96.dist-info/RECORD` & `few_shot_priming-0.0.99.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 few_shot_priming/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 few_shot_priming/baseline.py,sha256=PmEtr5ZGcWfgVmuu9x8bPX8YYWi1txt_Z0_c9gTS4-s,5889
 few_shot_priming/conf.yaml,sha256=pNdMPbYBBtLUdqsCDS0i-FhG9A6TTCp2_laHFBFRe_I,624
-few_shot_priming/few_shot_stance.py,sha256=SKvkmjfU2C4hG18ReUvHld4W7FuukIES9lfGkTgGQe8,12598
+few_shot_priming/few_shot_stance.py,sha256=XMx3BMvgDKjBj9z7lGEpIbIx1facu3vA13Xt3jqDi68,12600
 few_shot_priming/ibm_baseline.py,sha256=h23bLZC2l9CWzF8C77TEqjvBzthLTncXkY5DF6QUd94,444
 few_shot_priming/data/claim_stance_dataset_v1.csv,sha256=8bIwWvKIPnQGNzTqrhHvidKpN478vOF1ZBQzLuxjrcg,1017422
 few_shot_priming/experiment/test.csv,sha256=w7FbPgLdLbWlenjHftFUsNQ2KenxL3inkWoTEtyKQks,518571
 few_shot_priming/experiment/train.csv,sha256=5DFZjmGZY1dlAcfF2Lnz1U8T8gaL67VVorXhnrE7Xpk,240003
 few_shot_priming/experiment/validation.csv,sha256=B2Myom84yS40faRcMGyytPV2j-Af3YMa1IPtzjizLko,178874
-few_shot_priming-0.0.96.dist-info/METADATA,sha256=bV09TWzx5USkxQJQFnqot5EJjsF72264VCrVjWNR3Zw,6860
-few_shot_priming-0.0.96.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-few_shot_priming-0.0.96.dist-info/top_level.txt,sha256=incVNauAhdZ1aJWVERG4ifiKeG4bmLKy6tdy4Li4rdY,17
-few_shot_priming-0.0.96.dist-info/RECORD,,
+few_shot_priming-0.0.99.dist-info/METADATA,sha256=9wOEDiooS-yYOdz8geAq7mW2jAvcuXcO6xmv7IPc4-U,6860
+few_shot_priming-0.0.99.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+few_shot_priming-0.0.99.dist-info/top_level.txt,sha256=incVNauAhdZ1aJWVERG4ifiKeG4bmLKy6tdy4Li4rdY,17
+few_shot_priming-0.0.99.dist-info/RECORD,,
```

