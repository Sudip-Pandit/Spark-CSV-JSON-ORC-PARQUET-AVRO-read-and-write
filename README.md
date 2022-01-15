# Spark-CSV-JSON-ORC-PARQUET-AVRO-read-and-write
This repository contains speak read and write with different file formats.

# Start spark-shell

# How to read csv file in spark?

  ![image](https://user-images.githubusercontent.com/70854976/149605090-28d25920-029d-4460-af8f-101db090a4d6.png)
  
  ![image](https://user-images.githubusercontent.com/70854976/149605121-64979d0c-33b8-4977-804e-c45a5c99976d.png)
  
  val df = spark.read.format("csv").option("header","true").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/categories-header/ca
tegories-header_part-00000.csv/")

 

