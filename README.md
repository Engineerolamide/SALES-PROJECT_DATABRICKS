# SALES-ANALYTICS

This project demonstrates a modern data engineering workflow using Azure Data Factory, Azure Data Lake Storage, and Databricks. It follows the medallion architecture — organizing data into Bronze, Silver, and Gold layers for scalable transformation and analytics.

ARCHITECTURE OVERVIEW
![Architecture Diagram](architecture.png)

- Bronze Layer: Raw ingestion from source systems
- Silver Layer: Cleaned and enriched data
- Gold Layer: Aggregated, business-ready datasets

 TOOLS USED

- Azure Data Factory (ADF): Orchestration of data pipelines
- Azure Data Lake Storage (ADLS): Scalable cloud storage
- Databricks: Data transformation using PySpark
- GitHub: Version control and collaboration


ADF PIPELINES

| Pipeline | File | Purpose |
|----------|------|---------|
| Ingestion | [`ingest_pipeline.json`](adf-pipelines/ingest_pipeline.json) | Pulls raw data into ADLS |

DATASETS

| File | Description |
|------|-------------|
| [`sales_data.csv`](datasets/sales_data.csv) | Sample sales data used for pipeline |
| [`README.md`](datasets/README.md) | Schema and source info |


HOW TO RUN

1. Clone this repo
2. Deploy ADF pipelines using the JSON templates
3. Mount ADLS in Databricks
4. Run notebooks in order: Bronze → Silver → Gold
5. Explore results in `/mnt/...` or visualize in Power BI

CONTACT

For questions or collaboration, feel free to open an issue or reach out via email: Olamidehgold@gmail.com

