# Docker Crash Course for Java Developers

## Learn Docker creating containers for Spring Boot APIs and Microservices

Learn Docker Fundamentals? Yes.   Create Containers for Microservices? Yes.     Create Containers for Full Stack Applications? Yes. Of Course. Hands-on? Of course.

Do you have ZERO experience with Docker? No Problem.

Do you want to learn to create containers for Java Spring Boot Applications and Microservices using Docker with an easy to learn, step by step approach?

Are you ready to learn about Docker and take the next step in your programming career?

Look No Further!

Architectures are moving towards Microservices and Cloud. Docker makes it easy to containerize your applications and make them cloud ready.

Docker is the No 1 Tool to Containerize your Java Spring Boot Applications. Learning Docker would help you streamline your deployment processes and experiment easily with new frameworks and tools. 

In this handson course, we will containerize - create docker images and create containers - for a variety of Spring Boot Applications:
- REST APIs - Hello World and Todo - Jar
- Todo Web Application War
- Full Stack Application with React and Spring Boot
- CCS and CES Microservices
- Eureka Naming Server and Zuul API Gateway

This course would be a perfect first step as an introduction to Docker.

You will be using containerizing a variety of projects created with  React (Frontend Framework), Spring Boot (REST API Framework), Spring (Dependency Management), Spring Security (Authentication and Authorization - Basic and JWT), BootStrap (Styling Pages), Maven (dependencies management), Node (npm), Visual Studio Code (TypeScript IDE), Eclipse (Java IDE) and Tomcat Embedded Web Server. We will help you set up each one of these.

## What you'll learn
- You will Learn the Fundamentals of Docker from Zero, no previous experience required
- You will learn the important Docker Concepts - Registry, Repository, Tag, Image,  Container and Volumes
- You will learn the important Docker commands  
- You will understand the Docker Architecture
- You will create Docker images for 8 Java Spring Boot Projects
- You will learn to use Dockerfile to Automate Building of your Docker Image
- You will learn to use various maven plugins - Dockerfile Spotify Plugin, JIB Plugin and Fabric8 Docker Maven Plugin - to create Docker images
- You will learn to create best practices with creating Docker Images - Improve Caching of Docker Images and create Multi Stage Docker Builds.
- You will Containerize Java Spring Boot Todo Web Application talking with MySQL
- You will Containerize Java Spring Boot React Full Stack Application with Docker
- You will Containerize CCS, CES Microservices, Eureka Naming Server and Zuul API Gateway with Docker and Run them using Docker Compose
- You will learn to run MySQL, RabbitMQ and Zipkin as Docker Containers
- You will learn the basics of Docker Networking - HOST, BRIDGE and NONE
- You will learn to use Docker Compose to Manage Your Containers
- You will learn the basics of Microservices


## Requirements
- You have an attitude to learn while having fun :)
- You have some programming experience with Java, Spring and Spring Boot
- You DO NOT need to have any experience with Docker
- We will help you install Eclipse, Visual Studio Code, Git client, Docker Desktop and Node JS (for npm)

## Who is this course for
- You are a Java Spring Boot developer getting started with the Cloud
- You want to containerize your Java applications with Docker
- You are a Java Developer and You are curious about Docker
- You want to learn to containerize a Java Spring Boot full stack application with Docker
- You want to learn to play with Docker and Spring Boot Microservices - Service Registry, Distributed Tracing and Zuul API Gateway

## Step By Step Details

### Introduction to the Course
- Deploy Spring Boot Applications to Docker - Course Overview
- Deploy Spring Boot Applications to Docker - Getting Started

### Getting Started with Docker
- Installing Docker - Docker
- Your First Docker Usecase - Deploy a Spring Boot Application
- Important Docker Concepts - Registry, Repository, Tag, Image and Container
- Playing with Docker Images and Containers
- Understanding Docker Architecture - Docker Client, Docker Engine
- Why is Docker Popular
- Playing with Docker Images
- Playing with Docker Containers
- Playing with Docker Commands - stats, system
- Importing Docker Projects

### Containerizing Java Spring Boot Hello World Rest API with Docker
- Setting up 01 Spring Boot Hello World Rest API in Local 
- Build Docker Image Manually for 01 Hello World Rest API
- Use Dockerfile to Build Docker Image
- Understanding Docker Image Layers, Caching and Dockerfile Instructions
- Using Dockerfile Spotify Plugin to Create Docker Images
- Create a generic reusable Dockerfile
- Improving Caching of Docker Images by Adding Libraries in a Separate Step
- Using JIB Plugin to Create Docker Images
- Using Fabric8 Docker Maven Plugin to Create Docker Images

### Containerizing Java Spring Boot Todo Web Application with Docker
- Setting up 02 Spring Boot Todo Web Application in Local 
- Create Docker Image for Spring Boot Todo Web Application
- Understanding ENTRYPOINT, CMD, COPY and ADD instructions
- Pushing 02 Spring Boot Todo Web Application to Docker Hub

