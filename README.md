# AWS + DevOps Sample Java Web Application

This is a small JSP-based Java web application packaged as `sample.war` for the Jenkins, Docker, Docker Hub, Ansible, Kubernetes, and Tomcat learning project.

## Requirements
- Java web server: Apache Tomcat 10.1 or newer (Tomcat 10.1 is recommended)
- Java 11 or newer

## Build the WAR with Maven
This project includes a Maven `pom.xml`. Run:
```bash
mvn clean package
```
The resulting WAR is created at `target/sample.war`.

## Deploy to Tomcat
Copy `target/sample.war` to Tomcat's `webapps/` directory, then start/restart Tomcat. Open:
`http://SERVER_IP:8080/sample/`

## Important
The supplied WAR is a prebuilt, minimal JSP web application. For a reproducible pipeline, build it from source using Maven in Jenkins rather than relying on a manually copied binary.
