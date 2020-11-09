# Despliegue a Google Kubernete Engine


## accesso a gcloud 
_Abrir el terminal y ejecute el siguiente commando_
```
gcloud container clusters get-credentials cluster-1 --zone us-central1-c --project sing-in-dev-284714
```

## comandos de ejecucion de microservicio backend
_Aplicar esos comando para el despliegue de app backend_

```
kubectl apply -f farmaciaturno-configmap.yaml
kubectl apply -f farmaciaturno-deployment.yaml
kubectl apply -f farmaciaturno-service.yaml
```

## comandos de ejecucion de aplicacion
_Aplicar esos comando para el despliegue de app frontend_

```
kubectl apply -f farmaciaturno-frontend-deployment.yaml
kubectl apply -f farmaciaturno-frontend-service.yaml
```
