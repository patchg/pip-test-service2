---
service: my-service
system: pip
owners: [team-name]
last-reviewed: 2026-03-16
tags: [api, microservice]
---

# Architecture: my-service

## Overview

Brief description of what this service does and its role in the system.

## Components

- **Component 1**: Description
- **Component 2**: Description

## Data Flow

```
[Client] --> [API Gateway] --> [my-service] --> [Database]
```

## Design Decisions

### Decision 1: [Title]
- **Context**: Why this decision was needed
- **Decision**: What was chosen
- **Consequences**: Trade-offs

## Security

- Authentication: [Method]
- Authorization: [RBAC / scopes]
- Data encryption: TLS in transit, AES-256 at rest

## Monitoring

- Metrics: [Key metrics]
- Alerts: [Critical alerts]
