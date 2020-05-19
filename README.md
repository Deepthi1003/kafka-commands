# kafka-commands

This command helps to run the zookeeper service
``` .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties ```

To run the kafka service. Enter this command
``` .\bin\windows\kafka-server-start.bat .\config\server.properties ``` 

To create the topic in kafka use this command 
``` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic hive ```

To find out the topics in the kafka
``` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list ```

To delete any topic in the kafka 
``` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --delete --topic hive1 ```

To start the kafka producer  
``` .\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic hive ```
 
To start the kafka consumer 
 ``` .\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic hive --from-beginning ```




