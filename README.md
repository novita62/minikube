# Learn Kubernetes Using PHP

- Run minikube on local
```
minikube start
```

- Use the kubectl create command to create a Deployment that manages a Pod
```
kubectl create deployment hello-php --image=gcr.io/hello-minikube-zero-install/hello-php

```

- View the Deployment
```
kubectl get deployments
```

- View the Pod
```
kubectl get pods

```

- View cluster events
```
kubectl get events
```

- View the kubectl configuration
```
kubectl config view
```

- Expose the Pod to the public internet using the kubectl expose command
```
kubectl expose deployment hello-php --type=LoadBalancer --port=80
```

- View the Service you just created
```
kubectl get services
```

- Run service
```
minikube service hello-php
```
