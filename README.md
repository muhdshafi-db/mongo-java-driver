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
MongoClient mongoClient = new MongoClient( "localhost" , 27017 );
```
