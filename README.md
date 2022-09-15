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

## How to maven install a jar
```sh
# example: copy the jar and it's pom.xml to a dir under .jars and:
$ mvn install:install-file \
    -Dfile=.jars/birt-runtime/4.9.0-20220915/org.eclipse.birt.runtime_4.9.0-20220315.jar \
    -DpomFile=.jars/birt-runtime/4.9.0-20220915/pom.xml \
    -DlocalRepositoryPath=. \
    -DcreateChecksum=true
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

Programmatically create the Engine and Render the PDF report, using database for data ingestion.
```xml
<dependencies>
  <dependency>
    <groupId>net.floulabs.birt.runtime</groupId>
    <artifactId>org.eclipse.birt.runtime_4.9.0-20220315</artifactId>
    <version>4.9.0</version>
  </dependency>
</dependencies>
```

**IMPORTANT**: I have removed a lot of dependencies obsolete for my use case, supplied by the ReportEngine lib folder of the Birt Runtime. It is used *ONLY* for PDF reports, using database for data (i.e. MySQL).