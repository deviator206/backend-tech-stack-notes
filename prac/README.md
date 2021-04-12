# Getting Started

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.4.4/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.4.4/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.4.4/reference/htmlsingle/#boot-features-developing-web-applications)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)



### Kafka Installation
> brew install kafka

##### Start the Zookeeper
> zookeeper-server-start /usr/local/etc/kafka/zookeeper.properties

##### Start Kafka
> kafka-server-start /usr/local/etc/kafka/server.properties

##### Create Topic
$ kafka-topics --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test

#### Initialize Producer
> kafka-console-producer --broker-list localhost:9092 --topic test


#### Initialize Consumer
$ kafka-console-consumer --bootstrap-server localhost:9092 --topic test --from-beginning


#### SpringBoot- initialize Kafka Properties
https://www.maestralsolutions.com/spring-boot-implementation-for-apache-kafka-with-kafka-tool/


