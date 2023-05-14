# Comparing `tmp/nazo_image_utils-0.0.2.tar.gz` & `tmp/nazo_image_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_image_utils-0.0.2.tar", last modified: Sun May 14 05:59:28 2023, max compression
+gzip compressed data, was "nazo_image_utils-0.0.3.tar", last modified: Sun May 14 09:39:57 2023, max compression
```

## Comparing `nazo_image_utils-0.0.2.tar` & `nazo_image_utils-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/
--rw-rw-rw-   0        0        0      125 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3747 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2839 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/nazo_image_utils/
--rw-rw-rw-   0        0        0      123 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/__init__.py
--rw-rw-rw-   0        0        0     7345 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/process_image.py
--rw-rw-rw-   0        0        0   314004 2023-05-14 05:59:27.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.cpp
--rw-rw-rw-   0        0        0     1319 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyi
--rw-rw-rw-   0        0        0     4651 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyx
-drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/
--rw-rw-rw-   0        0        0     3747 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1640 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:39:57.813816 nazo_image_utils-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      125 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5022 2023-05-14 09:39:57.813816 nazo_image_utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 09:39:57.813816 nazo_image_utils-0.0.3/nazo_image_utils/
+-rw-rw-rw-   0        0        0      123 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/nazo_image_utils/__init__.py
+-rw-rw-rw-   0        0        0     7345 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/nazo_image_utils/process_image.py
+-rw-rw-rw-   0        0        0   315013 2023-05-14 09:39:56.000000 nazo_image_utils-0.0.3/nazo_image_utils/rand_image.cpp
+-rw-rw-rw-   0        0        0     1317 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/nazo_image_utils/rand_image.pyi
+-rw-rw-rw-   0        0        0     4784 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/nazo_image_utils/rand_image.pyx
+drwxrwxrwx   0        0        0        0 2023-05-14 09:39:57.813816 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/
+-rw-rw-rw-   0        0        0     5022 2023-05-14 09:39:57.000000 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-05-14 09:39:57.000000 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 09:39:57.000000 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-14 09:39:57.000000 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-14 09:39:57.000000 nazo_image_utils-0.0.3/nazo_image_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1618 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 09:39:57.813816 nazo_image_utils-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-05-14 09:39:19.000000 nazo_image_utils-0.0.3/setup.py
```

### Comparing `nazo_image_utils-0.0.2/PKG-INFO` & `nazo_image_utils-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: nazo_image_utils
-Version: 0.0.2
-Summary: A tool for generating random images
-Author-email: bymoye <s3moye@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/bymoye/nazo_image_utils
-Project-URL: Bug Tracker, https://github.com/bymoye/nazo_image_utils/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Cython
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Nazo Image Utils
 
 Nazo Image Utils 是一个用于处理随机图像和图像处理的 Python 包。它包含两个类：`RandImage` 和 `ProcessImage`。
 
 ## 安装
 
 您可以使用 pip 安装 Nazo Image Utils：
```

### Comparing `nazo_image_utils-0.0.2/nazo_image_utils/process_image.py` & `nazo_image_utils-0.0.3/nazo_image_utils/process_image.py`

 * *Files identical despite different names*

### Comparing `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.cpp` & `nazo_image_utils-0.0.3/nazo_image_utils/rand_image.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1017,29 +1017,29 @@
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange {
   int __pyx_n;
   int stop;
   int step;
 };
 struct __pyx_opt_args_16nazo_image_utils_10rand_image_9RandImage_process;
 
-/* "nazo_image_utils/rand_image.pyx":59
+/* "nazo_image_utils/rand_image.pyx":60
  *         free(urls)
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):             # <<<<<<<<<<<<<<
  *         """
  *         URL
  */
 struct __pyx_opt_args_16nazo_image_utils_10rand_image_9RandImage_process {
   int __pyx_n;
   PyObject *platform;
   PyObject *encode;
   PyObject *size;
 };
 
