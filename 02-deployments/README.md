# Deployments
This folder contains Kubernetes deployment manifest examples.

# Commands

``` bash
kubectl apply -f nginx-scale-deployment.yaml
kubectl get deploy
kubectl get pods
kubectl scale deployment nginx-scale --replicas=10

```

# Rolling Update

``` bash
kubectl set image deployment/nginx-scale nginx=nginx:1.25
kubectl rollout status deployment nginx-scale
```

# Rollback

``` bash
kubectl rollout undo deployment nginx-scale
