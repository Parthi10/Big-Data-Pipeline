<p align="center">
  <img width="800" src="images/pipeline.png" alt="Pipeline diagram"></a>
</p>

## Big Data Pipeline

Made from programs which can, but don't have to, connect to each other.  

### Research and analysis

Before hammering a nail, get the right sized hammer.  
Data has to be gathered, enriched, analysed and stored.  
Apache Kafka, Apache Spark, Apache Hive and Redis seem like the right tools the job.  

[Here]((https://github.com/MislavJaksic/KnowledgeRepository/tree/master/BigData)) is how I came to that conclusion.  

### [Data Source to Kafka](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Data-Source-To-Kafka)

* a.k.a. Kafka Producer
* transports data from a CSV file to Kafka
* Python

### [Kafka To Hive](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Kafka-To-Hive/src/main/java/mjaksic/Kafka_To_Hive)

* a.k.a. Kafka Consumer
* transports data from Kafka to Apache Hive
* Java and Maven

### [Hive-Redis To Spark To Hive](https://github.com/MislavJaksic/Big-Data-Pipeline/tree/master/Hive-Redis-To-Spark-To-Hive/src/main/java/mjaksic/Hive_Redis_To_Spark_To_Hive)

1) takes data from Apache Hive and Redis
2) combines data into a single object
3) sends objects into Apache Spark for analysis
4) stores results back into Apache Hive

* Java and Maven
