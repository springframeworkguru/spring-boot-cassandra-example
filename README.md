# spring-boot-cassandra-example

Install docker and start cassandra in localhost using following command:

```sh
mkdir -p ~/cassandra
docker run -it --name cassandra4 -v ~/cassandra:/var/lib/cassandra -p 127.0.0.1:9042:9042 -p 127.0.0.1:9160:9160 -d cassandra:4.0

cd ~/spring-boot-cassandra-example
mvn clean spring-boot:run
```

Then head to http://localhost:8080/product in your browser
