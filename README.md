
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

minikube -n flask-redis-k8s service flask
curl -v --resolve myflask.local:80:127.0.0.1 http://myflask.local/



kubectl -n flask-redis-k8s get ingress
minikube tunnel
curl -v --resolve myflask.example.com:80:127.0.0.1 http://myflask.example.com

```

