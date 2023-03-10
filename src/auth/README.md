# Authorization Service
This is a Authorization Service.

* Creating Virtual Environment
> python3 -m venv venv
> 
> source ./venv/bin/activate

* Installing prerequisites
> pip3 install flask flask_mysqldb pyjwt

* Creating requirements.txt
> pip3 freeze > requirements.txt

* Building a docker container
> docker build .

* Tagging the docker container
> docker tag "SHA256 text for the built image" "Your Docker Hub Account/auth:latest"

* Pushing the docker container
> docker push "Your Docker Hub Account/auth:latest"

* Applying pods to Kubernetes
> kubectl apply -f ./

* Deleting pods from Kubernetes
> kubectl delete -f ./

* Scaling the number of pods
> kubectl scale deployment --replicas=1 auth