Apache Kafka
=================
### Install Kafka ###
Follow instructions in https://kafka.apache.org/quickstart

### Start Zookeper from kafka folder run below coomand ###
    .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.propeies

### Start Kafka from kafka folder run below coomand ###
    .\bin\windows\kafka-server-start.bat .\config\server.properties

### DeliveryApp ###
    spring.kafka.producer.bootstrap-servers=localhost:9092
    spring.kafka.producer.key-serializer=org.apache.kafka.common.serialization.StringSerializer
    spring.kafka.producer.value-serializer=org.apache.kafka.common.serialization.StringSerializer
Run the DeliveryApp microservice add above to application.propeties as per your host 
    

    

### UserApp ###
    
    
