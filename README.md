# Personal Finance Management Application

## Overview

This project is a Personal Finance Management application developed using Java - Spring Boot. The application is designed with a clean architecture, oriented towards microservices, and leverages functional and reactive programming paradigms.

## Features

- **Income and Expense Management**: Manually record and categorize transactions, with automatic classification of transactions.
- **Budgets and Savings**: Create and track custom budgets, set savings goals, and monitor progress.
- **Reports and Analysis**: Generate monthly and annual financial reports, and visualize income vs. expenses with charts.
- **Bank Integration**: Synchronize with bank accounts to automatically import transactions and receive notifications for suspicious activities or budget limits.
- **Reminders and Alerts**: Set reminders for bill payments and receive alerts when budget limits are reached.
- **Financial Planning**: Simulate financial scenarios and receive financial advice based on data analysis.

## Architecture

The application is built using a microservices architecture, with each service responsible for a specific domain. The services communicate via RESTful APIs and are designed to be independently deployable and scalable.

### Microservices

1. **User Service**: Manages user authentication, authorization, and profile management.
2. **Transaction Service**: Handles the recording and management of financial transactions.
3. **Budget Service**: Manages the creation and tracking of budgets.
4. **Report Service**: Generates financial reports and visualizations.
5. **Bank Integration Service**: Synchronizes with bank accounts and other financial services.

### Technologies Used

- **Java - Spring Boot**: Core framework for building and configuring the application.
- **Spring WebFlux**: For building reactive, non-blocking applications.
- **Spring Data**: For data access with support for SQL (PostgreSQL) and NoSQL (MongoDB) databases.
- **Spring Security**: For implementing authentication and authorization.
- **Kafka or RabbitMQ**: For asynchronous communication between microservices.
- **Docker and Kubernetes**: For containerization and orchestration, enabling easy deployment and scalability.
- **GraphQL**: For efficient and flexible data querying.
- **OAuth2**: For secure integration with banking and third-party services.

## Getting Started

### Prerequisites

- JDK 11 or later
- Docker
- Docker Compose (for local development)
- PostgreSQL (or other preferred database)
- Kafka or RabbitMQ (for message brokering)

### Setting Up the Development Environment

1. **Clone the Repository**
    ```bash
    git clone https://github.com/yourusername/finance-management-app.git
    cd finance-management-app
    ```

2. **Build the Application**
    ```bash
    ./mvnw clean install
    ```

3. **Run the Application with Docker Compose**
    ```bash
    docker-compose up
    ```

### Running Individual Microservices

Each microservice can be run individually for development and testing purposes. Navigate to the respective microservice directory and use the following commands:

1. **User Service**
    ```bash
    cd user-service
    ./mvnw spring-boot:run
    ```

2. **Transaction Service**
    ```bash
    cd transaction-service
    ./mvnw spring-boot:run
    ```

3. **Budget Service**
    ```bash
    cd budget-service
    ./mvnw spring-boot:run
    ```

4. **Report Service**
    ```bash
    cd report-service
    ./mvnw spring-boot:run
    ```

5. **Bank Integration Service**
    ```bash
    cd bank-integration-service
    ./mvnw spring-boot:run
    ```


