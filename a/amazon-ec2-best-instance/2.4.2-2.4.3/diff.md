# Comparing `tmp/amazon-ec2-best-instance-2.4.2.tar.gz` & `tmp/amazon-ec2-best-instance-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-qd4x97g3/amazon-ec2-best-instance-2.4.2.tar", last modified: Sat May 13 18:19:21 2023, max compression
+gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-upl4xy41/amazon-ec2-best-instance-2.4.3.tar", last modified: Sat May 13 19:00:41 2023, max compression
```

## Comparing `amazon-ec2-best-instance-2.4.2.tar` & `amazon-ec2-best-instance-2.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/
--rw-r--r--   0 alexey     (501) staff       (20)     7179 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     6615 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/README.md
--rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/pyproject.toml
--rw-r--r--   0 alexey     (501) staff       (20)      792 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)      184 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/setup.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/
--rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/SpotUtils.py
--rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    20934 2023-05-13 18:09:20.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     7179 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      774 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       41 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/top_level.txt
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 18:19:21.000000 amazon-ec2-best-instance-2.4.2/test/
--rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test.py
--rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test1.py
--rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test10.py
--rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test11.py
--rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test2.py
--rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test5.py
--rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test6.py
--rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test7.py
--rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test8.py
--rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test9.py
--rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test_azs.py
--rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-2.4.2/test/test_cache.py
--rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_2.py
--rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_5.py
--rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_6.py
--rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-2.4.2/test/test_cache_7.py
--rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.2/test/test_clients.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/
+-rw-r--r--   0 alexey     (501) staff       (20)     7353 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)     6789 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-2.4.3/README.md
+-rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/pyproject.toml
+-rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-2.4.3/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/
+-rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/SpotUtils.py
+-rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/__init__.py
+-rw-r--r--   0 alexey     (501) staff       (20)    20934 2023-05-13 18:09:20.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     7353 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      774 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/top_level.txt
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-13 19:00:41.000000 amazon-ec2-best-instance-2.4.3/test/
+-rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test1.py
+-rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test10.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test11.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test6.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test8.py
+-rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test9.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test_azs.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-2.4.3/test/test_cache.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_6.py
+-rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-2.4.3/test/test_cache_7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.4.3/test/test_clients.py
```

### Comparing `amazon-ec2-best-instance-2.4.2/PKG-INFO` & `amazon-ec2-best-instance-2.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 2.4.2
+Version: 2.4.3
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
@@ -23,23 +23,23 @@
 # Install
 pip install amazon-ec2-best-instance
 
 # Options
 
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
-* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand.
+* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
-* **architecture** Optional. String. The architectures supported by the instance type.
-* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
+* **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
+* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
 * **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
-* **availability_zones** Optional. List<String>. Availability zones
+* **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
 
 ## Simple
 
 ```
```

### Comparing `amazon-ec2-best-instance-2.4.2/README.md` & `amazon-ec2-best-instance-2.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # Install
 pip install amazon-ec2-best-instance
 
 # Options
 
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
-* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand.
+* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
-* **architecture** Optional. String. The architectures supported by the instance type.
-* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
+* **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
+* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
 * **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
-* **availability_zones** Optional. List<String>. Availability zones
+* **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
 
 ## Simple
 
 ```
```

### Comparing `amazon-ec2-best-instance-2.4.2/setup.cfg` & `amazon-ec2-best-instance-2.4.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amazon-ec2-best-instance
-version = 2.4.2
+version = 2.4.3
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 project_urls = 
@@ -14,14 +14,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	boto3 >=1.23.10
 	lambda-thread-pool >=0.0.2
+	requests >= 2.30.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/SpotUtils.py` & `amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/SpotUtils.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance/main.py` & `amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance/main.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/PKG-INFO` & `amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 2.4.2
+Version: 2.4.3
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
@@ -23,23 +23,23 @@
 # Install
 pip install amazon-ec2-best-instance
 
 # Options
 
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
-* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand.
+* **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
-* **architecture** Optional. String. The architectures supported by the instance type.
-* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
+* **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
+* **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
 * **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
-* **availability_zones** Optional. List<String>. Availability zones
+* **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
 
 ## Simple
 
 ```
```

### Comparing `amazon-ec2-best-instance-2.4.2/src/amazon_ec2_best_instance.egg-info/SOURCES.txt` & `amazon-ec2-best-instance-2.4.3/src/amazon_ec2_best_instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test.py` & `amazon-ec2-best-instance-2.4.3/test/test.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test1.py` & `amazon-ec2-best-instance-2.4.3/test/test1.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test10.py` & `amazon-ec2-best-instance-2.4.3/test/test10.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test11.py` & `amazon-ec2-best-instance-2.4.3/test/test11.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test2.py` & `amazon-ec2-best-instance-2.4.3/test/test2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test4.py` & `amazon-ec2-best-instance-2.4.3/test/test4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test5.py` & `amazon-ec2-best-instance-2.4.3/test/test5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test6.py` & `amazon-ec2-best-instance-2.4.3/test/test6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test7.py` & `amazon-ec2-best-instance-2.4.3/test/test7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test8.py` & `amazon-ec2-best-instance-2.4.3/test/test8.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test9.py` & `amazon-ec2-best-instance-2.4.3/test/test9.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_azs.py` & `amazon-ec2-best-instance-2.4.3/test/test_azs.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_2.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_3.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_3.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_4.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_5.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_6.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_cache_7.py` & `amazon-ec2-best-instance-2.4.3/test/test_cache_7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.4.2/test/test_clients.py` & `amazon-ec2-best-instance-2.4.3/test/test_clients.py`

 * *Files identical despite different names*

