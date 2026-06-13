## Kubernetes manifests

This directory provides dedicated plain Kubernetes manifests for this project:

- `deployment.yaml`
- `service.yaml`
- `ingress.yaml`

Before applying:

- Set the Deployment image tag to the exact version you want to run.
- Replace the Ingress host (`it-tools.local`) with your real domain.

### PV/PVC requirement

`it-tools` is a stateless frontend application served by nginx and does not require persistent storage for runtime operation.
For that reason, `PersistentVolume` and `PersistentVolumeClaim` manifests are intentionally not included.
