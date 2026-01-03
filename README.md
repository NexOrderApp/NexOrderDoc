# NexOrder – Cloud-Native Microservices Platform

NexOrder is a **cloud-native, event-driven microservices platform** built to demonstrate **production-aligned backend architecture** using **.NET, Azure, and modern design patterns**.

The project focuses on **clean architecture, scalability, security, and cloud-native integrations**, rather than UI-heavy features.

---

## 🚀 Platform Overview

NexOrder is composed of multiple independent microservices, each owning its domain and data, communicating asynchronously via messaging and secured centrally using an API Gateway.

**Key architectural goals:**
- Loose coupling between services
- Centralized authentication & API security
- Event-driven communication
- Cloud-first deployment approach
- Production-grade configuration and secret management

---

## 🧩 Microservices

| Service | Responsibility | Repository |
|------|---------------|-----------|
| **User Service** | User management and user-related data | https://github.com/NexOrderApp/NexOrder.UserService |
| **Product Service** | Product catalog and product lifecycle events | https://github.com/NexOrderApp/NexOrder.ProductService |
| **Order Service** | Order creation and order processing | https://github.com/NexOrderAppl/NexOrder.OrderService |
| **Auth Service** | Token-based authentication and JWT issuance | https://github.com/NexOrderApp/NexOrder.AuthService |

---

## 🏗️ Architecture

- **Azure Functions** for serverless microservices
- **Azure API Management (APIM)** as the API Gateway
- **JWT-based authentication** enforced at APIM level
- **Azure Service Bus (Topics & Subscriptions)** for asynchronous communication
- **SQL Server / Azure SQL** for persistence
- **Azure Key Vault** for secrets and configuration
- **GitHub Actions** for CI/CD pipelines

---

## 🔐 Security & Authentication

- Authentication handled via **Azure API Management**
- JWT validation using `validate-jwt` policies
- Tokens issued by **Auth Service**
- Services remain stateless and secure

---

## 📦 Messaging & Event-Driven Design

- Azure Service Bus Topics & Subscriptions
- Domain events published and consumed asynchronously
- Enables loose coupling and scalability

---

## 🗄️ Data Persistence

- Database per microservice
- Entity Framework Core (Code First)
- Fluent API configurations
- No shared databases

---

## ⚙️ CI/CD & Deployment

- GitHub Actions per service
- Build, migrate, and deploy Function Apps
- Secure config via App Settings and Key Vault

---

## 🧠 Design Principles

- Clean Architecture
- CQRS with MediatR
- SOLID principles
- Separation of concerns

---

## 🎯 Purpose

Learning-focused project to demonstrate real-world backend architecture and Azure integrations.

---

## 🛠️ Tech Stack

- .NET, Azure Functions
- Azure APIM, Service Bus, Key Vault
- SQL Server / Azure SQL
- JWT Authentication
- GitHub Actions

---

## 📄 License

For learning and demonstration purposes.
