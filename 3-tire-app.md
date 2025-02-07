# Three-Tier Application

<kbd>![image](img/3-tire.png)</kbd>

## Overview

A **three-tier application** is a software architecture pattern that separates an application into three layers:

1. **Presentation Layer (Frontend)**
2. **Business Logic Layer (Application Layer)**
3. **Data Layer (Database Layer)**

## Layers in a Three-Tier Architecture

### 1. Presentation Layer (Frontend)

- **User Interface (UI)**: The part of the application that users interact with.
- **Client-Side**: Runs on the user's device (browser, mobile app, or desktop app).
- **Technologies**:
  - Web: HTML, CSS, JavaScript (React, Angular, Vue.js)
  - Mobile: Android (Kotlin), iOS (Swift)
  - Desktop: Electron, JavaFX, .NET

### 2. Business Logic Layer (Application Layer)

- **Application Server**: Handles requests from the frontend and processes business logic.
- **Middleware**: Software that connects the frontend and backend services.
- **REST API (Representational State Transfer)**: A common architecture for communication between layers.
- **Microservices**: A design approach where the business logic is split into smaller, independent services.
- **Technologies**:
  - Programming Languages: Java (Spring Boot), Python (Django, Flask), Node.js, .NET (C#)
  - Web Servers: Apache Tomcat, Nginx, IIS
  - API Protocols: REST, GraphQL, gRPC

### 3. Data Layer (Database Layer)

- **Database Management System (DBMS)**: Stores and manages data.
- **SQL Database**: Structured databases like MySQL, PostgreSQL, and Microsoft SQL Server.
- **NoSQL Database**: Unstructured databases like MongoDB, Cassandra, and Redis.
- **ORM (Object-Relational Mapping)**: A framework that helps interact with databases using objects (e.g., Hibernate for Java, SQLAlchemy for Python).

## Additional Key Concepts

- **Load Balancer**: Distributes traffic between multiple servers to improve performance.
- **Scalability**: The ability of an application to handle increased load by adding more resources.
- **Authentication & Authorization**:
  - **OAuth, JWT, SAML**: Security standards for user authentication.
  - **RBAC (Role-Based Access Control)**: Defines permissions based on user roles.
- **Containerization & Orchestration**:
  - **Docker**: Encapsulates applications into lightweight containers.
  - **Kubernetes**: Manages and scales containerized applications.
- **Caching**:
  - **Redis, Memcached**: Used to store frequently accessed data for faster retrieval.

## Advantages of a Three-Tier Architecture

- **Scalability**: Each layer can scale independently.
- **Security**: Data layer is isolated from direct user access.
- **Maintainability**: Easier to update and manage different components separately.
- **Flexibility**: Can use different technologies for each layer.
