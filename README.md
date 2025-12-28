# Bee Delivery SaaS Platform

## Project Overview
Bee Delivery is a comprehensive On-Demand Delivery Solution engineered for enterprise scalability. It features a microservice-ready architecture comprising a robust Java Spring Boot backend, a responsive Vue.js management dashboard, and a mobile web client for end-users.

## Architecture Structure

The repository is organized as a Monorepo to streamline development and deployment:

### 🔌 Backend Services
- **server-api/**: The primary RESTful API gateway handling order dispatch, payment processing (Stripe/PayPal integration ready), and user authentication.
- **server-core/**: Shared business logic, utility libraries, and database entities ensuring code reusability across modules.
- **Tech Stack**: Java 8+, Spring Boot, JPA/Hibernate, MySQL, Redis (Caching).

### 💻 Frontend Applications
- **admin-dashboard/**: A feature-rich Single Page Application (SPA) for platform administrators and restaurant merchants.
  - Features: Real-time order tracking, menu management, sales analytics.
  - Stack: Vue.js, Element UI, Vuex.

- **mobile-web-client/**: A progressive web application (H5) optimized for mobile browsers, allowing customers to browse menus and place orders without installing native apps.
  - Stack: Vue.js, Vant UI.

## Getting Started

### 1. Backend Setup
Navigate to the `server-api` directory and configure your `application.yml` with your local database credentials.
```bash
cd server-api
mvn clean install
mvn spring-boot:run