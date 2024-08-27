# Docker Assignment 1

Overview
This project demonstrates how to use Docker and Docker Compose to containerize a Spring Boot application with a MySQL database. The application is a simple Spring Boot service connected to a MySQL database. The application is on prt 8080. For Bonus Question have added db transaction and created multi-container application and configured in yml file.

Steps to run or start the application:
1. Clone the Repository (DockerFile is located in the root of the application)
2. Build the Docker image:
   docker build -t spring-boot-app .
   docker-compose up --build
   (This command builds the Docker image and starts the application and database services.)
3. Application should run on port http://localhost:8080
4. To see the running list containers: docker ps
5. To stop the containers: docker-compose down
6. Remove stopped containers and volumes: docker-compose rm -v
7. Push Docker Image to a Registry Tag the Docker image : docker tag spring-boot-app your-dockerhub-username/spring-boot-app
8. Push the Docker image to Docker Hub: docker push your-dockerhub-username/spring-boot-app
9. Pull Docker Image from a Registry Pull the Docker image from Docker Hub: docker pull your-dockerhub-username/spring-boot-app
10. Run the Docker image locally: docker run -d -p 8080:8080 username/spring-boot-app
