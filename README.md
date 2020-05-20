# kafka-example

- To run this project, clone the repo first.
- To start kafka service from kafka folder in powershell by using the command ``` .\bin\windows\kafka-server-start.bat .\config\server.properties ```
- To start the zookeeper from the kafka folder using the command  ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties ```
- To create a topic in new powershel using the command ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic test```
- To run as consumer, we have to use the command ```java -cp target/kafka-example-1.0-SNAPSHOT-jar-with-dependencies.jar nwmissouri.bigdatarethima.Consumer test group1```
- To run as producer, we have to run the command ```java -cp target/kafka-example-1.0-SNAPSHOT-jar-with-dependencies.jar nwmissouri.bigdatarethima.ProducerSentenceRandom test```
