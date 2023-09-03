minikube start --driver=docker --insecure-registry="192.168.1.6:5000"

minikube kubectl -- apply -f cloudru-app.yml

minikube kubectl -- port-forward service/cloudru-service 8000:8000 --namespace cloudru-namespace