# RabbitMQ Service
This is RabbitMQ Service.

* Running minikube tunnel (Open a new terminal tap)
> minikube tunnel

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 rabbitmq
