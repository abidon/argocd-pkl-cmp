# Pkl ArgoCD Config Management Plugin

> [!WARNING]  
> This project is still in its early development phase and should not be used in production.

## Install

```bash
kubectl apply -f pkl-argocd-cmp/manifests/1-pkl-argo-cmp-configmap.yaml
kubectl -n argocd patch deployments/argocd-repo-server --patch-file pkl-argocd-cmp/manifests/2-argocd-repo-server.patch.yaml
```
