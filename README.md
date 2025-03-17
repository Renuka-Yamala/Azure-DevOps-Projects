# Azure-DevOps-Projects

# Pre-requisites:
1)AWS-CLI installed

2)kubectl installed

3)eksctl installed

4)Docker image pushed to docker Hub

* First thorugh Azure pipeline push an image to dockerhub using yaml file


* Create a EKS cluster in AWS using below command
```
eksctl create cluster --name my-cluster --region us-east-1 --nodes 1
kubectl get nodes

```

* Create a Kubernetes Deployment Manifest

```
kubectl apply -f deployment.yml
kubectl get deployments
kubectl get pods
kubectl get services
```
* Access the application using the external ip address:application port through browser

* Create a Kubernetes Service Connection:

Go to Project Settings > Service Connections in Azure DevOps.


