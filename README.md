# Kafka_Realtime_Streaming_to_Cassandra
This project demonstrates a data pipeline that simulates stock data using a producer, which is then streamed to Apache Kafka, and finally consumed by a consumer that stores the data in Cassandra.

## Architecture

![kafka](https://github.com/user-attachments/assets/ab6a13d2-0ff8-42cb-8a89-92f386733694)

## Technologies
- Python
- Docker
- Apache Kafka
- Apache Zookeeper
- Apache Cassandra

## Setup and Execution Instructions

### 1. Install dependencies:
- Run the following command to prepare your Python environment:

```yaml
pip install -r requirements.txt
```

### 2. Run Docker containers:
- Run this command to start Kafka, Zookeeper, and Cassandra:

```yaml
docker-compose up -d
```

### 3. Run the Producer:
- Open and run the **KafkaProducer.ipynb** notebook in Jupyter.
- This notebook will start sending data from **AMZN.csv** to Kafka.

### 4. Run the Consumer:
- Open and run the **KafkaConsumer.ipynb** notebook in Jupyter.
- This notebook will listen to the Kafka topic and store the data in Cassandra.

## Verifying the Results
You can use CQL (Cassandra Query Language) to query the Cassandra database and verify that the data has been stored correctly.


