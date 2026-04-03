# GitOps-Based Kubernetes Application Deployment using ArgoCD (EKS) 

## Project Overview

This project demonstrates a GitOps workflow using ArgoCD on AWS EKS where all deployments are managed through Git.

* No manual kubectl apply
* Fully automated deployment using ArgoCD

---

## Architecture

Developer → GitHub → ArgoCD → EKS Cluster → Kubernetes

---

## Tech Stack

* Docker
* Kubernetes (EKS)
* ArgoCD
* GitHub
* AWS EC2

---

## Infrastructure Setup

### EC2 Instance

EC2

<img width="837" height="357" alt="image" src="https://github.com/user-attachments/assets/df5eca7c-380b-4938-a493-c00b813e4a86" />


### EKS Cluster

EKS

<img width="848" height="355" alt="image" src="https://github.com/user-attachments/assets/fb2ec892-7c0c-4986-861a-5ddff88ac9c7" />


### Docker Image

DockerHub Repository

<img width="844" height="350" alt="image" src="https://github.com/user-attachments/assets/4a4a8bf3-4001-41e4-af0e-7de3a4f26976" />

DockerHub

### GitHub Repository

GitHub

---

## ArgoCD Setup

### ArgoCD Dashboard

ArgoCD

### Auto Sync Enabled

Auto Sync

### Sync Details

Sync Details

---

## Kubernetes Resources

### Pods Running

Pods

### Service (LoadBalancer)

Service

---

## Application Output

### Initial Version (v1)

Output

---

## GitOps Working Proof

### Code Change (GitHub Commit)

GitHub Change

### Updated Output (v2)

Output Change

---

## GitOps Workflow

* Developer updates code
* Pushes changes to GitHub
* ArgoCD detects changes automatically
* Syncs application with Kubernetes
* Updated version deployed without manual intervention

---

## Commands Used

```bash
# Build Docker Image
docker build -t riyajkalawant/gitops-app:v1 .

# Push Image
docker push riyajkalawant/gitops-app:v1

# Check Pods
kubectl get pods

# Check Services
kubectl get svc
```

---

## Key Features

GitOps-based deployment
Automated sync using ArgoCD
Self-healing enabled
Scalable Kubernetes deployment
No manual cluster changes

---

## Learnings

Importance of Git as source of truth
ArgoCD automation and sync
Kubernetes YAML structure
Debugging deployment issues

---

## Conclusion

Successfully implemented a production-style GitOps pipeline using ArgoCD and AWS EKS with automated deployments.

---

## Author

Riyaj Kalawant
# GitOps-Based Kubernetes Application Deployment using ArgoCD (EKS)

## Project Overview

This project demonstrates a GitOps workflow using ArgoCD on AWS EKS where all deployments are managed through Git.

* No manual kubectl apply
* Fully automated deployment using ArgoCD

---

## Architecture

Developer → GitHub → ArgoCD → EKS Cluster → Kubernetes

---

## Tech Stack

* Docker
* Kubernetes (EKS)
* ArgoCD
* GitHub
* AWS EC2

---

## Infrastructure Setup

### EC2 Instance

EC2

### EKS Cluster

EKS

### Docker Image

DockerHub Repository
DockerHub

### GitHub Repository

GitHub

---

## ArgoCD Setup

### ArgoCD Dashboard

ArgoCD

### Auto Sync Enabled

Auto Sync

### Sync Details

Sync Details

---

## Kubernetes Resources

### Pods Running

Pods

### Service (LoadBalancer)

Service

---

## Application Output

### Initial Version (v1)

Output

---

## GitOps Working Proof

### Code Change (GitHub Commit)

GitHub Change

### Updated Output (v2)

Output Change

---

## GitOps Workflow

* Developer updates code
* Pushes changes to GitHub
* ArgoCD detects changes automatically
* Syncs application with Kubernetes
* Updated version deployed without manual intervention

---

## Commands Used

```bash
# Build Docker Image
docker build -t riyajkalawant/gitops-app:v1 .

# Push Image
docker push riyajkalawant/gitops-app:v1

# Check Pods
kubectl get pods

# Check Services
kubectl get svc
```

---

## Key Features

GitOps-based deployment
Automated sync using ArgoCD
Self-healing enabled
Scalable Kubernetes deployment
No manual cluster changes

---

## Learnings

Importance of Git as source of truth
ArgoCD automation and sync
Kubernetes YAML structure
Debugging deployment issues

---

## Conclusion

Successfully implemented a production-style GitOps pipeline using ArgoCD and AWS EKS with automated deployments.

---

## Author

Riyaj Kalawant
vv
