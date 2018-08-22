
**PubSub Java client for Kafka:**

Tested on Ubuntu 18.04, openjdk version "1.8.0_181"

**Step 1 --- Setup Kafka Broker:**

Follow this link. It's very easy to setup.
https://kafka.apache.org/quickstart

**Step 2 --- Download this repo "KafkaAPIClient-master" and Compile the code:**

        cd KafkaAPIClient-master/
        mvn clean compile assembly:single
        
        Start the consumer:
        java -cp target/KafkaAPIClient-1.0-SNAPSHOT-jar-with-dependencies.jar com.spnotes.kafka.simple.Consumer test group1
        
        Start the producer:
        java -cp target/KafkaAPIClient-0-SNAPSHOT-jar-with-dependencies.jar com.spnotes.kafka.simple.Producer test
        
        Enter a message in the producer console and check to see whether that message appears in the consumer. Try a few
        messages.
        
You can check this Ignition forum link.

https://forum.inductiveautomation.com/t/ignition-apache-kafka-build-massively-scalable-projects-demo/19317

Thanks to:
https://www.javaworld.com/article/3060078/big-data/big-data-messaging-with-kafka-part-1.html

