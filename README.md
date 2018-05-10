# Topera's Hello World #011
## Advanced Tests with a local SonarQube server

Steps

* Run a local SonarQube server with default configuration. You can install one with docker in few minutes with:
    * $ sudo docker run -d --name sonarqube -p 9000:9000 -p 9092:9092 sonarqube
* Check if SonarQube is running
    * http://localhost:9000
* Run sonar analysis:
    * $ gradle clean sonarqube
* Access the running server and check the result:
    * http://localhost:9000

Tech Stack
* IntelliJ IDEA 2017.2.6
* Gradle 4.0

To take a look in other projects, please see https://github.com/topera/index
