# Kubernetes Manifests

This repository contains Kubernetes YAML manifests for learning, practice, and DevOps portfolio building.

## Topics Covered
- Pods
- Deployments
- Services
- ConfigMaps
- Secrets
- Ingress

## Tools
- Kubernetes
- kubectl
- YAML
- Docker

## Purpose
To demonstrate practical Kubernetes deployment and configuration concepts used in DevOps and platform engineering.


## Useful Commands

```bash
kubectl apply -f 01-pods/nginx-pod.yaml
kubectl get pods
kubectl describe pod nginx-pod
kubectl logs nginx-pod

kubectl apply -f 02-deployments/nginx-deployment.yaml
kubectl get deployments
kubectl get pods

kubectl apply -f 03-services/nginx-service.yaml
kubectl get svc
```

## Current Examples

### Pod
Basic Nginx pod manifest.

### Deployment
Nginx deployment with 3 replicas.

### Service
ClusterIP service to expose Nginx internally inside the Kubernetes cluster.

## How to Apply

```bash
kubectl apply -f 01-pods/nginx-pod.yaml
kubectl apply -f 02-deployments/nginx-deployment.yaml
kubectl apply -f 03-services/nginx-service.yaml
```

## ConfigMap and Secret Example

```bash
kubectl apply -f 04-configmaps/app-configmap.yaml
kubectl apply -f 05-secrets/app-secret.yaml
kubectl apply -f 02-deployments/nginx-deployment-with-env.yaml

kubectl get configmap
kubectl get secret
kubectl get pods

kubectl exec -it <pod-name> -- env
```
