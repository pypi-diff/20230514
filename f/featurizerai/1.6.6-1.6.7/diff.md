# Comparing `tmp/featurizerai-1.6.6.tar.gz` & `tmp/featurizerai-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.6.6.tar", last modified: Sun Apr 30 01:34:33 2023, max compression
+gzip compressed data, was "featurizerai-1.6.7.tar", last modified: Sun May 14 02:10:17 2023, max compression
```

## Comparing `featurizerai-1.6.6.tar` & `featurizerai-1.6.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.027009 featurizerai-1.6.6/
--rw-rw-rw-   0        0        0     1100 2023-04-29 00:34:12.000000 featurizerai-1.6.6/LICENSE
--rw-rw-rw-   0        0        0       89 2023-04-29 00:34:12.000000 featurizerai-1.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0      879 2023-04-30 01:34:33.027009 featurizerai-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-29 00:34:12.000000 featurizerai-1.6.6/pyproject.toml
--rw-rw-rw-   0        0        0      123 2023-04-30 01:34:33.035597 featurizerai-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1378 2023-04-30 01:33:44.000000 featurizerai-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:34:32.972860 featurizerai-1.6.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.011252 featurizerai-1.6.6/src/features/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/authenticate.py
--rw-rw-rw-   0        0        0     4329 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/create_stream.py
--rw-rw-rw-   0        0        0      979 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/custom_schema.py
--rw-rw-rw-   0        0        0     4984 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/materialize.py
--rw-rw-rw-   0        0        0     6710 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/test.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.027009 featurizerai-1.6.6/src/featurizerai.egg-info/
--rw-rw-rw-   0        0        0      879 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:10:17.986184 featurizerai-1.6.7/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.7/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.7/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:10:17.986259 featurizerai-1.6.7/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.7/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-05-14 02:10:17.986485 featurizerai-1.6.7/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-05-14 02:09:53.000000 featurizerai-1.6.7/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:10:17.982581 featurizerai-1.6.7/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:10:17.984899 featurizerai-1.6.7/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.7/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.7/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.7/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1318 2023-05-14 02:09:30.000000 featurizerai-1.6.7/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4872 2023-04-30 04:27:45.000000 featurizerai-1.6.7/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     6558 2023-04-30 00:07:16.000000 featurizerai-1.6.7/src/features/test.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:10:17.986020 featurizerai-1.6.7/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:10:17.000000 featurizerai-1.6.7/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      415 2023-05-14 02:10:17.000000 featurizerai-1.6.7/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-05-14 02:10:17.000000 featurizerai-1.6.7/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-05-14 02:10:17.000000 featurizerai-1.6.7/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-05-14 02:10:17.000000 featurizerai-1.6.7/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.6.6/LICENSE` & `featurizerai-1.6.7/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Tom Chen (tomchen.org)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Tom Chen (tomchen.org)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `featurizerai-1.6.6/PKG-INFO` & `featurizerai-1.6.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: featurizerai
-Version: 1.6.6
-Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakglobal/featurizerai
-Author: Burak
-Author-email: burakgblobal@gmail.com
-Keywords: featurizer,package
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Provides-Extra: dev
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: featurizerai
+Version: 1.6.7
+Summary: Python library for Featurizer AI
+Home-page: https://github.com/burakglobal/featurizerai
+Author: Burak
+Author-email: burakgblobal@gmail.com
+Keywords: featurizer,package
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Provides-Extra: dev
+License-File: LICENSE
```

