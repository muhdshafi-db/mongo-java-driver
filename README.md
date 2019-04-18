# mongo-java-driver
## maven dependency
```
 <dependency>
    <groupId>org.mongodb</groupId>
    <artifactId>mongo-java-driver</artifactId>
    <version>3.10.2</version>
 </dependency>
```
## Creating MongoDB Java Connection 
### Connect to MongoDB server 
``` java

    MongoClient mongoClient = new MongoClient(); //connects to default host and port i.e 127.0.0.1:27017
    // or
    MongoClient mongoClient = new MongoClient( "localhost" ); //connects to default port i.e 27017
    // or
    MongoClient mongoClient = new MongoClient( "localhost" , 27017 ); // should use this always

    // or, to connect to a replica set, with auto-discovery of the primary
    MongoClient mongoClient = new MongoClient(Arrays.asList(new ServerAddress("localhost", 27017),
                                          new ServerAddress("localhost", 27018),
                                          new ServerAddress("localhost", 27019)));

```
