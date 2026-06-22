# Spring Boot DevOps App

This project is a simple Spring Boot application that I built while learning DevOps concepts. The main goal was not just to create a Java application, but also to understand how modern applications are built, containerized, and automated using DevOps tools.

## What I Built

* A Spring Boot application with a simple REST API
* Dockerized the application using a Dockerfile
* Created a GitHub Actions workflow for Continuous Integration (CI)
* Automated the build process using Maven
* Generated build artifacts automatically on every push

## Technologies Used

* Java
* Spring Boot
* Maven
* Docker
* GitHub Actions
* Git & GitHub

## Project Structure

```text
spring-boot-devops-app
├── .github/workflows
├── src
├── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## How to Run the Application

### Clone the Repository

```bash
git clone https://github.com/siddhantnigam012-crypto/spring-boot-devops-app.git
cd spring-boot-devops-app
```

### Run Using Maven

```bash
./mvnw spring-boot:run
```

### Build the JAR File

```bash
./mvnw clean package
```

### Run the JAR File

```bash
java -jar target/*.jar
```

## Docker Setup

### Build Docker Image

```bash
docker build -t spring-boot-devops-app .
```

### Run Docker Container

```bash
docker run -p 8080:8080 spring-boot-devops-app
```

## CI Pipeline

The GitHub Actions workflow automatically:

* Checks out the source code
* Sets up Java
* Builds the project using Maven
* Generates the JAR file
* Uploads build artifacts

This removes the need to manually build the application every time changes are pushed to GitHub.

## What I Learned

While working on this project, I learned:

* How Spring Boot applications are structured
* The difference between source code and build artifacts
* How Docker packages an application into a container
* How GitHub Actions automates repetitive tasks
* Basic Continuous Integration (CI) concepts
* Maven build lifecycle and JAR generation

## Next Steps

* Deploy the application
* Extend the pipeline into a complete CI/CD workflow
* Learn Kubernetes for container orchestration
* Add cloud deployment using AWS

## Author

Siddhant Nigam

Cloud Computing Student | Learning DevOps and Cloud Technologies
