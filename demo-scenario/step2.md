Before Starting the Kafka Server we have to start the Zookeeper which keeps track of status of the Kafka cluster nodes and it also keeps track of Kafka topics, partitions etc.

## Task

Run the below **command** to start the Zookeeper server

`bin/zookeeper-server-start.sh config/zookeeper.properties & `{{execute}}

Once the Zookeeper is up and running we can start the kafka server now. Each kafka server is nothing but the brokers. 
So to have multiple brokers in our kafka cluster we will need to start multiple servers by below **command**

`bin/kafka-server-start.sh config/server.properties & `{{execute}}

each broker will have it's own server.properties file