-/* "nazo_image_utils/rand_image.pyx":17
+/* "nazo_image_utils/rand_image.pyx":18
  *     const char* MOBILE = b"mobile"
  * 
  * cdef class RandImage:             # <<<<<<<<<<<<<<
  *     cdef:
  *         int imgpc_total, imgmb_total
  */
 struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage {
@@ -1782,83 +1782,83 @@
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
-/* "nazo_image_utils/rand_image.pyx":24
+/* "nazo_image_utils/rand_image.pyx":25
  *         char* domain
  * 
  *     cdef inline char* pc(self) nogil:             # <<<<<<<<<<<<<<
  *         return self.imgpc[cy_random_below(self.imgpc_total)]
  * 
  */
 
 static CYTHON_INLINE char *__pyx_f_16nazo_image_utils_10rand_image_9RandImage_pc(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "nazo_image_utils/rand_image.pyx":25
+  /* "nazo_image_utils/rand_image.pyx":26
  * 
  *     cdef inline char* pc(self) nogil:
  *         return self.imgpc[cy_random_below(self.imgpc_total)]             # <<<<<<<<<<<<<<
  * 
  *     cdef inline char* mobile(self) nogil:
  */
   __pyx_r = (__pyx_v_self->imgpc[__pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_v_self->imgpc_total)]);
   goto __pyx_L0;
 
-  /* "nazo_image_utils/rand_image.pyx":24
+  /* "nazo_image_utils/rand_image.pyx":25
  *         char* domain
  * 
  *     cdef inline char* pc(self) nogil:             # <<<<<<<<<<<<<<
  *         return self.imgpc[cy_random_below(self.imgpc_total)]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "nazo_image_utils/rand_image.pyx":27
+/* "nazo_image_utils/rand_image.pyx":28
  *         return self.imgpc[cy_random_below(self.imgpc_total)]
  * 
  *     cdef inline char* mobile(self) nogil:             # <<<<<<<<<<<<<<
  *         return self.imgmb[cy_random_below(self.imgmb_total)]
  * 
  */
 
 static CYTHON_INLINE char *__pyx_f_16nazo_image_utils_10rand_image_9RandImage_mobile(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "nazo_image_utils/rand_image.pyx":28
+  /* "nazo_image_utils/rand_image.pyx":29
  * 
  *     cdef inline char* mobile(self) nogil:
  *         return self.imgmb[cy_random_below(self.imgmb_total)]             # <<<<<<<<<<<<<<
  * 
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:
  */
   __pyx_r = (__pyx_v_self->imgmb[__pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_v_self->imgmb_total)]);
   goto __pyx_L0;
 
-  /* "nazo_image_utils/rand_image.pyx":27
+  /* "nazo_image_utils/rand_image.pyx":28
  *         return self.imgpc[cy_random_below(self.imgpc_total)]
  * 
  *     cdef inline char* mobile(self) nogil:             # <<<<<<<<<<<<<<
  *         return self.imgmb[cy_random_below(self.imgmb_total)]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "nazo_image_utils/rand_image.pyx":30
+/* "nazo_image_utils/rand_image.pyx":31
  *         return self.imgmb[cy_random_below(self.imgmb_total)]
  * 
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  */
 
@@ -1885,70 +1885,70 @@
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("generate_img_urls", 0);
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 
-  /* "nazo_image_utils/rand_image.pyx":31
+  /* "nazo_image_utils/rand_image.pyx":32
  * 
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:
  *         cdef int i             # <<<<<<<<<<<<<<
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  *         cdef char* _hash
  */
   /*try:*/ {
 
-    /* "nazo_image_utils/rand_image.pyx":32
+    /* "nazo_image_utils/rand_image.pyx":33
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:
  *         cdef int i
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))             # <<<<<<<<<<<<<<
  *         cdef char* _hash
  *         if urls == NULL:
  */
     __pyx_v_urls = ((char **)malloc((__pyx_v_number * (sizeof(char *)))));
 
-    /* "nazo_image_utils/rand_image.pyx":34
+    /* "nazo_image_utils/rand_image.pyx":35
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  *         cdef char* _hash
  *         if urls == NULL:             # <<<<<<<<<<<<<<
  *             with gil:
  *                 raise MemoryError("Failed to allocate memory for URLs array")
  */
     __pyx_t_1 = ((__pyx_v_urls == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "nazo_image_utils/rand_image.pyx":35
+      /* "nazo_image_utils/rand_image.pyx":36
  *         cdef char* _hash
  *         if urls == NULL:
  *             with gil:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("Failed to allocate memory for URLs array")
  * 
  */
       {
           #ifdef WITH_THREAD
           PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
           #endif
           /*try:*/ {
 
-            /* "nazo_image_utils/rand_image.pyx":36
+            /* "nazo_image_utils/rand_image.pyx":37
  *         if urls == NULL:
  *             with gil:
  *                 raise MemoryError("Failed to allocate memory for URLs array")             # <<<<<<<<<<<<<<
  * 
  *         for i in range(number):
  */
-            __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L8_error)
+            __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_Raise(__pyx_t_2, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __PYX_ERR(0, 36, __pyx_L8_error)
+            __PYX_ERR(0, 37, __pyx_L8_error)
           }
 
-          /* "nazo_image_utils/rand_image.pyx":35
+          /* "nazo_image_utils/rand_image.pyx":36
  *         cdef char* _hash
  *         if urls == NULL:
  *             with gil:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("Failed to allocate memory for URLs array")
  * 
  */
           /*finally:*/ {
@@ -1957,127 +1957,127 @@
               __Pyx_PyGILState_Release(__pyx_gilstate_save);
               #endif
               goto __pyx_L4_error;
             }
           }
       }
 
-      /* "nazo_image_utils/rand_image.pyx":34
+      /* "nazo_image_utils/rand_image.pyx":35
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  *         cdef char* _hash
  *         if urls == NULL:             # <<<<<<<<<<<<<<
  *             with gil:
  *                 raise MemoryError("Failed to allocate memory for URLs array")
  */
     }
 
-    /* "nazo_image_utils/rand_image.pyx":38
+    /* "nazo_image_utils/rand_image.pyx":39
  *                 raise MemoryError("Failed to allocate memory for URLs array")
  * 
  *         for i in range(number):             # <<<<<<<<<<<<<<
  *             _hash = self.mobile() if strcmp(method, MOBILE) == 0 else self.pc()
  *             urls[i] = <char*>malloc(256 * sizeof(char))
  */
     __pyx_t_3 = __pyx_v_number;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "nazo_image_utils/rand_image.pyx":39
+      /* "nazo_image_utils/rand_image.pyx":40
  * 
  *         for i in range(number):
  *             _hash = self.mobile() if strcmp(method, MOBILE) == 0 else self.pc()             # <<<<<<<<<<<<<<
  *             urls[i] = <char*>malloc(256 * sizeof(char))
  *             if urls[i] == NULL:
  */
       if (((strcmp(__pyx_v_method, __pyx_v_16nazo_image_utils_10rand_image_MOBILE) == 0) != 0)) {
         __pyx_t_6 = __pyx_f_16nazo_image_utils_10rand_image_9RandImage_mobile(__pyx_v_self);
       } else {
         __pyx_t_6 = __pyx_f_16nazo_image_utils_10rand_image_9RandImage_pc(__pyx_v_self);
       }
       __pyx_v__hash = __pyx_t_6;
 
-      /* "nazo_image_utils/rand_image.pyx":40
+      /* "nazo_image_utils/rand_image.pyx":41
  *         for i in range(number):
  *             _hash = self.mobile() if strcmp(method, MOBILE) == 0 else self.pc()
  *             urls[i] = <char*>malloc(256 * sizeof(char))             # <<<<<<<<<<<<<<
  *             if urls[i] == NULL:
  *                 for j in range(i):
  */
       (__pyx_v_urls[__pyx_v_i]) = ((char *)malloc((0x100 * (sizeof(char)))));
 
-      /* "nazo_image_utils/rand_image.pyx":41
+      /* "nazo_image_utils/rand_image.pyx":42
  *             _hash = self.mobile() if strcmp(method, MOBILE) == 0 else self.pc()
  *             urls[i] = <char*>malloc(256 * sizeof(char))
  *             if urls[i] == NULL:             # <<<<<<<<<<<<<<
  *                 for j in range(i):
  *                     free(urls[j])
  */
       __pyx_t_1 = (((__pyx_v_urls[__pyx_v_i]) == NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "nazo_image_utils/rand_image.pyx":42
+        /* "nazo_image_utils/rand_image.pyx":43
  *             urls[i] = <char*>malloc(256 * sizeof(char))
  *             if urls[i] == NULL:
  *                 for j in range(i):             # <<<<<<<<<<<<<<
  *                     free(urls[j])
  *                 free(urls)
  */
         __pyx_t_7 = __pyx_v_i;
         __pyx_t_8 = __pyx_t_7;
         for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
           __pyx_v_j = __pyx_t_9;
 
-          /* "nazo_image_utils/rand_image.pyx":43
+          /* "nazo_image_utils/rand_image.pyx":44
  *             if urls[i] == NULL:
  *                 for j in range(i):
  *                     free(urls[j])             # <<<<<<<<<<<<<<
  *                 free(urls)
  *                 with gil:
  */
           free((__pyx_v_urls[__pyx_v_j]));
         }
 
-        /* "nazo_image_utils/rand_image.pyx":44
+        /* "nazo_image_utils/rand_image.pyx":45
  *                 for j in range(i):
  *                     free(urls[j])
  *                 free(urls)             # <<<<<<<<<<<<<<
  *                 with gil:
  *                     raise MemoryError("Failed to allocate memory for URL string")
  */
         free(__pyx_v_urls);
 
-        /* "nazo_image_utils/rand_image.pyx":45
+        /* "nazo_image_utils/rand_image.pyx":46
  *                     free(urls[j])
  *                 free(urls)
  *                 with gil:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to allocate memory for URL string")
  * 
  */
         {
             #ifdef WITH_THREAD
             PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
             #endif
             /*try:*/ {
 
-              /* "nazo_image_utils/rand_image.pyx":46
+              /* "nazo_image_utils/rand_image.pyx":47
  *                 free(urls)
  *                 with gil:
  *                     raise MemoryError("Failed to allocate memory for URL string")             # <<<<<<<<<<<<<<
  * 
  *             snprintf(urls[i], 256, b"%s/%s/%s.%s.%s", self.domain, img_format, _hash, size, img_format)
  */
-              __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L18_error)
+              __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L18_error)
               __Pyx_GOTREF(__pyx_t_2);
               __Pyx_Raise(__pyx_t_2, 0, 0, 0);
               __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __PYX_ERR(0, 46, __pyx_L18_error)
+              __PYX_ERR(0, 47, __pyx_L18_error)
             }
 
-            /* "nazo_image_utils/rand_image.pyx":45
+            /* "nazo_image_utils/rand_image.pyx":46
  *                     free(urls[j])
  *                 free(urls)
  *                 with gil:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to allocate memory for URL string")
  * 
  */
             /*finally:*/ {
@@ -2086,45 +2086,45 @@
                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                 #endif
                 goto __pyx_L4_error;
               }
             }
         }
 
-        /* "nazo_image_utils/rand_image.pyx":41
+        /* "nazo_image_utils/rand_image.pyx":42
  *             _hash = self.mobile() if strcmp(method, MOBILE) == 0 else self.pc()
  *             urls[i] = <char*>malloc(256 * sizeof(char))
  *             if urls[i] == NULL:             # <<<<<<<<<<<<<<
  *                 for j in range(i):
  *                     free(urls[j])
  */
       }
 
-      /* "nazo_image_utils/rand_image.pyx":48
+      /* "nazo_image_utils/rand_image.pyx":49
  *                     raise MemoryError("Failed to allocate memory for URL string")
  * 
  *             snprintf(urls[i], 256, b"%s/%s/%s.%s.%s", self.domain, img_format, _hash, size, img_format)             # <<<<<<<<<<<<<<
  * 
  *         return urls
  */
       (void)(snprintf((__pyx_v_urls[__pyx_v_i]), 0x100, ((char const *)"%s/%s/%s.%s.%s"), __pyx_v_self->domain, __pyx_v_img_format, __pyx_v__hash, __pyx_v_size, __pyx_v_img_format));
     }
 
-    /* "nazo_image_utils/rand_image.pyx":50
+    /* "nazo_image_utils/rand_image.pyx":51
  *             snprintf(urls[i], 256, b"%s/%s/%s.%s.%s", self.domain, img_format, _hash, size, img_format)
  * 
  *         return urls             # <<<<<<<<<<<<<<
  * 
  *     cdef inline void _free_urls(self,char **urls, int n) nogil:
  */
     __pyx_r = __pyx_v_urls;
     goto __pyx_L3_return;
   }
 
-  /* "nazo_image_utils/rand_image.pyx":31
+  /* "nazo_image_utils/rand_image.pyx":32
  * 
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:
  *         cdef int i             # <<<<<<<<<<<<<<
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  *         cdef char* _hash
  */
   /*finally:*/ {
@@ -2138,15 +2138,15 @@
       #ifdef WITH_THREAD
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L1_error;
     }
   }
 
-  /* "nazo_image_utils/rand_image.pyx":30
+  /* "nazo_image_utils/rand_image.pyx":31
  *         return self.imgmb[cy_random_below(self.imgmb_total)]
  * 
  *     cdef char** generate_img_urls(self, int number,const char* img_format, const char* method, const char* size) nogil:             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef char** urls = <char**>malloc(number * sizeof(char*))
  */
 
@@ -2160,91 +2160,91 @@
   __pyx_L0:;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "nazo_image_utils/rand_image.pyx":52
+/* "nazo_image_utils/rand_image.pyx":53
  *         return urls
  * 
  *     cdef inline void _free_urls(self,char **urls, int n) nogil:             # <<<<<<<<<<<<<<
  *         cdef int i
  *         for i in range(n):
  */
 
 static CYTHON_INLINE void __pyx_f_16nazo_image_utils_10rand_image_9RandImage__free_urls(CYTHON_UNUSED struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *__pyx_v_self, char **__pyx_v_urls, int __pyx_v_n) {
   int __pyx_v_i;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "nazo_image_utils/rand_image.pyx":54
+  /* "nazo_image_utils/rand_image.pyx":55
  *     cdef inline void _free_urls(self,char **urls, int n) nogil:
  *         cdef int i
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             if urls[i] != NULL:
  *                 free(urls[i])
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "nazo_image_utils/rand_image.pyx":55
+    /* "nazo_image_utils/rand_image.pyx":56
  *         cdef int i
  *         for i in range(n):
  *             if urls[i] != NULL:             # <<<<<<<<<<<<<<
  *                 free(urls[i])
  *         free(urls)
  */
     __pyx_t_4 = (((__pyx_v_urls[__pyx_v_i]) != NULL) != 0);
     if (__pyx_t_4) {
 
-      /* "nazo_image_utils/rand_image.pyx":56
+      /* "nazo_image_utils/rand_image.pyx":57
  *         for i in range(n):
  *             if urls[i] != NULL:
  *                 free(urls[i])             # <<<<<<<<<<<<<<
  *         free(urls)
  * 
  */
       free((__pyx_v_urls[__pyx_v_i]));
 
-      /* "nazo_image_utils/rand_image.pyx":55
+      /* "nazo_image_utils/rand_image.pyx":56
  *         cdef int i
  *         for i in range(n):
  *             if urls[i] != NULL:             # <<<<<<<<<<<<<<
  *                 free(urls[i])
  *         free(urls)
  */
     }
   }
 
