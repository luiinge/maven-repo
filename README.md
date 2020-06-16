# Temporary Maven Repository for hosted projects

This repository can be used as a regular Maven repository, in order to download 
the artifacts while they are not published in Maven Central.

Simply add the following code into the `pom.xml` file of any project that requires
those dependencies:

```xml
    <repositories>
        <repository>
            <id>github</id>
            <url>https://luiinge.github.io/maven-repo</url>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>
```
