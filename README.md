# Docker and Kubernetes Deployment Guide

This project demonstrates how to set up **Node-RED** and **RabbitMQ** using Docker, and **MinIO** using Kubernetes.

## Docker Setup

To run the Docker setup, follow the instructions provided in the respective Dockerfiles for **Node-RED** and **RabbitMQ**.

## Kubernetes Setup

To run the Kubernetes setup for **MinIO**, follow these steps:

1. Scale the MinIO deployment:
    ```sh
    kubectl scale deployment minio --replicas=1
    ```
2. Port-forward the MinIO services:
    ```sh
    kubectl port-forward svc/minio 9000:9000
    kubectl port-forward svc/minio 9001:9001
    ```

Note: The conversion from Dockerfile to Kubernetes was done with a Kompose file.