-  /* "nazo_image_utils/rand_image.pyx":57
+  /* "nazo_image_utils/rand_image.pyx":58
  *             if urls[i] != NULL:
  *                 free(urls[i])
  *         free(urls)             # <<<<<<<<<<<<<<
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):
  */
   free(__pyx_v_urls);
 
-  /* "nazo_image_utils/rand_image.pyx":52
+  /* "nazo_image_utils/rand_image.pyx":53
  *         return urls
  * 
  *     cdef inline void _free_urls(self,char **urls, int n) nogil:             # <<<<<<<<<<<<<<
  *         cdef int i
  *         for i in range(n):
  */
 
   /* function exit code */
 }
 
-/* "nazo_image_utils/rand_image.pyx":59
+/* "nazo_image_utils/rand_image.pyx":60
  *         free(urls)
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):             # <<<<<<<<<<<<<<
  *         """
  *         URL
  */
 
@@ -2298,19 +2298,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_16nazo_image_utils_10rand_image_9RandImage_1process)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_number); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_number); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         __pyx_t_6 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
@@ -2320,31 +2320,31 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_6 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[6] = {__pyx_t_5, __pyx_v_ua, __pyx_t_3, __pyx_v_platform, __pyx_v_encode, __pyx_v_size};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[6] = {__pyx_t_5, __pyx_v_ua, __pyx_t_3, __pyx_v_platform, __pyx_v_encode, __pyx_v_size};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         {
-          __pyx_t_7 = PyTuple_New(5+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_New(5+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           if (__pyx_t_5) {
             __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
           }
           __Pyx_INCREF(__pyx_v_ua);
           __Pyx_GIVEREF(__pyx_v_ua);
           PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_ua);
@@ -2356,15 +2356,15 @@
           __Pyx_INCREF(__pyx_v_encode);
           __Pyx_GIVEREF(__pyx_v_encode);
           PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_6, __pyx_v_encode);
           __Pyx_INCREF(__pyx_v_size);
           __Pyx_GIVEREF(__pyx_v_size);
           PyTuple_SET_ITEM(__pyx_t_7, 4+__pyx_t_6, __pyx_v_size);
           __pyx_t_3 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -2379,40 +2379,40 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "nazo_image_utils/rand_image.pyx":70
+  /* "nazo_image_utils/rand_image.pyx":71
  *         """
  *         cdef const char* img_format
  *         img_format = URLWEBP if webp_supported(ua) else URLJPEG             # <<<<<<<<<<<<<<
  *         cdef int i
  *         if encode == b"json":
  */
   if ((__pyx_f_12webp_support_12webp_support_webp_supported(__pyx_v_ua, 0) != 0)) {
     __pyx_t_8 = __pyx_v_16nazo_image_utils_10rand_image_URLWEBP;
   } else {
     __pyx_t_8 = __pyx_v_16nazo_image_utils_10rand_image_URLJPEG;
   }
   __pyx_v_img_format = __pyx_t_8;
 
-  /* "nazo_image_utils/rand_image.pyx":72
+  /* "nazo_image_utils/rand_image.pyx":73
  *         img_format = URLWEBP if webp_supported(ua) else URLJPEG
  *         cdef int i
  *         if encode == b"json":             # <<<<<<<<<<<<<<
  *             number = min(max(number, 1), 10)
  *         else:
  */
-  __pyx_t_9 = (__Pyx_PyBytes_Equals(__pyx_v_encode, __pyx_n_b_json, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_9 = (__Pyx_PyBytes_Equals(__pyx_v_encode, __pyx_n_b_json, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_t_10 = (__pyx_t_9 != 0);
   if (__pyx_t_10) {
 
-    /* "nazo_image_utils/rand_image.pyx":73
+    /* "nazo_image_utils/rand_image.pyx":74
  *         cdef int i
  *         if encode == b"json":
  *             number = min(max(number, 1), 10)             # <<<<<<<<<<<<<<
  *         else:
  *             number = 1
  */
     __pyx_t_11 = 10;
@@ -2427,154 +2427,154 @@
     if (((__pyx_t_11 < __pyx_t_12) != 0)) {
       __pyx_t_13 = __pyx_t_11;
     } else {
       __pyx_t_13 = __pyx_t_12;
     }
     __pyx_v_number = __pyx_t_13;
 
-    /* "nazo_image_utils/rand_image.pyx":72
+    /* "nazo_image_utils/rand_image.pyx":73
  *         img_format = URLWEBP if webp_supported(ua) else URLJPEG
  *         cdef int i
  *         if encode == b"json":             # <<<<<<<<<<<<<<
  *             number = min(max(number, 1), 10)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "nazo_image_utils/rand_image.pyx":75
+  /* "nazo_image_utils/rand_image.pyx":76
  *             number = min(max(number, 1), 10)
  *         else:
  *             number = 1             # <<<<<<<<<<<<<<
  *         cdef char** urls = self.generate_img_urls(number, img_format, platform, size)
  *         # urls1
  */
   /*else*/ {
     __pyx_v_number = 1;
   }
   __pyx_L3:;
 
-  /* "nazo_image_utils/rand_image.pyx":76
+  /* "nazo_image_utils/rand_image.pyx":77
  *         else:
  *             number = 1
  *         cdef char** urls = self.generate_img_urls(number, img_format, platform, size)             # <<<<<<<<<<<<<<
  *         # urls1
  *         if encode != b"json":
  */
   if (unlikely(__pyx_v_platform == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 76, __pyx_L1_error)
+    __PYX_ERR(0, 77, __pyx_L1_error)
   }
-  __pyx_t_14 = __Pyx_PyBytes_AsString(__pyx_v_platform); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyBytes_AsString(__pyx_v_platform); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
   if (unlikely(__pyx_v_size == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 76, __pyx_L1_error)
+    __PYX_ERR(0, 77, __pyx_L1_error)
   }
-  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_size); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_size); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
   __pyx_v_urls = ((struct __pyx_vtabstruct_16nazo_image_utils_10rand_image_RandImage *)__pyx_v_self->__pyx_vtab)->generate_img_urls(__pyx_v_self, __pyx_v_number, __pyx_v_img_format, __pyx_t_14, __pyx_t_15);
 
-  /* "nazo_image_utils/rand_image.pyx":78
+  /* "nazo_image_utils/rand_image.pyx":79
  *         cdef char** urls = self.generate_img_urls(number, img_format, platform, size)
  *         # urls1
  *         if encode != b"json":             # <<<<<<<<<<<<<<
  *             py_url = PyBytes_FromString(urls[0])
  *             self._free_urls(urls, number)
  */
-  __pyx_t_10 = (__Pyx_PyBytes_Equals(__pyx_v_encode, __pyx_n_b_json, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_10 = (__Pyx_PyBytes_Equals(__pyx_v_encode, __pyx_n_b_json, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 79, __pyx_L1_error)
   __pyx_t_9 = (__pyx_t_10 != 0);
   if (__pyx_t_9) {
 
-    /* "nazo_image_utils/rand_image.pyx":79
+    /* "nazo_image_utils/rand_image.pyx":80
  *         # urls1
  *         if encode != b"json":
  *             py_url = PyBytes_FromString(urls[0])             # <<<<<<<<<<<<<<
  *             self._free_urls(urls, number)
  *             return py_url
  */
-    __pyx_t_1 = PyBytes_FromString((__pyx_v_urls[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_1 = PyBytes_FromString((__pyx_v_urls[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_py_url = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "nazo_image_utils/rand_image.pyx":80
+    /* "nazo_image_utils/rand_image.pyx":81
  *         if encode != b"json":
  *             py_url = PyBytes_FromString(urls[0])
  *             self._free_urls(urls, number)             # <<<<<<<<<<<<<<
  *             return py_url
  * 
  */
     __pyx_f_16nazo_image_utils_10rand_image_9RandImage__free_urls(__pyx_v_self, __pyx_v_urls, __pyx_v_number);
 
-    /* "nazo_image_utils/rand_image.pyx":81
+    /* "nazo_image_utils/rand_image.pyx":82
  *             py_url = PyBytes_FromString(urls[0])
  *             self._free_urls(urls, number)
  *             return py_url             # <<<<<<<<<<<<<<
  * 
  *         py_urls = [urls[i].decode('utf-8') for i in range(number)]
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_py_url);
     __pyx_r = __pyx_v_py_url;
     goto __pyx_L0;
 
-    /* "nazo_image_utils/rand_image.pyx":78
+    /* "nazo_image_utils/rand_image.pyx":79
  *         cdef char** urls = self.generate_img_urls(number, img_format, platform, size)
  *         # urls1
  *         if encode != b"json":             # <<<<<<<<<<<<<<
  *             py_url = PyBytes_FromString(urls[0])
  *             self._free_urls(urls, number)
  */
   }
 
-  /* "nazo_image_utils/rand_image.pyx":83
+  /* "nazo_image_utils/rand_image.pyx":84
  *             return py_url
  * 
  *         py_urls = [urls[i].decode('utf-8') for i in range(number)]             # <<<<<<<<<<<<<<
  * 
  *         #
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = __pyx_v_number;
     __pyx_t_16 = __pyx_t_6;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_7genexpr__pyx_v_i = __pyx_t_17;
       __pyx_t_18 = (__pyx_v_urls[__pyx_7genexpr__pyx_v_i]);
-      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 83, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 84, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
   } /* exit inner scope */
   __pyx_v_py_urls = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "nazo_image_utils/rand_image.pyx":86
+  /* "nazo_image_utils/rand_image.pyx":87
  * 
  *         #
  *         self._free_urls(urls, number)             # <<<<<<<<<<<<<<
  * 
  *         return py_urls
  */
   __pyx_f_16nazo_image_utils_10rand_image_9RandImage__free_urls(__pyx_v_self, __pyx_v_urls, __pyx_v_number);
 
-  /* "nazo_image_utils/rand_image.pyx":88
+  /* "nazo_image_utils/rand_image.pyx":89
  *         self._free_urls(urls, number)
  * 
  *         return py_urls             # <<<<<<<<<<<<<<
  * 
- *     def __cinit__(self, str pc_json_file, str mobile_json_file, bytes domain):
+ *     def __cinit__(self, str pc_json_file, str mobile_json_file, str domain):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_py_urls);
   __pyx_r = __pyx_v_py_urls;
   goto __pyx_L0;
 
-  /* "nazo_image_utils/rand_image.pyx":59
+  /* "nazo_image_utils/rand_image.pyx":60
  *         free(urls)
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):             # <<<<<<<<<<<<<<
  *         """
  *         URL
  */
 
@@ -2640,15 +2640,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ua)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_number)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("process", 0, 2, 5, 1); __PYX_ERR(0, 59, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("process", 0, 2, 5, 1); __PYX_ERR(0, 60, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_platform);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -2662,15 +2662,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "process") < 0)) __PYX_ERR(0, 59, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "process") < 0)) __PYX_ERR(0, 60, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -2679,31 +2679,31 @@
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_ua = ((PyObject*)values[0]);
-    __pyx_v_number = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_number == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L3_error)
+    __pyx_v_number = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_number == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
     __pyx_v_platform = ((PyObject*)values[2]);
     __pyx_v_encode = ((PyObject*)values[3]);
     __pyx_v_size = ((PyObject*)values[4]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("process", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 59, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("process", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 60, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_image_utils.rand_image.RandImage.process", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ua), (&PyBytes_Type), 1, "ua", 1))) __PYX_ERR(0, 59, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_platform), (&PyBytes_Type), 1, "platform", 1))) __PYX_ERR(0, 59, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encode), (&PyBytes_Type), 1, "encode", 1))) __PYX_ERR(0, 59, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_size), (&PyBytes_Type), 1, "size", 1))) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ua), (&PyBytes_Type), 1, "ua", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_platform), (&PyBytes_Type), 1, "platform", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encode), (&PyBytes_Type), 1, "encode", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_size), (&PyBytes_Type), 1, "size", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_r = __pyx_pf_16nazo_image_utils_10rand_image_9RandImage_process(((struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *)__pyx_v_self), __pyx_v_ua, __pyx_v_number, __pyx_v_platform, __pyx_v_encode, __pyx_v_size);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2721,15 +2721,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 3;
   __pyx_t_2.platform = __pyx_v_platform;
   __pyx_t_2.encode = __pyx_v_encode;
   __pyx_t_2.size = __pyx_v_size;
-  __pyx_t_1 = __pyx_vtabptr_16nazo_image_utils_10rand_image_RandImage->process(__pyx_v_self, __pyx_v_ua, __pyx_v_number, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_16nazo_image_utils_10rand_image_RandImage->process(__pyx_v_self, __pyx_v_ua, __pyx_v_number, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2738,18 +2738,18 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_image_utils/rand_image.pyx":90
+/* "nazo_image_utils/rand_image.pyx":91
  *         return py_urls
  * 
- *     def __cinit__(self, str pc_json_file, str mobile_json_file, bytes domain):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, str pc_json_file, str mobile_json_file, str domain):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i
  */
 
 /* Python wrapper */
 static int __pyx_pw_16nazo_image_utils_10rand_image_9RandImage_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_16nazo_image_utils_10rand_image_9RandImage_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -2783,48 +2783,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pc_json_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mobile_json_file)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 91, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_domain)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 91, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_pc_json_file = ((PyObject*)values[0]);
     __pyx_v_mobile_json_file = ((PyObject*)values[1]);
     __pyx_v_domain = ((PyObject*)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 91, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_image_utils.rand_image.RandImage.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pc_json_file), (&PyUnicode_Type), 1, "pc_json_file", 1))) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mobile_json_file), (&PyUnicode_Type), 1, "mobile_json_file", 1))) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_domain), (&PyBytes_Type), 1, "domain", 1))) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pc_json_file), (&PyUnicode_Type), 1, "pc_json_file", 1))) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mobile_json_file), (&PyUnicode_Type), 1, "mobile_json_file", 1))) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_domain), (&PyUnicode_Type), 1, "domain", 1))) __PYX_ERR(0, 91, __pyx_L1_error)
   __pyx_r = __pyx_pf_16nazo_image_utils_10rand_image_9RandImage_2__cinit__(((struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *)__pyx_v_self), __pyx_v_pc_json_file, __pyx_v_mobile_json_file, __pyx_v_domain);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -2855,47 +2855,47 @@
   int __pyx_t_12;
   int __pyx_t_13;
   Py_ssize_t __pyx_t_14;
   char const *__pyx_t_15;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_t_17;
   int __pyx_t_18;
