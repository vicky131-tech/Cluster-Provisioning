# Kubernetes Cluster Provisioning Project

## Project Overview

This project demonstrates Kubernetes cluster provisioning and application deployment using Kubernetes manifests. The project deploys an NGINX application with multiple replicas and exposes it using a Kubernetes Service.

The objective of this project is to demonstrate foundational Kubernetes concepts including:

- Deployments
- Replica management
- Pods
- Services
- Load Balancing
- Declarative Infrastructure
- Containerized Application Deployment

---

## Architecture

The project provisions:

- A Kubernetes Deployment
- 7 NGINX Pod replicas
- A LoadBalancer Service for external access

---

## Project Structure

```bash
.
├── deployment.yaml
├── service.yaml
└── README.md
```

---

## Technologies Used

- Kubernetes
- Docker
- NGINX
- YAML
- Git
- GitHub

---

## Deployment Configuration

### Deployment

The `deployment.yaml` file defines:

- NGINX container image
- Replica count
- Pod labels and selectors
- Container port configuration

### Service

The `service.yaml` file exposes the application using:

- Kubernetes Service
- LoadBalancer type
- Port mapping configuration

---

## Replica Configuration

The deployment is configured with:

```yaml
replicas: 7
```

This ensures Kubernetes maintains 7 running NGINX Pods for high availability and scalability.

---

## How to Deploy

### Clone Repository

```bash
git clone https://github.com/vicky131-tech/cluster-provisioning.git
```

### Navigate Into Project Directory

```bash
cd cluster-provisioning
```

### Apply Kubernetes Manifests

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

---

## Verify Deployment

### Check Deployments

```bash
kubectl get deployments
```

### Check Pods

```bash
kubectl get pods
```

### Check Services

```bash
kubectl get services
```

---

## Expected Output

- 7 running NGINX Pods
- Active Kubernetes Deployment
- LoadBalancer Service exposing the application

---

## Learning Objectives

This project demonstrates understanding of:

- Kubernetes Deployments
- ReplicaSets
- Pod orchestration
- Kubernetes Services
- YAML configuration files
- Infrastructure as Code (IaC)
- Git version control
- GitHub repository management

---

## Future Improvements

Potential enhancements for this project include:

- Ingress Controller integration
- Horizontal Pod Autoscaling
- CI/CD pipeline with GitHub Actions
- Helm chart packaging
- Monitoring with Prometheus and Grafana
- Persistent storage configuration

---

## Author

Victoria Oyewole

Cloud & DevOps Engineer

GitHub: https://github.com/vicky131-tech