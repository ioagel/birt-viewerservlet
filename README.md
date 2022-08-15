# Maven Repo

Always required in `pom.xml`
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
```


## Birt viewer-servlet v4.8.0

Supports using a servlet to render the PDF report
```xml
<dependencies>
  <dependency>
    <groupId>net.floulabs.birt</groupId>
    <artifactId>org.eclipse.birt.viewer-servlet</artifactId>
    <version>4.8.0</version>
  </dependency>
</dependencies>
```

## Birt Runtime v4.9.0

Programmatically create the Engine and Render the PDF report
```xml
<dependencies>
  <dependency>
    <groupId>net.floulabs.birt</groupId>
    <artifactId>org.eclipse.birt.runtime_4.9.0-20220315.jar</artifactId>
    <version>4.9.0</version>
  </dependency>
</dependencies>
```