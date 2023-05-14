# Comparing `tmp/redcat-0.0.1a182.tar.gz` & `tmp/redcat-0.0.1a198.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.1a182.tar", max compression
+gzip compressed data, was "redcat-0.0.1a198.tar", max compression
```

## Comparing `redcat-0.0.1a182.tar` & `redcat-0.0.1a198.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1501 2023-05-12 13:45:55.644109 redcat-0.0.1a182/LICENSE
--rw-r--r--   0        0        0     1594 2023-05-12 13:45:55.648110 redcat-0.0.1a182/README.md
--rw-r--r--   0        0        0     4382 2023-05-12 13:45:55.648110 redcat-0.0.1a182/pyproject.toml
--rw-r--r--   0        0        0      227 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/__init__.py
--rw-r--r--   0        0        0    18686 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/base.py
--rw-r--r--   0        0        0     2428 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/comparators.py
--rw-r--r--   0        0        0   128571 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/tensor.py
--rw-r--r--   0        0        0    51342 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/tensorseq.py
--rw-r--r--   0        0        0    12134 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/utils.py
--rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 redcat-0.0.1a182/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-14 06:53:03.592352 redcat-0.0.1a198/LICENSE
+-rw-r--r--   0        0        0     1594 2023-05-14 06:53:03.592352 redcat-0.0.1a198/README.md
+-rw-r--r--   0        0        0     4382 2023-05-14 06:53:03.592352 redcat-0.0.1a198/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/__init__.py
+-rw-r--r--   0        0        0    17892 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/base.py
+-rw-r--r--   0        0        0     2428 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/comparators.py
+-rw-r--r--   0        0        0     4559 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/list.py
+-rw-r--r--   0        0        0   138063 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/tensor.py
+-rw-r--r--   0        0        0    50431 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0    12134 2023-05-14 06:53:03.596352 redcat-0.0.1a198/src/redcat/utils.py
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 redcat-0.0.1a198/PKG-INFO
```

### Comparing `redcat-0.0.1a182/LICENSE` & `redcat-0.0.1a198/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a182/README.md` & `redcat-0.0.1a198/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a182/pyproject.toml` & `redcat-0.0.1a198/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.1a182"
+version = "0.0.1a198"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
```

### Comparing `redcat-0.0.1a182/src/redcat/base.py` & `redcat-0.0.1a198/src/redcat/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,37 +29,37 @@
         r"""The data in the batch."""
 
     ###############################
     #     Creation operations     #
     ###############################
 
     @abstractmethod
-    def clone(self, *args, **kwargs) -> TBatch:
+    def clone(self) -> TBatch:
         r"""Creates a copy of the current batch.
 
-        Args:
-            *args: See the documentation of ``torch.Tensor.clone``
-            **kwargs: See the documentation of ``torch.Tensor.clone``
-
         Returns:
-            ``BaseBatchedTensor``: A copy of the current batch.
+            ``BaseBatch``: A copy of the current batch.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch_copy = batch.clone()
             >>> batch_copy
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=0)
         """
 
+    #################################
+    #     Comparison operations     #
+    #################################
+
     @abstractmethod
     def allclose(
         self, other: Any, rtol: float = 1e-5, atol: float = 1e-8, equal_nan: bool = False
     ) -> bool:
         r"""Indicates if two batches are equal within a tolerance or not.
 
         Args:
@@ -119,15 +119,15 @@
         Args:
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Returns:
-            ``BaseBatchedTensor``: A new batch with permuted data.
+            ``BaseBatch``: A new batch with permuted data.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
@@ -171,15 +171,15 @@
 
         Args:
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Returns:
-            ``BaseBatchedTensor``:  A new batch with shuffled data.
+            ``BaseBatch``:  A new batch with shuffled data.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
@@ -262,14 +262,17 @@
         Args:
             chunks (int): Specifies the number of chunks.
 
         Returns:
             tuple: The batch split into chunks along the batch
                 dimension.
 
+        Raises:
+            RuntimeError if the number of chunks is incorrect
+
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).chunk_along_batch(chunks=3)
@@ -428,39 +431,14 @@
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).split_along_batch(2)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
         """
 
