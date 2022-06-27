
# Kafka Pub-Sub example

Simple app for pratice Kafka pub-sub architecture. With this application, you can publish a message in kafka topic "example" through an endpoint. The application also reads the kafka topic and show data to you in the console
## Run Locally

Donwload apache Kafka from step 1 - "get kafka", Extract and enter to the kafka folder

```bash
https://kafka.apache.org/quickstart
```

Extract on your computer and open the folder.

```bash
  $ tar -xzf kafka_2.13-3.2.0.tgz
  $ cd kafka_2.13-3.2.0
```
Start Kafka Environment

```bash
  $ bin/zookeeper-server-start.sh config/zookeeper.properties
  $ bin/kafka-server-start.sh config/server.properties
```

Clone this project to yout computer 
```bash 
  $ git clone https://github.com/Natanista/kafka-example.git
```

Open the project with your favorite IDE and start it.




## API Reference

#### Post a message to kafka-topic "Example"

```http
  POST /api/v1/messages
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `message` | `string` | **Required**. Message content |


## Tech Stack


**Server:** Kafka, Spring Boot 

