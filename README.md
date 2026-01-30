# Example Voting App - Kubernetes Learning & Training

## Overview

This repository is a learning and training resource for Kubernetes orchestration. It uses the Docker example voting app as the test microservice application to demonstrate Kubernetes deployments, services, and cluster management.

## About the Example Voting App

The example voting app is a distributed application that demonstrates microservices architecture with the following components:

- **Vote Service**: Frontend application where users can vote
- **Result Service**: Frontend application to display voting results
- **Worker**: Backend service that processes votes
- **Database**: Stores voting data
- **Redis**: In-memory cache for vote queue

## Repository Structure

This repository contains Kubernetes specifications organized by resource type:

- `k8s-specifications/deployments/` - Kubernetes deployment manifests for all services
- `k8s-specifications/services/` - Kubernetes service manifests for networking

## Getting Started

To deploy the voting app on a Kubernetes cluster, apply the manifests in the `k8s-specifications` directory:

```bash
kubectl apply -f k8s-specifications/
```

## Learning Goals

This project demonstrates key Kubernetes concepts including:

- Deploying multi-tier microservices
- Service discovery and networking
- Data persistence with databases
- Caching strategies with Redis
- Container orchestration best practices

## Requirements

- A running Kubernetes cluster
- `kubectl` CLI configured with cluster access
- Docker images for the voting app components

---

Happy learning with Kubernetes!
