Intuit Java DevKit QB API Helper
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
    <groupId>com.intuit.code.devkit</groupId>
    <artifactId>ipp-java-qbapihelper</artifactId>
    <version>1.2.0</version>
</dependency>
```

To upload a new jar to the maven repository:
--------------------------------------------
`mvn deploy:deploy-file -DgroupId=com.intuit.code.devkit -DartifactId=ipp-java-qbapihelper -Dversion=1.2.0 -Dpackaging=jar -Dfile=ipp-java-qbapihelper-1.2.0.jar -DrepositoryId=aws-release -Durl=s3://maven.leadoperations.co/release`
