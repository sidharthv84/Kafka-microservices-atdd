# Kafka-microservices-atdd

# Kafka Installation:
brew install kafka

# Start Kafka:
zookeeper-server-start /usr/local/etc/kafka/zookeeper.properties
kafka-server-start /usr/local/etc/kafka/server.properties

# Command to create Kafka topics:
kafka-topics --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic sid

# Producer:
kafka-console-producer --broker-list localhost:9092 --topic test

# Consumer:
kafka-console-consumer --bootstrap-server localhost:9092 --topic test --from-beginning


