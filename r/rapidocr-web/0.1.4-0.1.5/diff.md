# Comparing `tmp/rapidocr_web-0.1.4-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42709 bytes, number of entries: 13
--rw-r--r--  2.0 unx       74 b- defN 23-Apr-19 06:04 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1652 b- defN 23-Apr-19 06:04 rapidocr_web/api.py
--rw-r--r--  2.0 unx     1128 b- defN 23-Apr-19 06:04 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     2954 b- defN 23-Apr-19 06:04 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-Apr-19 06:04 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-Apr-19 06:04 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-Apr-19 06:04 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-Apr-19 06:04 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     4576 b- defN 23-Apr-19 06:04 rapidocr_web-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 06:04 rapidocr_web-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 23-Apr-19 06:04 rapidocr_web-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-19 06:04 rapidocr_web-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-19 06:04 rapidocr_web-0.1.4.dist-info/RECORD
-13 files, 125252 bytes uncompressed, 40859 bytes compressed:  67.4%
+Zip file size: 42990 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       73 b- defN 23-May-14 02:33 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-May-14 02:33 rapidocr_web/api.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-May-14 02:33 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-May-14 02:33 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-May-14 02:33 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-May-14 02:33 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-May-14 02:33 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-May-14 02:33 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       96 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1101 b- defN 23-May-14 02:34 rapidocr_web-0.1.5.dist-info/RECORD
+13 files, 126258 bytes uncompressed, 41140 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.4.dist-info/METADATA
+Filename: rapidocr_web-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.4.dist-info/WHEEL
+Filename: rapidocr_web-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.4.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.4.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.4.dist-info/RECORD
+Filename: rapidocr_web-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_web/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
-# @Contact: liekkaskono@163.com
+# @Contact: liekkaskono@163.com
```

## rapidocr_web/api.py

```diff
@@ -1,18 +1,20 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
+import base64
+import io
 import json
 from pathlib import Path
 
 import cv2
 import numpy as np
 import uvicorn
-from fastapi import FastAPI, UploadFile
+from fastapi import FastAPI, Form, UploadFile
 from PIL import Image
 from rapidocr_onnxruntime import RapidOCR
 
 
 class OCRAPIUtils():
     def __init__(self) -> None:
         self.ocr = RapidOCR()
@@ -38,17 +40,26 @@
 
 @app.get("/")
 async def root():
     return {'message': 'Welcome to RapidOCR Server!'}
 
 
 @app.post('/ocr')
-async def ocr(image: UploadFile):
-    image = Image.open(image.file)
-    ocr_res = processor(image)
+async def ocr(image_file: UploadFile = None, image_data: str = Form(None)):
+    if image_file:
+        img = Image.open(image_file.file)
+    elif image_data:
+        img_bytes = str.encode(image_data)
+        img_b64decode = base64.b64decode(img_bytes)
+        img = Image.open(io.BytesIO(img_b64decode))
+    else:
+        raise ValueError(
+            'When sending a post request, data or files must have a value.')
+
+    ocr_res = processor(img)
     return ocr_res
 
 
 def main():
     parser = argparse.ArgumentParser('rapidocr_api')
     parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
                         help='IP Address')
```

## rapidocr_web/ocrweb.py

```diff
@@ -2,15 +2,19 @@
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 from pathlib import Path
 from wsgiref.simple_server import make_server
 
 from flask import Flask, render_template, request
-from rapidocr_web.task import OCRWebUtils
+
+try:
+    from rapidocr_web.task import OCRWebUtils
+except:
+    from task import OCRWebUtils
 
 root_dir = Path(__file__).resolve().parent
 
 app = Flask(__name__, template_folder='templates')
 app.config['MAX_CONTENT_LENGTH'] = 3 * 1024 * 1024
 processor = OCRWebUtils()
```

## rapidocr_web/task.py

```diff
@@ -14,15 +14,15 @@
 
 
 class OCRWebUtils():
     def __init__(self) -> None:
         self.ocr = RapidOCR()
         self.WebReturn = namedtuple(
             'WebReturn',
-            ['image', 'total_elapse', 'elapse_part', 'rec_res'])
+            ['image', 'total_elapse', 'elapse_part', 'rec_res', 'det_boxes'])
 
     def __call__(self, img_content: str) -> namedtuple:
         if img_content is None:
             raise ValueError('img is None')
         img = self.prepare_img(img_content)
         ocr_res, elapse = self.ocr(img)
         return self.get_web_result(img, ocr_res, elapse)
@@ -40,29 +40,31 @@
                        img: np.ndarray,
                        ocr_res: List,
                        elapse: List) -> Tuple[Union[str, List, str, str]]:
         if ocr_res is None:
             total_elapse, elapse_part = 0, ''
             img_str = self.img_to_base64(img)
             rec_res = json.dumps([], indent=2, ensure_ascii=False)
