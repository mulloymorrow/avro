# avro
## Mirror of Apache Avro. 
There is a fix in this snapshot that I wanted my maven project to depend on. 
To depend on this maven artifact, add the following to your pom.xml:

```xml
  <properties>
        <avro.version>1.8.0.24p-SNAPSHOT</avro.version>
  </properties>
    
  <repositories>
        <repository>
            <id>avro-mvn-repo</id>
            <url>https://raw.github.com/mulloymorrow/avro/mvn-repo/</url>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>

    <dependencies>
        <dependency>
            <groupId>org.apache.avro</groupId>
            <artifactId>avro</artifactId>
            <version>${avro.version}</version>
        </dependency>
    </dependencies>
```
