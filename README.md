# Spark-CSV-JSON-ORC-PARQUET-AVRO-read-and-write
This repository contains speak read and write with different file formats.

# Start spark-shell --master yarn --packages com.databricks:spark-avro_2.10:2.0.1

# How to read csv file in spark?

  ![image](https://user-images.githubusercontent.com/70854976/149605090-28d25920-029d-4460-af8f-101db090a4d6.png)
  
  ![image](https://user-images.githubusercontent.com/70854976/149605121-64979d0c-33b8-4977-804e-c45a5c99976d.png)
  
# code
val df = spark.read.format("csv").option("header","true").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/categories-header/ca
tegories-header_part-00000.csv/")

# How to read JSON file in spark?

  ![image](https://user-images.githubusercontent.com/70854976/149605264-249e54b9-19c8-4e10-998b-701ca22f4b1d.png)
  
  ![image](https://user-images.githubusercontent.com/70854976/149605287-8e3eefec-63de-4204-84e3-872fa882bc26.png)

# code
val df = spark.read.format("json").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/categories-header/ca
tegories-header_part-00000.json/")


 

