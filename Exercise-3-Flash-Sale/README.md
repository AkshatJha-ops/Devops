# Exercise 3: Scaling Flask App Using ReplicaSets

## Objective
Deploy a Flask-based flash sale application on Kubernetes, scale it from 3 to 5 replicas, and verify self-healing.

## Real-Life Use Case
During an e-commerce flash sale, traffic can increase suddenly. Kubernetes ReplicaSets maintain the desired number of application Pods.

## Technologies
- Python 3.11
- Flask
- Gunicorn
- Docker
- Kubernetes
- Minikube
- kubectl

## Application Endpoints
- `/` - Displays the Big Sale welcome message and serving Pod.
- `/buy?user=123` - Simulates a purchase and returns the product, user, and serving Pod.
- `/health` - Health-check endpoint.

## Implementation Steps
1. Created the Flask application in `app.py`.
2. Created a Dockerfile to package the application.
3. Built the image `flashsale:1.0`.
4. Loaded the image into Minikube.
5. Created a ReplicaSet with 3 replicas.
6. Exposed the application using a Kubernetes Service.
7. Scaled the ReplicaSet to 5 replicas.
8. Deleted a Pod and verified that Kubernetes created a replacement.
9. Verified Pod status and node distribution.

## Key Observations
- Initially, 3 application Pods were configured.
- Scaling increased the desired number of replicas to 5.
- All 5 Pods ran on the single Minikube node.
- When one Pod was deleted, the ReplicaSet created a replacement.
- The Service provides a stable endpoint for accessing the application.

## Result
Successfully deployed and scaled the Flash Sale Flask application using a Kubernetes ReplicaSet. Verified replica scaling and automatic Pod replacement.

## Evidence
Screenshots of the running Pods, scaling operation, self-healing test, and application endpoints are available in the `screenshots` directory.
