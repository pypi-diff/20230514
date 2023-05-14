# Comparing `tmp/spatialgeometry-1.0.3.tar.gz` & `tmp/spatialgeometry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialgeometry-1.0.3.tar", last modified: Wed Dec  7 04:16:45 2022, max compression
+gzip compressed data, was "spatialgeometry-1.1.0.tar", last modified: Sun May 14 05:41:57 2023, max compression
```

## Comparing `spatialgeometry-1.0.3.tar` & `spatialgeometry-1.1.0.tar`

### file list

```diff
@@ -1,413 +1,415 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3870 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3152 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      727 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.639048 spatialgeometry-1.0.3/spatialgeometry/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.643048 spatialgeometry-1.0.3/spatialgeometry/core/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.643048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (122)    12799 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (122)      122 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (122)      894 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/KLUSupport
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (122)      991 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/PaStiXSupport
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (122)      900 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (122)      888 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (122)      797 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (122)      803 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.639048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.647048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (122)    24934 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (122)    18760 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (122)     3974 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.647048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    25441 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.655048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (122)    19214 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (122)    16782 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (122)     8217 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     7018 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (122)     2738 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (122)    41673 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    12488 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (122)    14075 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    18648 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (122)     4429 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (122)     5981 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (122)     6990 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (122)    63841 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (122)     4745 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (122)     7909 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)    36282 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)     8256 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (122)    31529 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (122)    24484 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (122)    25360 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (122)     9870 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (122)    14670 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)      988 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)    11654 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (122)     5841 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (122)     5759 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (122)    21679 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)    38812 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)    11543 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)     8238 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (122)     7256 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (122)    11281 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (122)    60784 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)     7156 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (122)    24343 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    23856 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (122)     3620 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (122)    12884 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (122)     9207 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (122)    20748 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    49193 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     7336 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (122)    53832 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (122)     7756 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (122)    19195 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (122)    17821 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (122)     5656 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (122)    17033 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (122)     4284 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (122)     7522 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (122)     6143 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (122)    14999 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)     6837 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (122)     9368 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (122)     6170 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     8700 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (122)    21641 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (122)    17606 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (122)    13567 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (122)    38277 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)     3488 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (122)    35168 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (122)    11997 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.639048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.655048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (122)    15223 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)     8102 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    64608 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.655048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (122)    17160 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)    13344 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    87891 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.655048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (122)    16540 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)   119355 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     9490 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (122)    24820 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxr-xr-x   0 runner    (1001) docker     (122)   102394 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.655048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (122)    17317 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (122)    26903 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (122)     5251 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (122)    67696 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)     3770 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (122)    35534 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    57047 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.635048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (122)      691 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (122)    17541 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)    16159 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    33615 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (122)    22503 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)     6815 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)   189525 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)    51286 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (122)    14251 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)     6765 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    64465 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    21200 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.659048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (122)     7428 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (122)    12539 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (122)    27786 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (122)    21856 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (122)     2626 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.663048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (122)    16728 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (122)     8024 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    36894 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.663048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (122)     6686 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (122)    20921 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (122)     8334 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (122)      607 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (122)    40146 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.667048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (122)   108448 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (122)    20104 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    15948 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (122)     6936 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)     5106 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)    21724 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     6368 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)     5582 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (122)    21354 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    11570 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)     9958 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     5209 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)     6164 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (122)    20987 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    13867 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)    14722 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (122)    10571 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)    14678 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)     6707 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.667048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (122)    23156 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (122)    19876 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (122)    21931 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (122)     4892 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (122)    15555 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (122)     6696 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (122)    10949 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/IntegralConstant.h
--rwxr-xr-x   0 runner    (1001) docker     (122)     4268 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (122)    52909 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (122)    46661 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    29336 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (122)    10676 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (122)    12003 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (122)    35762 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (122)    12559 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)    17274 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (122)    22970 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)    17176 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)     9716 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)    14349 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (122)     5575 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (122)    23640 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (122)    21078 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (122)    35182 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (122)    22764 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (122)    18939 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (122)     8403 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (122)    20726 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (122)    11962 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (122)     8955 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (122)     9812 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (122)    34367 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (122)     6862 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (122)     8063 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (122)    61930 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (122)     7664 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (122)     6190 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (122)     5945 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (122)    23611 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (122)     6771 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (122)     6850 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (122)     8887 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (122)    15036 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (122)    14940 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (122)    13379 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (122)    16383 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.671048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/KLUSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    11555 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (122)     3439 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (122)    32383 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (122)    15727 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (122)    22069 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (122)    13693 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (122)    16105 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (122)    61681 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (122)     5248 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    22249 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    20092 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (122)    25498 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (122)    23429 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (122)    26768 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (122)    14641 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (122)    54214 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (122)    32988 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (122)     5099 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (122)    14743 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (122)    15957 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.675048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (122)    24216 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.679048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (122)    10670 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (122)    13166 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    11368 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (122)    24360 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (122)     6485 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (122)    13606 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (122)    25524 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)     4757 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (122)    13256 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     5808 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (122)    12589 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (122)    57475 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)    17451 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     7329 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (122)     7593 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (122)    15600 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (122)    25889 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (122)     4424 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (122)     8704 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (122)     6437 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (122)     6827 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     8127 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (122)     9657 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (122)    33316 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (122)     4303 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (122)     7602 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (122)     4974 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (122)    12837 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)     6712 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (122)     6584 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (122)     3681 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (122)    10217 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (122)     8485 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (122)     9028 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (122)     4979 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (122)    29167 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (122)     5338 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     2809 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    34324 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (122)    24456 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.683048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (122)     2913 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (122)    30560 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (122)     7834 2022-12-07 04:16:34.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (122)  1058369 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (122)      474 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)    14060 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)    21431 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)    59020 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)    12283 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (122)     6915 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/linalg.h
--rw-r--r--   0 runner    (1001) docker     (122)     9445 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/scene.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/core/scene.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/spatialgeometry/geom/
--rw-r--r--   0 runner    (1001) docker     (122)    11734 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/geom/CollisionShape.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      587 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/geom/SceneGroup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8866 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/geom/SceneNode.py
--rw-r--r--   0 runner    (1001) docker     (122)    10706 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/geom/Shape.py
--rw-r--r--   0 runner    (1001) docker     (122)      473 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/geom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.687048 spatialgeometry-1.0.3/spatialgeometry/tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9309 2022-12-07 04:16:35.000000 spatialgeometry-1.0.3/spatialgeometry/tools/stdout_supress.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 04:16:45.643048 spatialgeometry-1.0.3/spatialgeometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3870 2022-12-07 04:16:45.000000 spatialgeometry-1.0.3/spatialgeometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19581 2022-12-07 04:16:45.000000 spatialgeometry-1.0.3/spatialgeometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-07 04:16:45.000000 spatialgeometry-1.0.3/spatialgeometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      180 2022-12-07 04:16:45.000000 spatialgeometry-1.0.3/spatialgeometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-12-07 04:16:45.000000 spatialgeometry-1.0.3/spatialgeometry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.377576 spatialgeometry-1.1.0/spatialgeometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.377576 spatialgeometry-1.1.0/spatialgeometry/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.381576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.377576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.381576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.381576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.389576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41673 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12488 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63841 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36282 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38812 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60784 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23856 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49193 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53832 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38277 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.373576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64608 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    87891 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119355 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   102394 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67696 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57047 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.373576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.393576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33615 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    22503 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   189525 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64465 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27786 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36894 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.397576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40146 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.401576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)   108448 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.405576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23156 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4892 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52909 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46661 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29336 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.405576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.405576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34367 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61930 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.405576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32383 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61681 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22249 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.409576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.413576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    54214 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.413576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.417576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058369 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59020 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/linalg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/scene.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/core/scene.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/spatialgeometry/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/geom/CollisionShape.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/geom/SceneGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/geom/SceneNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/geom/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/geom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/spatialgeometry/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/spatialgeometry/tools/stdout_supress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.377576 spatialgeometry-1.1.0/spatialgeometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-14 05:41:57.000000 spatialgeometry-1.1.0/spatialgeometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19601 2023-05-14 05:41:57.000000 spatialgeometry-1.1.0/spatialgeometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:41:57.000000 spatialgeometry-1.1.0/spatialgeometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-14 05:41:57.000000 spatialgeometry-1.1.0/spatialgeometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 05:41:57.000000 spatialgeometry-1.1.0/spatialgeometry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:41:57.421576 spatialgeometry-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-14 05:41:46.000000 spatialgeometry-1.1.0/tests/test_Shape.py
```

### Comparing `spatialgeometry-1.0.3/LICENSE` & `spatialgeometry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/PKG-INFO` & `spatialgeometry-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialgeometry
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Shape and Geometry Description Package
 Author-email: Jesse Haviland <j.haviland@qut.edu.au>, Peter Corke <rvc@petercorke.com>
 License: MIT License
         
         Copyright (c) 2021 Jesse Haviland
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,32 +32,34 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: collision
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Spatial Geometry
 
