AdvancedJavaSpringBootProject - URL Shortener

This is a Spring Boot-based URL shortener application designed for advanced use cases,
integrating MySQL for data storage, JWT for secure authentication,
Maven for build automation, and Docker for containerization.

Features

URL Shortening: Converts long URLs into short, unique links.
JWT Authentication: Secure the API with JSON Web Token (JWT) authentication.
MySQL Database: Stores shortened URLs and their mappings.
Docker: Containerizes the application for easy deployment.
Maven: Build automation using Maven.

Requirements

Before running this project, ensure that you have the following installed on your system:
JDK 11 or higher
MySQL Database Server
Maven
Docker

Getting Started

1. Clone the repository
   
Clone this repository to your local machine using:
git clone https://github.com/your-username/AdvancedAJavaSpringBootProject.git


3. Set up MySQL Database
    
Create a MySQL database for the application:
CREATE DATABASE urlshortener;
Update the application.properties file with your MySQL credentials:
spring.datasource.url=jdbc:mysql://localhost:3306/urlshortener
spring.datasource.username=root
spring.datasource.password=password

4.Build the Project using Maven

Navigate to the project directory and run the following command to build the project:
mvn clean install

5. Docker Setup (Optional)
   
To run the project using Docker, you need to build the Docker image. Make sure Docker is installed on your system and run the following:
docker build -t urlshortener-app .
docker run -p 8080:8080 urlshortener-app
This will start the application on http://localhost:8080.

5. Running the Application
Once built and set up, you can run the application using:

mvn spring-boot:run
This will start the Spring Boot application on http://localhost:8080.
