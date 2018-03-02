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
* Extra: if local sonar is running and the plugin **SVG Badges** is installed, you can see bellow a badge with statistics of last sonar analysis:
    <img src="http://localhost:9000/api/badges/measure?metric=ncloc&key=my:project"/>
    

Tech Stack
* IntelliJ IDEA 2017.2.6
* Gradle 4.0

To take a look in other tutorials, please see https://github.com/topera/hello-world-index
