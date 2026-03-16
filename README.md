# Service Name

> Created from [pip-service-template](https://github.com/patchg/pip-service-template).
> The `/docs` folder automatically syncs to [docs-central](https://github.com/patchg/docs-central) on every push to `main`.

## Getting Started

1. Rename placeholders — search for `my-service` and replace with your service name
2. Fill out `/docs/architecture.md`, `/docs/dependencies.yaml`, and `/docs/runbook.md`
3. Push to `main` — docs sync automatically to docs-central

## Doc Mirror Setup

Already included in this template:

| File | Purpose |
|------|---------|
| `.doc-mirror.yml` | Configures what syncs and where |
| `.github/workflows/sync-docs.yml` | Triggers sync on push to `docs/**` |

The `DOC_MIRROR_TOKEN` secret must be added to this repo once after creation.
Run the [Onboard Service Repo](https://github.com/patchg/.github/actions/workflows/onboard-service.yml) workflow if you created this repo manually rather than from the template.
