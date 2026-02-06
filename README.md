# DynamoDB Design Patterns

A curated collection of DynamoDB design patterns, focused on single-table design, access patterns, and scalable data modeling for real-world serverless applications.

This repository is intended as a **practical reference** for engineers who want to go beyond basic CRUD usage of DynamoDB and understand how to design **production-ready NoSQL data models**.

---

## 🎯 Purpose

The goal of this repository is to:

- Demonstrate **how to design DynamoDB tables based on access patterns**
- Explore **single-table design** and when (and when not) to use it
- Show real-world patterns used in **serverless architectures**
- Document **design decisions**, trade-offs, and constraints
- Serve as a **learning and interview reference** for senior-level discussions

This is **not** a beginner tutorial, nor a generic AWS SDK showcase.

---

## 🧠 Core Principles

All designs in this repository follow these principles:

- **Access patterns first**  
  Tables are designed starting from *how data is queried*, not from entities.

- **Single-table where it makes sense**  
  Multiple entity types can coexist in one table when it reduces complexity and cost.

- **Minimal GSIs**  
  Secondary indexes are added only when access patterns cannot be satisfied by the primary keys.

- **Explicit trade-offs**  
  Every pattern includes an explanation of *why* it exists and *what it optimizes*.

- **Production-oriented**  
  Patterns consider scalability, cost, consistency, and operational simplicity.

---

## 🧱 Patterns Covered

This repository will progressively cover patterns such as:

- Single-Table Core Pattern
- One-to-Many and Many-to-One relationships
- Hierarchical data (adjacency lists)
- Time-based and event data
- Connection/session tracking (e.g. WebSocket use cases)
- Conditional writes and idempotency
- Versioning and soft deletes
- TTL and lifecycle management
- Indexing strategies (GSI / LSI)

Each pattern is documented with:
- Access patterns
- Table design (PK / SK)
- Example items
- Query examples
- Design rationale

---

## 🛠 Tech Stack

Examples may include:

- Amazon DynamoDB
- AWS SDK (Node.js / TypeScript or Python)
- AWS Lambda
- AWS SAM / CloudFormation
- DynamoDB Local (for local testing)

The focus is **data modeling**, not framework-specific code.

---

## 👤 Who This Is For

- Backend / Cloud engineers working with AWS
- Engineers transitioning from SQL to NoSQL
- Senior developers preparing for system design interviews
- Anyone designing **serverless systems at scale**


---

## 📌 Status

🚧 Work in progress  
Patterns and examples are added incrementally as the repository evolves.

