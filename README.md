# Azure Databricks Delta Analytics

This repository demonstrates how to build a modern analytics architecture using Azure Databricks, Delta Lake, and other Azure services. Whether you're working with data, analytics, or AI, this repository provides insights on how to unify your workloads at any scale.

## Solution Overview

- **Azure Databricks**: The core of our solution. It seamlessly integrates with other services.
- **Data Lake Storage Gen2**: Stores various data types (structured, unstructured, semi-structured), both batch and streaming data.
- **Delta Lake**: Curates and refines data in an open-source format.
- **Medallion Architecture**:
    - **Bronze Layer**: Holds raw data.
    - **Silver Layer**: Contains cleaned, filtered data.
    - **Gold Layer**: Stores aggregated data for business analytics.
![delta-lake-medallion-architecture-2](https://github.com/AnthonyByansi/azure-databricks-delta-analytics/assets/101401469/b589cf7f-999b-4e82-82c3-ae4228e2ff20)


## Data Science Workflow

1. **Ingestion**:
    - Raw streaming data from **Azure Event Hubs** is ingested by **Azure Databricks**.
    - Raw batch data is loaded into **Data Lake Storage Gen2** via **Data Factory**.

2. **Data Preparation and Exploration**:
    - Data scientists use the ingested data for tasks such as:
        - Data preparation
        - Data exploration
        - Model preparation
        - Model training

3. **Machine Learning**:
    - **MLflow** manages parameter, metric, and model tracking in data science code runs.
    - Code flexibility: Use SQL, Python, R, or Scala.
    - Leverage popular open-source libraries like Koalas, Pandas, and scikit-learn.

4. **Model Deployment**:
    - Models are stored in the **MLflow Model Registry**.
    - Accessible via batch, streaming, and REST APIs.

## Get Started

1. Clone this repository.
2. Set up your Azure Databricks workspace.
3. Explore the notebooks and examples provided.

## Feedback

We'd love to hear your feedback! If you have suggestions, use cases, or pricing considerations, let us know by providing feedback.
