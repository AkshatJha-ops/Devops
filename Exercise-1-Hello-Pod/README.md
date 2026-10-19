# Exercise 1: Kubernetes Hello Pod

## Business Problem
Simulate the Zepto storefront using the Nginx container image.

## Objective
Deploy Nginx on Kubernetes and expose it using a NodePort Service.

## Tools Used
- Docker Desktop
- Minikube
- kubectl
- Kubernetes
- Nginx

## Implementation
1. Started the Minikube cluster.
2. Created the hello-k8s Pod.
3. Verified the Pod was Running.
4. Exposed the Pod using a NodePort Service.
5. Opened the Nginx welcome page in the browser.
6. Verified the Service endpoint.

## Resources
- Pod: hello-k8s
- Image: nginx:latest
- Container port: 80
- Service type: NodePort

## Result
The Nginx welcome page was successfully accessed through the local Kubernetes cluster.

## Evidence
See the screenshots folder.
