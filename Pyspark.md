
# Introduction to Pyspark

## Spark
* Apache Spark is a distributed computing framework designed to handle complex, high value data processing.
* Works on multiple machines called as clusters.
* Works similar to [Hadoop](https://www.google.com/search?q=what+is+hadoop&oq=what+is+hadoop&gs_lcrp=EgRlZGdlKgoIABAAGLEDGIAEMgoIABAAGLEDGIAEMgcIARAAGIAEMgcIAhAAGIAEMgcIAxAAGIAEMgcIBBAAGIAEMgcIBRAAGIAEMgcIBhAAGIAEMgcIBxAAGIAEMggICBDpBxj8VTIHCAkQ6wcYQNIBCDI5MzJqMGoxqAIAsAIA&sourceid=chrome&ie=UTF-8&safe=active&ssui=on)

## Pyspark
* Python plugin for Spark framework.

## Features
* In Memory processing - very fast compared to hadoop map reduce
* Distributed processing - process data across multiple machines (cluster)
* Scalable - can handle GBs even PBs of data
* Fault Tolerant - can recover from failures. (redundant data stored in multiple machines)

## Use Cases
* ETL / ELT processing
* Streaming Data processing eg: Kafka
* Batch Processing - daily, hourly transactions/logs
* Machine Learning - Training ML models on huge datasets
* Data Quality and Transformations - Cleaning, joins, aggregations, window functions etc

## Spark building blocks
* Spark Core - Base spark engine for distributed computing
* Spark SQL - To use SQL Operations on data
* Dataframe API - Table like structure for data Operations
* Streaming - Real time data pipeline
* MLlib - Machine Learning library
* GraphX - Graph Processing

## Spark Architecture
Spark follows a master slave architecture. Spark execution starts at the main machine called driver. Subsequent tasks are processed by executor. 

Program which gets the command from driver node(master) and executor(slave) is called cluster manager.

### Components of spark architecture
* Driver Program - Main controller of spark application
* Spark Session/ Spark context - entry point of a spark application
* Cluster manager - allocates resources to spark eg: YARN, Kubernetes
* Executors - Workers that run the actual data processing
* Tasks - Smallest unit of data computation
* DAG Scheduler/ Task Scheduler - Plan and Schedule tasks for execution

