# Comparing `tmp/mini-lightning-0.2.0.tar.gz` & `tmp/mini-lightning-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini-lightning-0.2.0.tar", last modified: Mon Apr  3 10:07:28 2023, max compression
+gzip compressed data, was "mini-lightning-0.2.1.tar", last modified: Sun May 14 15:34:58 2023, max compression
```

## Comparing `mini-lightning-0.2.0.tar` & `mini-lightning-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1063 2022-09-17 07:21:40.000000 mini-lightning-0.2.0/LICENSE
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       24 2022-09-07 13:36:40.000000 mini-lightning-0.2.0/MANIFEST.in
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/PKG-INFO
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     3841 2023-03-26 15:35:20.000000 mini-lightning-0.2.0/README.md
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/mini_lightning/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      106 2023-02-24 13:16:36.000000 mini-lightning-0.2.0/mini_lightning/__init__.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)    44134 2023-04-02 05:43:57.000000 mini-lightning-0.2.0/mini_lightning/_mini_lightning.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1365 2023-03-24 17:17:30.000000 mini-lightning-0.2.0/mini_lightning/_types.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)    11791 2023-03-24 17:20:17.000000 mini-lightning-0.2.0/mini_lightning/_utils.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1210 2023-03-19 07:36:09.000000 mini-lightning-0.2.0/mini_lightning/_visualize.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     3326 2023-04-02 05:49:42.000000 mini-lightning-0.2.0/mini_lightning/_warmup_lrs.py
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/mini_lightning.egg-info/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-04-03 10:07:28.000000 mini-lightning-0.2.0/mini_lightning.egg-info/PKG-INFO
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      505 2023-04-03 10:07:28.000000 mini-lightning-0.2.0/mini_lightning.egg-info/SOURCES.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)        1 2023-04-03 10:07:28.000000 mini-lightning-0.2.0/mini_lightning.egg-info/dependency_links.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       88 2023-04-03 10:07:28.000000 mini-lightning-0.2.0/mini_lightning.egg-info/requires.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       15 2023-04-03 10:07:28.000000 mini-lightning-0.2.0/mini_lightning.egg-info/top_level.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       87 2023-03-26 13:29:02.000000 mini-lightning-0.2.0/requirements.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       38 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/setup.cfg
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1259 2023-03-26 17:13:44.000000 mini-lightning-0.2.0/setup.py
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-04-03 10:07:28.806496 mini-lightning-0.2.0/tests/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     2181 2023-03-16 17:26:26.000000 mini-lightning-0.2.0/tests/test_lrs.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      184 2023-03-09 12:27:51.000000 mini-lightning-0.2.0/tests/test_mini_lightning.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     2219 2023-03-09 12:28:08.000000 mini-lightning-0.2.0/tests/test_utils.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      977 2023-03-09 12:28:17.000000 mini-lightning-0.2.0/tests/test_visualize.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1063 2022-09-17 07:21:40.000000 mini-lightning-0.2.1/LICENSE
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       24 2022-09-07 13:36:40.000000 mini-lightning-0.2.1/MANIFEST.in
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/PKG-INFO
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     3841 2023-03-26 15:35:20.000000 mini-lightning-0.2.1/README.md
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/mini_lightning/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      106 2023-02-24 13:16:36.000000 mini-lightning-0.2.1/mini_lightning/__init__.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)    46084 2023-05-14 15:32:31.000000 mini-lightning-0.2.1/mini_lightning/_mini_lightning.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1401 2023-05-04 16:37:55.000000 mini-lightning-0.2.1/mini_lightning/_types.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)    11778 2023-05-10 13:09:19.000000 mini-lightning-0.2.1/mini_lightning/_utils.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1210 2023-03-19 07:36:09.000000 mini-lightning-0.2.1/mini_lightning/_visualize.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     3326 2023-04-02 05:49:42.000000 mini-lightning-0.2.1/mini_lightning/_warmup_lrs.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/mini_lightning.egg-info/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/PKG-INFO
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      505 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/SOURCES.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)        1 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/dependency_links.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      100 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/requires.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       15 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/top_level.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       99 2023-05-09 15:54:03.000000 mini-lightning-0.2.1/requirements.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       38 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/setup.cfg
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1259 2023-05-04 16:40:28.000000 mini-lightning-0.2.1/setup.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/tests/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     2181 2023-03-16 17:26:26.000000 mini-lightning-0.2.1/tests/test_lrs.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      184 2023-03-09 12:27:51.000000 mini-lightning-0.2.1/tests/test_mini_lightning.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     2219 2023-03-09 12:28:08.000000 mini-lightning-0.2.1/tests/test_utils.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      977 2023-03-09 12:28:17.000000 mini-lightning-0.2.1/tests/test_visualize.py
```

### Comparing `mini-lightning-0.2.0/LICENSE` & `mini-lightning-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/PKG-INFO` & `mini-lightning-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-lightning
-Version: 0.2.0
+Version: 0.2.1
 Summary: Mini-Lightning is a lightweight machine learning training library, which is a mini version of Pytorch-Lightning with only 1k lines of code. It has the advantages of faster, more concise and more flexible.
 Home-page: https://github.com/ustcml/mini-lightning/
 Author: Jintao Huang
 Author-email: huangjintao@mail.ustc.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mini-lightning-0.2.0/README.md` & `mini-lightning-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/mini_lightning/_mini_lightning.py` & `mini-lightning-0.2.1/mini_lightning/_mini_lightning.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # Email: huangjintao@mail.ustc.edu.cn
 # Date:
 
 from ._types import *
 from ._utils import (
     en_parallel, de_parallel, get_dist_setting, select_device,
     logger, write_to_yaml, write_to_csv, read_from_yaml,
-    print_model_info, load_ckpt, save_ckpt, ModelCheckpoint
+    print_model_info, load_ckpt, save_ckpt, ModelCheckpoint, ResumeFromCkpt
 )
 
 
