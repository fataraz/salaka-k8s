### `enable ingress controller in minikube`
minikube addons enable ingress

### `create expose service in minikube`
minikube service <name> --url
minikube service salaka --url -n development


### `create namespace`
kubectl create ns development

### `start yaml`
kubectl create -f salaka.yaml -n development

### `apply yaml`
kubectl apply -f salaka.yaml -n development

### `restart deployment`
kubectl rollout restart deployment salaka -n development

### `describe`
kubectl describe deployment salaka -n development

### `pod`
kubectl get pod -n development

### `Expose`
kubectl expose deployment salaka --port=5001 --target-port=5000

### `logs`
kubectl logs <pod> -n development

### `nodes`
kubectl get nodes

### `create secret manual`
echo -n `string` | base64

kubectl port-forward -n development


### `edit /etc/hosts`
sudo vim /etc/hosts
ip-address url

### `checking error`
kubectl describe pod <name-pod> -n development
