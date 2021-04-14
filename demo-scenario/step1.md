In this Step we will Set up the Environment and download the kafka.

## Task

Let's first set up the java by executing below commands** one by one
`sudo add-apt-repository ppa:openjdk-r/ppa`{{execute}}
`sudo apt-get update`{{execute}}
`sudo apt-get install openjdk-8-jre`{{execute}}

Once it is installed you can verify it by the below command**

`java -version`{{execute}}

** In Case the wget is not working use the below command to install it
`sudo apt-get update`{{execute}}
`sudo apt-get install wget`{{execute}}

Let's first download the kafka executing the below **command**

`wget https://archive.apache.org/dist/kafka/2.4.0/kafka_2.11-2.4.0.tgz`{{execute}}


Extract the file 

`tar -xzf kafka_2.11-2.4.0.tgz`{{execute}}

cd into the extracted kafka folder

`cd kafka_2.11-2.4.0/`{{execute}}
