# Project Overview

## Project Name

Nomad Crew

## Description

An app for creating disposable groups for trips, featuring live location sharing, messaging, media sharing, and expense splitting.

# System Architecture

## 1. Frontend

### Technology

Svelte Kit

### Key Features

- User authentication
- Group creation/joining interface
- Live map with location tracking
- Chat functionality
- Media sharing interface
- Expense splitting tool

### Development Guidelines

- Embrace the simplicity and reactive nature of Svelte to write less, more readable code.
- Leverage Svelte Native's built-in state management for a more intuitive handling of app state.
- Prioritize performance optimizations inherent to Svelte Native, aiming for smooth, native-like experiences.
- Ensure thorough testing on multiple devices for compatibility and performance.
- Pay close attention to user privacy and data security, especially in location sharing features.

## 2. Backend

### Technology

Go with gRPC for service communication

### Services

- **User Service:** Handles user authentication and profile management.
- **Group Service:** Manages group creation, membership, and deletion.
- **Location Service:** Tracks and updates user locations.
- **Messaging Service:** Manages in-app messaging and notifications.
- **Media Service:** Handles uploading and retrieving media.
- **Expense Service:** Manages expense records and splitting functionality.

### Development Guidelines

- Ensure robust error handling and logging (consider using Zap for Go logging).
- Implement gRPC for efficient inter-service communication.
- Adhere to RESTful principles where applicable.

## 3. Database

### Primary Database

PostgreSQL

### Real-time Database

Redis

### Schema Design

Outline the initial database schema for user data, group data, locations, messages, and expenses. Use PostGIS extension for PostgreSQL for efficient geospatial queries.

### Development Guidelines

- Ensure database normalization for consistency.
- Implement proper indexing, especially for location-based queries.

## 4. Messaging and Event Streaming

### Technology

Apache Kafka

### Usage

- Real-time location updates.
- Message queue for chat and notification services.

### Development Guidelines

- Utilize Kafka topics efficiently to handle different data streams.
- Ensure fault tolerance and message durability.

## 5. Infrastructure

### Containerization

Docker

### Orchestration

Kubernetes (GCP)

### CI/CD

GitHub Actions with JFrog Artifactory

### Monitoring

Prometheus, Grafana, and Sentry

### Storage

MinIO for media

### Development Guidelines

- Define Dockerfile(s) for containerization of different services.
- Set up Kubernetes deployment and service configurations.
- Implement CI/CD pipelines for automated testing and deployment.
- Configure Prometheus and Grafana for monitoring and alerting.
- Integrate Sentry for real-time error tracking.

# Technical Design Document
Readers are encouraged to read and suggest updates to enrich it.
Check it out [here](#)

# Coding Standards and Practices

## Version Control

Git (GitHub)

## Code Reviews

Mandatory for all merges into the main branch.

## Documentation

Inline code comments and READMEs for each microservice.

## Testing

Unit tests and integration tests are required.

## Security

Follow [OWASP security standards](https://owasp.org/www-project-mobile-app-security/).

# Contribution Guidelines

## Getting Started

Instructions on setting up the development environment.
Follow [Github Flow](https://docs.github.com/en/get-started/quickstart/github-flow) for branching.

## Issue Tracking

Guidelines on reporting and assigning issues.

## Pull Requests

Process for submitting and reviewing pull requests.

## Code of Conduct

Outline expected behavior and contribution ethics.

# Project Roadmap

## Phase 1

Setup and basic functionality (User authentication, group creation, basic location sharing).

## Phase 2

Advanced features (Real-time location tracking, messaging).

## Phase 3

Additional features (Media sharing, expense splitting).

## Phase 4

Testing, deployment, and iterative improvements.

# Contact and Support

## Maintainers

List of project maintainers with contact information.

## Community

>[Slack](https://join.slack.com/t/slack-les9847/shared_invite/zt-2a0dqjzvk-YLC9TQFBExNnPFsH9yAB6g)
---
Generated using GPT-4
