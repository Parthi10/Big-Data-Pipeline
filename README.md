## Big Data Pipeline

The pipeline is made out of multiple pipe segments which can, but don't have to, connect to each other.  

### 1) Data Source to Kafka

* AKA Kafka Producer
* written in Python
* transports data from a CSV file to a Kafka topic

For more information, take a look at the project's [README](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Data-Source-To-Kafka).  

### 2) Hive-Redis To Spark To Hive 

* written in Java using Maven

1) Take data from both Apache Hive and Redis  
2) Combine it into a single data object using a user written function  
3) Send data objects into Apache Spark for analysis  
4) Store the results back into Apache Hive  

For more information, take a look at the project's [Javadocs](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Hive-Redis-To-Spark-To-Hive/doc) and [source code](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Hive-Redis-To-Spark-To-Hive/src/main/java/mjaksic/Hive_Redis_To_Spark_To_Hive).  

### 3) Kafka To Hive

* AKA Kafka Producer
* written in Java using Maven
* transports data from a Kafka topic to a row in Apache Hive table

For more information, take a look at the project's [Javadocs](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Kafka-To-Hive/doc) and [source code](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Kafka-To-Hive/src/main/java/mjaksic/Kafka_To_Hive).  

### Tutorial Analysis and Theoretical Foundation

Apache Kafka, Apache Spark, Apache Hive and Redis had to be studied first to make sure they are the right tools for the job.  
The results of this study can be read by following the [GitHub link](https://github.com/MislavJaksic/KnowledgeRepository/tree/master/BigData).  