# Springboot-Kafka-Wikimedia-Data-Processing
Real-time Wikimedia Data Processing with Spring Boot,Kafka and storing the data in MYSQL database.  

<img width="579" alt="image" src="https://github.com/kalyani33/Springboot-Kafka-Wikimedia-Data-Processing/assets/37569003/8d445816-5961-44b5-8c19-f2f05b1c9d08"><br/>


STEP 1: DOWNLOAD AND INSTALL KAFKA  
[https://dlcdn.apache.org/kafka/3.2.0/kafka_2.13-3.2.0.tgz](https://kafka.apache.org/quickstart)

STEP 2: START THE KAFKA ENVIRONMENT
## Start the ZooKeeper service
C:\Users\kalyani\Downloads\kafka>.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

## Start the Kafka broker service
C:\Users\kalyani\Downloads\kafka>.\bin\windows\kafka-server-start.bat .\config\server.properties

STEP 3: CREATE A TOPIC TO STORE YOUR EVENTS
C:\Users\kalyani\Downloads\kafka>.\bin\windows\kafka-topics.bat --create --topic topic_demo --bootstrap-server localhost:9092

STEP 4: WRITE SOME EVENTS INTO THE TOPIC
C:\Users\kalyani\Downloads\kafka>.\bin\windows\kafka-console-producer.bat --topic topic_demo --bootstrap-server localhost:9092
>hello world
>topic demo

STEP 5:  READ THE EVENTS
C:\Users\kalyani\Downloads\kafka>.\bin\windows\kafka-console-consumer.bat --topic topic_demo --from-beginning --bootstrap-server localhost:9092
hello world
topic demo
