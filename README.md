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
    server.port=8081
    spring.kafka.consumer.bootstrap-servers=localhost:9092
    spring.kafka.consumer.group-id=group-1
    spring.kafka.consumer.auto-offset-reset=earliest
    spring.kafka.consumer.key-deserializer=org.apache.kafka.common.serialization.StringDeserializer
    spring.kafka.consumer.value-deserializer=org.apache.kafka.common.serialization.StringDeserializer   
Run the UserApp microservice add above to application.propeties as per your host 
    
    
