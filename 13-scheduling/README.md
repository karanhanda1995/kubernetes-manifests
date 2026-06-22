# Kubernetes Scheduling

This folder contains examples of Kubernetes scheduling features such as Node Selectors, Node Affinity, Pod Affinity, Pod Anti-Affinity, Taints, and Tolerations.

# Commands

``` bash
kubectl get nodes --show-labels

kubectl label node worker-1 disktype=ssd

kubectl describe node worker-1

kubectl taint nodes worker-1 dedicated=database:NoSchedule

kubectl get pods -o wide
