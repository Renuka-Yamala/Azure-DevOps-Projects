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

```
 1  az --version
    2  clear
    3  az aks list
    4  az login
    5  az aks list
    6  az aks create --resource-group renu-rg --name renu-aks --node-count 1 --enable-addons monitoring --generate-ssh-keys
    7  az group create --name renu-rg --location eastus
    8  az aks create --resource-group renu-rg --name renu-aks --node-count 1 --enable-addons monitoring --generate-ssh-keys
    9  az provider register --namespace Microsoft.Insights
   10  az provider register --namespace Microsoft.OperationalInsights
   11  az provider show --namespace Microsoft.Insights --query "registrationState"
   12  az provider show --namespace Microsoft.OperationalInsights --query "registrationState"
   13  az provider show --namespace Microsoft.Insights --query "registrationState"
   14  az aks create --resource-group renu-rg --name renu-aks --node-count 1 --enable-addons monitoring --generate-ssh-keys
   15  az provider register --namespace Microsoft.ContainerService
   16  az provider show --namespace Microsoft.ContainerService --query "registrationState"
   17  clear
   18  az provider show --namespace Microsoft.ContainerService --query "registrationState"
   19  clear
   20  az aks create --resource-group renu-rg --name renu-aks --node-count 1 --enable-addons monitoring --generate-ssh-keys
   21  az aks get-credentials --resource-group renu-rg --name renu-aks
   22  kubectl get nodes
   23  az aks delete --name renu-aks --resource-group renu-rg --yes
   24  az group delete --name renu-rg --yes --no-wait
   25  history
```