### Containerizing Java Spring Boot Todo Web Application using MySQL with Docker
- Code Review of 03 Todo Web Application MySQL
- Running MySQL as Docker Container on Local
- Connect Spring Boot Todo Web App to MySQL on Local
- Create Docker Image for 03 Todo Web Application and Use Link to connect
- Exploring Docker Networking - HOST, BRIDGE and NONE
- Creating a Custom Network and Connect MySQL and WebApplication to the network
- Using Docker Volumes to Persist Data
- Playing with Docker Compose

### Containerize Java Spring Boot React Full Stack Application with Docker
- Exploring 04 Java Full Stack Spring Boot React App
- Running React Frontend in Local
- Containerizing Java REST API Backend
- Creating Multi Stage Docker Build for React Frontend Code
- Improve Front End Docker Build - dockerignore
- Using Multi Stage Docker Build for Java REST API Backend
- Running Java REST API Backend Docker Image
- Exploring Docker Compose
- Running Full Stack Application with Docker Compose
- Using Docker Compose for Java Spring Boot Todo Web Application with MySQL

### Getting started with CCS and CES Microservices on Docker
- Introduction to Microservices
- Advantages of Microservices
- Understanding Docker and Microservices - An Amazing Combo
- Overview of CCS and CES Spring Boot Microservices
- Create Docker Images and Containers for CCS and CES Microservices
- Run CCS and CES Microservices using Docker Compose

### Using Eureka Naming Service with Spring Boot Microservices and Docker
- Understanding the need for Service Registry
- Create Docker Images for Eureka Naming Server
- Configure and Run CES and CCS Microservices with Eureka Service

### Using Zuul API Gateway with Spring Boot Microservices and Docker
- Configure CES and CCS Microservices with Zuul API Gateway
- Use Docker Compose to Run Microservices with Zuul

### Distributed Tracing with Zipkin and RabbitMq
- Introduction to Zipkin and Update Microservices to Connect to Zipkin
- Using Docker Compose to Launch Zipkin, RabbitMq and Microservices
- Running Zipkin, RabbitMq and Microservices

## Diagrams

- Courtesy http://viz-js.com/

```
graph architecture {

node[style=filled,color="#59C8DE"]
//node [style=filled,color="#D14D28", fontcolor=white];
rankdir = TB
node[shape=record, width=3]

Containers, LocalImages [height=1]

DockerClient -- Daemon
Daemon -- Containers 
Daemon -- LocalImages
Daemon -- ImageRegistry

DockerClient[label=<Docker Client>]
ImageRegistry[label=<Image Registry <BR /><FONT POINT-SIZE="10">nginx<BR />mysql<BR />eureka<BR />your-app<BR /><BR /></FONT>>];
Daemon[label=<Docker Daemon>]


}


graph architecture {

node[style=filled,color="#59C8DE"]
//node [style=filled,color="#D14D28", fontcolor=white];
rankdir = TB
node[shape=record, width=2]
Hypervisor,HostOS, Hardware[shape=record, width=6.5, style=filled,color="#D14D28", fontcolor=white]
edge [width=0]
graph [pad=".75", ranksep="0.05", nodesep="0.25"];

Application1 -- Software1 [style=invis]
Application2 -- Software2 [style=invis]
Application3 -- Software3 [style=invis]

Software1 -- GuestOS1 [style=invis]
Software2 -- GuestOS2 [style=invis]
Software3 -- GuestOS3 [style=invis]
GuestOS1 -- Hypervisor [style=invis]
GuestOS2 -- Hypervisor [style=invis]
GuestOS3 -- Hypervisor [style=invis]
Hypervisor -- HostOS [style=invis]
HostOS -- Hardware [style=invis]

}


graph architecture {

node[style=filled,color="#59C8DE"]
//node [style=filled,color="#D14D28", fontcolor=white];
rankdir = TB
node[shape=record, width=2]
HostOS, CloudInfrastructure, DockerEngine[shape=record, width=6.5, style=filled,color="#D14D28", fontcolor=white]
edge [width=0]
graph [pad=".75", ranksep="0.05", nodesep="0.25"];
Container1,Container2,Container3[height=2]

Container1 -- DockerEngine [style=invis]
Container2 -- DockerEngine [style=invis]
Container3 -- DockerEngine [style=invis]
DockerEngine -- HostOS [style=invis]
HostOS -- CloudInfrastructure [style=invis]

}
```


### Commands Executed during the course

