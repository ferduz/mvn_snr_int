# Maven and Sonar Integration

Based on Docker Image of Sonar and Maven example project of [example]: https://github.com/gabrielf/maven-samples

## Install:

Clone repo

`git clone https://github.com/ferduz/mvn_snr_int.git`

Run Sonar Image

`cd mvn_snr_int`
`docker-compose up -d`

Run Maven

`mvn install`

Run Maven Test against SonarQube

`mvn sonar:sonar`

Check on sonar web

http://localhost

login 
user: admin
pass: bitnami

Check in the Dashboard that Parent Project Passed Test :)
