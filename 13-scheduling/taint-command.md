# Add Taint

```bash
kubectl taint nodes worker-1 dedicated=database:NoSchedule
```

# Remove Taint

```bash
kubectl taint nodes worker-1 dedicated=database:NoSchedule-
```