-  char *__pyx_t_19;
+  char const *__pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "nazo_image_utils/rand_image.pyx":94
+  /* "nazo_image_utils/rand_image.pyx":95
  *         cdef int i
  *         cdef bytes encoded_key
  *         with open(pc_json_file) as pc:             # <<<<<<<<<<<<<<
  *             temp = json.load(pc)
  *             self.imgpc_total = len(temp)
  */
   /*with:*/ {
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_pc_json_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_pc_json_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L3_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_3;
     __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -2905,139 +2905,139 @@
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __pyx_v_pc = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":95
+          /* "nazo_image_utils/rand_image.pyx":96
  *         cdef bytes encoded_key
  *         with open(pc_json_file) as pc:
  *             temp = json.load(pc)             # <<<<<<<<<<<<<<
  *             self.imgpc_total = len(temp)
  *             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_load); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_load); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_1)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
               __Pyx_INCREF(__pyx_t_1);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_pc) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_pc);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L7_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_v_temp = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":96
+          /* "nazo_image_utils/rand_image.pyx":97
  *         with open(pc_json_file) as pc:
  *             temp = json.load(pc)
  *             self.imgpc_total = len(temp)             # <<<<<<<<<<<<<<
  *             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))
  *             for i, key in enumerate(temp.keys()):
  */
-          __pyx_t_9 = PyObject_Length(__pyx_v_temp); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 96, __pyx_L7_error)
+          __pyx_t_9 = PyObject_Length(__pyx_v_temp); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 97, __pyx_L7_error)
           __pyx_v_self->imgpc_total = __pyx_t_9;
 
-          /* "nazo_image_utils/rand_image.pyx":97
+          /* "nazo_image_utils/rand_image.pyx":98
  *             temp = json.load(pc)
  *             self.imgpc_total = len(temp)
  *             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))             # <<<<<<<<<<<<<<
  *             for i, key in enumerate(temp.keys()):
  *                 encoded_key = key.encode('UTF-8')
  */
           __pyx_v_self->imgpc = ((char **)malloc((__pyx_v_self->imgpc_total * (sizeof(char *)))));
 
-          /* "nazo_image_utils/rand_image.pyx":98
+          /* "nazo_image_utils/rand_image.pyx":99
  *             self.imgpc_total = len(temp)
  *             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))
  *             for i, key in enumerate(temp.keys()):             # <<<<<<<<<<<<<<
  *                 encoded_key = key.encode('UTF-8')
  *                 self.imgpc[i] = <char*>malloc(len(encoded_key) + 1)
  */
           __pyx_t_10 = 0;
           __pyx_t_9 = 0;
           if (unlikely(__pyx_v_temp == Py_None)) {
             PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-            __PYX_ERR(0, 98, __pyx_L7_error)
+            __PYX_ERR(0, 99, __pyx_L7_error)
           }
-          __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_temp, 0, __pyx_n_s_keys, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_temp, 0, __pyx_n_s_keys, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_XDECREF(__pyx_t_4);
           __pyx_t_4 = __pyx_t_3;
           __pyx_t_3 = 0;
           while (1) {
             __pyx_t_13 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_11, &__pyx_t_9, &__pyx_t_3, NULL, NULL, __pyx_t_12);
             if (unlikely(__pyx_t_13 == 0)) break;
