# Configuration Management

This folder contains Kubernetes examples for Labels, Selectors, ConfigMaps, Secrets, and Environment Variables.

# Commands
```bash
kubectl get pods --show-labels
kubectl get pods -l app=nginx
kubectl describe pod nginx-labeled
kubectl get configmap
kubectl get secret
kubectl describe configmap application-config
kubectl describe secret application-secret
