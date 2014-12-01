Intuit Java DevKit Data
================================

Helper library for the QBO API

To use this library in another Maven Project:
---------------------------------------------

Add the following to the pom.xml for releases:

```
<repositories>
    <repository>
        <id>maven.leadoperations.co-release</id>
        <name>AWS S3 Release Repository</name>
        <url>http://maven.leadoperations.co/release</url>
    </repository>
</repositories>
```

or for snapshots:
```
<repositories>
    <repository>
        <id>maven.leadoperations.co-snapshot</id>
        <name>AWS S3 Snapshot Repository</name>
        <url>http://maven.leadoperations.co/snapshot</url>
        <snapshots>
            <enabled>true</enabled>
        </snapshots>
    </repository>
</repositories>
```

Then add the dependency:

```
<dependency>
    <groupId>com.intuit.code.devkit.v3</groupId>
    <artifactId>ipp-v3-java-data</artifactId>
    <version>2.3.2</version>
</dependency>
```

To upload a new jar to the maven repository:
--------------------------------------------
`mvn deploy:deploy-file -DgroupId=com.intuit.code.devkit.v3 -DartifactId=ipp-v3-java-data -Dversion=2.3.2 -Dpackaging=jar -Dfile=ipp-v3-java-data-2.3.2.jar -DrepositoryId=aws-release -Durl=s3://maven.leadoperations.co/release`
