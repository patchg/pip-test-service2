---
service: my-service
system: pip
criticality: medium
---

# Runbook: my-service

## Service Overview

- **Purpose**: What this service does
- **Criticality**: High / Medium / Low
- **On-Call Team**: team-name
- **Slack Channel**: #team-alerts

## Health Check

```bash
curl https://my-service.example.com/health
# Expected: 200 OK {"status":"healthy"}
```

## Common Issues

### Service Unavailable
```bash
kubectl get pods -n production | grep my-service
kubectl logs -n production deployment/my-service --tail=100
```

**Resolution:** `kubectl rollout restart deployment/my-service -n production`

## Deployment

```bash
./deploy.sh staging   # Deploy to staging
./deploy.sh production  # Deploy to production
```

### Rollback
```bash
kubectl rollout undo deployment/my-service -n production
```
