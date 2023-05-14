# Comparing `tmp/mongo_to_som-1.0.7.tar.gz` & `tmp/mongo_to_som-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_to_som-1.0.7.tar", last modified: Wed Apr 19 18:16:26 2023, max compression
+gzip compressed data, was "mongo_to_som-1.0.8.tar", last modified: Sun May 14 19:01:59 2023, max compression
```

## Comparing `mongo_to_som-1.0.7.tar` & `mongo_to_som-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/
--rw-rw-rw-   0        0        0     1140 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-19 18:15:58.000000 mongo_to_som-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.861684 mongo_to_som-1.0.7/mongo_to_som/
--rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.7/mongo_to_som/__init__.py
--rw-rw-rw-   0        0        0     7405 2023-04-19 18:13:44.000000 mongo_to_som-1.0.7/mongo_to_som/mongotosom.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.866681 mongo_to_som-1.0.7/mongo_to_som.egg-info/
--rw-rw-rw-   0        0        0     1140 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1428 2023-04-19 18:16:03.000000 mongo_to_som-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 19:01:59.006751 mongo_to_som-1.0.8/
+-rw-rw-rw-   0        0        0     1140 2023-05-14 19:01:59.005751 mongo_to_som-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-19 18:15:58.000000 mongo_to_som-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 19:01:58.997751 mongo_to_som-1.0.8/mongo_to_som/
+-rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.8/mongo_to_som/__init__.py
+-rw-rw-rw-   0        0        0     7447 2023-05-14 18:58:47.000000 mongo_to_som-1.0.8/mongo_to_som/mongotosom.py
+drwxrwxrwx   0        0        0        0 2023-05-14 19:01:59.004751 mongo_to_som-1.0.8/mongo_to_som.egg-info/
+-rw-rw-rw-   0        0        0     1140 2023-05-14 19:01:58.000000 mongo_to_som-1.0.8/mongo_to_som.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-14 19:01:58.000000 mongo_to_som-1.0.8/mongo_to_som.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 19:01:58.000000 mongo_to_som-1.0.8/mongo_to_som.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-14 19:01:58.000000 mongo_to_som-1.0.8/mongo_to_som.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 19:01:58.000000 mongo_to_som-1.0.8/mongo_to_som.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 19:01:59.006751 mongo_to_som-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2023-05-14 18:59:27.000000 mongo_to_som-1.0.8/setup.py
```

### Comparing `mongo_to_som-1.0.7/PKG-INFO` & `mongo_to_som-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_to_som
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mongo_to_som-1.0.7/mongo_to_som/mongotosom.py` & `mongo_to_som-1.0.8/mongo_to_som/mongotosom.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 import csv
 from numpy.ma.core import ceil
 from scipy.spatial import distance #distance calculation
 from sklearn.preprocessing import MinMaxScaler #normalisation
 from sklearn.model_selection import train_test_split
 import matplotlib.pyplot as plt
 from matplotlib import colors
-
+import time
 
 
 class mongo_to_som:
   def __init__(self, num_rows, num_cols, max_steps, max_m_distance, max_learning_rate, url, port, db, collection):
     self.num_rows = num_rows
     self.num_cols = num_cols
     self.max_steps = max_steps
     self.url = url
     self.port = port
     self.db = db
     self.collection = collection
     self.max_m_distance = max_m_distance
     self.max_learning_rate = max_learning_rate
 
+    start_time = time.time()
+
     client = MongoClient(self.url, self.port)
     db = client[self.db]
     collection = db[self.collection]
 
     data = list(collection.find())
     df = pd.DataFrame(data)
 
     # Calculate percentage of non-null values in each column
     threshold = 0.9
     col_perc = df.count() / df.shape[0]
 
-    #print(col_perc)
-
     # Filter columns based on percentage threshold
     keep_cols = col_perc[col_perc >= threshold].index.tolist()
     # Keep only the desired columns
     data = list(collection.find({}, {'_id': 0, **{col: 1 for col in keep_cols}}))
     df = pd.DataFrame(data)
 
     missing_cols = df.columns[df.isna().any()].tolist()
@@ -52,42 +52,38 @@
 
       df.loc[:, missing_cols] = imputed_values
 
     df.iloc[:, 1:].to_csv("output.txt", sep=',', index=False, header=False)
 
     with open('output.txt', 'r') as file:
       reader = csv.reader(file, delimiter=',')
-      self.num_cols = len(next(reader))
+      num_cols_txt = len(next(reader))
 
     data_file = "output.txt"
-    data_x = np.loadtxt(data_file, delimiter=",", skiprows=0, usecols=range(1, self.num_cols), dtype=np.float64)
-    data_y = np.loadtxt(data_file, delimiter=",", skiprows=0, usecols=(self.num_cols - 1,), dtype=np.int64)
+    data_x = np.loadtxt(data_file, delimiter=",", skiprows=0, usecols=range(1, num_cols_txt), dtype=np.float64)
+    data_y = np.loadtxt(data_file, delimiter=",", skiprows=0, usecols=(num_cols_txt - 1,), dtype=np.int64)
 
     # train and test split
     train_x, test_x, train_y, test_y = train_test_split(data_x, data_y, test_size=0.2, random_state=42)
     print(train_x.shape, train_y.shape, test_x.shape, test_y.shape)  # check the shapes
 
