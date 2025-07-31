# 🧪 UMBRELLA ACCESS CORE

High-security access control system core module for Umbrella Corporation facilities. This is the domain logic layer designed using **Clean Architecture** and **Domain-Driven Design (DDD)** principles to ensure modularity, testability, and maintainability.

---

## 📖 Overview

This repository represents the **pure domain logic** of the access system. No database, HTTP, or infrastructure dependencies — only the core business rules governing how personnel interact with secure areas, experiments, and other sensitive entities.

---

## 🧱 Project Structure

src/
├── domain/
│ ├── entities/
│ ├── value-objects/
│ ├── repositories/
├── application/
│ └── use-cases/
├── shared/
└── utils/


---

## 👥 Core Entities

| Entity     | Purpose                                                  |
|------------|----------------------------------------------------------|
| `Employee` | Represents authorized personnel. Manages roles and clearance levels. |
| `Experiment` | Tracks research operations, biological assets, and their classification. |
| `Zone`     | Represents secure physical or logical areas of containment. |

---

## 🚨 Domain Rules

- Employees are assigned a role and a clearance level from 0 to 5.
- Experiments are restricted to specific zones and clearance levels.
- Zones are categorized by security levels (Alpha, Beta, Delta, Hive).
- Access is granted based on role + clearance + zone policy.

---

## 🛡️ Technologies Used

- **TypeScript**: Strong typing and scalability
- **Zod**: Runtime schema validation for value safety
- **Clean Architecture**: Separation of concerns
- **Domain-Driven Design (DDD)**: Strategic modeling

---

## 🧪 Current Progress

- ✅ Initial project structure (Clean + DDD)
- ✅ `Employee` entity modeled with role & clearance
- ⏳ `Experiment` and `Zone` entities (in progress)
- ⏳ Domain service: access evaluator
- ⏳ Unit testing

---

## 📜 Documentation

You can find detailed technical decisions, diagrams, and architecture logs in the [`docs/`](./docs/) folder:

- [`docs/UMBRELLA_ARCHITECTURE_OVERVIEW.md`](./docs/UMBRELLA_ARCHITECTURE_OVERVIEW.md)

---

## 🧠 Mission Logs

Every week, a new phase of the system will be designed, implemented, and documented. Each module follows real-world architecture standards to simulate high-risk enterprise system development.

---

## 📡 Security Protocols

> Access to experiments and classified zones is **strictly enforced** by domain rules. No external actor may bypass core logic validation.

---

## 📈 Vision

This is part of the **Umbrella Engineering Initiative**, a full-stack architecture simulation using real-world best practices. The goal is to solidify advanced architecture skills using TypeScript while producing production-grade open-source projects.

