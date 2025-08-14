# Zidio Connect - Internship Project 

> **Internship Submission**: This project was developed as part of an internship program, demonstrating proficiency in full-stack development with both monolithic and microservices architectures.

A comprehensive professional networking and job portal platform built with both **Monolithic** and **Microservices** architectures, featuring React frontend and Spring Boot backend services.

## 📋 Internship Project Overview

**Intern Name**: [Your Name]  
**Internship Duration**: [Start Date] - [End Date]  
**Company**: [Company Name]  
**Mentor**: [Mentor Name]  
**Project Type**: Full-Stack Development with Dual Architecture Implementation

### Learning Objectives Achieved
- ✅ Monolithic vs Microservices Architecture Design
- ✅ Spring Boot & Spring Cloud Implementation
- ✅ React Frontend Development
- ✅ JWT Authentication & Security
- ✅ Database Design & Integration
- ✅ Service Discovery & API Gateway
- ✅ RESTful API Development

## 🏗️ Architecture Overview

This project demonstrates two different architectural approaches:

### 1. **Monolithic Architecture** (`Backend_java_spring/`)
- Single deployable unit containing all business logic
- Centralized database and configuration
- Simpler deployment and development setup

### 2. **Microservices Architecture** (`microservices/`)
- Distributed system with independent services
- Service discovery with Eureka Server
- API Gateway for request routing
- Individual databases per service

## 🚀 Features

- **User Authentication & Authorization** (JWT-based)
- **Student Profile Management**
- **Recruiter Dashboard**
- **Job Posting & Application System**
- **Professional Networking & Connections**
- **File Upload & Management**
- **Email Notifications**
- **Admin Panel**
- **Analytics & Reporting**

## 🛠️ Technology Stack

### Backend
- **Java 8/17**
- **Spring Boot 2.7.15**
- **Spring Cloud 2021.0.8**
- **Spring Security**
- **JWT Authentication**
- **PostgreSQL Database**
- **Maven Build Tool**

### Frontend
- **React 19.1.0**
- **React Router DOM**
- **Axios for API calls**
- **Tailwind CSS**
- **Lucide React Icons**

### Microservices Components
- **Eureka Server** (Service Discovery)
- **API Gateway** (Request Routing)
- **Auth Service** (Authentication)
- **Student Service** (Student Management)
- **Job Service** (Job Management)
- **Admin Service** (Admin Operations)
- **Email Service** (Notifications)
- **File Upload Service** (File Management)
- **Analytics Service** (Reporting)

## 📋 Prerequisites

- **Java 8+** (JDK 8 for monolithic, JDK 17 for microservices)
- **Node.js 16+** and **npm**
- **PostgreSQL 12+**
- **Maven 3.6+**

## 🗄️ Database Setup

1. Create PostgreSQL database:
```sql
CREATE DATABASE "zidio-new";
```

2. Update credentials in configuration files

## 🚀 Quick Start

### Option 1: Monolithic Architecture

```bash
# Backend
cd Backend_java_spring
mvn clean install
mvn spring-boot:run

# Frontend
cd Front_end_react
npm install
npm start
```

**Access**: Frontend: http://localhost:3000 | Backend: http://localhost:8080

### Option 2: Microservices Architecture

```bash
# Automated startup
cd microservices
start-services.bat

# Manual startup
cd microservices/eureka-server && mvn spring-boot:run
cd microservices/auth-service && mvn spring-boot:run
cd microservices/api-gateway && mvn spring-boot:run

# Frontend
cd Front_end_react
npm install
npm start
```

**Access**: Frontend: http://localhost:3000 | Gateway: http://localhost:8080 | Eureka: http://localhost:8761

## 🔧 Service Ports

| Service | Port | Description |
|---------|------|-------------|
| Eureka Server | 8761 | Service Discovery |
| API Gateway | 8080 | Request Router |
| Auth Service | 8081 | Authentication |
| Student Service | 8082 | Student Management |
| Job Service | 8084 | Job Management |

## 📁 Project Structure

```
zidio-connect/
├── Backend_java_spring/          # Monolithic Architecture
├── microservices/               # Microservices Architecture
│   ├── eureka-server/          # Service Discovery
│   ├── api-gateway/            # API Gateway
│   ├── auth-service/           # Authentication
│   └── start-services.bat      # Startup Script
└── Front_end_react/            # React Frontend
```

## 📝 Key API Endpoints

- `POST /api/auth/register` - User Registration
- `POST /api/auth/login` - User Login
- `GET /api/students/profile` - Student Profile
- `GET /api/jobs` - Job Listings
- `POST /api/jobs/{id}/apply` - Job Application

## 🧪 Testing

```bash
# Backend
cd Backend_java_spring && mvn test
cd microservices && mvn test

# Frontend
cd Front_end_react && npm test
```

## 📦 Production Build

```bash
# Frontend
cd Front_end_react && npm run build

# Backend
cd Backend_java_spring && mvn clean package
cd microservices && mvn clean package
```

## 🎯 Internship Achievements

- **Architecture Design**: Successfully implemented both monolithic and microservices patterns
- **Full-Stack Development**: Complete frontend-backend integration
- **Security Implementation**: JWT-based authentication system
- **Database Integration**: PostgreSQL with JPA/Hibernate
- **Service Communication**: Inter-service communication in microservices
- **API Development**: RESTful services with proper error handling

---

**Internship Project Completed Successfully** ✅
