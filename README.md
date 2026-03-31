# 🏥 MediPlus Project Platform

---

The **MediPlus Project Platform** is the core infrastructure repository for the microservices-based system.  
This repository aggregates essential platform-level services such as the **Config-Server**, **Service-Registry**, and **API Gateway** using Git submodules.

It acts as the foundation layer that enables configuration management, service discovery, and centralized request routing for all domain services in the system.

---

## 👤 Student Information

- **Student Name:** Charith Mihiranga Siriwardana
- **Student Number:** 2301691075
- **Slack:** https://ijse-eca-hdse-69-70.slack.com/team/U0AHD5TQ4H5
- **GCP Project ID:** ts-2130-eca-gdse-491417

---

## 📖 About

This repository is designed to manage and organize the core platform services required for running the MediPlus microservices ecosystem.  
Instead of duplicating code or maintaining separate setups, all foundational services are included as **Git submodules**, ensuring modularity and easy updates.

The platform enables:

- Centralized configuration management via Config-Server
- Dynamic service discovery using Service-Registry (Eureka)
- Unified request routing through API Gateway
- Scalable and maintainable microservice architecture

This structure simplifies development, deployment, and collaboration across multiple services.

---

## 🧩 Included Services

| Service           | Description                                      |
|------------------|--------------------------------------------------|
| Config-Server     | Centralized configuration management             |
| Service-Registry  | Service discovery using Netflix Eureka           |
| API Gateway       | Reactive request routing and entry point         |

---

## 📁 Repository Structure

```bash
medi-plus-platform/
├── config-server/      # Config Server (submodule)
├── service-registry/   # Eureka Service Registry (submodule)
├── api-gateway/        # API Gateway (submodule)
├── ecosystem.config.js
├── pom.xml
└── README.md
```

---

## 🔗 Git Submodules

This repository uses **Git submodules** to include individual services.

### Clone with submodules

```bash
git clone --recurse-submodules <repo-url>
```

### If already cloned

```bash
git submodule update --init --recursive
```

---

## ⚙️ Getting Started

### 🔄 Startup Order

1. Config-Server (9100)
2. Service-Registry (9001)
3. API Gateway (7001)

---

### ▶️ Run Services

Navigate into each submodule and run:

```bash
./mvnw spring-boot:run
```

---

## 🌐 Access Points

| Service          | URL                        |
|-----------------|----------------------------|
| Config-Server   | http://localhost:9100      |
| Service-Registry| http://localhost:9001      |
| API Gateway     | http://localhost:7001      |

---

## 🚀 Overview

This platform provides the **backbone of the MediPlus system**, enabling seamless communication between microservices and ensuring a scalable, maintainable, and production-ready architecture.

---