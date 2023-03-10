# Gateway Service
This is Gateway Service.

* Creating Virtual Environment
> python3 -m venv venv
> 
> source ./venv/bin/activate

* Installing prerequisites
> pip3 install pika flask flask_pymongo pymongo

* Creating requirements.txt
> pip3 freeze > requirements.txt

* Building docker container
> docker build .

* Tagging docker container
> docker tag <Sha256 text for the built image> <Your Docker Hub Account/gateway:latest>

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 gateway