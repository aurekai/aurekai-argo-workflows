# Quickstart — aurekai-argo-workflows

Run Aurekai pipeline templates as Argo Workflows.

## Requirements

- Kubernetes cluster with Argo Workflows installed
- `argo` CLI
- `akai` image: `ghcr.io/aurekai/aurekai:0.8.0-alpha.4`

## Submit Workflow

```bash
argo submit workflows/doctor-deep-workflow.yaml
argo submit workflows/aurekai-full-pipeline.yaml
```

## Validate

```bash
bash tests/validate-schemas.sh
bash tests/validate-scripts.sh
```
