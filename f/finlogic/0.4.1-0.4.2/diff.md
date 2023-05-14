# Comparing `tmp/finlogic-0.4.1.tar.gz` & `tmp/finlogic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.1.tar", last modified: Sun May  7 10:59:19 2023, max compression
+gzip compressed data, was "finlogic-0.4.2.tar", last modified: Sun May 14 15:29:06 2023, max compression
```

## Comparing `finlogic-0.4.1.tar` & `finlogic-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.1/LICENSE
--rw-r--r--   0        0        0     9725 2023-05-05 00:53:46.488832 finlogic-0.4.1/README.md
--rw-r--r--   0        0        0      423 2023-05-05 00:53:46.488832 finlogic-0.4.1/finlogic/__init__.py
--rw-r--r--   0        0        0    23311 2023-05-07 10:50:55.631688 finlogic-0.4.1/finlogic/company.py
--rw-r--r--   0        0        0      314 2023-05-07 10:50:55.631688 finlogic-0.4.1/finlogic/config.py
--rw-r--r--   0        0        0     7556 2023-05-07 10:50:55.631688 finlogic-0.4.1/finlogic/cvm.py
--rw-r--r--   0        0        0     7643 2023-05-07 10:50:55.631688 finlogic-0.4.1/finlogic/database.py
--rw-r--r--   0        0        0      687 2023-05-07 10:50:55.631688 finlogic-0.4.1/finlogic/language.py
--rw-r--r--   0        0        0      985 2023-05-07 10:59:19.583523 finlogic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     3396 2023-04-25 23:39:05.128133 finlogic-0.4.1/tests/test_company.py
--rw-r--r--   0        0        0      884 2023-05-04 10:34:46.695519 finlogic-0.4.1/tests/test_database.py
--rw-r--r--   0        0        0    11741 1970-01-01 00:00:00.000000 finlogic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.2/LICENSE
+-rw-r--r--   0        0        0     9612 2023-05-14 10:36:12.075362 finlogic-0.4.2/README.md
+-rw-r--r--   0        0        0      423 2023-05-12 00:21:10.028393 finlogic-0.4.2/finlogic/__init__.py
+-rw-r--r--   0        0        0    23323 2023-05-14 15:04:47.182513 finlogic-0.4.2/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.2/finlogic/config.py
+-rw-r--r--   0        0        0     9656 2023-05-14 15:04:47.183513 finlogic-0.4.2/finlogic/cvm.py
+-rw-r--r--   0        0        0     4357 2023-05-14 15:04:47.183513 finlogic-0.4.2/finlogic/database.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.2/finlogic/finprint.py
+-rw-r--r--   0        0        0     3223 2023-05-14 15:11:20.236277 finlogic-0.4.2/finlogic/fl_duckdb.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.2/finlogic/language.py
+-rw-r--r--   0        0        0     1005 2023-05-14 15:29:06.969571 finlogic-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.2/tests/test_company.py
+-rw-r--r--   0        0        0      902 2023-05-14 15:04:47.183513 finlogic-0.4.2/tests/test_database.py
+-rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 finlogic-0.4.2/PKG-INFO
```

### Comparing `finlogic-0.4.1/LICENSE` & `finlogic-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.1/README.md` & `finlogic-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,44 +14,36 @@
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
 
-Binary installers for the latest released version are available at the [Python
-Package Index (PyPI)](https://pypi.org/project/finlogic) and on [Conda](https://anaconda.org/conda-forge/finlogic).
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/finlogic).
 
 ```sh
 # PyPI:
 pip install finlogic
 ```
 
