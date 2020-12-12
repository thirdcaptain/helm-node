# Docker + Node.js

A Dockerized Node.js app in a helm chart deployment.

Node.js docker app:
Based on (https://fireship.io/lessons/docker-basics-tutorial-nodejs/) on Fireship.io. 

Helm chart template:
https://github.com/nodeshift/helm

Usage:
Install using:
`helm install nodeserver .`
But can't access app through:
http://${SAMPLE_NODE_IP}:${SAMPLE_NODE_PORT}

To access application, tunnel through minikube:
`kubectl get services`
`minikube service nodeserver-service`