# MYSQL node on Kubernetes using Kubernetes Artifacts

kubectl create namespace mysql

kubectl config set-context --current --namespace=mysql

kubectl create -f mysql-secret.yaml

kubectl create -f mysql-deployment.yaml

kubectl create -f mysql-configmap.yaml

kubectl create -f mysql-service.yaml

kubectl get pods --watch
