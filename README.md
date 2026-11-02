# Barista - Spring Boot Café Website

A modern café-themed web application built with Java, Spring Boot, HTML, CSS, and JavaScript. This project features a stylish landing page, contact form, reservation page, and Docker support for easy deployment.

## Overview

This project is designed to showcase a coffee shop or café brand with a responsive and visually appealing interface. It includes:

- Home page with hero section and call-to-action buttons
- About section
- Contact form
- Reservation page
- Responsive design for different screen sizes
- Dockerized deployment for portability and consistency

## Tech Stack

- Java 11
- Spring Boot 2.2.4
- Maven
- Thymeleaf
- HTML5
- CSS3
- JavaScript
- Docker

## Application Screenshots

Add the actual app screenshots into the `docs/images/` folder and use them in the README as shown below.

![Barista Home Page](docs/images/home-page.png)

![Barista Contact Page](docs/images/contact-page.png)

## Project Structure

```text
springboot-project/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── siddardha/
│       │           └── StartApplication.java
│       └── resources/
│           ├── application.properties
│           └── static/
│               ├── css/
│               ├── js/
│               ├── fonts/
│               ├── images/
│               ├── index.html
│               ├── reservation.html
│               └── ...
├── pom.xml
├── Dockerfile
├── README.md
├── .gitignore
└── docs/
    └── images/
```

## Prerequisites

Before running the application, make sure the following are installed:

- Java 11 or later
- Maven
- Docker (optional, for containerized deployment)

## Run the Application Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Jaya-prakash05/springboot-project.git
cd springboot-project
```

### 2. Build and Run with Maven

```bash
mvn clean install
mvn spring-boot:run
```

The application will run on:

```text
http://localhost:9090
```

## Docker Setup

### Build Docker Image

```bash
docker build -t springboot-project .
```

### Run Docker Container

```bash
docker run -d -p 9090:9090 --name springboot-project springboot-project
```

Then open:

```text
http://localhost:9090
```

## Features

- Responsive café landing page
- Contact form section
- Reservation interface
- Dynamic front-end styling
- Spring Boot backend configuration
- Containerized deployment using Docker

## Configuration

The app configuration is defined in `src/main/resources/application.properties`:

```properties
server.port=9090
spring.mvc.view.prefix=/static/
spring.mvc.view.suffix=.html
```

## Notes

This project is a simple yet complete example of a Spring Boot web application with front-end assets stored in the `static` folder. It is suitable for learning web application development, deployment, and Dockerization.

## Author

Jaya Prakash
