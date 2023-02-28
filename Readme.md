# Learn Kubernetes

Minikube is already install.

**Run minikube on Docker :**
```
minikube start --vm-driver=docker
```
---

**Basics commands for  ```kubectl``` :**
```
GET :

kubectl get node

kubectl get pod

kubectl get services

kubectl get deployment

kubectl get replicaset
(managing the replicas of a Pod)

CREATE :

kubectl create deployment [name] --image=[docker image]
(Create a resource from a file or from stdin, most basic configuration)

EDIT :

kubectl edit deployment [name]
(auto-generated configuration file with default value)

DELETE : 

kubectl delete deployment [deployment name]
```
---

**Debugging pod :**
```
kubectl logs [pod name]
(log to console)

kubectl exec -it [pod name] -- bin/bash
(get interactive terminal)

kubectl describe pod [pod name]
(get info about pod)
```
---

**Config file :**
```
CREATE :

kubectl apply -f [file name]

DELETE :

kubectl delete -f [file name]
```
---