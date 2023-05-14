# Comparing `tmp/stock_market_bytetheory-1.0.2.tar.gz` & `tmp/stock_market_bytetheory-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock_market_bytetheory-1.0.2.tar", last modified: Wed Apr 26 18:39:43 2023, max compression
+gzip compressed data, was "stock_market_bytetheory-1.0.3.tar", last modified: Sun May 14 19:34:16 2023, max compression
```

## Comparing `stock_market_bytetheory-1.0.2.tar` & `stock_market_bytetheory-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-26 18:39:43.912359 stock_market_bytetheory-1.0.2/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.2/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-26 18:39:43.912470 stock_market_bytetheory-1.0.2/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.2/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.2/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-04-26 18:39:43.912807 stock_market_bytetheory-1.0.2/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-26 18:39:43.901199 stock_market_bytetheory-1.0.2/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-26 18:39:43.903030 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)     4896 2023-04-26 18:37:06.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/SP500History.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/SectorIndustryTickerParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2281 2023-04-26 18:36:16.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/TickerLevelDataParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-26 18:39:43.912232 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/SP500_ind.csv
--rw-r--r--   0 robertblom   (501) staff       (20)    60623 2023-04-24 21:18:29.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/SP_500.xml
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-26 18:39:43.904061 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-26 18:39:43.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-04-26 18:39:43.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-04-26 18:39:43.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-04-26 18:39:43.000000 stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.387317 stock_market_bytetheory-1.0.3/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.3/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-05-14 19:34:16.387412 stock_market_bytetheory-1.0.3/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.3/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.3/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-05-14 19:34:16.387755 stock_market_bytetheory-1.0.3/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.380504 stock_market_bytetheory-1.0.3/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.381716 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)     5191 2023-05-14 19:29:32.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SP500History.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SectorIndustryTickerParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2281 2023-04-26 18:36:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/TickerLevelDataParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.387206 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP500_ind.csv
+-rw-r--r--   0 robertblom   (501) staff       (20)    60623 2023-04-24 21:18:29.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP_500.xml
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.382637 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/top_level.txt
```

### Comparing `stock_market_bytetheory-1.0.2/LICENSE` & `stock_market_bytetheory-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.2/setup.cfg` & `stock_market_bytetheory-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stock_market_bytetheory
-version = 1.0.2
+version = 1.0.3
 author = Robbie Blom
 description = Provides some sample stock data and helpers for supporting a stock samples app
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/SP500History.py` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SP500History.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,107 +1,134 @@
-from stock_market_bytetheory import SectorIndustryTickerParser
-from stock_market_bytetheory import TickerLevelDataParser
 import functools
 import pprint as pp
 
-class SP500History():
+from stock_market_bytetheory import SectorIndustryTickerParser, TickerLevelDataParser
 
+
+class SP500History:
     def __init__(self):
-        self.sectorIndustryTickerHierarchy = SectorIndustryTickerParser('SP_500.xml').parse()
-        self.tickerLevelData = TickerLevelDataParser('SP500_ind.csv').parse()
+        self.sectorIndustryTickerHierarchy = SectorIndustryTickerParser(
+            "SP_500.xml"
+        ).parse()
+        self.tickerLevelData = TickerLevelDataParser("SP500_ind.csv").parse()
 
     def getTickersForIndustry(self, industry, sector):
         tickers = self.sectorIndustryTickerHierarchy[sector][industry]
         return tickers
 
     def getAllSectorsAndIndustries(self):
-        return {sector: self.getIndustriesForSector(sector) for sector in self.sectorIndustryTickerHierarchy.keys()}
+        return {
+            sector: self.getIndustriesForSector(sector)
+            for sector in self.sectorIndustryTickerHierarchy.keys()
+        }
 
     def getIndustriesForSector(self, sector):
-        return [industry for industry in self.sectorIndustryTickerHierarchy[sector].keys()]
+        return [
+            industry for industry in self.sectorIndustryTickerHierarchy[sector].keys()
+        ]
 
     def getPricingMetricsForIndustry(self, industry, sector):
         metrics = []
         tickers = self.sectorIndustryTickerHierarchy[sector][industry]
         for ticker in tickers:
-            metrics.append(self.getAllMetricsForTicker(ticker))
+            try:
+                metrics.append(self.getAllMetricsForTicker(ticker))
+            except Exception as e:
+                print(e)
         return metrics
-    
+
     def getAllMetricsForTicker(self, ticker):
         return {
-            'ticker': ticker,
-            'vwap': self.getVolumeWeightedAveragePrice(ticker),
-            'avgOpen': self.getAverageOpenPrice(ticker)
+            "ticker": ticker,
+            "vwap": self.getVolumeWeightedAveragePrice(ticker),
+            "avgOpen": self.getAverageOpenPrice(ticker),
         }
 
     def getVolumeWeightedAveragePrice(self, ticker):
         # Return the volume weighted average price of the stock.  In order to do this,
         # first find the average price of the stock on each day.  Then, multiply that price with the
         # volume on that day.  Take the sum of these values. Finally, divide that value by the sum of all the volumes.
         # (note: average price for each day = (high + low + close)/3)
-
         sumOfWeightedDailyPrices = 0
         sumOfDailyVolume = 0
-        # pp.pprint(self.tickerLevelData.keys())
-        # pp.pprint(self.tickerLevelData['GOOG'])
         for dayOfPriceData in self.tickerLevelData[ticker]:
-            # print(dayOfPriceData)
-            [date, openPrice, highPrice, lowPrice, closePrice, volumeForDay] = dayOfPriceData
-            averagePrice = self.computeAveragePriceForDay(highPrice, lowPrice, closePrice)
-            sumOfWeightedDailyPrices += self.computeWeightedPriceForDay(averagePrice, volumeForDay)
+            [
+                date,
+                openPrice,
+                highPrice,
+                lowPrice,
+                closePrice,
+                volumeForDay,
+            ] = dayOfPriceData
+            averagePrice = self.computeAveragePriceForDay(
+                highPrice, lowPrice, closePrice
+            )
+            sumOfWeightedDailyPrices += self.computeWeightedPriceForDay(
+                averagePrice, volumeForDay
+            )
             sumOfDailyVolume += volumeForDay
-        return float(sumOfWeightedDailyPrices/sumOfDailyVolume)
+        return float(sumOfWeightedDailyPrices / sumOfDailyVolume)
 
     def computeAveragePriceForDay(self, high, low, close):
         return (high + low + close) / 3
 
     def computeWeightedPriceForDay(self, averagePrice, volume):
         return averagePrice * volume
 
     def getAverageOpenPrice(self, ticker):
         return self.sumOfAllOpenPrices(ticker) / self.numberOfOpenPrices(ticker)
-        
+
     def sumOfAllOpenPrices(self, ticker):
         def addOpenPrices(runningSum, dayPrice):
-            openPrice =  dayPrice[2]
+            openPrice = dayPrice[2]
             return runningSum + openPrice
 
         return functools.reduce(addOpenPrices, self.tickerLevelData[ticker], 0)
 
     def numberOfOpenPrices(self, ticker):
         return len(self.tickerLevelData[ticker])
 
     def findReturn(self, ticker, start, end):
         # Uses the opening price on the starting date, and the closing price on the ending date.
         openPriceOnStartDate = self.findOpenPriceOnStartDate(ticker, start)
         closePriceOnEndDate = self.findClosePriceOnEndDate(ticker, end)
-        return float((closePriceOnEndDate - openPriceOnStartDate)/openPriceOnStartDate)
+        return float(
+            (closePriceOnEndDate - openPriceOnStartDate) / openPriceOnStartDate
+        )
 
     def findOpenPriceOnStartDate(self, ticker, startDatetime):
         for dayOfPriceData in self.tickerLevelData[ticker]:
             openPrice = dayOfPriceData[1]
             priceDay = dayOfPriceData[0].day
             priceMonth = dayOfPriceData[0].month
             priceYear = dayOfPriceData[0].year
             startDay = startDatetime[1]
             startMonth = startDatetime[0]
             startYear = startDatetime[2]
-            if(priceDay == startDay and priceMonth == startMonth and priceYear == startYear):
+            if (
+                priceDay == startDay
+                and priceMonth == startMonth
+                and priceYear == startYear
+            ):
                 return openPrice
         else:
-            message = startDatetime.strftime('No data exists for this ticker on the start date of %d, %b %Y')
+            message = startDatetime.strftime(
+                "No data exists for this ticker on the start date of %d, %b %Y"
+            )
             raise Exception(message)
 
     def findClosePriceOnEndDate(self, ticker, closeDatetime):
         for dayOfPriceData in self.tickerLevelData[ticker]:
             closePrice = dayOfPriceData[4]
             priceDay = dayOfPriceData[0].day
             priceMonth = dayOfPriceData[0].month
             priceYear = dayOfPriceData[0].year
             endDay = closeDatetime[1]
             endMonth = closeDatetime[0]
             endYear = closeDatetime[2]
-            if(priceDay == endDay and priceMonth == endMonth and priceYear == endYear):
+            if priceDay == endDay and priceMonth == endMonth and priceYear == endYear:
                 return closePrice
         else:
-            message = closeDatetime.strftime('No data exists for this ticker on the end date of %d, %b %Y')
-            raise Exception(message)
+            message = closeDatetime.strftime(
+                "No data exists for this ticker on the end date of %d, %b %Y"
+            )
+            raise Exception(message)
```

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/SectorIndustryTickerParser.py` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SectorIndustryTickerParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/TickerLevelDataParser.py` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/TickerLevelDataParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/SP500_ind.csv` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP500_ind.csv`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory/data/SP_500.xml` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP_500.xml`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.2/src/stock_market_bytetheory.egg-info/SOURCES.txt` & `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

