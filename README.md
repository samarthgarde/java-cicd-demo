# Simple Java Web Application

A simple Java web application demonstrating an automated CI/CD pipeline using GitHub, Jenkins, Maven, and Apache Tomcat.

## Project Overview

This project demonstrates how source code changes can be automatically built, tested, packaged, and deployed to an Apache Tomcat server using Jenkins.

## CI/CD Workflow

Developer
   ↓
GitHub
   ↓
GitHub Webhook
   ↓
Jenkins
   ↓
Maven Build
   ↓
Maven Test
   ↓
WAR Package
   ↓
Apache Tomcat
   ↓
Web Application

## Technologies Used

- Java
- JSP
- Maven
- Jenkins
- Git & GitHub
- Apache Tomcat
- GitHub Webhooks
- ngrok

## Project Structure

```text
java-cicd-demo/
├── pom.xml
├── Jenkinsfile
├── README.md
├── .gitignore
└── src/
    ├── main/
    │   └── webapp/
    │       └── index.jsp
    └── test/
        └── java/
```

## CI/CD Pipeline

The CI/CD pipeline is set up to automate the build, test, and deployment process:

1.**Build:** Maven is used to compile the code and package it into a WAR file.
2.**Deploy:** The WAR file is deployed to Apache Tomcat for testing and production.
3.**Automation:** Jenkins orchestrates the entire pipeline, ensuring seamless integration and deployment.

## Commit History

- **Main Commit:** Updated index.jsp and configured the CI/CD pipeline.
- **First Commit:** Initial project setup with pom.xml and basic structure.
