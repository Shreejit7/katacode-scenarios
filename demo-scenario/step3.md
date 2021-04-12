As the Zookeeper and Kafka server is running now, lets create some topics and try to send and recieve messages in real-time

## Task

Run the below **command** to create a Topic

`bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic first_topic `{{execute}}

In the above command we connect to the bootstrap-server (i.e. broker) to create the topic.

To confirm that the topic is created in the broker we can use the below **command**

`bin/kafka-topics.sh --list --bootstrap-server localhost:9092 `{{execute}}
