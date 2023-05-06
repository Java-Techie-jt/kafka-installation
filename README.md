# kafka-installation

# Command uses 

### Move into Kafka container
```docker exec -it <kafka_conatiner_id> /bin/sh```
### Go inside kafka installation folder
```cd /opt/kafka_<version>/bin```
### Create Kafka topic
```kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic quickstart```
### Start Producer app (CLI)
```kafka-console-producer.sh --topic quickstart --bootstrap-server localhost:9092```
### Start consumer app (CLI)
```kafka-console-consumer.sh --topic quickstart --from-beginning --bootstrap-server localhost:9092```
