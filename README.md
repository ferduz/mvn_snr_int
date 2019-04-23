# Maven and Sonar Integration

Based on Docker Image of Sonar and Maven example project of https://github.com/gabrielf/maven-samples


* Prerequisites: Docker and Maven installed

## Install:

Clone repo

`git clone https://github.com/ferduz/mvn_snr_int.git`

Run Sonar Image

`cd mvn_snr_int`

`docker-compose up -d`

Run Maven

`cd maven-samples`

`mvn install`

Run Maven Test against SonarQube

`mvn sonar:sonar`

Check on sonar web

http://localhost

login 
user: admin
pass: bitnami

Check in the Dashboard that Parent Project Passed Test :)


* Setup your own Maven project takeing a look to SETUP.md