-<!--
-```sh
-# Conda:
-conda install -c conda-forge finlogic
-```
--->
-
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0)
-- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
+- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0
+- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0
 - [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [Rich](https://github.com/Textualize/rich) \>= 13.0.0
 
 ---
 
 ## Quick Start
 
-### Create FinLogic Local Database
+### Create FinLogic Database
 
-The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 21 millions rows of accounting values and loading it into FinLogic Database for local data analysis.
-In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed and loaded into the database, which will be a lot faster.
+The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 8 millions rows of accounting values and loading it into FinLogic Database for local data analysis. In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed, which will be faster.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
 >>> fl.update_database()
 
@@ -66,15 +58,15 @@
 | FinLogic Database Info      |                       Value |
 | :-------------------------- | --------------------------: |
 | Data path                   | /.../FinLogic/finlogic/data |
 | File size (MB)              |                       301.0 |
 | Last update call            |         2022-04-20 07:29:08 |
 | Last modified               |         2022-04-20 07:31:48 |
 | Last updated data           |         2022-04-17 13:09:01 |
-| Accounting rows             |                  18,757,249 |
+| Accounting rows             |                   8,757,249 |
 | Unique accounting codes     |                       2,008 |
 | Number of companies         |                       1,037 |
 | Unique Financial Statements |                      13,172 |
 | First Financial Statement   |                  2009-01-31 |
 | Last Financial Statement    |                  2023-03-31 |
 
 ```python
```

### Comparing `finlogic-0.4.1/finlogic/company.py` & `finlogic-0.4.2/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     method has to use engine='python' to work with category dtype. N.B. Only
     FinLogic Dataframe uses category dtype for efficiency.
 
 """
 from typing import Literal
 import numpy as np
 import pandas as pd
-from .config import fldb
 from .language import language_df
+from .finprint import print_dict
+from .fl_duckdb import execute
 
 
 class Company:
     """A class to represent a company financial data.
 
     This class provides methods to create financial reports and to calculate
     financial indicators based on a company's accounting data. The class also
@@ -82,30 +83,28 @@
             KeyError: If the given identifier isn't found in Finlogic Database.
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
-        query = """
-            SELECT DISTINCT co_id, co_fiscal_id
-            FROM reports
-        """
-        df = fldb.execute(query).df()
-        if identifier in df["co_id"].to_list():
-            self._co_id = identifier
-            mask = df["co_id"] == identifier
-            self._co_fiscal_id = df.loc[mask, "co_fiscal_id"].item()
-        elif identifier in df["co_fiscal_id"].to_list():
-            self._co_fiscal_id = identifier
-            mask = df["co_fiscal_id"] == identifier
-            self._co_id = df.loc[mask, "co_id"].item()
+        query = f"""
+            SELECT DISTINCT cvm_id, tax_id, name_id
+              FROM reports
+             WHERE CAST(cvm_id AS VARCHAR) = '{identifier}'
+                OR tax_id = '{identifier}'
+        """
+        df = execute(query, "df")
+        if not df.empty:
+            self._cvm_id = df.loc[0, "cvm_id"]
+            self.tax_id = df.loc[0, "tax_id"]
+            self.name_id = df.loc[0, "name_id"]
+            self._identifier = identifier
         else:
-            raise KeyError("Company 'identifier' not found in FinLogic Database")
-        self._identifier = identifier
+            raise KeyError(f"Company 'identifier' {identifier} not found.")
         # If object was already initialized, reset company dataframe
         if self._initialized:
             self._set_co_df()
 
     @property
     def acc_method(self) -> Literal["consolidated", "separate"]:
         """Gets or sets the accounting method for registering investments in
@@ -240,39 +239,36 @@
         """Sets the company data frame.
 
         This method creates a data frame with the company's financial
         statements.
         """
         # Create the company data frame
         query = f"""
-            SELECT  *
-            FROM    reports
-            WHERE   co_id = {self._co_id} AND acc_method = '{self._acc_method}'
-            ORDER   BY acc_code, period_reference, period_end
+            SELECT *
+              FROM reports
+             WHERE cvm_id = {self._cvm_id}
+               AND acc_method = '{self._acc_method}'
+             ORDER BY acc_code, period_reference, period_end
         """
-        co_df = fldb.execute(query).df()
+        co_df = execute(query, "df")
 
         # Change acc_unit only for accounts different from 3.99
         co_df["acc_value"] = np.where(
             co_df["acc_code"].str.startswith("3.99"),
             co_df["acc_value"],
             co_df["acc_value"] / self._acc_unit,
         )
+        annual_reports = co_df.query('report_type == "ANNUAL"')
+        self._first_annual = annual_reports["period_end"].min()
+        self._last_annual = annual_reports["period_end"].max()
+        quarterly_reports = co_df.query('report_type == "QUARTERLY"')
+        self._last_quarterly = quarterly_reports["period_end"].max()
 
-        self._name = co_df["co_name"].iloc[0]
-        expr = 'report_type == "ANNUAL"'
-        self._first_annual = co_df.query(expr)["period_end"].min()
-        self._last_annual = co_df.query(expr)["period_end"].max()
-        expr = 'report_type == "QUARTERLY"'
-        self._last_quarterly = co_df.query(expr)["period_end"].max()
-
-        # Drop columns that are already company properties
-        co_df.drop(
-            columns=["co_name", "co_id", "co_fiscal_id", "acc_method"], inplace=True
-        )
+        # Drop columns that are already company atributes
+        co_df.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
 
         # Keep only the newest 'report_version' in df
         cols = [
             "report_type",
             "report_version",
             "period_reference",
             "period_order",
@@ -285,28 +281,29 @@
         # Ascending order --> last is the newest report_version
         co_df.drop_duplicates(cols, keep="last", inplace=True, ignore_index=True)
 
         # Set company data frame
         self._co_df = co_df
 
     def info(self) -> dict:
-        """Return a dictionay with company info."""
+        """Print a concise summary of a company."""
         company_info = {
-            "Name": self._name,
-            "CVM ID": self._co_id,
-            "Fiscal ID (CNPJ)": self._co_fiscal_id,
+            "Name": self.name_id,
+            "CVM ID": self._cvm_id,
+            "Fiscal ID (CNPJ)": self.tax_id,
             "Total Accounting Rows": len(self._co_df.index),
-            "Selected Tax Rate": self._tax_rate,
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
+            "Selected Tax Rate": self._tax_rate,
             "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
             "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
             "Last Quarterly Report": self._last_quarterly.strftime("%Y-%m-%d"),
         }
-        return company_info
+        print_dict(info_dict=company_info, table_name="Company Info")
+        return None
 
     def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # keep only last quarterly fs
         if self._last_annual > self._last_quarterly:
             df = dfi.query('report_type == "ANNUAL"').copy()
             df.query(
                 "period_order == 'PREVIOUS' or \
@@ -449,14 +446,16 @@
         report_df = self._build_report(df)
         report_df.set_index(keys="acc_code", drop=True, inplace=True)
         # Show only selected years
         if num_years > 0:
             cols = report_df.columns.to_list()
             cols = cols[0:2] + cols[-num_years:]
             report_df = report_df[cols]
+        # Fill NaN values with 0
+        report_df.fillna(0, inplace=True)
         return report_df
 
     def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
         if self._last_annual > self._last_quarterly:
             return dfi.query('report_type == "ANNUAL"').copy()
 
         df1 = dfi.query("period_end == @self._last_quarterly").copy()
```

### Comparing `finlogic-0.4.1/finlogic/cvm.py` & `finlogic-0.4.2/finlogic/cvm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""CVM Portal data management."""
+"""Module to download and process CVM data."""
 import re
-from typing import List
+from typing import List, Dict
 import zipfile as zf
 from pathlib import Path
+import duckdb
 import pandas as pd
 import requests
 from . import config as cfg
 
 URL_DFP = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
 
 CHECKMARK = "\033[32m\u2714\033[0m"
-CVM_DIR = cfg.DATA_PATH / "cvm"
-# Create CVM_DIR if it does not exist
-Path.mkdir(CVM_DIR, parents=True, exist_ok=True)
 
 
-def get_files_urls(cvm_url) -> List[str]:
+def get_file_urls(cvm_url) -> List[str]:
     """Return a list of available CVM files.
 
     Urls with CVM raw files:
     https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/
     https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/
     Links example:
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/dfp_cia_aberta_2020.zip
@@ -36,134 +34,143 @@
     available_files.extend(matches)
     available_files.sort()
     # Add the base url to the filename
     available_file_urls = [cvm_url + filename for filename in available_files]
     return available_file_urls
 
 
-def get_all_files_urls() -> List[str]:
+def get_all_file_urls() -> List[str]:
     """Return a list of all available CVM files."""
-    urls_dfp = get_files_urls(URL_DFP)
-    urls_itr = get_files_urls(URL_ITR)
+    urls_dfp = get_file_urls(URL_DFP)
+    urls_itr = get_file_urls(URL_ITR)
     # Get only the last 3 QUARTERLY reports
     urls_itr = urls_itr[-3:]
     urls = urls_dfp + urls_itr
     return urls
 
 
-def update_cvm_file(url: str, s) -> str:
+def update_raw_file(url: str, s: requests.Session) -> Path:
     """Update raw file from CVM portal. Return a Path if file is updated."""
     filename = url[-23:]  # filename = end of url
-    filepath = Path(CVM_DIR, filename)
+    filepath = cfg.CVM_RAW_DIR / filename
     headers = s.head(url).headers
-    # Get the filesize from the local file
     filesize = filepath.stat().st_size if filepath.exists() else 0
-    # Compare the filesize with the Content-Length header
     if filesize == int(headers["Content-Length"]):
-        # File is the same, no need to update it
-        print(f"    - {filename} already updated.")
+        print(f"    - {filename} is the same -> skip.")
         return None
     r = s.get(url)
     if r.status_code != 200:
         return None
 
-    # Save the file with Pathlib
+    # Save file with Pathlib
     filepath.write_bytes(r.content)
     print(f"    {CHECKMARK} {filename} updated.")
 
-    return filename
+    return filepath
 
 
-def update_cvm_files(urls: str) -> List[str]:
+def update_raw_files(urls: str) -> List[Path]:
     """Update CVM raw files."""
     s = requests.Session()
-    updated_filenames = []
-    for url in urls:
-        updated_filenames.append(update_cvm_file(url, s))
+    updated_filepaths = [update_raw_file(url, s) for url in urls]
     s.close()
-    updated_filenames = [filename for filename in updated_filenames if filename]
-    return updated_filenames
+    return [filepath for filepath in updated_filepaths if filepath is not None]
 
 
-def read_cvm_file(cvm_filename: str) -> pd.DataFrame:
+def read_raw_file(filepath: Path) -> pd.DataFrame:
     """Read annual file, process it, save the result and return the file path."""
-    df = pd.DataFrame()
-    cvm_filepath = Path(CVM_DIR, cvm_filename)
-    annual_zipfile = zf.ZipFile(cvm_filepath)
-    child_filenames = annual_zipfile.namelist()
+    cvm_zipfile = zf.ZipFile(filepath)
+    child_filenames = cvm_zipfile.namelist()
 
-    df_list = []
-    for child_filename in child_filenames[1:]:
-        child_file = annual_zipfile.open(child_filename)
-
-        # Only "DT_INI_EXERC" and "COLUNA_DF" have missing values.
-        child_df = pd.read_csv(
-            child_file,
-            sep=";",
-            encoding="iso-8859-1",
-            true_values=["S"],
-            false_values=["N"],
-        )
-        # Currency column has only one value (BRL) so it is not necessary.
-        child_df = child_df.drop(columns=["MOEDA"])
-
-        # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
-        if cvm_filepath.name.startswith("dfp"):
-            child_df["TIPO"] = "ANNUAL"
-        else:
-            child_df["TIPO"] = "QUARTERLY"
+    # Filename example for the first file in zip: "dfp_cia_aberta_2022.csv"
+    # Do not read the first file, since it is a metadata file.
+    child_filenames = child_filenames[1:]
 
+    df_list = []
+    for child_filename in child_filenames:
+        child_zf = cvm_zipfile.open(child_filename)
+        child_df = pd.read_csv(child_zf, sep=";", encoding="iso-8859-1")
         df_list.append(child_df)
-
     df = pd.concat(df_list, ignore_index=True)
-    df["ARQUIVO"] = cvm_filepath.name
-    # Convert string columns to categorical.
-    columns = df.select_dtypes(include="object").columns
-    df[columns] = df[columns].astype("category")
     return df
 
 
-def format_cvm_df(df: pd.DataFrame) -> pd.DataFrame:
+def remove_empty_spaces(s: pd.Series) -> pd.Series:
+    """Remove empty spaces in a pandas Series of strings."""
+    s_unique_original = pd.Series(s.unique())
+    s_unique_adjusted = s_unique_original.replace("\s+", " ", regex=True).str.strip()
+    mapping_dict = dict(zip(s_unique_original, s_unique_adjusted))
+    return s.map(mapping_dict)
+
+
+def process_df(df: pd.DataFrame, filepath: Path) -> pd.DataFrame:
     """Format a cvm dataframe."""
     columns_translation = {
-        "DENOM_CIA": "co_name",
-        "CD_CVM": "co_id",
-        "CNPJ_CIA": "co_fiscal_id",
-        "TIPO": "report_type",
+        "DENOM_CIA": "name_id",
+        "CD_CVM": "cvm_id",
+        "CNPJ_CIA": "tax_id",
         "VERSAO": "report_version",
         "DT_REFER": "period_reference",
         "DT_INI_EXERC": "period_begin",
         "DT_FIM_EXERC": "period_end",
         "ORDEM_EXERC": "period_order",
         "CD_CONTA": "acc_code",
         "DS_CONTA": "acc_name",
         "ST_CONTA_FIXA": "acc_fixed",
         "VL_CONTA": "acc_value",
-        "COLUNA_DF": "equity_statement_column",
-        "ARQUIVO": "data_source",
+        "COLUNA_DF": "equity_statement",
         # Columns below will be dropped after processing.
         "GRUPO_DFP": "report_group",
+        "MOEDA": "Currency",
         "ESCALA_MOEDA": "currency_unit",
     }
     df = df.rename(columns=columns_translation)[columns_translation.values()]
 
+    # Currency column has only one value (BRL) so it is not necessary.
+    df = df.drop(columns=["Currency"])
+
+    # Remove rows with acc_value == 0 and acc_fixed == False
+    df.query("acc_value != 0 or acc_fixed == True", inplace=True)
+
+    # report_version max. value is aprox. 9, so it can be uint8 (0 to 255)
+    df["report_version"] = df["report_version"].astype("uint8")
+    # cvm_id from max. value is 600_000, so it can be uint32 (0 to 4_294_967_295)
+    df["cvm_id"] = df["cvm_id"].astype("uint32")
+    # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
+    # In database, "report_type" is positioned after "tax_id" -> position = 3
+    if filepath.name.startswith("dfp"):
+        df.insert(loc=3, column="report_type", value="ANNUAL")
+    else:
+        df.insert(loc=3, column="report_type", value="QUARTERLY")
+
+    # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
+    columns = ["name_id", "acc_name", "equity_statement"]
+    df[columns] = df[columns].apply(remove_empty_spaces)
+
+    # Convert string columns to categorical before mapping.
+    columns = df.select_dtypes(include="object").columns
+    df[columns] = df[columns].astype("category")
+
+    # "acc_fixed" values are: 'S', 'N'
+    map_dic = {"S": True, "N": False}
+    df["acc_fixed"] = df["acc_fixed"].map(map_dic).astype(bool)
     # currency_unit values are ['MIL', 'UNIDADE']
-    map_dict = {"UNIDADE": 1, "MIL": 1000}
-    df["currency_unit"] = df["currency_unit"].map(map_dict).astype(int)
+    map_dic = {"UNIDADE": 1, "MIL": 1000}
+    df["currency_unit"] = df["currency_unit"].map(map_dic).astype(int)
 
     # Do not ajust acc_value for 3.99 codes.
     df["acc_value"] = df["acc_value"].where(
         df["acc_code"].str.startswith("3.99"),
         df["acc_value"] * df["currency_unit"],
     )
     df.drop(columns=["currency_unit"], inplace=True)
 
     # "period_order" values are: 'ÚLTIMO', 'PENÚLTIMO'
-    map_dict = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
-    df["period_order"] = df["period_order"].map(map_dict)
+    map_dic = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
+    df["period_order"] = df["period_order"].map(map_dic)
     """
     acc_method -> Financial Statemen Type
     Consolidated and Separate Financial Statements (IAS 27/2003)
     df['GRUPO_DFP'].unique() result:
         'DF Consolidado - Balanço Patrimonial Ativo',
         'DF Consolidado - Balanço Patrimonial Passivo',
         'DF Consolidado - Demonstração das Mutações do Patrimônio Líquido',
@@ -178,26 +185,60 @@
         'DF Individual - Demonstração de Valor Adicionado',
         'DF Individual - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
-    map_dict = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
-    df.insert(9, "acc_method", df["report_group"].str[3:6].map(map_dict))
+    map_dic = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
+    df.insert(9, "acc_method", df["report_group"].str[3:6].map(map_dic))
     # 'GRUPO_DFP' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
+
     # Correct/harmonize some account texts.
-    df["acc_name"].replace(to_replace=["\xa0ON\xa0", "On"], value="ON", inplace=True)
-    # From 20_636_037 rows 2_383 were duplicated on 2023-04-30 -> remove duplicates
+    # df["acc_name"].replace(to_replace=["\xa0ON\xa0", "On"], value="ON", inplace=True)
+
+    # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
+    # Few of them have different values in "acc_value". Only one them will be kept.
+    # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
     cols.remove("acc_value")
-    df.drop_duplicates(subset=cols, keep="last", inplace=True)
+    df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
+
+    # Add column for file source and file modification time.
+    df["file_source"] = filepath.name
+    df["file_mtime"] = filepath.stat().st_mtime
 
     return df
 
 
-def process_cvm_file(cvm_filename: str) -> pd.DataFrame:
-    """Read and format a CVM file."""
-    df = read_cvm_file(cvm_filename)
-    df = format_cvm_df(df)
-    return df
+def save_processed_df(df: pd.DataFrame, filepath: Path) -> None:
+    """Save a processed dataframe as a csv file."""
+    with duckdb.connect() as con:
+        sql = f"""
+            CREATE TEMP TABLE tbl AS SELECT * FROM df;
+            ALTER TABLE tbl ALTER period_reference TYPE DATE;
+            ALTER TABLE tbl ALTER period_begin TYPE DATE;
+            ALTER TABLE tbl ALTER period_end TYPE DATE;
+            COPY tbl TO '{filepath}' (FORMAT 'PARQUET', COMPRESSION 'zstd')
+        """
+        con.execute(sql)
+
+
+def process_file(raw_filepath: Path) -> Path:
+    """Read, process and save a CVM file."""
+    df = read_raw_file(raw_filepath)
+    df = process_df(df, raw_filepath)
+    processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".parquet")
+    save_processed_df(df, processed_filepath)
+    print(f"    {CHECKMARK} {raw_filepath.name} processed.")
+    return processed_filepath
+
+
+def get_raw_files_mtime() -> Dict[str, float]:
+    """Return a dictionary with the files and their modification time."""
+    raw_filepaths = list(cfg.CVM_RAW_DIR.glob("*.zip"))
+    raw_filepaths.sort()
+    files_mtime = {}
+    for filepath in raw_filepaths:
+        files_mtime[filepath.name] = filepath.stat().st_mtime
+    return files_mtime
```

### Comparing `finlogic-0.4.1/finlogic/language.py` & `finlogic-0.4.2/finlogic/language.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from . import config as cfg
 
 INTERIM_DIR = cfg.DATA_PATH / "interim"
 LANGUAGE_DF_PATH = INTERIM_DIR / "pten_df.csv"
 URL_LANGUAGE = "https://raw.githubusercontent.com/fe-lipe-c/finlogic_datasets/master/data/pten_df.csv"  # noqa
 
-# Create interim folder if itdoes not exist.
+# Create interim folder if it does not exist.
 Path.mkdir(INTERIM_DIR, parents=True, exist_ok=True)
 
 # Start/load language file data
 if LANGUAGE_DF_PATH.is_file():
     language_df = pd.read_csv(LANGUAGE_DF_PATH)
 else:
     language_df = pd.DataFrame()
```

### Comparing `finlogic-0.4.1/pyproject.toml` & `finlogic-0.4.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "duckdb>=0.7.0",
+    "rich>=13.0.0",
 ]