+            boxes = ''
         else:
             boxes, txts, scores = list(zip(*ocr_res))
             rec_res = list(zip(range(len(txts)), txts, scores))
             rec_res = json.dumps(rec_res, indent=2, ensure_ascii=False)
 
             det_im = self.draw_text_det_res(np.array(boxes), img)
             img_str = self.img_to_base64(det_im)
 
             total_elapse = reduce(lambda x, y: float(x)+float(y), elapse)
             elapse_part = ','.join([f'{x:.4f}' for x in elapse])
 
         web_return = self.WebReturn(image=img_str,
                                     total_elapse=f'{total_elapse:.4f}',
                                     elapse_part=elapse_part,
-                                    rec_res=rec_res)
+                                    rec_res=rec_res,
+                                    det_boxes=boxes)
         return json.dumps(web_return._asdict())
 
     @staticmethod
     def img_to_base64(img) -> str:
         img = cv2.imencode('.png', img)[1]
         img_str = str(base64.b64encode(img))[2:-1]
         return img_str
```

## Comparing `rapidocr_web-0.1.4.dist-info/METADATA` & `rapidocr_web-0.1.5.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-web
-Version: 0.1.4
+Version: 0.1.5
 Summary: A cross platform OCR Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
@@ -71,27 +71,43 @@
        -p PORT, --port PORT  IP port
        ```
    - Example:
        ```bash
        $ rapidocr_api -ip 0.0.0.0 -p 9003
        ```
 3. Use
-    ```python
-    import requests
+    - Send image data by file format.
+        ```python
+        import requests
+
+        url = 'http://localhost:9003/ocr'
+        img_path = '../python/tests/test_files/ch_en_num.jpg'
+
+        with open(img_path, 'rb') as f:
+            file_dict = {'image_file': (img_path, f, 'image/png')}
+            response = requests.post(url, files=file_dict, timeout=60)
+
+        print(response.json())
+        ```
+    - Send image data by base64 format.
+        ```python
+        import base64
+        import requests
+
+        url = 'http://localhost:9003/ocr'
+        img_path = '../python/tests/test_files/ch_en_num.jpg'
 
-    url = 'http://localhost:9003/ocr'
-    img_path = '../python/tests/test_files/ch_en_num.jpg'
+        with open(img_path, 'rb') as fa:
+            img_str = base64.b64encode(fa.read())
 
-    with open(img_path, 'rb') as f:
-        file_dict = {'image': (img_path, f, 'image/png')}
-        response = requests.post(url, files=file_dict, timeout=60)
+        payload = {'image_data': img_str}
+        resp = requests.post(url, data=payload)
 
-    res_rec = response.json()
-    print(res_rec)
-    ```
+        print(resp.json())
+        ```
 4. Output
     <details>
     <summary>Click to expand</summary>
 
     ```json
     {
         "0": {
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.4 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.5 Summary: A cross
 platform OCR Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -20,25 +20,30 @@
 [-h] [-ip IP] [-p PORT] optional arguments: -h, --help show this help message
 and exit -ip IP, --ip IP IP Address -p PORT, --port PORT IP port ``` - Example:
 ```bash $ rapidocr_web -ip "0.0.0.0" -p 9003 ``` 3. Open `http://localhost:
 9003/` to view, enjoy it. ### API Use 1. Install`rapidocr_web[api]` ```bash $
 pip install rapidocr_web[api] ``` 2. Run - Usage: ```bash $ rapidocr_api -
 h usage: rapidocr_api [-h] [-ip IP] [-p PORT] optional arguments: -h, --help
 show this help message and exit -ip IP, --ip IP IP Address -p PORT, --port PORT
-IP port ``` - Example: ```bash $ rapidocr_api -ip 0.0.0.0 -p 9003 ``` 3. Use
-```python import requests url = 'http://localhost:9003/ocr' img_path = '../
-python/tests/test_files/ch_en_num.jpg' with open(img_path, 'rb') as f:
-file_dict = {'image': (img_path, f, 'image/png')} response = requests.post(url,
-files=file_dict, timeout=60) res_rec = response.json() print(res_rec) ``` 4.
-Output  Click to expand ```json { "0": { "rec_txt": "é¦æ¸¯æ·±å³æ½è¡ï¼",
-"dt_boxes": [ [265, 18], [472, 231], [431, 271], [223, 59] ], "score":
-"0.8175641223788261" }, "1": { "rec_txt": "ä¸ä¸æ¥æ§å«", "dt_boxes": [
-[388, 15], [636, 257], [587, 307], [339, 65] ], "score": "0.8293875356515249"
-}, "2": { "rec_txt": "ä¸ä¸é´å®Bè¶å", "dt_boxes": [ [215, 84], [509,
-413], [453, 463], [159, 134] ], "score": "0.8626169338822365" }, "3":
-{ "rec_txt": "bè¶ä»ªå¨æ¥æ§å«", "dt_boxes": [ [128, 135], [430, 478], [366,
-534], [64, 192] ], "score": "0.8449362441897392" }, "4": { "rec_txt":
-"å å¾®ä¿¡eee", "dt_boxes": [ [58, 189], [268, 450], [209, 498], [0, 236] ],
-"score": "0.8176911813872201" }, "5": { "rec_txt": "å¯é®å¯", "dt_boxes": [
-[493, 261], [617, 384], [577, 423], [454, 300] ], "score": "0.7494261413812637"
-} } ```  ### See details for [RapidOCR](https://github.com/RapidAI/RapidOCR/
-tree/main/ocrweb).
+IP port ``` - Example: ```bash $ rapidocr_api -ip 0.0.0.0 -p 9003 ``` 3. Use -
+Send image data by file format. ```python import requests url = 'http://
+localhost:9003/ocr' img_path = '../python/tests/test_files/ch_en_num.jpg' with
+open(img_path, 'rb') as f: file_dict = {'image_file': (img_path, f, 'image/
+png')} response = requests.post(url, files=file_dict, timeout=60) print
+(response.json()) ``` - Send image data by base64 format. ```python import
+base64 import requests url = 'http://localhost:9003/ocr' img_path = '../python/
+tests/test_files/ch_en_num.jpg' with open(img_path, 'rb') as fa: img_str =
+base64.b64encode(fa.read()) payload = {'image_data': img_str} resp =
+requests.post(url, data=payload) print(resp.json()) ``` 4. Output  Click to
+expand ```json { "0": { "rec_txt": "é¦æ¸¯æ·±å³æ½è¡ï¼", "dt_boxes": [ [265,
+18], [472, 231], [431, 271], [223, 59] ], "score": "0.8175641223788261" }, "1":
+{ "rec_txt": "ä¸ä¸æ¥æ§å«", "dt_boxes": [ [388, 15], [636, 257], [587,
+307], [339, 65] ], "score": "0.8293875356515249" }, "2": { "rec_txt":
+"ä¸ä¸é´å®Bè¶å", "dt_boxes": [ [215, 84], [509, 413], [453, 463], [159,
+134] ], "score": "0.8626169338822365" }, "3": { "rec_txt":
+"bè¶ä»ªå¨æ¥æ§å«", "dt_boxes": [ [128, 135], [430, 478], [366, 534], [64,
+192] ], "score": "0.8449362441897392" }, "4": { "rec_txt": "å å¾®ä¿¡eee",
+"dt_boxes": [ [58, 189], [268, 450], [209, 498], [0, 236] ], "score":
+"0.8176911813872201" }, "5": { "rec_txt": "å¯é®å¯", "dt_boxes": [ [493,
+261], [617, 384], [577, 423], [454, 300] ], "score": "0.7494261413812637" } }
+```  ### See details for [RapidOCR](https://github.com/RapidAI/RapidOCR/tree/
+main/ocrweb).
```

## Comparing `rapidocr_web-0.1.4.dist-info/RECORD` & `rapidocr_web-0.1.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-rapidocr_web/__init__.py,sha256=m-UGKHJ-31qL7pBis4nfoFz5fzb-dXsiTLNqY-xpSoA,74
-rapidocr_web/api.py,sha256=APjnOV0aTw_yDOoru84MsEh4RcQ_cHUHuGOxKy0Xk9k,1652
-rapidocr_web/ocrweb.py,sha256=fw9XEBoJZqUjbH19izaHJvXfQ-prwO_LoPjQuE3g8QY,1128
-rapidocr_web/task.py,sha256=l6PrccgTQDcvS8ZppZMfYuIPCYK-6ym_-02NWRm4Uak,2954
+rapidocr_web/__init__.py,sha256=JmySAOGOURKrbjdme2lVdTbDKaclr00IBKeVIa0_n30,73
+rapidocr_web/api.py,sha256=57p1b0HrWEU1UNmTmm_l9qK85wMC4ugYiUJzs9mk1-Y,2030
+rapidocr_web/ocrweb.py,sha256=Tl5a_ujmZ47WUFyHJ02u0kI--6HWGrizDlcJ9X9Nqmg,1179
+rapidocr_web/task.py,sha256=UVgdPds1NeZTtBnh_hjZiULUKOs_J1cU_hcQDm1Y5ts,3043
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.4.dist-info/METADATA,sha256=F1RczImG1PKzwPrw9UaAu9pUxKIUsRqDMJzr3SudA7s,4576
-rapidocr_web-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.4.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
-rapidocr_web-0.1.4.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.4.dist-info/RECORD,,
+rapidocr_web-0.1.5.dist-info/METADATA,sha256=m76vYV6b6n6s-rvRF-jVooEl6Gd-PDnujYX-KMEGP-0,5065
+rapidocr_web-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.5.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
+rapidocr_web-0.1.5.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.5.dist-info/RECORD,,
```

