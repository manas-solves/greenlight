# Greenlight API

[![Build status](https://img.shields.io/github/actions/workflow/status/manas-solves/greenlight/CI.yml?label=CI&branch=main)](https://github.com/manas-solves/greenlight/actions/workflows/CI.yml)
[![Codecov branch](https://img.shields.io/codecov/c/github/manas-solves/greenlight/main.svg)](https://codecov.io/gh/manas-solves/greenlight)
[![Go Report Card](https://goreportcard.com/badge/github.com/manas-solves/greenlight)](https://goreportcard.com/report/github.com/manas-solves/greenlight)

A production-ready RESTful API built with **Go** and **PostgreSQL**, designed with a focus on scalability, security, and observable systems architecture. This project serves as a capstone demonstrating advanced backend engineering principles.

🚀 **Live API Documentation:** [manas-solves.github.io/greenlight](https://manas-solves.github.io/greenlight/)

---

## 🛠 Technical Stack
* **Language:** Go 1.24+ (utilizing structured logging and workspace modules)
* **Database:** PostgreSQL 15 (with complex filtering, full-text search, and ACID compliance)
* **Infrastructure:** Docker & Docker-Compose for containerized local development
* **CI/CD:** GitHub Actions for automated testing and Codecov for quality assurance

## 🌟 Key Engineering Features
* **Advanced Concurrency:** Implemented graceful shutdowns and background goroutines for non-blocking email delivery.
* **Security-First Architecture:** Custom middleware for rate limiting (token-bucket), CORS handling, and secure authentication using stateless tokens.
* **Database Optimization:** Built-in support for optimistic concurrency control (preventing race conditions during updates) and advanced PostgreSQL indexing.
* **Automated Tooling:** Managed via `Taskfile` to automate migrations, builds, and integration testing.

## 🚦 Getting Started (WSL2 / Docker)
1. **Clone the repo:** `git clone https://github.com/manas-solves/greenlight.git`
2. **Start Infrastructure:** `docker-compose up -d`
3. **Run Tests:** `task test`

---
