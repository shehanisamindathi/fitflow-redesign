# FitFlow Redesign

Technology selection and architecture for the redesign of FitFlow, an AI-powered
fitness tracking app (IT3060 Human Computer Interaction, Lab Sheet 05).

## Goals

* AI-personalised workout plans
* Private social circles and challenges
* Camera-based nutrition logging
* Fast, offline-capable, accessible and secure (GDPR/CCPA-aware)

## Tech stack

|Layer|Technology|
|-|-|
|Mobile|React Native (Expo)|
|Web|React / Next.js|
|Core API|NestJS (TypeScript)|
|AI service|Python FastAPI|
|Database|PostgreSQL + Redis + S3|
|Authentication|AWS Cognito (JWT)|
|On-device AI|TensorFlow Lite, ML Kit|

## Repository structure

* `frontend/`    mobile and web apps
* `backend/`     core API
* `ai-service/`  AI microservice
* `docs/`        tech stack, comparison matrix, architecture diagram, ADR

## Documentation

* [Tech stack summary](docs/tech-stack.md)
* [Comparison matrix](docs/comparison-matrix.md)
* [Architecture diagram](docs/architecture.png)
* [ADR-001](docs/adr-001-tech-stack.md)s

## Author

Samindathi MMS (IT 22337030), Group Number

