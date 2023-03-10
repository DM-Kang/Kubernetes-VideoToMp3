# Converter Service
This is a Converter Service.

* Add the record below to /etc/hosts
> 127.0.0.1   kubernetes.docker.internal
>
> 127.0.0.1   mp3converter.com

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
> docker tag "SHA256 text for the built image" "Your Docker Hub Account/converter:latest"

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 converter
