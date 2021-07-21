1. install minikube
2. minikube start
3. add docker image from previous tasks to docker hub with name "nodeapp"
4. minikube addons enable ingress
5. kubectl apply -f deploy.yaml
6. kubectl scale deploy nodejs-app --replicas 2
7. kubectl apply -f service.yaml
8. kubectl get ingress ("ADDRESS -> 192.168.49.2")
9. nano /etc/hosts add "192.168.49.2 uklon.com.ua"
10. kubectl apply -f ingress-rules.yaml