```
docker container exec unruffled_tereshkova ls /tmp
docker container cp target/hello-world-rest-api.jar 54cf414254e48d5f68c4d468b2dd4cbdd95d17f9e2074fdb9df7f64987697f2b:/tmp
docker container commit unruffled_tereshkova bbnsdevelop/hello-world-rest-api:manual 
docker run -p 8080:8080 bbnsdevelop/hello-world-rest-api:manual
docker container commit --change='CMD ["java","-jar","/tmp/hello-world-rest-api.jar"]' unruffled_tereshkova bbnsdevelop:hello-world-rest-api:manual2
docker run -p 8080:8080 bbnsdevelop/hello-world-rest-api:manual2
docker inspect bbnsdevelop/hello-world-rest-api:dockerfile1
docker history bbnsdevelop/hello-world-rest-api:dockerfile1

docker build -t bbnsdevelop/hello-world-rest-api:dockerfile1 .
docker run -p 8080:8080 bbnsdevelop/hello-world-rest-api:dockerfile1
docker history bbnsdevelop/hello-world-rest-api:dockerfile1

docker run -p 8080:8080 bbnsdevelop/hello-world-rest-api:0.0.1-SNAPSHOT

mvn docker:build
docker run -p 8080:8080 webservices/01-hello-world-rest-api

docker run -dit 51297c224d60
docker container exec 7714 ls /maven
docker run -p 8080:8080 01-hello-world-rest-api:latest

#/02-todo-web-application-h2/
docker run -p 8080:8080 bbnsdevelop/todo-web-application-h2:0.0.1-SNAPSHOT
docker run -p 8080:8080 bbnsdevelop/todo-web-application-h2:0.0.1-SNAPSHOT ping google.com
docker run -p 8080:8080 bbnsdevelop/hello-world-rest-api:dockerfile1 param1 param2
docker run -p 8080:8080 bbnsdevelop/todo-web-application-mysql:0.0.1-SNAPSHOT

docker run -p 8080:8080 --network=host  bbnsdevelop/todo-web-application-mysql:0.0.1-SNAPSHOT ping http://localhost:8080 

docker network ls
docker inspect bridge
docker container run -p 8080:8080 --link=mysql -e RDS_HOSTNAME=mysql  bbnsdevelop/todo-web-application-mysql:0.0.1-SNAPSHOT

docker network create web-application-mysql-network
docker run --detach --env MYSQL_ROOT_PASSWORD=dummypassword --env MYSQL_USER=todos-user --env MYSQL_PASSWORD=dummytodos --env MYSQL_DATABASE=todos --name mysql --publish 3306:3306 --network=web-application-mysql-network mysql:5.7
docker container run -p 8080:8080 --network=web-application-mysql-network -e RDS_HOSTNAME=mysql  bbnsdevelop/todo-web-application-mysql:0.0.1-SNAPSHOT
docker container restart mysql
docker container run -p 8080:8080 --network=web-application-mysql-network -e RDS_HOSTNAME=mysql  bbnsdevelop/todo-web-application-mysql:0.0.1-SNAPSHOT

docker container prune


docker run --detach --env MYSQL_ROOT_PASSWORD=dummypassword --env MYSQL_USER=todos-user --env MYSQL_PASSWORD=dummytodos --env MYSQL_DATABASE=todos --name mysql --publish 3306:3306 --network=web-application-mysql-network --volume mysql-database-volume:/var/lib/mysql  mysql:5.7


#/04-spring-boot-react-full-stack-h2/restful-web-services/
docker tag 3f4765872126 bbnsdevelop/rest-api-full-stack:2stagebuild
docker run -p 8080:8080 bbnsdevelop/rest-api-full-stack:2stagebuild

npm install
npm start
npm run build

docker network create currency-network
docker run -p 8000:8000 --network=currency-network --name=currency-exchange-service bbnsdevelop/currency-exchange-service:0.0.1-SNAPSHOT
docker run -p 8100:8100 --network=currency-network --name=currency-conversion-service --env CURRENCY_EXCHANGE_URI=http://currency-exchange-service:8000 -d bbnsdevelop/currency-conversion-service:0.0.1-SNAPSHOT

docker-compose up
docker-compose up -d
docker-compose scale currency-conversion-service=2
docker-compose logs
docker-compose logs -f

docker system prun
docker system prune -a

docker search mysql
docker images
docker tag bbnsdevelop/todo-rest-api-h2:1.0.0.RELEASE latest
docker rmi latest:latest
docker pull mysql
docker image ls --format='{{json .}}'

docker container run -p 5000:5000 -d bbnsdevelop/todo-rest-api-h2:1.0.0.RELEASE
docker container pause 6478
docker container unpause 6478

docker run -p 5000:5000 bbnsdevelop/todo-rest-api-h2:0.0.1-SNAPSHOT
docker run -p 5000:5000 -d bbnsdevelop/todo-rest-api-h2:0.0.1-SNAPSHOT
docker run -p 5000:5000 -d --restart=always bbnsdevelop/todo-rest-api-h2:0.0.1-SNAPSHOT

docker events
docker top c710
docker stats
docker run -m 512m --cpu-quota 50000
docker system df

docker container stop 1b1
docker container kill 9b8

docker-compose config
docker-compose images
docker-compose ps
docker-compose top
docker-compose pause
docker-compose unpause
docker-compose rm
docker-compose build
docker-compose events

Deleted Networks:
web-application-mysql-network
03-todo-web-application-mysql_todo-web-application-network
currency-network
05-microservices_currency-compose-network
```
