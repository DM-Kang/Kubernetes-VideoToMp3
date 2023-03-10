# Converter Service
This is a Converter Service.

* Creating Virtual Environment
> python3 -m venv venv
> 
> source ./venv/bin/activate

* Installing prerequisites
> pip3 install pika pyMongo
> pip install moviepy

* Creating requirements.txt
> pip3 freeze > requirements.txt

* Building docker container
> docker build .

* Tagging docker container
> docker tag <Sha256 text for the built image> <Your Docker Hub Account/converter:latest>

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 converter