-# Note: global_epoch, batch_idx starts for 0. global_step starts from 1.
+# Note: global_epoch, batch_idx start from 0. 
+#   global_step starts from 1.
 __all__ = ["LModule", "LDataModule", "Trainer"]
 #
 
 
 class LModule:
     def __init__(
         self,
@@ -43,14 +44,19 @@
     @property
     def global_epoch(self) -> int:
         # global_epoch starts from 0
         assert self.trainer is not None
         return self.trainer.global_epoch
 
     @property
+    def global_optimizer_step(self) -> int:
+        assert self.trainer is not None
+        return self.trainer.global_optimizer_step
+
+    @property
     def device(self) -> Optional[Device]:
         assert self.trainer is not None
         return self.trainer.device
 
     #
     def log(self, k: str, v: Union[Tensor, float], *, prog_bar_mean=True) -> None:
         """
@@ -76,14 +82,18 @@
         device = trainer.device
         #
         for s in self._models:
             model: Module = getattr(self, s)
             model.to(device)
             model = en_parallel(model, trainer.parallel_mode, trainer.sync_bn)
             setattr(self, s, model)
+        # 
+        for o in self.optimizers:
+            o.load_state_dict(o.state_dict())  # to device
+        # 
         for metric in self.metrics.values():
             metric.to(device)
 
     @classmethod
     def batch_to_device(cls, batch: Any, device: Device) -> Any:
         if callable(getattr(batch, "to", None)):
             # Ref: https://github.com/Lightning-AI/lightning/blob/master/src/lightning_lite/utilities/apply_func.py
@@ -97,14 +107,16 @@
             res = {}
             for k, v in batch.items():
                 res[k] = cls.batch_to_device(v, device)
         elif isinstance(batch, Sequence) and not isinstance(batch, str):
             res = []
             for b in batch:
                 res.append(cls.batch_to_device(b, device))
+        elif isinstance(batch, (int, float)):
+            res = batch
         else:
             raise TypeError(f"batch: {batch}, {type(batch)}")
         return res
 
     def optimizer_step(self, opt_idx: int) -> None:
         # note: skipping the update behavior at the first step may result in a warning in lr_scheduler.
         #   Don't worry about that ~.
@@ -311,15 +323,15 @@
         runs_dir: str,
         model_checkpoint: Optional[ModelCheckpoint] = None,
         n_accumulate_grad: Union[int, Dict[int, int]] = 1,
         amp: bool = False,
         gradient_clip_norm: Optional[float] = None,
         sync_bn: bool = False,
         replace_sampler_ddp: bool = True,
-        resume_from_ckpt: Optional[str] = None,
+        resume_from_ckpt: Union[str, ResumeFromCkpt, None] = None,
         #
         tb_every_n_steps: int = 10,
         prog_bar_n_steps: int = 1,
         deterministic:  Optional[bool] = None,
         benchmark: Optional[bool] = None,
         verbose: bool = True,
     ) -> None:
@@ -433,14 +445,15 @@
         self.benchmark = benchmark
         #
         self.scaler = GradScaler(enabled=amp)
         self.best_metric: Optional[float] = None
         self.best_ckpt_path: Optional[str] = None
         self.last_ckpt_path: Optional[str] = None
         self.global_step = 0
+        self.global_optimizer_step = 0
         self.global_epoch = -1
         # for log
         self._new_mes: Dict[str, float] = {}
         self._prog_bar_mean: Dict[str, bool] = {}
         # check inf nan
         self._found_inf = False
         self._found_nan = False
@@ -476,16 +489,25 @@
             #
             self.tb_logger = SummaryWriter(self.tb_dir)
             hparams = lmodel.hparams
             self.save_hparams(hparams)
         #
         self.resume_from_ckpt = resume_from_ckpt
         if resume_from_ckpt is not None:
-            self._load_ckpt(resume_from_ckpt)
-            logger.info(f"Using ckpt: {resume_from_ckpt}")
+            rfc = resume_from_ckpt
+            if isinstance(rfc, str):
+                self._load_ckpt(rfc, False, False, False)
+                logger.info(f"Using ckpt: {rfc}")
+            elif isinstance(rfc, ResumeFromCkpt):
+                if rfc.ckpt_path is not None:
+                    self._load_ckpt(rfc.ckpt_path, rfc.load_optimizers, rfc.load_message, False)
+                    logger.info(f"Using ckpt: {rfc.ckpt_path}, resume_from_ckpt: {rfc}")
+            else:
+                raise ValueError(f"resume_from_ckpt: {rfc}")
+            
         lmodel.trainer_init(self)
         for s in lmodel._models:
             model: Module = getattr(lmodel, s)
             print_model_info(s, model, None)
 
     @staticmethod
     def _get_version(runs_dir: str) -> int:
@@ -561,16 +583,18 @@
         elif mode == "last" and self.last_ckpt_path is not None:
             os.remove(self.last_ckpt_path)
 
     def _result_saving(self, mes: Dict[str, float]) -> None:
         if self.rank not in {-1, 0}:
             return
         mc = self.model_checkpoint
-        val_mode_val = self.global_epoch  # validation_mode_value
-        if mc.val_mode == "step":
+        
+        if mc.val_mode == "epoch":
+            val_mode_val = self.global_epoch  # validation_mode_value
+        else:
             val_mode_val = self.global_step
         #
         mode = mes["mode"]
         write_to_yaml({f"{mode}[{mc.val_mode}={val_mode_val}]": mes}, self.result_yaml_path, mode="a")
         if mc.write_result_csv:
             self.write_csv_from_yaml()
 
@@ -596,15 +620,15 @@
             r = []
             for k in keys:
                 r.append(d[k] if k in d else "")
             res.append(r)
         write_to_csv(res, self.result_csv_path, mode="w")
 
     @staticmethod
-    def _better_equal(metric: float, old_metric: Optional[float], higher_is_better: bool) -> bool:
+    def _is_better_than(metric: float, old_metric: Optional[float], higher_is_better: bool) -> bool:
         if old_metric is None:
             return True
         if higher_is_better:
             return metric >= old_metric
         else:
             return metric <= old_metric
 
@@ -612,48 +636,59 @@
         if self.rank not in {-1, 0}:
             return
         lmodel = self.lmodel
         mc = self.model_checkpoint
         kwargs: Dict[str, Any] = {
             "global_step": self.global_step,
             "global_epoch": self.global_epoch,
+            "global_optimizer_step": self.global_optimizer_step,
             "core_metric": {
                 "name": mc.core_metric_name,
                 "higher_is_better": mc.higher_is_better,
                 "best_value": self.best_metric
             }
         }
         model_list = {s: de_parallel(getattr(lmodel, s)) for s in lmodel._models}
         optimizers = lmodel.optimizers if mc.saving_optimizers else []
         save_ckpt(fpath, model_list, optimizers, **kwargs)
 
-    def _load_ckpt(self, fpath: str) -> None:
+    def _load_ckpt(self, fpath: str, load_optimizers: bool = False, load_mes: bool = False, strict: bool = True) -> None:
         map_location = self.device
-        models_state_dict, _,  _ = load_ckpt(fpath, map_location)
+        models_state_dict, optimizers_state_dict,  mes = load_ckpt(fpath, map_location)
         lmodel = self.lmodel
+        if load_optimizers:
+            for optimizer, o_sd in zip(self.lmodel.optimizers,optimizers_state_dict):
+                optimizer.load_state_dict(o_sd)
+        if load_mes:
+            self.global_step = mes["global_step"]
+            self.global_epoch = mes["global_epoch"]
+            self.global_optimizer_step = mes.get("global_optimizer_step", 0)
         #
         for k, state_dict in models_state_dict.items():
             model: Module = getattr(lmodel, k)
-            model.load_state_dict(state_dict)
+            load_sd_mes = model.load_state_dict(state_dict, strict=strict)
+            if strict is False:
+                logger.info(load_sd_mes)
 
     def _model_saving(self, core_metric: Optional[float]) -> None:
         if self.rank not in {-1, 0}:
             return
         #
         metric_str = ""
         mc = self.model_checkpoint
-        val_mode_val = self.global_epoch
-        if mc.val_mode == "step":
+        if mc.val_mode == "epoch":
+            val_mode_val = self.global_epoch
+        else:
             val_mode_val = self.global_step
         #
         if core_metric is not None:
             assert mc.higher_is_better is not None
             tag = "+" if mc.higher_is_better else "-"
             metric_str = f"-{mc.core_metric_name}[{tag}]={core_metric:.6f}"
-            if self._better_equal(core_metric, self.best_metric, mc.higher_is_better):
+            if self._is_better_than(core_metric, self.best_metric, mc.higher_is_better):
                 self._remove_ckpt("best")
                 self.best_metric = core_metric
                 ckpt_fname = f"best-{mc.val_mode}={val_mode_val}{metric_str}.ckpt"
                 self.best_ckpt_path = os.path.join(self.ckpt_dir, ckpt_fname)
                 self._save_ckpt(self.best_ckpt_path)
                 logger.info((f"Best model, saving model `{ckpt_fname}`"))
         #
@@ -674,15 +709,15 @@
         res.update(self._metrics_compute(mean_metrics))
         if mode == "result":
             res["global_epoch"] = self.global_epoch
             return res
         # prog_bar
         prog_bar_res = {}
         for k in res.keys():
-            if not self.verbose and (k in {"global_step"} or k.startswith("lr") or k.startswith("grad_norm")):
+            if not self.verbose and (k == "global_step" or k.startswith("lr") or k.startswith("grad_norm")):
                 continue
             prog_bar_res[k] = res[k]
         return prog_bar_res
 
     def _reduce_mes(self, mes: Dict[str, float], device: Device) -> Dict[str, float]:
         """not inplace"""
         assert self.rank >= 0
@@ -716,14 +751,15 @@
                                 num_workers=dataloader.num_workers, pin_memory=dataloader.pin_memory,
                                 drop_last=dataloader.drop_last, collate_fn=dataloader.collate_fn)
         return dataloader
 
     def _optimize_step(self) -> None:
         lmodel = self.lmodel
         scaler = self.scaler
+        self.global_optimizer_step += 1
         for opt_idx, opt in enumerate(lmodel.optimizers):
             if self.gradient_clip_norm is not None:
                 scaler.unscale_(opt)
                 grad_norm = clip_grad_norm_(  # scalar
                     (p for pg in opt.param_groups for p in pg["params"]),
                     max_norm=self.gradient_clip_norm, error_if_nonfinite=False
                 )
@@ -810,29 +846,31 @@
             self._metrics_update(_mean_metrics, self._new_mes, self._prog_bar_mean, device, True)
             _rec_mes.update(self._new_mes)
             # prog_bar
             if (batch_idx + 1) % self.prog_bar_n_steps == 0:
                 prog_bar_mes = self._get_res_mes(_mean_metrics, _rec_mes, "prog_bar")
                 if self.rank >= 0:
                     prog_bar_mes = self._reduce_mes(prog_bar_mes, device)
-                #
-                if self.version is not None:
+                    #
+                if self.rank in {-1, 0}:
                     prog_bar_mes["v"] = self.version
+                    prog_bar_mes["global_step"] = str(int(prog_bar_mes["global_step"]))
                 prog_bar.set_postfix(prog_bar_mes, refresh=False)  # rank > 0 disable.
                 prog_bar.update(self.prog_bar_n_steps)
             # tensorboard
             if self.global_step % self.tb_every_n_steps == 0:
                 tb_mes = self._get_res_mes(_mean_metrics, _rec_mes, "tb")
                 if self.rank >= 0:
                     tb_mes = self._reduce_mes(tb_mes, device)
                 self._tb_logger_add_scalars(tb_mes, self.global_step)
             # val
             if mc.val_mode == "step" and self.global_step % mc.val_every_n == 0:
                 res_mes = self._get_res_mes(_mean_metrics, _rec_mes, "result")
-                prog_bar.fp.write("\n")
+                if not prog_bar.disable:
+                    prog_bar.fp.write("\n")
                 prog_bar.refresh()
                 self._val_and_save_after_train(val_dataloader, res_mes)
         #
         if (batch_idx + 1 - prog_bar.n) > 0:
             prog_bar.update(batch_idx + 1 - prog_bar.n)
         prog_bar.close()
         res_mes = self._get_res_mes(_mean_metrics, _rec_mes, "result")
@@ -848,14 +886,15 @@
         #
         if self.rank not in {-1, 0}:
             dist.barrier()
             return None, {}
         #
         lmodel = self.lmodel
         device = self.device
+        mc = self.model_checkpoint
         #
         model_r = {}
         for s in lmodel._models:
             model: Module = getattr(lmodel, s)
             model_r[s] = model
             model = de_parallel(model)
             setattr(lmodel, s, model)
@@ -907,32 +946,37 @@
             prog_bar.close()
         #
         res_mes = self._get_res_mes(_mean_metrics, _rec_mes, "result")
         #
         with torch.no_grad():
             metrics = val_test_epoch_end()
         res_mes.update(metrics)
-        self._tb_logger_add_scalars(res_mes, self.global_epoch)
+        if mc.val_mode == "epoch":
+            step = self.global_epoch
+        else:
+            step = self.global_step
+        self._tb_logger_add_scalars(res_mes, step)
         #
         core_metric = None
         if len(metrics) > 0:
             logger.info(self._get_epoch_end_string(metrics))
             if stage == "val":
-                core_metric_name = "val_" + self.model_checkpoint.core_metric_name
+                core_metric_name = "val_" + mc.core_metric_name
                 core_metric = metrics[core_metric_name]
         # recover
         for s, model in model_r.items():
             setattr(lmodel, s, model)
         for k, b in metrics_r.items():
             lmodel.metrics[k]._to_sync = b
             lmodel.metrics[k].sync_on_compute = b
         #
         if self.rank == 0:
             dist.barrier()
-        res_mes.update({"global_epoch": self.global_epoch, "global_step": self.global_step})
+        res_mes.update({"global_epoch": self.global_epoch, "global_step": self.global_step, 
+                        "global_optimizer_step": self.global_optimizer_step})
         return core_metric, res_mes
 
     def _val_and_save_after_train(self, val_dataloader: Optional[DataLoader], train_mes: Dict[str, float]) -> None:
         if self._last_optimize:
             self._optimize_step()
         core_metric, val_mes = self._val_test(val_dataloader, "val", "  Val: ")
         val_mes.update(train_mes)
@@ -949,27 +993,27 @@
         self.lmodel.training_epoch_start()
 
     def _test(self, dataloader: Optional[DataLoader],
               model_type: Literal["last", "best"]) -> None:
         #
         if model_type == "best":
             assert self.best_ckpt_path is not None
-            self._load_ckpt(self.best_ckpt_path)
+            self._load_ckpt(self.best_ckpt_path, False, True, True)
             title = f"Test Best(Epoch={self.global_epoch})"
         else:
             title = f"Test Last(Epoch={self.global_epoch})"
         desc = title + ": "
         #
         _, res_mes = self._val_test(dataloader, "test", desc)
         res_mes["mode"] = f"test_{model_type}"
         self._result_saving(res_mes)
         #
         if model_type == "best":
             assert self.last_ckpt_path is not None
-            self._load_ckpt(self.last_ckpt_path)
+            self._load_ckpt(self.last_ckpt_path, False, True, True)
 
     def _best_ckpt_is_last(self) -> bool:
         if self.best_ckpt_path is None or self.last_ckpt_path is None:
             return False
 
         best_ckpt_fname = os.path.basename(self.best_ckpt_path)
         m = re.match(r"best-(epoch|step)=(\d+)", best_ckpt_fname)
@@ -990,15 +1034,15 @@
             assert mc.core_metric_name is not None
             assert mc.higher_is_better is not None
         #
         self.lmodel.training_epoch_start()
         train_mes = {}
         for _ in range(self.global_epoch + 1, self.max_epochs):
             self.global_epoch += 1
-            train_mes = self._train_epoch(train_dataloader, val_dataloader, )
+            train_mes = self._train_epoch(train_dataloader, val_dataloader)
             if mc.val_mode == "epoch" and (self.global_epoch + 1) % mc.val_every_n == 0:
                 self._val_and_save_after_train(val_dataloader, train_mes)
         if self._last_val:
             self._val_and_save_after_train(val_dataloader, train_mes)
         cuda.empty_cache()
 
     def test(self, dataloader: Optional[DataLoader], test_best: bool = True, test_last: bool = True) -> None:
```

### Comparing `mini-lightning-0.2.0/mini_lightning/_types.py` & `mini-lightning-0.2.1/mini_lightning/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 import math
 import datetime as dt
 import platform 
 import logging
+from logging import Logger, Handler
 import random
 import csv
 import time
 from bisect import bisect_right
 from copy import deepcopy
 from collections import defaultdict
 from typing import List, Any, Dict, Optional, Tuple, Callable, Union, Sequence, Mapping, Literal, Set,  TypeVar
```

### Comparing `mini-lightning-0.2.0/mini_lightning/_utils.py` & `mini-lightning-0.2.1/mini_lightning/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __all__ = [
     "get_dist_setting", "logger",
     "en_parallel", "de_parallel", "de_sync_batchnorm", "select_device",
     "_remove_keys", "_key_add_suffix", "freeze_layers", "stat_array",
     "test_time", "seed_everything", "time_synchronize",
     "print_model_info", "write_to_yaml", "read_from_yaml", "write_to_csv",
     "get_date_now", "load_ckpt", "save_ckpt",
-    "ModelCheckpoint", "HParamsBase", "parse_device_ids"
+    "ModelCheckpoint", "ResumeFromCkpt", "parse_device_ids"
 ]
 #
 
 
 def get_dist_setting() -> Tuple[int, int, int]:
     """return rank, local_rank, world_size"""
     rank = int(os.getenv("RANK", -1))
@@ -25,17 +25,17 @@
     return rank, local_rank, world_size
 
 
 def _get_logger() -> logging.Logger:
     level = logging.INFO
     name = "mini-lightning"
     #
-    logger = logging.getLogger(name)
+    logger: Logger = logging.getLogger(name)
     logger.setLevel(level)
-    handler = logging.StreamHandler()
+    handler: Handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter(f"[%(levelname)s: {name}] %(message)s"))
     handler.setLevel(level)
     logger.addHandler(handler)
     return logger
 
 
 #
@@ -152,22 +152,23 @@
                 requires_grad = False
                 break
         if verbose:
             logger.info(f"Setting {n}.requires_grad: {requires_grad}")
         p.requires_grad_(requires_grad)
 
 
-def stat_array(x: ndarray) -> Tuple[Tuple[float, float, float, float], str]:
-    """statistics. return: (mean, std, max_, min_), stat_str"""
+def stat_array(x: ndarray) -> Tuple[Tuple[float, float, float, float, int], str]:
+    """statistics. return: (mean, std, min_, max_, _len), stat_str"""
     mean = x.mean().item()
     std = x.std().item()
-    max_ = x.max().item()
     min_ = x.min().item()
-    stat_str = f"{mean:.6f}±{std:.6f}, max={max_:.6f}, min={min_:.6f}"
-    return (mean, std, max_, min_), stat_str
+    max_ = x.max().item()
+    len_ = sum(x.shape)
+    stat_str = f"{mean:.6f}±{std:.6f}, min={min_:.6f}, max={max_:.6f}, len={len_}"
+    return (mean, std, min_, max_, len_), stat_str
 
 
 _T = TypeVar("_T")
 
 
 def test_time(func: Callable[[], _T], number: int = 1, warmup: int = 0,
               timer: Optional[Callable[[], float]] = None) -> _T:
@@ -319,43 +320,45 @@
         # Define what is a good model (for model saving)
         core_metric_name: Optional[str] = None,  # e.g. "acc".
         higher_is_better: Optional[bool] = None,  # e.g. True
         # note: the last epoch/step will always be validated
         val_every_n: int = 1,  # val_every_n_epoch or val_every_n_steps
         val_mode: Literal["epoch", "step"] = "epoch",
         #
+        saving_optimizers: bool = False,  # state_dict
+
         write_result_csv: bool = True,
-        saving_optimizers: bool = False,
     ) -> None:
         #
         self.core_metric_name = core_metric_name
         self.higher_is_better = higher_is_better
         self.val_every_n = val_every_n
-        self.val_mode = val_mode
-        self.write_result_csv = write_result_csv
+        self.val_mode: Literal["epoch", "step"] = val_mode
         self.saving_optimizers = saving_optimizers
+        self.write_result_csv = write_result_csv
 
     def __repr__(self) -> str:
         attr_str = ", ".join([f"{k}={v!r}" for k, v in self.__dict__.items()])
         return f"{self.__class__.__name__}({attr_str})"
 
 
-class HParamsBase:
-    def __init__(self, device_ids: List[int], dataloader_hparams: Dict[str, Any],
-                 optim_name: str, optim_hparams: Dict[str, Any], trainer_hparams: Dict[str, Any],
-                 warmup: Optional[int] = None, lrs_hparams: Optional[Dict[str, Any]] = None) -> None:
-        self.device_ids = device_ids
-        self.dataloader_hparams = dataloader_hparams
-        self.optim_name = optim_name
-        self.optim_hparams = optim_hparams
-        self.trainer_hparams = trainer_hparams
-        if warmup is not None:
-            self.warmup = warmup
-        if lrs_hparams is not None:
-            self.lrs_hparams = lrs_hparams
+class ResumeFromCkpt:
+    def __init__(
+        self,
+        ckpt_path: str,   # e.g. `trainer.last_ckpt_path`, `*.ckpt`
+        load_optimizers: bool = False,
+        load_message: bool = False,  # global_step, global_epoch...
+    ) -> None:
+        self.ckpt_path = ckpt_path
+        self.load_optimizers = load_optimizers
+        self.load_message = load_message
+
+    def __repr__(self) -> str:
+        attr_str = ", ".join([f"{k}={v!r}" for k, v in self.__dict__.items()])
+        return f"{self.__class__.__name__}({attr_str})"
 
 
 def parse_device_ids() -> List[int]:
     parser = ArgumentParser()
     parser.add_argument("--device_ids", "-d", nargs="*", type=int,
                         default=[0], help="e.g. [], [0], [0, 1, 2]. --device_ids; --device_ids 0; -d 0 1 2")
     opt: Namespace = parser.parse_args()  # options
```

### Comparing `mini-lightning-0.2.0/mini_lightning/_visualize.py` & `mini-lightning-0.2.1/mini_lightning/_visualize.py`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/mini_lightning/_warmup_lrs.py` & `mini-lightning-0.2.1/mini_lightning/_warmup_lrs.py`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/mini_lightning.egg-info/PKG-INFO` & `mini-lightning-0.2.1/mini_lightning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-lightning
-Version: 0.2.0
+Version: 0.2.1
 Summary: Mini-Lightning is a lightweight machine learning training library, which is a mini version of Pytorch-Lightning with only 1k lines of code. It has the advantages of faster, more concise and more flexible.
 Home-page: https://github.com/ustcml/mini-lightning/
 Author: Jintao Huang
 Author-email: huangjintao@mail.ustc.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mini-lightning-0.2.0/setup.py` & `mini-lightning-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 setup(
     name="mini-lightning",
-    version="0.2.0",
+    version="0.2.1",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/ustcml/mini-lightning/",
     author="Jintao Huang",
     author_email="huangjintao@mail.ustc.edu.cn",
```

### Comparing `mini-lightning-0.2.0/tests/test_lrs.py` & `mini-lightning-0.2.1/tests/test_lrs.py`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/tests/test_utils.py` & `mini-lightning-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.0/tests/test_visualize.py` & `mini-lightning-0.2.1/tests/test_visualize.py`

 * *Files identical despite different names*