-            if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 98, __pyx_L7_error)
+            if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 99, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
-            if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 98, __pyx_L7_error)
+            if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 99, __pyx_L7_error)
             __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_3));
             __pyx_t_3 = 0;
             __pyx_v_i = __pyx_t_10;
             __pyx_t_10 = (__pyx_t_10 + 1);
 
-            /* "nazo_image_utils/rand_image.pyx":99
+            /* "nazo_image_utils/rand_image.pyx":100
  *             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))
  *             for i, key in enumerate(temp.keys()):
  *                 encoded_key = key.encode('UTF-8')             # <<<<<<<<<<<<<<
  *                 self.imgpc[i] = <char*>malloc(len(encoded_key) + 1)
  *                 strcpy(self.imgpc[i], encoded_key)
  */
             if (unlikely(__pyx_v_key == Py_None)) {
               PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-              __PYX_ERR(0, 99, __pyx_L7_error)
+              __PYX_ERR(0, 100, __pyx_L7_error)
             }
-            __pyx_t_3 = PyUnicode_AsUTF8String(__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L7_error)
+            __pyx_t_3 = PyUnicode_AsUTF8String(__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_XDECREF_SET(__pyx_v_encoded_key, ((PyObject*)__pyx_t_3));
             __pyx_t_3 = 0;
 
-            /* "nazo_image_utils/rand_image.pyx":100
+            /* "nazo_image_utils/rand_image.pyx":101
  *             for i, key in enumerate(temp.keys()):
  *                 encoded_key = key.encode('UTF-8')
  *                 self.imgpc[i] = <char*>malloc(len(encoded_key) + 1)             # <<<<<<<<<<<<<<
  *                 strcpy(self.imgpc[i], encoded_key)
  * 
  */
             if (unlikely(__pyx_v_encoded_key == Py_None)) {
               PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-              __PYX_ERR(0, 100, __pyx_L7_error)
+              __PYX_ERR(0, 101, __pyx_L7_error)
             }
-            __pyx_t_14 = PyBytes_GET_SIZE(__pyx_v_encoded_key); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 100, __pyx_L7_error)
+            __pyx_t_14 = PyBytes_GET_SIZE(__pyx_v_encoded_key); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 101, __pyx_L7_error)
             (__pyx_v_self->imgpc[__pyx_v_i]) = ((char *)malloc((__pyx_t_14 + 1)));
 
-            /* "nazo_image_utils/rand_image.pyx":101
+            /* "nazo_image_utils/rand_image.pyx":102
  *                 encoded_key = key.encode('UTF-8')
  *                 self.imgpc[i] = <char*>malloc(len(encoded_key) + 1)
  *                 strcpy(self.imgpc[i], encoded_key)             # <<<<<<<<<<<<<<
  * 
  *         with open(mobile_json_file) as mb:
  */
             if (unlikely(__pyx_v_encoded_key == Py_None)) {
               PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-              __PYX_ERR(0, 101, __pyx_L7_error)
+              __PYX_ERR(0, 102, __pyx_L7_error)
             }
-            __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L7_error)
+            __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L7_error)
             (void)(strcpy((__pyx_v_self->imgpc[__pyx_v_i]), __pyx_t_15));
           }
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":94
+          /* "nazo_image_utils/rand_image.pyx":95
  *         cdef int i
  *         cdef bytes encoded_key
  *         with open(pc_json_file) as pc:             # <<<<<<<<<<<<<<
  *             temp = json.load(pc)
  *             self.imgpc_total = len(temp)
  */
         }
@@ -3048,36 +3048,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("nazo_image_utils.rand_image.RandImage.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 95, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 95, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          if (__pyx_t_17 < 0) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (__pyx_t_17 < 0) __PYX_ERR(0, 95, __pyx_L9_except_error)
           __pyx_t_18 = ((!(__pyx_t_17 != 0)) != 0);
           if (__pyx_t_18) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_3, __pyx_t_1);
             __pyx_t_4 = 0; __pyx_t_3 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 94, __pyx_L9_except_error)
+            __PYX_ERR(0, 95, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -3095,56 +3095,56 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_2) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 95, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L18;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L1_error;
     __pyx_L18:;
   }
 
-  /* "nazo_image_utils/rand_image.pyx":103
+  /* "nazo_image_utils/rand_image.pyx":104
  *                 strcpy(self.imgpc[i], encoded_key)
  * 
  *         with open(mobile_json_file) as mb:             # <<<<<<<<<<<<<<
  *                     temp = json.load(mb)
  *                     self.imgmb_total = len(temp)
  */
   /*with:*/ {
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_mobile_json_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_mobile_json_file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L19_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L19_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L19_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L19_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_3;
     __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -3154,139 +3154,139 @@
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_6);
         /*try:*/ {
           __pyx_v_mb = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":104
+          /* "nazo_image_utils/rand_image.pyx":105
  * 
  *         with open(mobile_json_file) as mb:
  *                     temp = json.load(mb)             # <<<<<<<<<<<<<<
  *                     self.imgmb_total = len(temp)
  *                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L23_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L23_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_load); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L23_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_load); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L23_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_1)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
               __Pyx_INCREF(__pyx_t_1);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_mb) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_mb);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L23_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L23_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF_SET(__pyx_v_temp, __pyx_t_4);
           __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":105
+          /* "nazo_image_utils/rand_image.pyx":106
  *         with open(mobile_json_file) as mb:
  *                     temp = json.load(mb)
  *                     self.imgmb_total = len(temp)             # <<<<<<<<<<<<<<
  *                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))
  *                     for i, key in enumerate(temp.keys()):
  */
-          __pyx_t_11 = PyObject_Length(__pyx_v_temp); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 105, __pyx_L23_error)
+          __pyx_t_11 = PyObject_Length(__pyx_v_temp); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 106, __pyx_L23_error)
           __pyx_v_self->imgmb_total = __pyx_t_11;
 
-          /* "nazo_image_utils/rand_image.pyx":106
+          /* "nazo_image_utils/rand_image.pyx":107
  *                     temp = json.load(mb)
  *                     self.imgmb_total = len(temp)
  *                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))             # <<<<<<<<<<<<<<
  *                     for i, key in enumerate(temp.keys()):
  *                         encoded_key = key.encode('UTF-8')
  */
           __pyx_v_self->imgmb = ((char **)malloc((__pyx_v_self->imgmb_total * (sizeof(char *)))));
 
-          /* "nazo_image_utils/rand_image.pyx":107
+          /* "nazo_image_utils/rand_image.pyx":108
  *                     self.imgmb_total = len(temp)
  *                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))
  *                     for i, key in enumerate(temp.keys()):             # <<<<<<<<<<<<<<
  *                         encoded_key = key.encode('UTF-8')
  *                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1
  */
           __pyx_t_10 = 0;
           __pyx_t_11 = 0;
           if (unlikely(__pyx_v_temp == Py_None)) {
             PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-            __PYX_ERR(0, 107, __pyx_L23_error)
+            __PYX_ERR(0, 108, __pyx_L23_error)
           }
-          __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_temp, 0, __pyx_n_s_keys, (&__pyx_t_9), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L23_error)
+          __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_temp, 0, __pyx_n_s_keys, (&__pyx_t_9), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L23_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_XDECREF(__pyx_t_4);
           __pyx_t_4 = __pyx_t_3;
           __pyx_t_3 = 0;
           while (1) {
             __pyx_t_13 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_9, &__pyx_t_11, &__pyx_t_3, NULL, NULL, __pyx_t_12);
             if (unlikely(__pyx_t_13 == 0)) break;
-            if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 107, __pyx_L23_error)
+            if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 108, __pyx_L23_error)
             __Pyx_GOTREF(__pyx_t_3);
-            if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 107, __pyx_L23_error)
+            if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 108, __pyx_L23_error)
             __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_3));
             __pyx_t_3 = 0;
             __pyx_v_i = __pyx_t_10;
             __pyx_t_10 = (__pyx_t_10 + 1);
 
-            /* "nazo_image_utils/rand_image.pyx":108
+            /* "nazo_image_utils/rand_image.pyx":109
  *                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))
  *                     for i, key in enumerate(temp.keys()):
  *                         encoded_key = key.encode('UTF-8')             # <<<<<<<<<<<<<<
  *                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1
  *                         strcpy(self.imgmb[i], encoded_key)
  */
             if (unlikely(__pyx_v_key == Py_None)) {
               PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-              __PYX_ERR(0, 108, __pyx_L23_error)
+              __PYX_ERR(0, 109, __pyx_L23_error)
             }
-            __pyx_t_3 = PyUnicode_AsUTF8String(__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L23_error)
+            __pyx_t_3 = PyUnicode_AsUTF8String(__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L23_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_XDECREF_SET(__pyx_v_encoded_key, ((PyObject*)__pyx_t_3));
             __pyx_t_3 = 0;
 
-            /* "nazo_image_utils/rand_image.pyx":109
+            /* "nazo_image_utils/rand_image.pyx":110
  *                     for i, key in enumerate(temp.keys()):
  *                         encoded_key = key.encode('UTF-8')
  *                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1             # <<<<<<<<<<<<<<
  *                         strcpy(self.imgmb[i], encoded_key)
- *         self.domain = domain
+ *         self.domain = strdup(domain.encode('utf-8'))
  */
             if (unlikely(__pyx_v_encoded_key == Py_None)) {
               PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-              __PYX_ERR(0, 109, __pyx_L23_error)
+              __PYX_ERR(0, 110, __pyx_L23_error)
             }
-            __pyx_t_14 = PyBytes_GET_SIZE(__pyx_v_encoded_key); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 109, __pyx_L23_error)
+            __pyx_t_14 = PyBytes_GET_SIZE(__pyx_v_encoded_key); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 110, __pyx_L23_error)
             (__pyx_v_self->imgmb[__pyx_v_i]) = ((char *)malloc((__pyx_t_14 + 1)));
 
