install minikube
minikube start
add docker image from previous tasks to docker hub with name "nodeapp"
minikube addons enable ingress
kubectl apply -f deploy.yaml
kubectl scale deploy nodejs-app --replicas 2
kubectl apply -f service.yaml
kubectl get ingress
"ADDRESS -> 192.168.49.2"
nano /etc/hosts add "192.168.49.2 uklon.com.ua"
kubectl apply -f ingress-rules.yaml
