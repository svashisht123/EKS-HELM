# api-eks-helm

This repository is for our EKS deployments via Helm.

Helm is a tool for managing Charts. Charts are packages of pre-configured Kubernetes resources.

The docker images tags are updated in values.yaml and the corresponding image is pulled from the ECR repository and deployed on EKS via helm.

Currently DEV namespace is being used, and the following pods are running(for example):

$ kubectl get pods -n dev
NAME                                               READY   STATUS    RESTARTS   AGE
demo-api-cluster-app-deployment-5b7b4c998c-7dxxc   1/1     Running   0          6m58s