-            /* "nazo_image_utils/rand_image.pyx":110
+            /* "nazo_image_utils/rand_image.pyx":111
  *                         encoded_key = key.encode('UTF-8')
  *                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1
  *                         strcpy(self.imgmb[i], encoded_key)             # <<<<<<<<<<<<<<
- *         self.domain = domain
+ *         self.domain = strdup(domain.encode('utf-8'))
  * 
  */
             if (unlikely(__pyx_v_encoded_key == Py_None)) {
               PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-              __PYX_ERR(0, 110, __pyx_L23_error)
+              __PYX_ERR(0, 111, __pyx_L23_error)
             }
-            __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L23_error)
+            __pyx_t_15 = __Pyx_PyBytes_AsString(__pyx_v_encoded_key); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L23_error)
             (void)(strcpy((__pyx_v_self->imgmb[__pyx_v_i]), __pyx_t_15));
           }
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "nazo_image_utils/rand_image.pyx":103
+          /* "nazo_image_utils/rand_image.pyx":104
  *                 strcpy(self.imgpc[i], encoded_key)
  * 
  *         with open(mobile_json_file) as mb:             # <<<<<<<<<<<<<<
  *                     temp = json.load(mb)
  *                     self.imgmb_total = len(temp)
  */
         }
@@ -3297,36 +3297,36 @@
         __pyx_L23_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("nazo_image_utils.rand_image.RandImage.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 103, __pyx_L25_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 104, __pyx_L25_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 103, __pyx_L25_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L25_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 103, __pyx_L25_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 104, __pyx_L25_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          if (__pyx_t_18 < 0) __PYX_ERR(0, 103, __pyx_L25_except_error)
+          if (__pyx_t_18 < 0) __PYX_ERR(0, 104, __pyx_L25_except_error)
           __pyx_t_17 = ((!(__pyx_t_18 != 0)) != 0);
           if (__pyx_t_17) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_3, __pyx_t_1);
             __pyx_t_4 = 0; __pyx_t_3 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 103, __pyx_L25_except_error)
+            __PYX_ERR(0, 104, __pyx_L25_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L24_exception_handled;
         }
         __pyx_L25_except_error:;
@@ -3344,47 +3344,50 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_2) {
           __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 103, __pyx_L1_error)
+          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 104, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         goto __pyx_L22;
       }
       __pyx_L22:;
     }
     goto __pyx_L34;
     __pyx_L19_error:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L1_error;
     __pyx_L34:;
   }
 
-  /* "nazo_image_utils/rand_image.pyx":111
+  /* "nazo_image_utils/rand_image.pyx":112
  *                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1
  *                         strcpy(self.imgmb[i], encoded_key)
- *         self.domain = domain             # <<<<<<<<<<<<<<
+ *         self.domain = strdup(domain.encode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   if (unlikely(__pyx_v_domain == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 111, __pyx_L1_error)
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
+    __PYX_ERR(0, 112, __pyx_L1_error)
   }
-  __pyx_t_19 = __Pyx_PyBytes_AsWritableString(__pyx_v_domain); if (unlikely((!__pyx_t_19) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
-  __pyx_v_self->domain = __pyx_t_19;
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_domain); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_19 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_19) && PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_v_self->domain = strdup(__pyx_t_19);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_image_utils/rand_image.pyx":90
+  /* "nazo_image_utils/rand_image.pyx":91
  *         return py_urls
  * 
- *     def __cinit__(self, str pc_json_file, str mobile_json_file, bytes domain):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, str pc_json_file, str mobile_json_file, str domain):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -3401,16 +3404,16 @@
   __Pyx_XDECREF(__pyx_v_pc);
   __Pyx_XDECREF(__pyx_v_temp);
   __Pyx_XDECREF(__pyx_v_mb);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_image_utils/rand_image.pyx":113
- *         self.domain = domain
+/* "nazo_image_utils/rand_image.pyx":114
+ *         self.domain = strdup(domain.encode('utf-8'))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         if self.imgpc is not NULL:
  */
 
 /* Python wrapper */
