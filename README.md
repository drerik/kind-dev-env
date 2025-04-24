# kind-dev-env

Local Kind development environments

## Cluster definitions

### kind-1cp-3w-basic

Deploys a basic cluster with the following features:

- 1 Control Plane node
- 3 Worker nodes

```bash
kind create cluster --config kind-1cp-3w-basic/kind-config.yaml
```

### kind-1cp-3w-ingress

Deploys a basic cluster with the following features:

- 1 Control Plane node
- 3 Worker nodes
- Ingress ports exposed to localhost port 8080 and 8443 

```bash
kind create cluster --config kind-1cp-3w-ingress/kind-config.yaml
kubectl apply -k manifests/ingress/
```

