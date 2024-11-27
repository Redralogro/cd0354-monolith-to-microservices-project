# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![Dockerhub](./dockerhub.png)
* GitHub repository’s settings showing CircleCI webhook (I prefer to use CircleCI)
![Github webhook](./webhook.png)
* CircleCI showing a successful build and deploy job
![CircleCI](./cicd.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![get pods](./getpods.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![describe service](./describe-service-1.png)
![describe service](./describe-service-2.png)
![describe service](./describe-service-3.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![describe hpa](./describe-hpa.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![describe hpa](./getlogs.png)

## Addition (optional)
* Create posts

![Create Posts](./create-posts.png)