@@ -3429,151 +3432,178 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "nazo_image_utils/rand_image.pyx":115
+  /* "nazo_image_utils/rand_image.pyx":116
  *     def __dealloc__(self):
  *         cdef int i
  *         if self.imgpc is not NULL:             # <<<<<<<<<<<<<<
  *             for i in range(self.imgpc_total):
  *                 if self.imgpc[i] is not NULL:
  */
   __pyx_t_1 = ((__pyx_v_self->imgpc != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_image_utils/rand_image.pyx":116
+    /* "nazo_image_utils/rand_image.pyx":117
  *         cdef int i
  *         if self.imgpc is not NULL:
  *             for i in range(self.imgpc_total):             # <<<<<<<<<<<<<<
  *                 if self.imgpc[i] is not NULL:
  *                     free(self.imgpc[i])
  */
     __pyx_t_2 = __pyx_v_self->imgpc_total;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "nazo_image_utils/rand_image.pyx":117
+      /* "nazo_image_utils/rand_image.pyx":118
  *         if self.imgpc is not NULL:
  *             for i in range(self.imgpc_total):
  *                 if self.imgpc[i] is not NULL:             # <<<<<<<<<<<<<<
  *                     free(self.imgpc[i])
  *             free(self.imgpc)
  */
       __pyx_t_1 = (((__pyx_v_self->imgpc[__pyx_v_i]) != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "nazo_image_utils/rand_image.pyx":118
+        /* "nazo_image_utils/rand_image.pyx":119
  *             for i in range(self.imgpc_total):
  *                 if self.imgpc[i] is not NULL:
  *                     free(self.imgpc[i])             # <<<<<<<<<<<<<<
  *             free(self.imgpc)
  * 
  */
         free((__pyx_v_self->imgpc[__pyx_v_i]));
 
-        /* "nazo_image_utils/rand_image.pyx":117
+        /* "nazo_image_utils/rand_image.pyx":118
  *         if self.imgpc is not NULL:
  *             for i in range(self.imgpc_total):
  *                 if self.imgpc[i] is not NULL:             # <<<<<<<<<<<<<<
  *                     free(self.imgpc[i])
  *             free(self.imgpc)
  */
       }
     }
 
-    /* "nazo_image_utils/rand_image.pyx":119
+    /* "nazo_image_utils/rand_image.pyx":120
  *                 if self.imgpc[i] is not NULL:
  *                     free(self.imgpc[i])
  *             free(self.imgpc)             # <<<<<<<<<<<<<<
  * 
  *         if self.imgmb is not NULL:
  */
     free(__pyx_v_self->imgpc);
 
-    /* "nazo_image_utils/rand_image.pyx":115
+    /* "nazo_image_utils/rand_image.pyx":116
  *     def __dealloc__(self):
  *         cdef int i
  *         if self.imgpc is not NULL:             # <<<<<<<<<<<<<<
  *             for i in range(self.imgpc_total):
  *                 if self.imgpc[i] is not NULL:
  */
   }
 
-  /* "nazo_image_utils/rand_image.pyx":121
+  /* "nazo_image_utils/rand_image.pyx":122
  *             free(self.imgpc)
  * 
  *         if self.imgmb is not NULL:             # <<<<<<<<<<<<<<
  *             for i in range(self.imgmb_total):
  *                 if self.imgmb[i] is not NULL:
  */
   __pyx_t_1 = ((__pyx_v_self->imgmb != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_image_utils/rand_image.pyx":122
+    /* "nazo_image_utils/rand_image.pyx":123
  * 
  *         if self.imgmb is not NULL:
  *             for i in range(self.imgmb_total):             # <<<<<<<<<<<<<<
  *                 if self.imgmb[i] is not NULL:
  *                     free(self.imgmb[i])
  */
     __pyx_t_2 = __pyx_v_self->imgmb_total;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "nazo_image_utils/rand_image.pyx":123
+      /* "nazo_image_utils/rand_image.pyx":124
  *         if self.imgmb is not NULL:
  *             for i in range(self.imgmb_total):
  *                 if self.imgmb[i] is not NULL:             # <<<<<<<<<<<<<<
  *                     free(self.imgmb[i])
  *             free(self.imgmb)
  */
       __pyx_t_1 = (((__pyx_v_self->imgmb[__pyx_v_i]) != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "nazo_image_utils/rand_image.pyx":124
+        /* "nazo_image_utils/rand_image.pyx":125
  *             for i in range(self.imgmb_total):
  *                 if self.imgmb[i] is not NULL:
  *                     free(self.imgmb[i])             # <<<<<<<<<<<<<<
  *             free(self.imgmb)
+ * 
  */
         free((__pyx_v_self->imgmb[__pyx_v_i]));
 
-        /* "nazo_image_utils/rand_image.pyx":123
+        /* "nazo_image_utils/rand_image.pyx":124
  *         if self.imgmb is not NULL:
  *             for i in range(self.imgmb_total):
  *                 if self.imgmb[i] is not NULL:             # <<<<<<<<<<<<<<
  *                     free(self.imgmb[i])
  *             free(self.imgmb)
  */
       }
     }
 
-    /* "nazo_image_utils/rand_image.pyx":125
+    /* "nazo_image_utils/rand_image.pyx":126
  *                 if self.imgmb[i] is not NULL:
  *                     free(self.imgmb[i])
  *             free(self.imgmb)             # <<<<<<<<<<<<<<
+ * 
+ *         if self.domain is not NULL:
  */
     free(__pyx_v_self->imgmb);
 
-    /* "nazo_image_utils/rand_image.pyx":121
+    /* "nazo_image_utils/rand_image.pyx":122
  *             free(self.imgpc)
  * 
  *         if self.imgmb is not NULL:             # <<<<<<<<<<<<<<
  *             for i in range(self.imgmb_total):
  *                 if self.imgmb[i] is not NULL:
  */
   }
 
-  /* "nazo_image_utils/rand_image.pyx":113
- *         self.domain = domain
+  /* "nazo_image_utils/rand_image.pyx":128
+ *             free(self.imgmb)
+ * 
+ *         if self.domain is not NULL:             # <<<<<<<<<<<<<<
+ *             free(self.domain)
+ */
+  __pyx_t_1 = ((__pyx_v_self->domain != NULL) != 0);
+  if (__pyx_t_1) {
+
+    /* "nazo_image_utils/rand_image.pyx":129
+ * 
+ *         if self.domain is not NULL:
+ *             free(self.domain)             # <<<<<<<<<<<<<<
+ */
+    free(__pyx_v_self->domain);
+
+    /* "nazo_image_utils/rand_image.pyx":128
+ *             free(self.imgmb)
+ * 
+ *         if self.domain is not NULL:             # <<<<<<<<<<<<<<
+ *             free(self.domain)
+ */
+  }
+
+  /* "nazo_image_utils/rand_image.pyx":114
+ *         self.domain = strdup(domain.encode('utf-8'))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cdef int i
  *         if self.imgpc is not NULL:
  */
 
   /* function exit code */
@@ -3901,58 +3931,58 @@
   {&__pyx_n_b_source, __pyx_k_source, sizeof(__pyx_k_source), 0, 0, 0, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_ua, __pyx_k_ua, sizeof(__pyx_k_ua), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 38, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 99, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "nazo_image_utils/rand_image.pyx":36
+  /* "nazo_image_utils/rand_image.pyx":37
  *         if urls == NULL:
  *             with gil:
  *                 raise MemoryError("Failed to allocate memory for URLs array")             # <<<<<<<<<<<<<<
  * 
  *         for i in range(number):
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory_for_UR); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory_for_UR); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "nazo_image_utils/rand_image.pyx":46
+  /* "nazo_image_utils/rand_image.pyx":47
  *                 free(urls)
  *                 with gil:
  *                     raise MemoryError("Failed to allocate memory for URL string")             # <<<<<<<<<<<<<<
  * 
  *             snprintf(urls[i], 256, b"%s/%s/%s.%s.%s", self.domain, img_format, _hash, size, img_format)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory_for_UR_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory_for_UR_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "nazo_image_utils/rand_image.pyx":94
+  /* "nazo_image_utils/rand_image.pyx":95
  *         cdef int i
  *         cdef bytes encoded_key
  *         with open(pc_json_file) as pc:             # <<<<<<<<<<<<<<
  *             temp = json.load(pc)
  *             self.imgpc_total = len(temp)
  */
-  __pyx_tuple__4 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -3967,25 +3997,25 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "nazo_image_utils/rand_image.pyx":59
+  /* "nazo_image_utils/rand_image.pyx":60
  *         free(urls)
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):             # <<<<<<<<<<<<<<
  *         """
  *         URL
  */
-  __pyx_tuple__7 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_ua, __pyx_n_s_number, __pyx_n_s_platform, __pyx_n_s_encode, __pyx_n_s_size); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_ua, __pyx_n_s_number, __pyx_n_s_platform, __pyx_n_s_encode, __pyx_n_s_size); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_image_utils_rand_image_pyx, __pyx_n_s_process, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_image_utils_rand_image_pyx, __pyx_n_s_process, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 60, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -4058,24 +4088,24 @@
   /*--- Type init code ---*/
   __pyx_vtabptr_16nazo_image_utils_10rand_image_RandImage = &__pyx_vtable_16nazo_image_utils_10rand_image_RandImage;
   __pyx_vtable_16nazo_image_utils_10rand_image_RandImage.pc = (char *(*)(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *))__pyx_f_16nazo_image_utils_10rand_image_9RandImage_pc;
   __pyx_vtable_16nazo_image_utils_10rand_image_RandImage.mobile = (char *(*)(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *))__pyx_f_16nazo_image_utils_10rand_image_9RandImage_mobile;
   __pyx_vtable_16nazo_image_utils_10rand_image_RandImage.generate_img_urls = (char **(*)(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *, int, char const *, char const *, char const *))__pyx_f_16nazo_image_utils_10rand_image_9RandImage_generate_img_urls;
   __pyx_vtable_16nazo_image_utils_10rand_image_RandImage._free_urls = (void (*)(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *, char **, int))__pyx_f_16nazo_image_utils_10rand_image_9RandImage__free_urls;
   __pyx_vtable_16nazo_image_utils_10rand_image_RandImage.process = (PyObject *(*)(struct __pyx_obj_16nazo_image_utils_10rand_image_RandImage *, PyObject *, int, int __pyx_skip_dispatch, struct __pyx_opt_args_16nazo_image_utils_10rand_image_9RandImage_process *__pyx_optional_args))__pyx_f_16nazo_image_utils_10rand_image_9RandImage_process;
-  if (PyType_Ready(&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_dictoffset && __pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_dict, __pyx_vtabptr_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_RandImage, (PyObject *)&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_16nazo_image_utils_10rand_image_RandImage.tp_dict, __pyx_vtabptr_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_RandImage, (PyObject *)&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_16nazo_image_utils_10rand_image_RandImage) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __pyx_ptype_16nazo_image_utils_10rand_image_RandImage = &__pyx_type_16nazo_image_utils_10rand_image_RandImage;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -4347,51 +4377,51 @@
  * from nazo_rand.nazo_rand cimport cy_random_below
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_json, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_json, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_image_utils/rand_image.pyx":13
+  /* "nazo_image_utils/rand_image.pyx":14
  * 
  * cdef:
  *     const char* URLWEBP = b'webp'             # <<<<<<<<<<<<<<
  *     const char* URLJPEG = b'jpeg'
  *     const char* MOBILE = b"mobile"
  */
   __pyx_v_16nazo_image_utils_10rand_image_URLWEBP = ((char const *)"webp");
 
-  /* "nazo_image_utils/rand_image.pyx":14
+  /* "nazo_image_utils/rand_image.pyx":15
  * cdef:
  *     const char* URLWEBP = b'webp'
  *     const char* URLJPEG = b'jpeg'             # <<<<<<<<<<<<<<
  *     const char* MOBILE = b"mobile"
  * 
  */
   __pyx_v_16nazo_image_utils_10rand_image_URLJPEG = ((char const *)"jpeg");
 
-  /* "nazo_image_utils/rand_image.pyx":15
+  /* "nazo_image_utils/rand_image.pyx":16
  *     const char* URLWEBP = b'webp'
  *     const char* URLJPEG = b'jpeg'
  *     const char* MOBILE = b"mobile"             # <<<<<<<<<<<<<<
  * 
  * cdef class RandImage:
  */
   __pyx_v_16nazo_image_utils_10rand_image_MOBILE = ((char const *)"mobile");
 
-  /* "nazo_image_utils/rand_image.pyx":59
+  /* "nazo_image_utils/rand_image.pyx":60
  *         free(urls)
  * 
  *     cpdef process(self, bytes ua, int number, bytes platform=b"pc",bytes encode=b"", bytes size=b"source"):             # <<<<<<<<<<<<<<
  *         """
  *         URL
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_16nazo_image_utils_10rand_image_9RandImage_1process, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RandImage_process, NULL, __pyx_n_s_nazo_image_utils_rand_image, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_16nazo_image_utils_10rand_image_9RandImage_1process, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RandImage_process, NULL, __pyx_n_s_nazo_image_utils_rand_image, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_16nazo_image_utils_10rand_image_RandImage->tp_dict, __pyx_n_s_process, __pyx_t_1) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_16nazo_image_utils_10rand_image_RandImage->tp_dict, __pyx_n_s_process, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_16nazo_image_utils_10rand_image_RandImage);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
```

### Comparing `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyi` & `nazo_image_utils-0.0.3/nazo_image_utils/rand_image.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
 class RandImage:
-    def __init__(self, pc_json_path: str, mobile_json_path: str, domain: bytes) -> None:
+    def __init__(self, pc_json_path: str, mobile_json_path: str, domain: str) -> None:
         """初始化
 
         Args:
             pc_json_path (str): pc_json文件路径
 
             mobile_json_path (str): mobile_json文件路径
```

### Comparing `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyx` & `nazo_image_utils-0.0.3/nazo_image_utils/rand_image.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # cython: language_level=3
 # distutils: language = c++
 import json
 from webp_support.webp_support cimport webp_supported
 from nazo_rand.nazo_rand cimport cy_random_below
 from libc.string cimport strcmp
 from libc.string cimport strcpy
+from libc.string cimport strdup
 from libc.stdlib cimport malloc, free
 from libc.stdio cimport snprintf
 from cpython.bytes cimport PyBytes_FromString
 
 cdef:
     const char* URLWEBP = b'webp'
     const char* URLJPEG = b'jpeg'
@@ -83,15 +84,15 @@
         py_urls = [urls[i].decode('utf-8') for i in range(number)]
 
         # 释放内存
         self._free_urls(urls, number)
 
         return py_urls
 
-    def __cinit__(self, str pc_json_file, str mobile_json_file, bytes domain):
+    def __cinit__(self, str pc_json_file, str mobile_json_file, str domain):
         cdef str key
         cdef int i
         cdef bytes encoded_key
         with open(pc_json_file) as pc:
             temp = json.load(pc)
             self.imgpc_total = len(temp)
             self.imgpc = <char**>malloc(self.imgpc_total * sizeof(char*))
@@ -104,22 +105,25 @@
                     temp = json.load(mb)
                     self.imgmb_total = len(temp)
                     self.imgmb = <char**>malloc(self.imgmb_total * sizeof(char*))
                     for i, key in enumerate(temp.keys()):
                         encoded_key = key.encode('UTF-8')
                         self.imgmb[i] = <char*>malloc(len(encoded_key) + 1)  # +1 用于空终止字符
                         strcpy(self.imgmb[i], encoded_key)
-        self.domain = domain
+        self.domain = strdup(domain.encode('utf-8'))
 
     def __dealloc__(self):
         cdef int i
         if self.imgpc is not NULL:
             for i in range(self.imgpc_total):
                 if self.imgpc[i] is not NULL:
                     free(self.imgpc[i])
             free(self.imgpc)
 
         if self.imgmb is not NULL:
             for i in range(self.imgmb_total):
                 if self.imgmb[i] is not NULL:
                     free(self.imgmb[i])
-            free(self.imgmb)
+            free(self.imgmb)
+        
+        if self.domain is not NULL:
+            free(self.domain)
```

### Comparing `nazo_image_utils-0.0.2/nazo_image_utils.egg-info/PKG-INFO` & `nazo_image_utils-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 Metadata-Version: 2.1
-Name: nazo-image-utils
-Version: 0.0.2
+Name: nazo_image_utils
+Version: 0.0.3
 Summary: A tool for generating random images
 Author-email: bymoye <s3moye@gmail.com>
-License: MIT
+License: MIT License
+        
+        Copyright (c) 2023 迷与谜
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/bymoye/nazo_image_utils
 Project-URL: Bug Tracker, https://github.com/bymoye/nazo_image_utils/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Nazo Image Utils
 
 Nazo Image Utils 是一个用于处理随机图像和图像处理的 Python 包。它包含两个类：`RandImage` 和 `ProcessImage`。
 
 ## 安装
```

### Comparing `nazo_image_utils-0.0.2/pyproject.toml` & `nazo_image_utils-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 00000100: 7375 7070 6f72 7422 2c20 226e 617a 6f2d  support", "nazo-
 00000110: 7261 6e64 225d 0d0a 6275 696c 642d 6261  rand"]..build-ba
 00000120: 636b 656e 6420 3d20 2273 6574 7570 746f  ckend = "setupto
 00000130: 6f6c 732e 6275 696c 645f 6d65 7461 220d  ols.build_meta".
 00000140: 0a0d 0a0d 0a5b 6d65 7461 6461 7461 5d0d  .....[metadata].
 00000150: 0a6e 616d 6520 3d20 226e 617a 6f5f 696d  .name = "nazo_im
 00000160: 6167 655f 7574 696c 7322 0d0a 7665 7273  age_utils"..vers
-00000170: 696f 6e20 3d20 2230 2e30 2e31 220d 0a61  ion = "0.0.1"..a
+00000170: 696f 6e20 3d20 2230 2e30 2e33 220d 0a61  ion = "0.0.3"..a
 00000180: 7574 686f 7220 3d20 2262 796d 6f79 6522  uthor = "bymoye"
 00000190: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 000001a0: 2022 7333 6d6f 7965 4067 6d61 696c 2e63   "s3moye@gmail.c
 000001b0: 6f6d 220d 0a72 6561 646d 6520 3d20 2252  om"..readme = "R
 000001c0: 4541 444d 452e 6d64 220d 0a64 6573 6372  EADME.md"..descr
 000001d0: 6970 7469 6f6e 203d 2022 4120 746f 6f6c  iption = "A tool
 000001e0: 2066 6f72 2067 656e 6572 6174 696e 6720   for generating 
 000001f0: 7261 6e64 6f6d 2069 6d61 6765 7322 0d0a  random images"..
 00000200: 7572 6c20 3d20 2268 7474 7073 3a2f 2f67  url = "https://g
 00000210: 6974 6875 622e 636f 6d2f 6279 6d6f 7965  ithub.com/bymoye
 00000220: 2f6e 617a 6f5f 696d 6167 655f 7574 696c  /nazo_image_util
 00000230: 7322 0d0a 0d0a 0d0a 5b70 726f 6a65 6374  s"......[project
 00000240: 5d0d 0a6e 616d 653d 226e 617a 6f5f 696d  ]..name="nazo_im
 00000250: 6167 655f 7574 696c 7322 0d0a 7665 7273  age_utils"..vers
-00000260: 696f 6e20 3d20 2230 2e30 2e32 220d 0a61  ion = "0.0.2"..a
+00000260: 696f 6e20 3d20 2230 2e30 2e33 220d 0a61  ion = "0.0.3"..a
 00000270: 7574 686f 7273 203d 205b 0d0a 2020 2020  uthors = [..    
 00000280: 7b20 6e61 6d65 203d 2022 6279 6d6f 7965  { name = "bymoye
 00000290: 222c 2065 6d61 696c 203d 2022 7333 6d6f  ", email = "s3mo
 000002a0: 7965 4067 6d61 696c 2e63 6f6d 2220 7d2c  ye@gmail.com" },
 000002b0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 000002c0: 3d22 4120 746f 6f6c 2066 6f72 2067 656e  ="A tool for gen
 000002d0: 6572 6174 696e 6720 7261 6e64 6f6d 2069  erating random i
@@ -84,20 +84,19 @@
 00000530: 2c0d 0a20 2020 205d 0d0a 6465 7065 6e64  ,..    ]..depend
 00000540: 656e 6369 6573 203d 205b 0d0a 2020 2020  encies = [..    
 00000550: 2250 696c 6c6f 7722 2c0d 0a20 2020 2022  "Pillow",..    "
 00000560: 756a 736f 6e22 2c0d 0a20 2020 2022 7471  ujson",..    "tq
 00000570: 646d 222c 0d0a 2020 2020 2277 6562 702d  dm",..    "webp-
 00000580: 7375 7070 6f72 7422 2c0d 0a20 2020 2022  support",..    "
 00000590: 6e61 7a6f 2d72 616e 6422 2c0d 0a5d 0d0a  nazo-rand",..]..
-000005a0: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
-000005b0: 6c73 5d0d 0a70 6163 6b61 6765 7320 3d20  ls]..packages = 
-000005c0: 5b22 6e61 7a6f 5f69 6d61 6765 5f75 7469  ["nazo_image_uti
-000005d0: 6c73 225d 0d0a 0d0a 5b70 726f 6a65 6374  ls"]....[project
-000005e0: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
-000005f0: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
-00000600: 7468 7562 2e63 6f6d 2f62 796d 6f79 652f  thub.com/bymoye/
-00000610: 6e61 7a6f 5f69 6d61 6765 5f75 7469 6c73  nazo_image_utils
-00000620: 220d 0a22 4275 6720 5472 6163 6b65 7222  ".."Bug Tracker"
-00000630: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000640: 7562 2e63 6f6d 2f62 796d 6f79 652f 6e61  ub.com/bymoye/na
-00000650: 7a6f 5f69 6d61 6765 5f75 7469 6c73 2f69  zo_image_utils/i
-00000660: 7373 7565 7322 0d0a                      ssues"..
+000005a0: 6c69 6365 6e73 6520 3d20 7b20 6669 6c65  license = { file
+000005b0: 203d 2022 4c49 4345 4e53 4522 207d 0d0a   = "LICENSE" }..
+000005c0: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+000005d0: 0d0a 2248 6f6d 6570 6167 6522 203d 2022  .."Homepage" = "
+000005e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005f0: 6f6d 2f62 796d 6f79 652f 6e61 7a6f 5f69  om/bymoye/nazo_i
+00000600: 6d61 6765 5f75 7469 6c73 220d 0a22 4275  mage_utils".."Bu
+00000610: 6720 5472 6163 6b65 7222 203d 2022 6874  g Tracker" = "ht
+00000620: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000630: 2f62 796d 6f79 652f 6e61 7a6f 5f69 6d61  /bymoye/nazo_ima
+00000640: 6765 5f75 7469 6c73 2f69 7373 7565 7322  ge_utils/issues"
+00000650: 0d0a                                     ..
```

### Comparing `nazo_image_utils-0.0.2/setup.py` & `nazo_image_utils-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         compiler_directives={
             "language_level": 3,
             "boundscheck": False,
             "wraparound": False,
             "binding": True,
         },
     ),
-    license="MIT",
     package_data={
         "": [
             "nazo_image_utils/rand_image.pyi",
             "nazo_image_utils/rand_image.pyx",
             "nazo_image_utils/process_image.py",
         ]
     },
```

