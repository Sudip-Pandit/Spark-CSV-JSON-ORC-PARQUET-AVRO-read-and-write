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

# How to read ORC file in spark?

  ![image](https://user-images.githubusercontent.com/70854976/149605512-2beedd04-2aa0-48a3-bc5d-5f50f9568479.png)
  
  ![image](https://user-images.githubusercontent.com/70854976/149605531-b65e2375-544a-43d6-8881-0a8883461224.png)
  
# Code

val df = spark.read.format("orc").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/products_orc/products_orc_part-00000-0af8db31-47a8-417a-91f6-ee94f0128263-c000.snappy.orc/")

# How to read avro file in spark?

  ![image](https://user-images.githubusercontent.com/70854976/149605633-70440e30-ffe3-418c-9794-de561048d1e2.png)
  
# Code

val df = spark.read.format("avro").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/prod
ucts_avro/part-m-00000.avro/")



 

