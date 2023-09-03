helm install helm-cloudrucamp-app ./helm

minikube kubectl -- port-forward service/cloudru-service 8000:8000 --namespace helm-cloudru-ns