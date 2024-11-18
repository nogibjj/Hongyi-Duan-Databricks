# Hongyi-Duan-Databricks

[![Data Pipeline](https://github.com/nogibjj/Hongyi-Duan-Databricks/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/Hongyi-Duan-Databricks/actions/workflows/cicd.yml)

This repository demonstrates the implementation and usage of **Databricks**, a unified data analytics platform, for performing various data engineering and data science tasks. The repository contains files and scripts that showcase key functionalities such as data ingestion, transformation, and exploratory data analysis.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [Usage](#usage)
5. [Databricks Features Used](#databricks-features-used)
6. [FAQs](#faqs)
7. [Acknowledgments](#acknowledgments)

---

## Overview
Databricks is an enterprise-level collaborative platform for big data analytics and machine learning. Built on Apache Spark, Databricks provides a unified environment for working with data engineering, data science, and business analytics projects.

This project includes examples of how to:
- Upload and manage files in Databricks File System (DBFS).
- Create and interact with notebooks for running PySpark and Python scripts.
- Perform basic data transformations and analysis using Python and Spark.
- Set up and manage a project using GitHub integration.

---

## Features
This project demonstrates the following Databricks capabilities:
- **Data Engineering**: Data ingestion from different sources, such as DBFS and external APIs.
- **Notebook Execution**: Running Python and PySpark scripts in an interactive environment.
- **File Management**: Uploading and reading files using Databricks' DBFS.
- **Integration**: GitHub integration for source control and CI/CD pipelines.
- **Exploratory Data Analysis (EDA)**: Analyzing datasets using Pandas and Spark DataFrames.

---

## Getting Started

### Prerequisites
To run this project, you need:
1. Access to a Databricks workspace.
2. Basic understanding of Python and Spark.
3. The following Python libraries installed:
   - `pandas`
   - `pyspark`
   - `openpyxl` (for reading Excel files)
   - Other dependencies listed in `requirements.txt`.

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/nogibjj/Hongyi-Duan-Databricks.git
   cd Hongyi-Duan-Databricks
   ```
2. Set up a virtual environment (optional):
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. Upload the necessary files to your Databricks workspace:
   - Navigate to **Data > DBFS > Upload File**.
   - Select the files from this repository.

<img width="1274" alt="1731903329150" src="https://github.com/user-attachments/assets/8ac603c3-18d6-4ea6-910c-23a1c5161c4c">

4. Import the `.py` scripts into a Databricks notebook or workspace.

---

## Usage

### Running on Databricks
1. Upload files such as `nba_elo_latest.csv` and `nba_draft_2015.csv` to DBFS.
2. Open the notebook or workspace where the scripts are imported.
3. Run the main script (`main.py`) using the following steps:
   - Set up your cluster in Databricks.
   - Attach the notebook to the cluster.
   - Execute the code cells.

<img width="1274" alt="1731903226569" src="https://github.com/user-attachments/assets/4c2f4652-bc8e-4de8-9ab8-ea1ba7e37f77">

### Local Development
You can run the scripts locally by executing:
```bash
python main.py
```

### File Management in DBFS
To list files in DBFS, you can use:
```python
dbutils.fs.ls("/FileStore/tables/")
```

---

## Databricks Features Used
1. **Databricks File System (DBFS):**
   - Used to store datasets (`nba_elo_latest.csv`, `nba_draft_2015.csv`) and scripts.
   - Accessible with paths like `/FileStore/tables/`.

2. **Notebooks:**
   - Interactive development environment for Python and PySpark scripts.

3. **Clusters:**
   - Computing resources for executing tasks at scale.

4. **Data Ingestion:**
   - Uploading and reading data using Pandas and Spark.

5. **Integration:**
   - GitHub Actions for CI/CD pipeline automation.

---