-    def take_along_batch(self, indices: BaseBatch | Tensor | Sequence) -> TBatch:
-        r"""Takes values along the batch dimension.
-
-        Args:
-            indices (``BaseBatch`` or ``Tensor`` or sequence):
-                Specifies the indices to take along the batch
-                dimension.
-
-        Returns:
-            ``BaseBatch``: The batch with the selected data.
-
-        Example usage:
-
-        .. code-block:: python
-
-            >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_batch(
-            ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]]))
-            ... )
-            tensor([[6, 5],
-                    [0, 7],
-                    [2, 9]], batch_dim=0)
-        """
-
     ########################
     #     mini-batches     #
     ########################
 
     def get_num_minibatches(self, batch_size: int, drop_last: bool = False) -> int:
         r"""Gets the number of mini-batches for a given batch size.
```

### Comparing `redcat-0.0.1a182/src/redcat/comparators.py` & `redcat-0.0.1a198/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a182/src/redcat/tensor.py` & `redcat-0.0.1a198/src/redcat/tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,53 @@
         return self._data
 
     @property
     def device(self) -> torch.device:
         r"""``torch.device``: The device where the batch data/tensor is."""
         return self._data.device
 
+    @property
+    def shape(self) -> torch.Size:
+        r"""``torch.Size``: The shape of the tensor."""
+        return self._data.shape
+
+    def dim(self) -> int:
+        r"""Gets the number of dimensions.
+
+        Returns:
+            int: The number of dimensions
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.ones(2, 3)).dim()
+            2
+        """
+        return self._data.dim()
+
+    def ndimension(self) -> int:
+        r"""Gets the number of dimensions.
+
+        Returns:
+            int: The number of dimensions
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.ones(2, 3)).ndimension()
+            2
+        """
+        return self.dim()
+
     def numel(self) -> int:
         r"""Gets the total number of elements in the tensor.
 
         Returns:
             int: The total number of elements
 
         Example usage:
@@ -2045,14 +2084,77 @@
         """
         self._data.sqrt_()
 
     ################################
     #     Reduction operations     #
     ################################
 
+    def max(self, *args, **kwargs) -> Tensor | torch.return_types.max:
+        r"""Computes the maximum of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.max``
+            **kwargs: See the documentation of ``torch.Tensor.max``
+
+        Returns:
+            ``torch.Tensor`` or ``torch.return_types.max``:
+                The maximum of all elements.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).max()
+            tensor(9)
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).max(dim=1)
+            torch.return_types.max(
+            values=tensor([4, 9]),
+            indices=tensor([4, 4]))
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).max(dim=1, keepdim=True)
+            torch.return_types.max(
+            values=tensor([[4], [9]]),
+            indices=tensor([[4], [4]]))
+        """
+        return torch.max(self, *args, **kwargs)
+
+    def max_along_batch(self, keepdim: bool = False) -> torch.return_types.max:
+        r"""Computes the maximum values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.return_types.max``: A batch with
+                the maximum values along the batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
+            ... ).max_along_batch()
+            torch.return_types.max(
+            values=tensor([4, 9]),
+            indices=tensor([4, 4]))
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
+            ... ).max_along_batch(keepdim=True)
+            torch.return_types.max(
+            values=tensor([[4], [9]]),
+            indices=tensor([[4], [4]]))
+        """
+        return self.max(dim=self._batch_dim, keepdim=keepdim)
+
     def mean(self, *args, **kwargs) -> Tensor:
         r"""Computes the mean of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.mean``
             **kwargs: See the documentation of ``torch.Tensor.mean``
 
@@ -2088,21 +2190,146 @@
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_seq()
+            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch()
             tensor([4.0, 5.0])
