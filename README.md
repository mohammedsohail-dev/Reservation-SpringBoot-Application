# Reservation System - Spring Boot Backend

![Java](https://img.shields.io/badge/Java-11-%23ED8B00?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-2.7.%2B-%236DB33F?logo=springboot)
![Maven](https://img.shields.io/badge/Maven-3.8.1-%23C71A36?logo=apachemaven)
![MongoDB](https://img.shields.io/badge/MongoDB-5.%2B-%2347A248?logo=mongodb)
![Keycloak](https://img.shields.io/badge/Keycloak-21.0.0-%23F7F7F7?logo=keycloak)

A secure Spring Boot backend application for reservation management with MongoDB persistence and Keycloak/ JWT authentication.

## Key Features

- **Secure REST API** with:
  - JWT authentication (jjwt 0.11.5)
  - Keycloak integration (21.0.0)
  - OAuth2 resource server
- **MongoDB** data persistence
- **Spring Security** with OAuth2 client/resource support
- **Developer Friendly**:
  - Lombok for boilerplate reduction
  - Spring Boot DevTools
  - Maven wrapper included

## Technology Stack

- **Core**: Java 11, Spring Boot 2.7+
- **Database**: MongoDB
- **Security**:
  - Spring Security 5.7.8
  - Keycloak 21.0.0
  - JJWT 0.11.5
- **Tools**:
  - Lombok
  - Maven 3.8.1

## UML Diagram
![image](https://github.com/user-attachments/assets/ea9cf090-bda6-4856-8ab5-a10a8c66c3da)


## Getting Started

### Prerequisites

- Java 11 JDK
- Maven 3.8+
- MongoDB 5+
- Keycloak server (optional) delete security folder for this

### Configure your MongoDB and Keycloak in application.properties:
- spring.data.mongodb.uri=mongodb://localhost:27017/reservations
- keycloak.realm=your-realm
- keycloak.auth-server-url=http://localhost:8080/auth
- keycloak.resource=your-client-id

### Build and run:
- mvn clean install
- mvn spring-boot:run
