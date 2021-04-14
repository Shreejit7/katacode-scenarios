Kafka comes with a command line client that will take input from a file or from standard input and send it out as messages to the Kafka cluster. By default, each line will be sent as a separate message.

Run the producer and then type a few messages into the console to send to the server.

ctrl-c to exit

`bin/kafka-console-producer.sh --broker-list localhost:9092 --topic first_topic `{{execute}}

You can type the message you want and press enter. All these messages will be saved in the topic

**Start the Consumer in a new terminal**

Kafka also has a command line consumer that will dump out messages to standard output, it should return the lines you typed in.

`bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic `{{execute}}

if we want to see all the message that is there in the topic then run the below command

`bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic --from-beginning `{{execute}}