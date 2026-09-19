# Recommended Technology Stack

| Layer | Technology | Rationale |
|---|---|---|
| Mobile frontend | React Native (Expo) | Fast cross-platform delivery, best code reuse with web |
| Web frontend | React / Next.js | Shares TypeScript code and design tokens with mobile |
| Core backend | NestJS (TypeScript) | Structured, real-time WebSocket gateways, shared language |
| AI microservice | Python FastAPI | Best AI/ML ecosystem, scales independently |
| Primary database | PostgreSQL | Relational data, ACID, analytics, health-data controls |
| Cache / real-time | Redis | Low-latency cache, pub/sub for social feed |
| File storage | AWS S3 | Encrypted, low-cost storage for meal photos |
| Authentication | AWS Cognito (JWT) | Compliance, cost, MFA |
| On-device AI | TensorFlow Lite + ML Kit | Personalisation and food recognition with less data leaving the phone |
| Notifications | FCM / APNs | Push delivery for iOS and Android |

See `comparison-matrix.md` for the scoring and `adr-001-tech-stack.md` for the decision record.
