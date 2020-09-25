# FirstApp
Tutorial : How to build a Spring Boot Web Application from Scratch

* This tutorial is built using Oracle JDK 8, Spring Boot, Spring Data, Thymeleaf.


- mvn package
- java -jar target/firstapp-1.0-SNAPSHOT.jar
- Open a browser and go to http://localhost:8080/posts

Run it in play with docker:


  git clone https://github.com/dieterjava/firstapp.git 

https://github.com/dieterjava/firstapp.git

cd firstapp


docker run -it --rm --name firstapp -v "$PWD":/usr/src/app -w /usr/src/app maven:3.2-jdk-8 mvn clean install

docker run -it -d --rm --name firstapp -p 18080:8080 -v "$PWD":/usr/src/app -w /usr/src/app maven:3.2-jdk-8 java -jar target/firstapp-1.0-SNAPSHOT.jar 

goto URL  .... play-with-docker.composts


- Building it from scratch : https://www.youtube.com/watch?v=VS8W-tEqIiw
- Building a CRUD Web Application with Spring Boot :https://www.youtube.com/watch?v=TcP5kFPq354