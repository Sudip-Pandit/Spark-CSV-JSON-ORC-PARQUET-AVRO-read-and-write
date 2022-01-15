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

  # Download spark avro jar 
     
     download avro jar from this link 
     https://mvnrepository.com/artifact/com.databricks/spark-avro_2.11/3.2.0
     
![image](https://user-images.githubusercontent.com/70854976/149633923-50e4e273-9652-45e8-b397-e41088dfeb34.png)

![image](https://user-images.githubusercontent.com/70854976/149634082-8e8e790c-5a1b-45d4-8d3f-501a94c3988f.png)

![image](https://user-images.githubusercontent.com/70854976/149634111-24b8f549-d0db-45b4-bf57-f1e81e3b3455.png)

     Have databricks jar already in the directory
     Now, start spark-sehll pointing to that directory
     
![image](https://user-images.githubusercontent.com/70854976/149634308-6f62fa34-6dd9-4bd2-9214-d0db17776b12.png)
![image](https://user-images.githubusercontent.com/70854976/149634338-c784f624-f248-4fca-8ac4-4cd1b0859910.png)

##### Data path 

![image](https://user-images.githubusercontent.com/70854976/149634445-b9b9a439-d108-4131-8b09-b7453695e7ed.png)

![image](https://user-images.githubusercontent.com/70854976/149634744-71abb245-c43f-4873-b719-087b02a4185f.png)


  ![image](https://user-images.githubusercontent.com/70854976/149605633-70440e30-ffe3-418c-9794-de561048d1e2.png)
  
# Code

val df = spark.read.format("avro").load("file:///C:/Users/Sudip/Downloads/CCA-175-practice-tests-resource-master/retail_db/prod
ucts_avro/part-m-00000.avro/")



 

