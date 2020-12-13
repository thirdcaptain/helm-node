# Docker + Node.js

A Dockerized Node.js app in a helm chart deployment.

Node.js docker app:

Based on Node.js Language Specifc GKE quickstart:

(https://cloud.google.com/kubernetes-engine/docs/quickstarts/deploying-a-language-specific-app#node.js)
(https://cloud.google.com/kubernetes-engine/docs/tutorials/hello-app#cloud-shell)


Helm chart template:
https://github.com/nodeshift/helm

Define parameters in values.yaml and Chart.yaml file

Usage:
cd into `nodeserver` directory
Install using:
`helm install nodeserver .`

For local testing:
To access application, tunnel through minikube:
`kubectl get services`
`minikube service nodeserver-service`