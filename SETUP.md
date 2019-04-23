Integrate Sonar-Scanner with Maven project in POM.XML

We will need to add the following dependency



<!-- https://mvnrepository.com/artifact/org.sonarsource.scanner.maven/sonar-maven-plugin -->
<dependency>
<groupId>org.sonarsource.scanner.maven</groupId>
<artifactId>sonar-maven-plugin</artifactId>
<version>3.2</version>
</dependency>

Followed by the profile

<profiles>
<profile>
<id>sonar</id>
<activation>
<activeByDefault>true</activeByDefault>
</activation>
<properties>
<!-- Optional URL to server. Default value is http://localhost:9000 but since we seated in docker that is 80, in this case we only place localhost -->
<sonar.host.url>
http://localhost
</sonar.host.url>
</properties>
</profile>
</profiles>