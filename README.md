# Url-Shortener-Service

# Shortify

A modern URL shortening service built with **NestJS**, **TypeScript**, **PostgreSQL**, and **Redis**.

Shortify is a backend-focused project created to explore how a production-ready URL shortener can be designed and implemented. The project emphasizes clean architecture, security, scalability, caching, and maintainable code over simply delivering features.

---

## Why This Project?

Most URL shorteners look simple on the surface, but they involve many interesting backend engineering challenges, such as:

* Generating unique short URLs
* Handling millions of redirects efficiently
* Reducing database load with caching
* Collecting analytics without slowing down redirects
* Designing secure authentication and authorization
* Building APIs that are easy to maintain and extend

This project is an opportunity to learn and apply these concepts in a single backend application.

---

## Tech Stack

| Category          | Technology              |
| ----------------- | ----------------------- |
| Language          | TypeScript              |
| Framework         | NestJS                  |
| Database          | PostgreSQL              |
| ORM               | Prisma                  |
| Cache             | Redis                   |
| Authentication    | JWT & Refresh Tokens    |
| API Documentation | Swagger                 |
| Testing           | Jest                    |
| Containerization  | Docker & Docker Compose |

---

## Features

### Authentication

* User Registration
* Secure Login
* JWT Authentication
* Refresh Tokens
* Role-Based Access Control

### URL Management

* Create Short URLs
* Custom Aliases
* Update & Delete URLs
* URL Expiration
* Password Protection
* Maximum Click Limit
* QR Code Generation

### Redirect Service

* Fast Redirect Endpoint
* Redis Cache
* Database Fallback
* Cache-Aside Pattern

### Analytics

* Total Clicks
* Unique Visitors
* Browser & Operating System
* Referrer Tracking
* Country Detection
* Daily Click Statistics
* Top Performing URLs

### Search

* Search URLs
* Search by Alias
* Pagination
* Sorting
* Filtering

### Security

* Input Validation
* Rate Limiting
* Global Exception Handling
* Audit Logging

---

## Architecture

```text
               Client
                  │
                  ▼
            REST Controllers
                  │
                  ▼
             Business Logic
                  │
        ┌─────────┴─────────┐
        ▼                   ▼
      Redis            PostgreSQL
```

The application follows a layered architecture to keep responsibilities separated and improve maintainability.

---

## Project Structure

```text
src
├── auth
├── users
├── urls
├── analytics
├── cache
├── common
├── config
├── database
├── prisma
└── main.ts
```

---

## Current Progress

* [ ] Project Setup
* [ ] Authentication
* [ ] URL Shortening
* [ ] Redirect Service
* [ ] Redis Integration
* [ ] Analytics
* [ ] Search
* [ ] Rate Limiting
* [ ] Testing
* [ ] Docker
* [ ] Documentation

---

## Design Goals

This project is being developed with the following principles in mind:

* Clean and modular architecture
* Readable and maintainable code
* Secure API design
* Scalable backend components
* Proper validation and error handling
* Performance optimization using caching
* Comprehensive testing
* Consistent development practices

---

## Future Improvements

The current scope focuses on a single backend service. Future iterations may include:

* Background jobs for analytics processing
* Distributed caching strategies
* Event-driven architecture
* API versioning
* Kubernetes deployment
* CI/CD pipeline
* Monitoring and observability
* Multi-region deployment

---

## Learning Outcomes

Building this project provides hands-on experience with:

* REST API Development
* Backend System Design
* Authentication & Authorization
* Database Modeling
* Redis Caching
* Docker
* Testing
* Production-Oriented Development

---

## License

This project is released under the MIT License.
