
```
brew update
brew upgrade
brew install minikube
brew upgrade minikube

minikube stop
minikube delete
minikube start --driver docker --memory 8192 --cpus 2 --nodes 1 --disk-size 30GB
minikube addons enable ingress
minikube addons enable metrics-server


kubectl config current-context
kubectl get nodes
kubectl apply -f manifest.yaml
```

