# CI/CD Pipeline for Java Web Application Using Jenkins

## Project Overview

This project demonstrates an end-to-end Continuous Integration and Continuous Deployment (CI/CD) pipeline for a Java Web Application using Jenkins, Maven, GitHub, Apache Tomcat, and AWS EC2.

The pipeline automatically builds and deploys the application whenever code changes are pushed to GitHub.

## Architecture

Developer

↓

GitHub Repository

↓

Jenkins Pipeline

↓

Maven Build

↓

WAR File Generation

↓

Apache Tomcat

↓

Java Web Application

## Technologies Used

* AWS EC2 (Amazon Linux 2023)
* Jenkins
* Git & GitHub
* Apache Maven
* Apache Tomcat
* Java 17
* Linux

## Project Structure

cicd-pipeline-java-web-application-using-jenkins/

├── pom.xml

├── Jenkinsfile

├── README.md

├── src/

│   └── main/

│       └── webapp/

│           ├── index.jsp

│           └── WEB-INF/

│               └── web.xml

└── screenshots/

## Prerequisites

* AWS Account
* EC2 Instance
* Java 17
* Maven
* Jenkins
* Apache Tomcat
* GitHub Repository

## Installation Steps

### Clone Repository

git clone https://github.com/SVignesh-Cloud/cicd-pipeline-java-web-application-using-jenkins.git

### Build Application

mvn clean package

### Deploy WAR File

cp target/java-webapp.war /opt/tomcat/webapps/

### Start Tomcat

cd /opt/tomcat/bin

./startup.sh

## Jenkins Pipeline Stages

### Stage 1: Source Code Checkout

Jenkins pulls source code from GitHub.

### Stage 2: Build

Maven compiles and packages the application into a WAR file.

### Stage 3: Deploy

Generated WAR file is deployed to Apache Tomcat.

## Application URL

http://YOUR_PUBLIC_IP:8081/java-webapp

## Features

* Automated Build Process
* Automated Deployment
* GitHub Integration
* Maven Build Automation
* Jenkins Pipeline Automation
* Tomcat Deployment
* CI/CD Workflow

## Screenshots

Add screenshots for:

* Jenkins Dashboard
* Jenkins Pipeline Build
* Maven Build Success
* Tomcat Running
* Application Running in Browser

## Challenges Faced

* Maven WAR Plugin Compatibility Issue with Java 17
* Tomcat Port Configuration
* Jenkins Integration Setup
* Deployment Automation

## Future Enhancements

* Docker Integration
* Kubernetes Deployment
* SonarQube Code Quality Checks
* Nexus Artifact Repository
* Automated Testing Stage
* AWS CodeDeploy Integration

## Author

Vignesh Vicky

AWS | Linux | DevOps | CCNA | Cloud Computing

## Conclusion

This project demonstrates a complete CI/CD implementation using Jenkins for automating the build and deployment of a Java Web Application in an AWS environment.