### Comparing `featurizerai-1.6.6/setup.py` & `featurizerai-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.6.6',
+    version='1.6.7',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.6.6/src/features/authenticate.py` & `featurizerai-1.6.7/src/features/authenticate.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import requests
-import base64
-
-class authenticate:
-    def __init__(self, base_url = 'http://0.0.0.0:4000'):
-        self.base_url = base_url
-
-    def authenticate(self, username, password):
-        url = f'{self.base_url}/authenticate'
-        credentials = f'{username}:{password}'.encode('ascii')
-        encoded_credentials = base64.b64encode(credentials).decode('ascii')
-        headers = {'Authorization': f'Basic {encoded_credentials}'}
-        response = requests.post(url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            return data.get('access_token'), data.get('token_type')
-        else:
-            return None, None
+import requests
+import base64
+
+class authenticate:
+    def __init__(self, base_url = 'http://0.0.0.0:4000'):
+        self.base_url = base_url
+
+    def authenticate(self, username, password):
+        url = f'{self.base_url}/authenticate'
+        credentials = f'{username}:{password}'.encode('ascii')
+        encoded_credentials = base64.b64encode(credentials).decode('ascii')
+        headers = {'Authorization': f'Basic {encoded_credentials}'}
+        response = requests.post(url, headers=headers)
+        if response.status_code == 200:
+            data = response.json()
+            return data.get('access_token'), data.get('token_type')
+        else:
+            return None, None
```

### Comparing `featurizerai-1.6.6/src/features/create_stream.py` & `featurizerai-1.6.7/src/features/create_stream.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import json
-import ast
-import logging
-from datetime import datetime
-from http.client import HTTPException
-
-from pymongo import MongoClient
-from pymongo.server_api import ServerApi
-from confluent_kafka import Consumer, KafkaError
-import certifi
-import os
-import threading
-import jwt
-
-class create_stream:
-    def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
-        self.topicname = topicname
-        self.kafka_connection = kafka_connection
-        self.mongo_connection = mongo_connection
-        self.timestamp_attr = timestamp_attr
-        self._stop_event = threading.Event()
-
-    def is_epoch(self, timestamp):
-        try:
-            datetime.fromtimestamp(int(timestamp))
-            return True
-        except ValueError:
-            return False
-
-    def _run(self, token):
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
-
-        consumer = Consumer(self.kafka_connection)
-        print(self.topicname)
-        consumer.subscribe([self.topicname])
-
-        while not self._stop_event.is_set():
-            msg = consumer.poll(10.0)
-            print("Poll executed")
-            print(msg)
-            if msg is None:
-                continue
-            if msg.error():
-                print("Consumer error: {}".format(msg.error()))
-            else:
-                message_value = ast.literal_eval(msg.value().decode("utf-8"))
-                print(message_value)
-
-                # New lines added for validation
-                if self.timestamp_attr not in message_value:
-                    print(
-                        f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
-                    continue
-
-                if self.is_epoch(message_value.get(self.timestamp_attr)):
-                    if self.is_epoch(message_value.get(self.timestamp_attr)):
-                        message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
-                    else:
-                        message_value[self.timestamp_attr] = datetime.now().timestamp()
-
-                raw_data_collection.insert_one(message_value)
-                print("Message received: {}".format(message_value))
-        consumer.close()
-
-    def start(self, token):
-        # authenicate token
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        mongo_db_featurizer = mongo_client['featurizer']
-        users_collection = mongo_db_featurizer["users"]
-        SECRET_KEY = "features"  # Change this to your desired secret key
-        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
-
-        try:
-            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
-            user_id: str = payload.get("user_id")
-            if user_id is None:
-                print("User not found")
-                return ("Invalid token")
-            print(user_id)
-            user = users_collection.find_one({"userid": user_id})
-            if user is None:
-                print("User not found")
-                return ("Invalid token")
-        except Exception as e:
-            print(e)
-            return ("Invalid token")
-
-
-        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
-            self._stop_event.clear()
-            self._consumer_thread = threading.Thread(target=self._run(self))
-            self._consumer_thread.start()
-            print('featurizerai: Started consumer thread.')
-        else:
-            print("Thread is already running. Cannot start it again.")
-
-    def stop(self):
-        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
-            self._stop_event.set()
-            self._consumer_thread.join()
-            print('featurizerai: Stopped consumer thread.')
-        else:
-            print("Thread is not running. Cannot stop it.")
+import json
+import ast
+import logging
+from datetime import datetime
+from http.client import HTTPException
+
+from pymongo import MongoClient
+from pymongo.server_api import ServerApi
+from confluent_kafka import Consumer, KafkaError
+import certifi
+import os
+import threading
+import jwt
+
+class create_stream:
+    def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
+        self.topicname = topicname
+        self.kafka_connection = kafka_connection
+        self.mongo_connection = mongo_connection
+        self.timestamp_attr = timestamp_attr
+        self._stop_event = threading.Event()
+
+    def is_epoch(self, timestamp):
+        try:
+            datetime.fromtimestamp(int(timestamp))
+            return True
+        except ValueError:
+            return False
+
+    def _run(self, token):
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
+
+        consumer = Consumer(self.kafka_connection)
+        print(self.topicname)
+        consumer.subscribe([self.topicname])
+
+        while not self._stop_event.is_set():
+            msg = consumer.poll(10.0)
+            print("Poll executed")
+            print(msg)
+            if msg is None:
+                continue
+            if msg.error():
+                print("Consumer error: {}".format(msg.error()))
+            else:
+                message_value = ast.literal_eval(msg.value().decode("utf-8"))
+                print(message_value)
+
+                # New lines added for validation
+                if self.timestamp_attr not in message_value:
+                    print(
+                        f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
+                    continue
+
+                if self.is_epoch(message_value.get(self.timestamp_attr)):
+                    if self.is_epoch(message_value.get(self.timestamp_attr)):
+                        message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
+                    else:
+                        message_value[self.timestamp_attr] = datetime.now().timestamp()
+
+                raw_data_collection.insert_one(message_value)
+                print("Message received: {}".format(message_value))
+        consumer.close()
+
+    def start(self, token):
+        # authenicate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print(user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+
+        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
+            self._stop_event.clear()
+            self._consumer_thread = threading.Thread(target=self._run(self))
+            self._consumer_thread.start()
+            print('featurizerai: Started consumer thread.')
+        else:
+            print("Thread is already running. Cannot start it again.")
+
+    def stop(self):
+        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
+            self._stop_event.set()
+            self._consumer_thread.join()
+            print('featurizerai: Stopped consumer thread.')
+        else:
+            print("Thread is not running. Cannot stop it.")
```

### Comparing `featurizerai-1.6.6/src/features/materialize.py` & `featurizerai-1.6.7/src/features/materialize.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import json
-import logging
-from datetime import datetime, timedelta
-import jwt
-from pymongo import MongoClient
-from pyspark.sql import SparkSession
-from pyspark.sql.functions import col, count
-from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
-from pyspark.sql import functions as F
-import certifi
-from pymongo.server_api import ServerApi
-from pyspark.sql.functions import col
-
-
-class materialize:
-    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
-        self.mongo_connection = mongo_connection
-        self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
-        self.groupby = groupby_value
-        self.groupby_attr = groupby_attr
-        self.token = token
-        self.schema = schema
-        self.sparksql = sparksql
-        self.partition_column = partition_column
-
-        self.spark = SparkSession.builder \
-            .appName("IncrementalAggregation") \
-            .master("local[*]") \
-            .getOrCreate()
-        self.spark.sparkContext.setLogLevel("ERROR")
-
-    def read_data_and_aggregate(self):
-
-
-        # authenticate token
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        mongo_db_featurizer = mongo_client['featurizer']
-        users_collection = mongo_db_featurizer["users"]
-        SECRET_KEY = "features"  # Change this to your desired secret key
-        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
-
-        try:
-            payload = jwt.decode(self.token, SECRET_KEY, algorithms=["HS256"])
-            user_id: str = payload.get("user_id")
-            if user_id is None:
-                print("User not found")
-                return ("Invalid token")
-            print("Authenticated user: " + user_id)
-            user = users_collection.find_one({"userid": user_id})
-            if user is None:
-                print("User not found")
-                return ("Invalid token")
-        except Exception as e:
-            print(e)
-            return ("Invalid token")
-
-        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
-        aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
-
-        raw_data = raw_data_collection.find()
-        raw_data_list = [doc for doc in raw_data]
-        df = self.spark.createDataFrame(raw_data_list, self.schema)
-
-        # Apply partitioning if the partition_column is specified
-        if self.partition_column:
-            print("Partitioning the DataFrame based on the column: " + self.partition_column)
-            raw_data_collection.create_index(self.partition_column)
-            raw_data_collection.create_index(self.groupby_attr)
-            df = df.repartition(col(self.partition_column))
-
-        # Filter the DataFrame based on the given device_id
-        df = df.filter(col(self.groupby_attr) == self.groupby)
-        start_time = self.aggregation_date
-        df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
-        df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
-        df.createOrReplaceTempView("temp_table")
-
-        # Define empty schema for DataFrame
-        schema = StructType([
-            StructField(self.groupby_attr, StringType(), True)
-        ])
-        # Create empty DataFrame
-        result_df = self.spark.createDataFrame([], schema)
-
-        # Execute the dynamic Spark SQL
-        for sql in self.sparksql:
-            sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
-            hour = int(sql.split("_")[2])
-            sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
-            sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
-            c_count = self.spark.sql(sql_with_timestamp_base)
-            result_df = result_df.join(c_count, self.groupby_attr, "full") \
-                .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
-
-        if result_df.isEmpty():
-            json_aggregated_data = "{'error': 'No data found'}"
-        else:
-            json_aggregated_data = result_df.toJSON().collect()[0]
-
-        if json_aggregated_data is not None:
-            aggregated_data_collection.update_one(
-                {"date": start_time, "aggregated_key": self.groupby},
-                {"$set": {"aggregated_data": json_aggregated_data}},
-                upsert=True
-            )
-        else:
-            logging.error("Serialized aggregated data is None, skipping update")
-
-        return json_aggregated_data
-
-
+import json
+import logging
+from datetime import datetime, timedelta
+import jwt
+from pymongo import MongoClient
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import col, count
+from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
+from pyspark.sql import functions as F
+import certifi
+from pymongo.server_api import ServerApi
+from pyspark.sql.functions import col
+
+
+class materialize:
+    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
+        self.mongo_connection = mongo_connection
+        self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
+        self.groupby = groupby_value
+        self.groupby_attr = groupby_attr
+        self.token = token
+        self.schema = schema
+        self.sparksql = sparksql
+        self.partition_column = partition_column
+
+        self.spark = SparkSession.builder \
+            .appName("IncrementalAggregation") \
+            .master("local[*]") \
+            .getOrCreate()
+        self.spark.sparkContext.setLogLevel("ERROR")
+
+    def read_data_and_aggregate(self):
+
+
+        # authenticate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(self.token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print("Authenticated user: " + user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
+        aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
+
+        raw_data = raw_data_collection.find()
+        raw_data_list = [doc for doc in raw_data]
+        df = self.spark.createDataFrame(raw_data_list, self.schema)
+
+        # Apply partitioning if the partition_column is specified
+        if self.partition_column:
+            print("Partitioning the DataFrame based on the column: " + self.partition_column)
+            raw_data_collection.create_index(self.partition_column)
+            raw_data_collection.create_index(self.groupby_attr)
+            df = df.repartition(col(self.partition_column))
+
+        # Filter the DataFrame based on the given device_id
+        df = df.filter(col(self.groupby_attr) == self.groupby)
+        start_time = self.aggregation_date
+        df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
+        df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
+        df.createOrReplaceTempView("temp_table")
+
+        # Define empty schema for DataFrame
+        schema = StructType([
+            StructField(self.groupby_attr, StringType(), True)
+        ])
+        # Create empty DataFrame
+        result_df = self.spark.createDataFrame([], schema)
+
+        # Execute the dynamic Spark SQL
+        for sql in self.sparksql:
+            sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
+            hour = int(sql.split("_")[2])
+            sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
+            sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
+            c_count = self.spark.sql(sql_with_timestamp_base)
+            result_df = result_df.join(c_count, self.groupby_attr, "full") \
+                .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
+
+        if result_df.isEmpty():
+            json_aggregated_data = "{'error': 'No data found'}"
+        else:
+            json_aggregated_data = result_df.toJSON().collect()[0]
+
+        if json_aggregated_data is not None:
+            aggregated_data_collection.update_one(
+                {"date": start_time, "aggregated_key": self.groupby},
+                {"$set": {"aggregated_data": json_aggregated_data}},
+                upsert=True
+            )
+        else:
+            logging.error("Serialized aggregated data is None, skipping update")
+
+        return json_aggregated_data
+
+
```

### Comparing `featurizerai-1.6.6/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.6.7/src/featurizerai.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: featurizerai
-Version: 1.6.6
-Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakglobal/featurizerai
-Author: Burak
-Author-email: burakgblobal@gmail.com
-Keywords: featurizer,package
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Provides-Extra: dev
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: featurizerai
+Version: 1.6.7
+Summary: Python library for Featurizer AI
+Home-page: https://github.com/burakglobal/featurizerai
+Author: Burak
+Author-email: burakgblobal@gmail.com
+Keywords: featurizer,package
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Provides-Extra: dev
+License-File: LICENSE
```

