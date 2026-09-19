# ADR-001: FitFlow Redesign Technology Stack

**Status:** Accepted (for this lab design)
**Date:** 19/09/2026

## Context
FitFlow needs a fast, cross-platform (iOS, Android, web) fitness app with AI-personalised workouts, real-time social features, camera-based nutrition logging, offline support and strong protection of health data. The team is mid-sized and needs quick delivery at controlled cost.

## Decision
React Native (Expo) and React/Next.js on the front end; NestJS for the core API and Python FastAPI as a separate AI microservice; PostgreSQL as primary database with Redis for caching/real-time and S3 for images; AWS Cognito for authentication; TensorFlow Lite and ML Kit for on-device AI.

## Alternatives considered
- Frontend: Flutter, Kotlin Multiplatform, Swift/SwiftUI
- Backend: Express, Go
- Database: MongoDB, Firebase Firestore, DynamoDB
- Auth: Firebase Auth, Auth0, Supabase Auth
- The case-study stack (React Native + Node/Express + Firebase)

## Rationale
Highest weighted score in the decision matrix; best balance of speed, cost, security/privacy for health data, AI integration and scalability; one TypeScript language across front end and core backend.

## Consequences
- Positive: faster delivery with shared code, strong data integrity and analytics, independent scaling of AI, clear compliance path.
- Negative / risks: more infrastructure than a Firebase-only stack, team needs TypeScript and Python skills, native ML modules need testing on both platforms, Redis must be operated.

## Review trigger
Re-evaluate if hosting must move to Google Cloud, user volume grows tenfold, or compliance requirements change.
