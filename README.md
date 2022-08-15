# Maven Repo

Always required in `pom.xml`
```xml
<repositories>
  <repository>
    <id>Github Maven repo</id>
    <url>https://raw.github.com/ioagel/maven-repo/master</url>
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

## Birt Report Engine API v4.9.0

Programmatically create the Engine and Render the PDF report, using database for data ingestion.
```xml
<dependencies>
  <dependency>
    <groupId>net.floulabs.birt</groupId>
    <artifactId>org.eclipse.birt.report.engine.api</artifactId>
    <version>4.9.0-20220815</version>
  </dependency>
</dependencies>
```

**IMPORTANT**: I have removed a lot of dependencies obsolete for my use case, supplied by the ReportEngine lib folder of the Birt Runtime. It is used *ONLY* for PDF reports, using database for data (i.e. MySQL).