# Spark-Based-Gas-Price-Forecasting
Apache Spark project analyzing and forecasting gas prices in France (2022–2024)


This project analyzes gas prices in France from 2022 to 2024 using Apache Spark.  
It includes data processing, visualization, feature engineering, and machine learning models
to forecast gas prices.

This work is part of a Big Data mini-project for academic purposes.

## Objectives
- Load and merge gas price datasets
- Clean and preprocess data with Spark
- Compute weekly statistics
- Create price indexes
- Visualize price trends
- Build ML models to forecast prices
- Evaluate model performance

## Dataset
Source:  
https://github.com/rvm-courses/GasPrices  

Files used:
- Gas prices (2022–2024)
- Gas stations file
- Services file

# PySpark Setup

### Install Java
Spark requires Java.

```bash
sudo apt install default-jdk
java -version

pip install pyspark
```

Set environment variables
Add to ~/.bashrc

```bash
nano ~/.bashrc
export JAVA_HOME=/usr/lib/jvm/default-java
export SPARK_HOME=$(python -c "import pyspark; print(pyspark.__path__[0])")
export PATH=$PATH:$SPARK_HOME/bin
```

