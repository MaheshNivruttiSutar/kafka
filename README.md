# **Kafka Integration Project**
This project demonstrates how to integrate and use Kafka for messaging between producers and consumers
using the `kafkajs` library in a Node.js environment.


## **Project Structure**
kafka-app/
├── admin.js       # Kafka admin script to create topics
├── client.js      # Kafka client configuration
├── producer.js    # Kafka producer to send messages
├── consumer.js    # Kafka consumer to receive messages
└── README.md      # Project documentation



## **Prerequisites**
- **Node.js:** Version 14 or later
- **Kafka:** A running Kafka instance (local or cloud-based)
- **Zookeeper:** Required for Kafka cluster management

## **Setup Instructions**
1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd kafka-app






How to run zookeeper:
docker run -p 2181:2181 zookeeper

How to run kafka:
docker run -p 9092:9092 \
-e KAFKA_ZOOKEEPER_CONNECT=192.168.220.114:2181 \
-e KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://192.168.220.114:9092 \
-e KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR=1 \
confluentinc/cp-kafka



Doc to refer:
https://kafka.js.org/docs/getting-started
https://www.openlogic.com/blog/using-kafka-zookeeper
https://zookeeper.apache.org/releases.html