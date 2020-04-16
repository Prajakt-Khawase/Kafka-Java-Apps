# Kafka-Java-Apps
This project addresses part 2 of the Kafka Java Apps assignment.

# Instructions to run the App
## Compile and Build a Fat Jar File
Open PowerShell as Administrator in the root project folder, compile the code using Maven and create an executable jar file. Generated artificacts can be found in the new 'target' folder.

mvn clean compile assembly:single

## 1.Start Zookeeper Service
Start and keep running the Zookeeper service.

zkserver

## 2.Start Kafka Service
Start and keep running the Kafka service. What directory must you be in?

 .\kafka-server-start.bat .\server.properties.

## 3.Start Consumer
Open PowerShell as Administrator in the root project folder, start the original consumer app:

java -cp target/kafka-case-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmsu.karanam.kafka.CustomConsumer 

## 4.Start Producer
Open a new PowerShell as Administrator in the root project folder, start the Producer app using topic test:

java -cp target/kafka-case-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmsu.karanam.kafka.CustomProducer

# Reference

<https://github.com/denisecase/kafka-case>