-version = "0.4.1"
+version = "0.4.2"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `finlogic-0.4.1/tests/test_company.py` & `finlogic-0.4.2/tests/test_company.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,36 @@
     def setUp(self):
         self.petro_sep = fl.Company(9512, acc_method="separate", acc_unit="billion")
         self.petro_con = fl.Company(9512, acc_method="consolidated", acc_unit="billion")
 
     def test_identifier(self):
         """Test the identifier method of the Company class.""" ""
         test_cvm_id = 4170
-        test_fiscal_id = "33.592.510/0001-54"
+        test_tax_id = "33.592.510/0001-54"
         self.petro_sep.identifier = test_cvm_id
-        self.assertEqual(self.petro_sep._co_id, test_cvm_id)
-        self.assertEqual(self.petro_sep._co_fiscal_id, test_fiscal_id)
+        self.assertEqual(self.petro_sep._cvm_id, test_cvm_id)
+        self.assertEqual(self.petro_sep.tax_id, test_tax_id)
 
-        self.petro_sep.identifier = test_fiscal_id
-        self.assertEqual(self.petro_sep._co_id, test_cvm_id)
-        self.assertEqual(self.petro_sep._co_fiscal_id, test_fiscal_id)
+        self.petro_sep.identifier = test_tax_id
+        self.assertEqual(self.petro_sep._cvm_id, test_cvm_id)
+        self.assertEqual(self.petro_sep.tax_id, test_tax_id)
 
         invalid_identifier = 99999999  # Use an invalid identifier here
 
         with self.assertRaises(
             KeyError, msg="Should raise a KeyError with an invalid identifier"
         ):
             self.petro_sep.identifier = invalid_identifier
 
-    def test_info(self):
+    def test_atributes(self):
         """Test the info method of the Company class."""
-        # Get the info
-        petro_info = self.petro_sep.info()
-        # Check the info
-        self.assertEqual(petro_info["Name"], "PETROLEO BRASILEIRO S.A. PETROBRAS")
-        self.assertEqual(petro_info["CVM ID"], 9512)
-        self.assertEqual(petro_info["Fiscal ID (CNPJ)"], "33.000.167/0001-01")
+        # Check the attributes
+        self.assertEqual(self.petro_sep.name_id, "PETROLEO BRASILEIRO S.A. PETROBRAS")
+        self.assertEqual(self.petro_sep._cvm_id, 9512)
+        self.assertEqual(self.petro_sep.tax_id, "33.000.167/0001-01")
 
     def test_report(self):
         """Test if the report method of the Company class returns the correct
         values."""
         petro_report = self.petro_con.report(report_type="assets")
         # Get Total Assets
         assets_2009 = round(petro_report.at["1", "2009-12-31"], 3)
```

