## Kubernetes manifests

This directory provides dedicated plain Kubernetes manifests for this project:

- `deployment.yaml`
- `service.yaml`
- `ingress.yaml`

### PV/PVC requirement

`it-tools` is a stateless frontend application served by nginx and does not require persistent storage for runtime operation.
For that reason, `PersistentVolume` and `PersistentVolumeClaim` manifests are intentionally not included.
