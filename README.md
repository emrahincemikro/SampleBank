# SampleBank


# **Microservice Architecture Patterns**

This document covers essential microservice design patterns with real-world implementation details. It provides a comprehensive overview for software developers and system architects.

---

## **1. Microservice Patterns**

### **Service per Database**
- Each microservice has its own database, ensuring loose coupling.
- **Examples:** 
  - PostgreSQL for Customer and Account services.
  - MongoDB for Transaction service.

### **API Gateway Pattern**
- Manages client requests, routes them to appropriate microservices, enhances security, and reduces complexity.
- **Example Framework:** Ocelot API Gateway.

---

## **2. Communication Patterns**

### **Request-Response**
- Synchronous communication between services.
- **Example Technology:** gRPC.

### **Event-Driven Architecture**
- Asynchronous communication using events published and consumed between services.
- **Technologies:** RabbitMQ, MassTransit.

---

## **3. Data Management Patterns**

### **Database per Service**
- Each microservice owns its database, ensuring data isolation.

### **CQRS (Command Query Responsibility Segregation)**
- Separates read and write operations for better scalability and performance.

### **Repository Pattern**
- Decouples data access logic from business logic.
- **Applied in:** Transaction Service.

---

## **4. Resilience Patterns**

### **Retry and Circuit Breaker**
- Ensures fault-tolerant HTTP communication.
- **Example Technology:** Polly with IHttpClientFactory.

### **Health Checks**
- Monitors microservice health and detects failures early.

---

## **5. Architectural Patterns**

### **Clean Architecture**
- Separation of concerns into different layers:
  - **Application**
  - **Domain**
  - **Infrastructure**
  - **Presentation**

### **Domain-Driven Design (DDD)**
- Keeps business logic at the core for better business understanding and maintainability.

---

## **6. Observability Patterns**

### **Centralized Logging**
- Unified logging system for monitoring and debugging.
- **Technologies:** Elastic Stack (ELK), SeriLog.

### **Distributed Tracing**
- Enables tracing of requests across services.
- **Technology:** Logstash.

---

## **7. Deployment Patterns**

### **Containerization**
- Ensures consistent deployment across environments.
- **Technology:** Docker Compose.

### **Environment Variable Configuration**
- Enables customization across environments without changing code.

---