### Comparing `finlogic-0.4.1/tests/test_database.py` & `finlogic-0.4.2/tests/test_database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import unittest
 import finlogic as fl
+from finlogic import fl_duckdb as fdb
 
 
 class TestDatabase(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
-        db_info = fl.database_info()
-        self.assertEqual(db_info["First financial statement"], "2009-01-31")
-        self.assertTrue(db_info["Accounting rows"] > 20_000_000)
+        db_info = fdb.get_info()
+        self.assertEqual(db_info["first_report"], "2009-01-31")
+        self.assertTrue(db_info["number_of_rows"] > 8_000_000)
 
     def test_search_company(self):
         """Test the search_company method of the Database module."""
         search_result = fl.search_company("petrobras")
         """
-            co_name                            co_id  co_fiscal_id
+            name_id                            cvm_id  tax_id
         0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
         1   PETROLEO BRASILEIRO S.A. PETROBRAS   9512  33.000.167/0001-01
         """
         # Check the results
-        self.assertEqual(set(search_result["id"]), {9512, 24295})
+        self.assertEqual(set(search_result["cvm_id"]), {9512, 24295})
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `finlogic-0.4.1/PKG-INFO` & `finlogic-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -31,14 +31,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: duckdb>=0.7.0
+Requires-Dist: rich>=13.0.0
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
@@ -55,44 +56,36 @@
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
 
-Binary installers for the latest released version are available at the [Python
-Package Index (PyPI)](https://pypi.org/project/finlogic) and on [Conda](https://anaconda.org/conda-forge/finlogic).
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/finlogic).
 
 ```sh
 # PyPI:
 pip install finlogic
 ```
 
-<!--
-```sh
-# Conda:
-conda install -c conda-forge finlogic
-```
--->
-
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0)
-- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
+- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0
+- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0
 - [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [Rich](https://github.com/Textualize/rich) \>= 13.0.0
 
 ---
 
 ## Quick Start
 
-### Create FinLogic Local Database
+### Create FinLogic Database
 
-The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 21 millions rows of accounting values and loading it into FinLogic Database for local data analysis.
-In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed and loaded into the database, which will be a lot faster.
+The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 8 millions rows of accounting values and loading it into FinLogic Database for local data analysis. In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed, which will be faster.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
 >>> fl.update_database()
 
@@ -107,15 +100,15 @@
 | FinLogic Database Info      |                       Value |
 | :-------------------------- | --------------------------: |
 | Data path                   | /.../FinLogic/finlogic/data |
 | File size (MB)              |                       301.0 |
 | Last update call            |         2022-04-20 07:29:08 |
 | Last modified               |         2022-04-20 07:31:48 |
 | Last updated data           |         2022-04-17 13:09:01 |
-| Accounting rows             |                  18,757,249 |
+| Accounting rows             |                   8,757,249 |
 | Unique accounting codes     |                       2,008 |
 | Number of companies         |                       1,037 |
 | Unique Financial Statements |                      13,172 |
 | First Financial Statement   |                  2009-01-31 |
 | Last Financial Statement    |                  2023-03-31 |
 
 ```python
```

