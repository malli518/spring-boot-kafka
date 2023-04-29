# spring-boot-kafka
Kafka Project 

# Download Kafka from below urls  :
https://kafka.apache.org/quickstart

# YouTube Link :
https://www.youtube.com/watch?v=U17DtHLOsTU&list=PLGRDMO4rOGcNLwoack4ZiTyewUcF6y6BU

# Kafka Terminologies : 
Clustor

Broker

Producer

Consumer

Topic

Partitions

Offsets

ConsumerGroup

# Start the ZooKeeper service
C:kafka> .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties


# Start the Kafka broker service
C:kafka> .\bin\windows\kafka-server-start.bat .\config\server.properties

#Create Kafka Topic
C:kafka> .\bin\windows\kafka-topics.bat --create --topic demotopic --bootstrap-server localhost:9092


#Producer to publish the messages to Topic
C:kafka> .\bin\windows\kafka-console-producer.bat --topic demotopic --bootstrap-server localhost:9092

#Consumer to read the messages from Topic
C:kafka> .\bin\windows\kafka-console-consumer.bat --topic demotopic --from-beginning --bootstrap-server localhost:9092


#Spring For Apache Kafka
https://docs.spring.io/spring-kafka/reference/html/#getting-started