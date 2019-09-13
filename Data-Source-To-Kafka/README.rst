Data Source to Kafka
====================

Transfers data from a CSV file to a Kafka topic.
Before each CSV line is cleaned before being sent to Kafka.


Using Kafka Producer
--------------------

Place a CSV file into "/src/kafka_producer".
Modify settings.py and the user defined cleaner functions.
Run the Kafka Producer with:

::

  python src/kafka_producer/kafka_csv_producer.py