-            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_seq(keepdim=True)
+            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch(keepdim=True)
             tensor([[4.0], [5.0]])
         """
         return self.mean(dim=self._batch_dim, keepdim=keepdim)
 
+    def median(self, *args, **kwargs) -> Tensor | torch.return_types.median:
+        r"""Computes the median of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.median``
+            **kwargs: See the documentation of ``torch.Tensor.median``
+
+        Returns:
+            ``torch.Tensor`` or ``torch.return_types.median``:
+                The median of all elements or per dimension.
+                The first tensor will be populated with the median
+                values and the second tensor, which must have dtype
+                long, with their indices in the dimension dim of input.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).median()
+            tensor(4)
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).median(dim=1)
+            torch.return_types.median(
+            values=tensor([2, 7]),
+            indices=tensor([2, 2]))
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).median(dim=1, keepdim=True)
+            torch.return_types.median(
+            values=tensor([[2], [7]]),
+            indices=tensor([[2], [2]]))
+        """
+        return torch.median(self, *args, **kwargs)
+
+    def median_along_batch(self, keepdim: bool = False) -> torch.return_types.median:
+        r"""Computes the median values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.return_types.median``:  The first tensor will
+                be populated with the median values and the second
+                tensor, which must have dtype long, with their indices
+                in the batch dimension of input.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
+            ... ).median_along_batch()
+            torch.return_types.median(
+            values=tensor([2, 7]),
+            indices=tensor([2, 2]))
+        """
+        return self.median(dim=self._batch_dim, keepdim=keepdim)
+
+    def min(self, *args, **kwargs) -> Tensor | torch.return_types.min:
+        r"""Computes the minimum of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.min``
+            **kwargs: See the documentation of ``torch.Tensor.min``
+
+        Returns:
+            ``torch.Tensor`` or ``torch.return_types.min``:
+                The minimum of all elements.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).min()
+            tensor(0)
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).min(dim=1)
+            torch.return_types.min(
+            values=tensor([0, 5]),
+            indices=tensor([0, 0]))
+            >>> BatchedTensor(torch.arange(10).view(2, 5)).min(dim=1, keepdim=True)
+            torch.return_types.min(
+            values=tensor([[0], [5]]),
+            indices=tensor([[0], [0]]))
+        """
+        return torch.min(self, *args, **kwargs)
+
+    def min_along_batch(self, keepdim: bool = False) -> torch.return_types.min:
+        r"""Computes the minimum values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.return_types.min``: A batch with
+                the minimum values along the batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
+            ... ).min_along_batch()
+            torch.return_types.min(
+            values=tensor([0, 5]),
+            indices=tensor([0, 0]))
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
+            ... ).min_along_batch(keepdim=True)
+            torch.return_types.min(
+            values=tensor([[0], [5]]),
+            indices=tensor([[0], [0]]))
+        """
+        return self.min(dim=self._batch_dim, keepdim=keepdim)
+
     def nanmean(self, *args, **kwargs) -> Tensor:
         r"""Computes the mean of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.nanmean``
             **kwargs: See the documentation of ``torch.Tensor.nanmean``
 
@@ -2126,14 +2353,43 @@
             >>> BatchedTensor(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nanmean(dim=1, keepdim=True)
             tensor([[2.0], [6.5]])
         """
         return torch.nanmean(self, *args, **kwargs)
 
+    def nanmean_along_batch(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the mean values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A batch with
+                the mean values along the batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ... ).nanmean_along_batch()
+            tensor([2.0, 6.5])
+            >>> BatchedTensor(
+            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ... ).nanmean_along_batch(keepdim=True)
+            tensor([[2.0, 6.5]])
+        """
+        return self.nanmean(dim=self._batch_dim, keepdim=keepdim)
+
     def nanmedian(self, *args, **kwargs) -> Tensor | torch.return_types.nanmedian:
         r"""Computes the median of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.nanmedian``
             **kwargs: See the documentation of ``torch.Tensor.nanmedian``
 
@@ -3499,14 +3755,37 @@
         self, split_size_or_sections: int | Sequence[int]
     ) -> tuple[BatchedTensor, ...]:
         return self.split(split_size_or_sections, dim=self._batch_dim)
 
     def take_along_batch(
         self, indices: BaseBatch[Tensor | Sequence] | Tensor | Sequence
     ) -> TBatchedTensor:
+        r"""Takes values along the batch dimension.
+
+        Args:
+            indices (``BaseBatch`` or ``Tensor`` or sequence):
+                Specifies the indices to take along the batch
+                dimension.
+
+        Returns:
+            ``BaseBatch``: The batch with the selected data.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_batch(
+            ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]]))
+            ... )
+            tensor([[6, 5],
+                    [0, 7],
+                    [2, 9]], batch_dim=0)
+        """
         return self.take_along_dim(indices, dim=self._batch_dim)
 
     def take_along_dim(
         self,
         indices: BaseBatch[Tensor | Sequence] | Tensor | Sequence,
         dim: int | None = None,
     ) -> TBatchedTensor:
```

### Comparing `redcat-0.0.1a182/src/redcat/tensorseq.py` & `redcat-0.0.1a198/src/redcat/tensorseq.py`

 * *Files 4% similar despite different names*

```diff
@@ -583,52 +583,42 @@
         check_seq_dims(get_seq_dims((self, other)))
         super().logical_xor_(other)
 
     ################################
     #     Reduction operations     #
     ################################
 
-    def max_along_seq(
-        self, keepdim: bool = False
-    ) -> tuple[BatchedTensor | BatchedTensorSeq, BatchedTensor | BatchedTensorSeq]:
+    def max_along_seq(self, keepdim: bool = False) -> torch.return_types.max:
         r"""Computes the maximum values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