+[![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
+[![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+
 [![PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://badge.fury.io/py/spatialgeometry)
 [![Anaconda version](https://anaconda.org/conda-forge/spatialgeometry/badges/version.svg)](https://anaconda.org/conda-forge/spatialgeometry)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spatialgeometry.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![Build Status](https://github.com/jhavl/spatialgeometry/workflows/build/badge.svg?branch=main)](https://github.com/jhavl/spatialgeometry/actions?query=workflow%3Abuild)
 [![codecov](https://codecov.io/gh/jhavl/spatialgeometry/branch/main/graph/badge.svg?token=YPmchbQi2v)](https://codecov.io/gh/jhavl/spatialgeometry)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jhavl/spatialgeometry.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jhavl/spatialgeometry/context:python)
 
 <table style="border:0px">
 <tr style="border:0px">
 <td style="border:0px">
 <img src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="200"></td>
 <td style="border:0px">
 A Python Shape and Geometry Package
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialgeometry Version: 1.0.3 Summary: A Shape and
+Metadata-Version: 2.1 Name: spatialgeometry Version: 1.1.0 Summary: A Shape and
 Geometry Description Package Author-email: Jesse Haviland
 haviland@qut.edu.au>, Peter Corke
 petercorke.com> License: MIT License Copyright (c) 2021 Jesse Haviland
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -21,28 +21,29 @@
 spatialgeometry Keywords: python,robotics,robotics-
 toolbox,kinematics,dynamics,motion-planning,trajectory-
 generation,jacobian,hessian,control,simulation,robot-manipulator,mobile-robot
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: collision Provides-
-Extra: dev Provides-Extra: docs License-File: LICENSE # Spatial Geometry [!
-[PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: collision Provides-Extra: dev Provides-Extra:
+docs License-File: LICENSE # Spatial Geometry [![A Python Robotics Package]
+(https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
+master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
+robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
+github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+[![PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://
 badge.fury.io/py/spatialgeometry) [![Anaconda version](https://anaconda.org/
 conda-forge/spatialgeometry/badges/version.svg)](https://anaconda.org/conda-
 forge/spatialgeometry) ![PyPI - Python Version](https://img.shields.io/pypi/
 pyversions/spatialgeometry.svg) [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![QUT Centre for
-Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/
-badge.svg)](https://qcr.github.io) [![Build Status](https://github.com/jhavl/
-spatialgeometry/workflows/build/badge.svg?branch=main)](https://github.com/
-jhavl/spatialgeometry/actions?query=workflow%3Abuild) [![codecov](https://
-codecov.io/gh/jhavl/spatialgeometry/branch/main/graph/
-badge.svg?token=YPmchbQi2v)](https://codecov.io/gh/jhavl/spatialgeometry) [!
-[Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jhavl/
-spatialgeometry.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jhavl/
-spatialgeometry/context:python)
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status]
+(https://github.com/jhavl/spatialgeometry/workflows/build/
+badge.svg?branch=main)](https://github.com/jhavl/spatialgeometry/
+actions?query=workflow%3Abuild) [![codecov](https://codecov.io/gh/jhavl/
+spatialgeometry/branch/main/graph/badge.svg?token=YPmchbQi2v)](https://
+codecov.io/gh/jhavl/spatialgeometry)
 [https://github.com/petercorke/robotics- A Python Shape and Geometry Package
 toolbox-python/raw/master/docs/figs/         * GitHub_repository
 RobToolBox_RoundLogoB.png]                   * Documentation
```

### Comparing `spatialgeometry-1.0.3/pyproject.toml` & `spatialgeometry-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 [project]
 
 name = "spatialgeometry"
 
 description = "A Shape and Geometry Description Package"
 
-version = "1.0.3"
+version = "1.1.0"
 
 authors = [
     { name = "Jesse Haviland", email = "j.haviland@qut.edu.au" },
     { name = "Peter Corke", email = "rvc@petercorke.com" },
 ]
 
-dependencies = [
-    "spatialmath-python~=1.0.0",
-]
+dependencies = ["spatialmath-python>=1.0.0"]
+
 
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 
 readme = "README.md"
 
 requires-python = ">=3.7"
 
-keywords = ["python", "robotics", "robotics-toolbox", "kinematics", "dynamics", "motion-planning", "trajectory-generation", "jacobian", "hessian", "control", "simulation", "robot-manipulator", "mobile-robot"]
+keywords = [
+    "python",
+    "robotics",
+    "robotics-toolbox",
+    "kinematics",
+    "dynamics",
+    "motion-planning",
+    "trajectory-generation",
+    "jacobian",
+    "hessian",
+    "control",
+    "simulation",
+    "robot-manipulator",
+    "mobile-robot",
+]
 
 classifiers = [
-        "Development Status :: 5 - Production/Stable",
-        # Indicate who your project is intended for
-        "Intended Audience :: Developers",
-        # Pick your license as you wish (should match "license" above)
-        "License :: OSI Approved :: MIT License",
-        # Specify the Python versions you support here.
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
+    "Development Status :: 5 - Production/Stable",
+    # Indicate who your project is intended for
+    "Intended Audience :: Developers",
+    # Pick your license as you wish (should match "license" above)
+    "License :: OSI Approved :: MIT License",
+    # Specify the Python versions you support here.
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 
 [project.urls]
 homepage = "https://github.com/jhavl/spatialgeometry"
 documentation = "https://jhavl.github.io/spatialgeometry/"
 repository = "https://github.com/jhavl/spatialgeometry"
 
 
-
 [project.optional-dependencies]
 
-collision = [
-    "pybullet"
-]
+collision = ["pybullet"]
 
 dev = [
     "black",
     "roboticstoolbox-python~=1.0.0",
     "swift-sim",
     "pytest",
     "pytest-cov",
     "flake8",
     "pyyaml",
 ]
 
-docs = [
-    "sphinx",
-    "sphinx_rtd_theme",
-    "sphinx-autorun", 
-]
-
+docs = ["sphinx", "sphinx_rtd_theme", "sphinx-autorun"]
 
 
 [build-system]
 
 requires = [
     "setuptools",
-    "oldest-supported-numpy"
+    "oldest-supported-numpy",
     # "numpy == 1.17.4",
 ]
 build-backend = "setuptools.build_meta"
 
 
-
 [tool.setuptools]
 
 packages = ["spatialgeometry", "spatialgeometry.geom", "spatialgeometry.tools"]
 
 
-
 [tool.black]
 
 line-length = 88
 target_version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 
@@ -107,15 +111,14 @@
     | dist
     | docs
   )/
 )
 '''
 
 
-
 [tool.flake8]
 
 max-line-length = 88
 extend-ignore = 'E203'
 
 
 [tool.cibuildwheel]
@@ -146,10 +149,7 @@
 # On an Linux Intel runner with qemu installed, build Intel and ARM wheels
 archs = ["x86_64", "aarch64"]
 
 [tool.cibuildwheel.windows]
 
 # On an Windows Intel runner build wheels
 archs = ["AMD64", "x86"]
-
-
-
```

### Comparing `spatialgeometry-1.0.3/setup.py` & `spatialgeometry-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Cholesky` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/CholmodSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Core` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Core`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Eigenvalues` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Geometry` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Householder` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/IterativeLinearSolvers` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Jacobi` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/KLUSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/LU` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/LU`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/MetisSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/OrderingMethods` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/PaStiXSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/PardisoSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/QR` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/QR`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/QtAlignedMalloc` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SPQRSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SVD` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/Sparse` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseCholesky` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseCore` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseLU` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SparseQR` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdDeque` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdList` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/StdVector` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/SuperLUSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/UmfPackSupport` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LDLT.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LLT.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Cholesky/LLT_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/CholmodSupport/CholmodSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArithmeticSequence.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Array.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArrayBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ArrayWrapper.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Assign.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/AssignEvaluator.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Assign_MKL.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/BandMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Block.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/BooleanRedux.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CommaInitializer.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ConditionEstimator.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CoreEvaluators.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CoreIterators.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseBinaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseNullaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseTernaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseUnaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/CwiseUnaryView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseCoeffsBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DenseStorage.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Diagonal.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DiagonalMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/DiagonalProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Dot.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/EigenBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ForceAlignedAccess.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Fuzzy.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GeneralProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GenericPacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/GlobalFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/IO.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/IndexedView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Inverse.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Map.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MapBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MathFunctionsImpl.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Matrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/MatrixBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NestByValue.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NoAlias.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/NumTraits.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PartialReduxEvaluator.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PermutationMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/PlainObjectBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Product.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ProductEvaluators.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Random.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Redux.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Ref.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Replicate.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Reshaped.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/ReturnByValue.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Reverse.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Select.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SelfAdjointView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SelfCwiseBinaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Solve.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SolveTriangular.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/SolverBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/StableNorm.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/StlIterators.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Stride.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Swap.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Transpose.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Transpositions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/TriangularMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/VectorBlock.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/VectorwiseOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/Visitor.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/CUDA/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/BFloat16.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/ConjHelper.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/Half.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/Settings.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/Default/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/GPU/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/MSA/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/NEON/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SSE/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SVE/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/Complex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/arch/ZVector/PacketMath.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/AssignmentFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/BinaryFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/NullaryFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/StlFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/TernaryFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/functors/UnaryFunctors.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/Parallelizer.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/SelfadjointRank2Update.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/BlasUtil.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ConfigureVectorization.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Constants.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/DisableStupidWarnings.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ForwardDeclarations.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/IndexedViewHelper.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/IntegralConstant.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/MKL_support.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Macros.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Memory.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/Meta.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ReenableStupidWarnings.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/ReshapedHelper.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/StaticAssert.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/SymbolicIndex.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Core/util/XprHelper.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/EigenSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealQZ.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Eigenvalues/Tridiagonalization.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/AlignedBox.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/AngleAxis.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/EulerAngles.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Homogeneous.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Hyperplane.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/OrthoMethods.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/ParametrizedLine.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Quaternion.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Rotation2D.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/RotationBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Scaling.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Transform.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Translation.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/Umeyama.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/BlockHouseholder.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/Householder.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Householder/HouseholderSequence.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/Jacobi/Jacobi.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/KLUSupport/KLUSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/Determinant.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/FullPivLU.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/InverseImpl.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/PartialPivLU.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/LU/arch/InverseSize4.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/MetisSupport/MetisSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Amd.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/OrderingMethods/Ordering.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/PardisoSupport/PardisoSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/FullPivHouseholderQR.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/HouseholderQR.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/BDCSVD.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/JacobiSVD.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/SVDBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SVD/UpperBidiagonalization.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/AmbiVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/CompressedStorage.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/MappedSparseMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseAssign.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseBlock.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseColEtree.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCompressedBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDenseProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseDot.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseFuzzy.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMap.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrixBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparsePermutation.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseProduct.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseRedux.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseRef.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSolverBase.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseTranspose.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseTriangularView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseUtil.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/SparseView.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseCore/TriangularSolver.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLUImpl.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Memory.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Structs.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Utils.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pivotL.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pruneL.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SparseQR/SparseQR.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdDeque.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdList.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/StdVector.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/StlSupport/details.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/Image.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/Kernel.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/RealSvd2x2.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/blas.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/lapack.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/misc/lapacke.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/BlockMethods.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/IndexedViewMethods.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/Eigen/src/plugins/ReshapedMethods.h` & `spatialgeometry-1.1.0/spatialgeometry/core/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/linalg.h` & `spatialgeometry-1.1.0/spatialgeometry/core/linalg.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/scene.cpp` & `spatialgeometry-1.1.0/spatialgeometry/core/scene.cpp`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/core/scene.h` & `spatialgeometry-1.1.0/spatialgeometry/core/scene.h`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/geom/CollisionShape.py` & `spatialgeometry-1.1.0/spatialgeometry/geom/CollisionShape.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 
         self._update_pyb()
 
         if not shape.pinit:
             shape._init_pob()
             shape._update_pyb()
 
+        shape._update_pyb()
+
         ret = p.getClosestPoints(self.co, shape.co, inf_dist)  # type: ignore
 
         try:
             return ret[0][8], np.array(ret[0][5]), np.array(ret[0][6])
         except ValueError:
             return None, None, None
         except IndexError:
```

### Comparing `spatialgeometry-1.0.3/spatialgeometry/geom/SceneGroup.py` & `spatialgeometry-1.1.0/spatialgeometry/geom/SceneGroup.py`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/geom/SceneNode.py` & `spatialgeometry-1.1.0/spatialgeometry/geom/SceneNode.py`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/geom/Shape.py` & `spatialgeometry-1.1.0/spatialgeometry/geom/Shape.py`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry/tools/stdout_supress.py` & `spatialgeometry-1.1.0/spatialgeometry/tools/stdout_supress.py`

 * *Files identical despite different names*

### Comparing `spatialgeometry-1.0.3/spatialgeometry.egg-info/PKG-INFO` & `spatialgeometry-1.1.0/spatialgeometry.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialgeometry
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Shape and Geometry Description Package
 Author-email: Jesse Haviland <j.haviland@qut.edu.au>, Peter Corke <rvc@petercorke.com>
 License: MIT License
         
         Copyright (c) 2021 Jesse Haviland
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,32 +32,34 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: collision
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Spatial Geometry
 
+[![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
+[![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+
 [![PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://badge.fury.io/py/spatialgeometry)
 [![Anaconda version](https://anaconda.org/conda-forge/spatialgeometry/badges/version.svg)](https://anaconda.org/conda-forge/spatialgeometry)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spatialgeometry.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![Build Status](https://github.com/jhavl/spatialgeometry/workflows/build/badge.svg?branch=main)](https://github.com/jhavl/spatialgeometry/actions?query=workflow%3Abuild)
 [![codecov](https://codecov.io/gh/jhavl/spatialgeometry/branch/main/graph/badge.svg?token=YPmchbQi2v)](https://codecov.io/gh/jhavl/spatialgeometry)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jhavl/spatialgeometry.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jhavl/spatialgeometry/context:python)
 
 <table style="border:0px">
 <tr style="border:0px">
 <td style="border:0px">
 <img src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="200"></td>
 <td style="border:0px">
 A Python Shape and Geometry Package
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialgeometry Version: 1.0.3 Summary: A Shape and
+Metadata-Version: 2.1 Name: spatialgeometry Version: 1.1.0 Summary: A Shape and
 Geometry Description Package Author-email: Jesse Haviland
 haviland@qut.edu.au>, Peter Corke
 petercorke.com> License: MIT License Copyright (c) 2021 Jesse Haviland
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -21,28 +21,29 @@
 spatialgeometry Keywords: python,robotics,robotics-
 toolbox,kinematics,dynamics,motion-planning,trajectory-
 generation,jacobian,hessian,control,simulation,robot-manipulator,mobile-robot
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: collision Provides-
-Extra: dev Provides-Extra: docs License-File: LICENSE # Spatial Geometry [!
-[PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: collision Provides-Extra: dev Provides-Extra:
+docs License-File: LICENSE # Spatial Geometry [![A Python Robotics Package]
+(https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
+master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
+robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
+github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+[![PyPI version](https://badge.fury.io/py/spatialgeometry.svg)](https://
 badge.fury.io/py/spatialgeometry) [![Anaconda version](https://anaconda.org/
 conda-forge/spatialgeometry/badges/version.svg)](https://anaconda.org/conda-
 forge/spatialgeometry) ![PyPI - Python Version](https://img.shields.io/pypi/
 pyversions/spatialgeometry.svg) [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![QUT Centre for
-Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/
-badge.svg)](https://qcr.github.io) [![Build Status](https://github.com/jhavl/
-spatialgeometry/workflows/build/badge.svg?branch=main)](https://github.com/
-jhavl/spatialgeometry/actions?query=workflow%3Abuild) [![codecov](https://
-codecov.io/gh/jhavl/spatialgeometry/branch/main/graph/
-badge.svg?token=YPmchbQi2v)](https://codecov.io/gh/jhavl/spatialgeometry) [!
-[Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jhavl/
-spatialgeometry.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jhavl/
-spatialgeometry/context:python)
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status]
+(https://github.com/jhavl/spatialgeometry/workflows/build/
+badge.svg?branch=main)](https://github.com/jhavl/spatialgeometry/
+actions?query=workflow%3Abuild) [![codecov](https://codecov.io/gh/jhavl/
+spatialgeometry/branch/main/graph/badge.svg?token=YPmchbQi2v)](https://
+codecov.io/gh/jhavl/spatialgeometry)
 [https://github.com/petercorke/robotics- A Python Shape and Geometry Package
 toolbox-python/raw/master/docs/figs/         * GitHub_repository
 RobToolBox_RoundLogoB.png]                   * Documentation
```

### Comparing `spatialgeometry-1.0.3/spatialgeometry.egg-info/SOURCES.txt` & `spatialgeometry-1.1.0/spatialgeometry.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -351,8 +351,9 @@
 spatialgeometry/core/Eigen/src/plugins/ReshapedMethods.h
 spatialgeometry/geom/CollisionShape.py
 spatialgeometry/geom/SceneGroup.py
 spatialgeometry/geom/SceneNode.py
 spatialgeometry/geom/Shape.py
 spatialgeometry/geom/__init__.py
 spatialgeometry/tools/__init__.py
-spatialgeometry/tools/stdout_supress.py
+spatialgeometry/tools/stdout_supress.py
+tests/test_Shape.py
```

