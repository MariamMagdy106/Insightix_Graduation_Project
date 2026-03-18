# 🧠 Intelligent Machine Monitoring & Failure Prediction System

### 🚀 .NET Clean Architecture API with AI Integration

---

## 📌 Overview

A **scalable, production-ready system** designed to monitor industrial machines and predict potential failures using **LSTM-based time-series analysis** and a **Clean Architecture backend built with ASP.NET Core**.

The system processes real-time data, detects anomalies, and enables proactive decision-making through intelligent predictions and structured backend design.

---

## 🎯 Core Capabilities

* 📡 Real-time machine data processing
* 🤖 AI-based failure prediction (LSTM)
* 🔔 Automated alerting for abnormal behavior
* 🔐 Secure APIs using JWT authentication
* ⚡ Modular and scalable backend design

---

## 🏗️ Architecture

This project follows **Clean Architecture (Onion Architecture)** to ensure clear separation between business logic and infrastructure concerns.

```id="7g3k2s"
┌──────────────────────────────┐
│         Presentation         │  Controllers, Hubs, Filters
├──────────────────────────────┤
│         Application          │  Services, DTOs, Validators
├──────────────────────────────┤
│         Infrastructure       │  Repositories, Data, EF Core
├──────────────────────────────┤
│            Domain            │  Core Entities & Interfaces
└──────────────────────────────┘
```

### 🔑 Key Principle

Inner layers remain independent from external frameworks, ensuring flexibility and long-term maintainability.

---

## 📁 Project Structure

```id="h9d2kp"
Graduation_Project/
├── Core/              # Domain models & interfaces
├── Data/              # DbContext & configurations
├── Extensions/        # Dependency injection setup
├── Filters/           # Cross-cutting concerns
├── Hubs/              # Real-time communication (SignalR)
├── Migrations/        # Database evolution
├── Modules/           # Feature-based structure
│   └── [Module]/
│       ├── DTOs/
│       ├── Repository/
│       ├── Service/
│       ├── Validators/
│       └── Controller
└── GlobalUsings.cs
```

---

## 🧩 Modular Design

Features are implemented using a **Vertical Slice approach**, where each module encapsulates:

* API contracts (DTOs)
* Data access logic
* Business rules
* Validation
* Endpoints

This structure improves scalability, readability, and team collaboration.

---

## ⚙️ Key Practices

* Repository & Service layers for clean separation
* DTOs to isolate domain from API contracts
* FluentValidation for structured input validation
* SignalR for real-time updates
* EF Core Migrations for controlled database changes

---

## 🤖 AI Component

* LSTM model trained on time-series machine data
* Detects patterns and predicts failures early
* Integrated with backend for seamless inference

---

## 🛠️ Tech Stack

* ASP.NET Core (.NET 8)
* Entity Framework Core
* SQL Server
* SignalR
* FluentValidation
* Python (LSTM)

---

## 🔄 Workflow

1.Machine sensors send real-time data
2. Backend processes and stores data
3. Data is passed to LSTM model for prediction
4. System detects anomalies or failures
5. Alerts are triggered via notifications/dashboard
6. Results are available for monitoring systems

Users monitor system status in real-time
---

## 📈 Highlights

* Clean, scalable architecture ready for extension
* AI-driven predictive capabilities
* Real-time communication support
* Secure and maintainable backend

---

## 🚀 Future Improvements

* Containerization & cloud deployment
* Advanced analytics dashboard
* Direct IoT integration

---

## 📄 Note

This project demonstrates strong capabilities in **software architecture, backend development, and AI integration** within a real-world use case.