-    # num_nurons = 5*np.sqrt(train_x.shape[0])
-    # grid_size = ceil(np.sqrt(num_nurons))
-    # print(grid_size)
-
     # main function
 
     train_x_norm = self.minmax_scaler(train_x)  # normalisation
 
     # initialising self-organising map
     num_dims = train_x_norm.shape[1]  # numnber of dimensions in the input data
     np.random.seed(40)
     som = np.random.random_sample(size=(self.num_rows, self.num_cols, num_dims))  # map construction
 
     # start training iterations
     for step in range(max_steps):
       if (step + 1) % 1000 == 0:
         print("Iteration: ", step + 1)  # print out the current iteration for every 1k
-      learning_rate, neighbourhood_range = self.decay(step, max_steps, max_learning_rate, self.max_m_distance)
+      learning_rate, neighbourhood_range = self.decay(step, max_steps, self.max_learning_rate, self.max_m_distance)
 
       t = np.random.randint(0, high=train_x_norm.shape[0])  # random index of traing data
       winner = self.winning_neuron(train_x_norm, t, som, self.num_rows, self.num_cols)
       for row in range(self.num_rows):
         for col in range(self.num_cols):
           if self.m_distance([row, col], winner) <= neighbourhood_range:
             som[row][col] += learning_rate * (train_x_norm[t] - som[row][col])  # update neighbour's weight
@@ -118,38 +114,40 @@
           label = 2
         else:
           label = max(label_list, key=label_list.count)
         label_map[row][col] = label
 
     title = ('Iteration ' + str(max_steps))
     cmap = colors.ListedColormap(['tab:green', 'tab:red', 'tab:orange'])
-    plt.imshow(label_map, cmap=cmap)
+    plt.imshow(label_map, cmap=cmap, extent=[0, self.num_cols, self.num_rows, 0])
     plt.colorbar()
     plt.title(title)
+
+    end_time = time.time()
+    time_difference = end_time - start_time
+    time_difference_rounded = round(time_difference)
+    print("Tool was running: ", time_difference_rounded, "seconds")
     plt.show()
 
     # reshape SOM into 3D array
     som_3d = som.reshape(self.num_rows * self.num_cols, num_dims)
 
     # create 3D scatter plot
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
     ax.scatter(som_3d[:, 0], som_3d[:, 1], som_3d[:, 2], c=label_map.flatten(), cmap='viridis')
-    ax.set_xlabel('Feature 1')
-    ax.set_ylabel('Feature 2')
-    ax.set_zlabel('Feature 3')
+    ax.set_xlabel('Axis X')
+    ax.set_ylabel('Axis Y')
+    ax.set_zlabel('Axis Z')
     plt.show()
 
     # create 3D scatter plot
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
     ax.scatter(som_3d[:, 0], som_3d[:, 1], som_3d[:, 2], c=label_map.flatten(), cmap='viridis')
-    ax.set_xlabel('Feature 1')
-    ax.set_ylabel('Feature 2')
-    ax.set_zlabel('Feature 3')
 
     # add lines between neighboring nodes
     for i in range(self.num_rows):
       for j in range(self.num_cols):
         if j < self.num_cols - 1:
           # add line between current node and its right neighbor
           ax.plot([som[i][j][0], som[i][j + 1][0]], [som[i][j][1], som[i][j + 1][1]], [som[i][j][2], som[i][j + 1][2]],
@@ -157,14 +155,15 @@
         if i < self.num_rows - 1:
           # add line between current node and its bottom neighbor
           ax.plot([som[i][j][0], som[i + 1][j][0]], [som[i][j][1], som[i + 1][j][1]], [som[i][j][2], som[i + 1][j][2]],
                   color='black', linewidth=0.5)
 
     plt.show()
 
+
   # Data Normalisation
   def minmax_scaler(self, data):
     scaler = MinMaxScaler()
     scaled = scaler.fit_transform(data)
     return scaled
 
   # Euclidean distance
```

### Comparing `mongo_to_som-1.0.7/mongo_to_som.egg-info/PKG-INFO` & `mongo_to_som-1.0.8/mongo_to_som.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-to-som
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mongo_to_som-1.0.7/setup.py` & `mongo_to_som-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="mongo_to_som",
     packages=["mongo_to_som"],
     include_package_data=True,
-    version='1.0.7',
+    version='1.0.8',
     description='Library to create Self-Organizing Map from MongoDB collection',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tomáš Peregrín',
     author_email="djtoso@gmail.com",
     license='MIT',
     classifiers=[
```

