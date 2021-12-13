# Maven Repo

## Birt viewer-servlet v4.8.0

- Usage in pom.xml

```xml
<repositories>
  <repository>
    <id>Github Maven repo</id>
    <url>https://raw.github.com/ioagel/maven-repo/maven</url>
    <releases>
      <enabled>true</enabled>
    </releases>
    <snapshots>
      <enabled>true</enabled>
    </snapshots>
  </repository>
</repositories>

<dependencies>
  <dependency>
    <groupId>net.floulabs.birt</groupId>
    <artifactId>org.eclipse.birt.viewer-servlet</artifactId>
    <version>4.8.0</version>
  </dependency>
</dependencies>
```
