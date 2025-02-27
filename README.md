# Challenge
- 

# Setup challenge in all namespace
```
k get namespace -oname | cut -d'/' -f2 | xargs -I{} kubectl apply -f  . -n {}
```

# Useful commands
```
kubectl exec -it netshoot -- bash

kubectl get pods -n {namespace} {name} -oyaml
kubectl edit pods -n {namespace} {name}

kubectl get deployments -n {namespace} {name} -oyaml
kubectl edit deployments -n {namespace} {name}

kubectl get service -n {namespace} {name} -oyaml
kubectl edit service -n {namespace} {name}
```
# k8s-lab-1
