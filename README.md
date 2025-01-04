# Docker and Kubernetes Deployment Guide

This project demonstrates how to set up **Node-RED** and **RabbitMQ** using Docker, and **MinIO** using Kubernetes.


to run kubernates need port-forward 

kubectl port-forward svc/minio 9000:9000
kubectl port-forward svc/minio 9001:9001

the convert from dockerfile to kubernates was  done with kompose file 


