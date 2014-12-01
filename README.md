Intuit IPP DevKit
=================

Since this library does not appear to be provided in a public maven repository, I'm hosting it.

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

Then add the dependencies:

```
<dependency>
    <groupId>com.intuit.code.devkit</groupId>
    <artifactId>ipp-java-qbapihelper</artifactId>
    <version>1.2.0</version>
</dependency>
<dependency>
    <groupId>com.intuit.code.devkit.v3</groupId>
    <artifactId>ipp-v3-java-data</artifactId>
    <version>2.3.2</version>
</dependency>
<dependency>
    <groupId>com.intuit.code.devkit.v3</groupId>
    <artifactId>ipp-v3-java-devkit</artifactId>
    <version>2.3.2</version>
</dependency>
```

You may also be required to add the following dependencies:
```
<dependency>
  <groupId>commons-configuration</groupId>
  <artifactId>commons-configuration</artifactId>
  <version>1.10</version>
</dependency>
<dependency>
  <groupId>commons-collections</groupId>
  <artifactId>commons-collections</artifactId>
  <version>3.2.1</version>
</dependency>
<dependency>
  <groupId>org.jvnet.jaxb2_commons</groupId>
  <artifactId>jaxb2-basics-runtime</artifactId>
  <version>0.6.5.1</version>
</dependency>
<dependency>
  <groupId>oauth.signpost</groupId>
  <artifactId>signpost-core</artifactId>
  <version>1.2.1.2</version>
</dependency>
<dependency>
  <groupId>oauth.signpost</groupId>
  <artifactId>signpost-commonshttp4</artifactId>
  <version>1.2.1.2</version>
</dependency>
```