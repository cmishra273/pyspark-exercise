# PySpark Assignment

## Project Overview
This project aims to process and analyze store location data using PySpark. The key tasks include data extraction, transformation, and anonymization to ensure GDPR compliance.

## Setup Instructions
1. Install dependencies:
    ```bash
    apt-get install openjdk-11-jdk-headless -qq > /dev/null
    wget -q https://archive.apache.org/dist/spark/spark-3.4.1/spark-3.4.1-bin-hadoop3.tgz
    tar xf spark-3.4.1-bin-hadoop3.tgz
    pip install findspark
    ```

2. Run the Jupyter notebook:
    - Ensure the data files are downloaded.
    - Follow the code cells to process the data.

## Logging
The logs are saved in `assignment.log`. It records data loading status and any potential issues.

## Data Processing
1. **Loading Data**: Data is loaded from JSON files.
2. **Combining Data**: Data from different brands is combined into a single DataFrame.
3. **Transformations**: Columns are extracted, transformed, and one-hot-encoded as required.
4. **Anonymization**: Sensitive data is anonymized to comply with GDPR.

## Output
The final processed data is saved as a Parquet file named `processed_data.parquet`.

