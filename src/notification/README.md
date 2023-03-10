# Notification Service
This is Notification Service.

* Creating Virtual Environment
> python3 -m venv venv
> 
> source ./venv/bin/activate

* Installing prerequisites
> pip3 install pika

* Creating requirements.txt
> pip3 freeze > requirements.txt

* Building docker container
> docker build .

* Tagging the docker container
> docker tag "SHA256 text for the built image" "Your Docker Hub Account/notification:latest"

* Pushing the docker container
> docker push "Your Docker Hub Account/notification:latest"

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 notification