-                the sequence dimension retained or not. If ``False``
-                the returned type is ``BatchedTensor``, otherwise it
-                is ``BatchedTensorSeq``. Default: ``False``
+                the sequence dimension retained or not.
+                Default: ``False``
 
         Returns:
-            ``BatchedTensor``: A batch with the maximum values along the
-                sequence dimension.
+            ``torch.return_types.max``: A batch with
+                the maximum values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).max_along_seq()
-            (tensor([4, 9], batch_dim=0), tensor([4, 4], batch_dim=0))
-            >>> BatchedTensorSeq(torch.arange(30).view(2, 5, 3)).max_along_seq(keepdim=True)
-            (tensor([[[12, 13, 14]], [[27, 28, 29]]], batch_dim=0, seq_dim=1),
-             tensor([[[4, 4, 4]], [[4, 4, 4]]], batch_dim=0, seq_dim=1))
-        """
-        values, indices = torch.max(self._data, dim=self._seq_dim, keepdim=keepdim)
-        if keepdim:
-            return (
-                BatchedTensorSeq(data=values, **self._get_kwargs()),
-                BatchedTensorSeq(data=indices, **self._get_kwargs()),
-            )
-        batch_dim = self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1
-        return (
-            BatchedTensor(data=values, batch_dim=batch_dim),
-            BatchedTensor(data=indices, batch_dim=batch_dim),
-        )
+            torch.return_types.max(
+            values=tensor([4, 9]),
+            indices=tensor([4, 4]))
+            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).max_along_seq(keepdim=True)
+            torch.return_types.max(
+            values=tensor([[4], [9]]),
+            indices=tensor([[4], [4]]))
+        """
+        return self.max(dim=self._seq_dim, keepdim=keepdim)
 
     def mean_along_seq(self, keepdim: bool = False) -> BatchedTensor | BatchedTensorSeq:
         r"""Computes the mean values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not. If ``False``
@@ -641,98 +631,105 @@
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(5, 2).float()).mean_along_seq()
+            >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq()
             tensor([2.0, 7.0])
-            >>> BatchedTensorSeq(torch.arange(10).view(5, 2).float()).mean_along_seq(keepdim=True)
+            >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq(keepdim=True)
             tensor([[2.0], [7.0]])
         """
         return self.mean(dim=self._seq_dim, keepdim=keepdim)
 
-    def median_along_seq(
-        self, keepdim: bool = False
-    ) -> tuple[BatchedTensor | BatchedTensorSeq, BatchedTensor | BatchedTensorSeq]:
+    def median_along_seq(self, keepdim: bool = False) -> torch.return_types.median:
         r"""Computes the median values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
-                the sequence dimension retained or not. If ``False``
-                the returned type is ``BatchedTensor``, otherwise it
-                is ``BatchedTensorSeq``. Default: ``False``
+                the sequence dimension retained or not.
+                Default: ``False``
 
         Returns:
-            ``BatchedTensor``: A batch with the median values along the
-                sequence dimension.
+            ``torch.return_types.median``:  The first tensor will
+                be populated with the median values and the second
+                tensor, which must have dtype long, with their indices
+                in the sequence dimension of input.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).median_along_seq()
-            (tensor([2, 7], batch_dim=0), tensor([2, 2], batch_dim=0))
-            >>> BatchedTensorSeq(torch.arange(30).view(2, 5, 3)).median_along_seq(keepdim=True)
-            (tensor([[[12, 13, 14]], [[27, 28, 29]]], batch_dim=0, seq_dim=1),
-             tensor([[[4, 4, 4]], [[4, 4, 4]]], batch_dim=0, seq_dim=1))
-        """
-        values, indices = torch.median(self._data, dim=self._seq_dim, keepdim=keepdim)
-        if keepdim:
-            return (
-                BatchedTensorSeq(data=values, **self._get_kwargs()),
-                BatchedTensorSeq(data=indices, **self._get_kwargs()),
-            )
-        batch_dim = self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1
-        return (
-            BatchedTensor(data=values, batch_dim=batch_dim),
-            BatchedTensor(data=indices, batch_dim=batch_dim),
-        )
-
-    def min_along_seq(
-        self, keepdim: bool = False
-    ) -> tuple[BatchedTensor | BatchedTensorSeq, BatchedTensor | BatchedTensorSeq]:
+            torch.return_types.median(
+            values=tensor([2, 7]),
+            indices=tensor([2, 2]))
+        """
+        return self.median(dim=self._seq_dim, keepdim=keepdim)
+
+    def min_along_seq(self, keepdim: bool = False) -> torch.return_types.min:
         r"""Computes the minimum values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
