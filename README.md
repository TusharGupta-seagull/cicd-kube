# End to End CI/CD Pileline using Jenkins

## About the Project
Created an end to end ci/cd pipeline using jenkins, sonarqube docker, helm kuberntes

## Prerequisites

### Jenkins-plugins
- Sonarqube scanner
- BuildTimestamp
- Pipeline Utility Steps
- Docker
- Docker pipeline

### Tools
- Helm
- Maven 3.9
- JDK 11
- SonarScanner 4.7 

## Flow of Execution
- EC2 Instance Setup for Jenkins server, Sonarqube server, Kops server.
- Create Dockerfile for mysql-database and push to dockerhub
- Setup Docker Engine in Jenkins
- Create Kubernetes Cluster using Kops
- Create Helm charts
- Test charts in K8s Cluster in test namespace
- Add Kops VM as Jenkins Slave
- Create Pipeline Code in Declarative style
- Create Jenkins job for pipeline
- Run & Test the job

## Technologies used in the vprofile application
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
## Database for vprofile application
Look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql