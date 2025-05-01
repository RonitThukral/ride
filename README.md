# 🚖 Uber-Like Microservices Backend App

A scalable backend for an Uber-like ride-hailing application built with Node.js and Express, following a microservices architecture. The system includes services for location tracking, driver management, ride handling, notifications, and payment processing. The services communicate via Kafka and utilize Redis for caching and temporary data storage. All services are containerized using Docker for easy deployment and scaling.

---

## 🧩 Microservices Overview

| Service       | Description                                               |
|---------------|-----------------------------------------------------------|
| **Location**  | Tracks and updates real-time locations of drivers/users.  |
| **Driver**    | Manages driver registration, authentication, and status. |
| **Ride**      | Handles ride requests, matching, and ride lifecycle.      |
| **Notification** | Sends SMS, email, or in-app notifications.           |
| **Payment**   | Processes payments, fare calculation, and transaction logs. |

---

## 🛠 Tech Stack

- **Node.js** & **Express.js** – Core backend framework
- **Kafka** – Message broker for event-driven communication
- **Redis** – Caching and session storage
- **MongoDB  – Primary database
- **Docker** – Containerization of services
- **Docker Compose** – Orchestrating multi-container services

---

## 🚀 Features

- Real-time ride matching and tracking
- Driver availability and location updates
- Secure payment handling with fare estimation
- Notification service with Kafka topic subscriptions
- Event-driven architecture for scalable communication
- RESTful API structure with Swagger UI

---

## 🐳 Docker Setup

### Prerequisites

- Docker & Docker Compose
- Kafka & Zookeeper (auto-launched via Docker)
- Redis

### Quick Start

```bash
git clone https://github.com/RonitThukral/uber-backend.git
cd backend
docker-compose up --build
