docker build -t yefriddavid/kube-api-go:v1 .
docker run --name burrito yefriddavid/kube-api-go:v1
curl -X GET http://172.17.0.2:8080/


kubectl create -f deploymenet.yml

kubectl get pods -w
minikube service api-service --url

