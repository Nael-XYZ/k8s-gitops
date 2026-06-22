# K8s GitOps 🔄

Complete GitOps workflow with ArgoCD, Helm, and Kustomize.

## Structure

```
├── apps/           # ArgoCD Application definitions
├── charts/         # Helm charts
├── overlays/       # Kustomize overlays (dev/staging/prod)
├── policies/       # OPA/Gatekeeper policies
└── secrets/        # Sealed secrets
```

## Deployment

```bash
# Apply ArgoCD apps
kubectl apply -f apps/

# Sync manually
argocd app sync production
```

## License

Apache 2.0