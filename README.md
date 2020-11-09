# Despliegue a Google Kubernete Engine


## accesso a gcloud 

gcloud container clusters get-credentials cluster-1 --zone us-central1-c --project sing-in-dev-284714


## comandos de ejecucion de microservicio backend

kubectl apply -f farmaciaturno-configmap.yaml
kubectl apply -f farmaciaturno-deployment.yaml
kubectl apply -f farmaciaturno-service.yaml


## comandos de ejecucion de aplicacion

kubectl apply -f farmaciaturno-frontend-deployment.yaml
kubectl apply -f farmaciaturno-frontend-service.yaml