-                the sequence dimension retained or not. If ``False``
-                the returned type is ``BatchedTensor``, otherwise it
-                is ``BatchedTensorSeq``. Default: ``False``
+                the sequence dimension retained or not.
+                Default: ``False``
 
         Returns:
-            ``BatchedTensor``: A batch with the minimum values along the
-                sequence dimension.
+            ``torch.return_types.min``: A batch with
+                the minimum values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).min_along_seq()
-            (tensor([0, 5], batch_dim=0), tensor([0, 0], batch_dim=0))
-            >>> BatchedTensorSeq(torch.arange(30).view(2, 5, 3)).min_along_seq(keepdim=True)
-            (tensor([[[ 0,  1,  2]], [[15, 16, 17]]], batch_dim=0, seq_dim=1),
-             tensor([[[0, 0, 0]], [[0, 0, 0]]], batch_dim=0, seq_dim=1))
-        """
-        values, indices = torch.min(self._data, dim=self._seq_dim, keepdim=keepdim)
-        if keepdim:
-            return (
-                BatchedTensorSeq(data=values, **self._get_kwargs()),
-                BatchedTensorSeq(data=indices, **self._get_kwargs()),
-            )
-        batch_dim = self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1
-        return (
-            BatchedTensor(data=values, batch_dim=batch_dim),
-            BatchedTensor(data=indices, batch_dim=batch_dim),
-        )
+            torch.return_types.min(
+            values=tensor([0, 5]),
+            indices=tensor([0, 0]))
+            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).min_along_seq(keepdim=True)
+            torch.return_types.min(
+            values=tensor([[0], [5]]),
+            indices=tensor([[0], [0]]))
+        """
+        return self.min(dim=self._seq_dim, keepdim=keepdim)
+
+    def nanmean_along_seq(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the mean values along the sequence dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A batch with
+                the mean values along the sequence dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensorSeq
+            >>> BatchedTensorSeq(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmean_along_seq()
+            tensor([2.0, 6.5])
+            >>> BatchedTensorSeq(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmean_along_seq(keepdim=True)
+            tensor([[2.0], [6.5]])
+        """
+        return self.nanmean(dim=self._seq_dim, keepdim=keepdim)
 
     def nanmedian_along_seq(self, keepdim: bool = False) -> torch.return_types.nanmedian:
         r"""Computes the median values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not.
@@ -745,16 +742,16 @@
                 in the sequence dimension of input.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
+            >>> from redcat import BatchedTensorSeq
+            >>> BatchedTensorSeq(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nanmedian_along_seq()
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
         """
         return self.nanmedian(dim=self._seq_dim, keepdim=keepdim)
@@ -772,16 +769,16 @@
                 sequence dimension.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
+            >>> from redcat import BatchedTensorSeq
+            >>> BatchedTensorSeq(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nansum_along_seq()
             tensor([20., 26.])
         """
         return self.nansum(dim=self._seq_dim, keepdim=keepdim)
 
     def prod_along_seq(self, keepdim: bool = False) -> Tensor:
@@ -797,18 +794,18 @@
                 the product values along the sequence dimension.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq()
+            >>> from redcat import BatchedTensorSeq
+            >>> BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq()
             tensor([ 120, 3024])
-            >>> BatchedTensor(
+            >>> BatchedTensorSeq(
             ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
             ... ).prod_along_seq(keepdim=True)
             tensor([[ 120], [3024]])
         """
         return self.prod(dim=self._seq_dim, keepdim=keepdim)
 
     def sum_along_seq(self, keepdim: bool = False) -> Tensor:
```

### Comparing `redcat-0.0.1a182/src/redcat/utils.py` & `redcat-0.0.1a198/src/redcat/utils.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a182/PKG-INFO` & `redcat-0.0.1a198/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.1a182
+Version: 0.0.1a198
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.1a182 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.1a198 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

