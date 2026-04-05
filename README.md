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

<img width="837" height="357" alt="image" src="https://github.com/user-attachments/assets/df5eca7c-380b-4938-a493-c00b813e4a86" />


### EKS Cluster

<img width="848" height="355" alt="image" src="https://github.com/user-attachments/assets/fb2ec892-7c0c-4986-861a-5ddff88ac9c7" />


### Docker Image

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/f8831e3e-90aa-4555-a284-eb4e899a9639" />

DockerHub

### GitHub Repositor

<img width="848" height="394" alt="image" src="https://github.com/user-attachments/assets/7be73ab9-cb37-416a-ae31-c19def706321" />



## ArgoCD Setup

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5e558fb9-e89f-45df-9a91-af9982d8b355" />


### Auto Sync Enabled

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5c464ee3-e93b-4558-8194-d7b17346c4e4" />


### Sync Details

<img width="850" height="426" alt="image" src="https://github.com/user-attachments/assets/9972dab1-1e15-42f5-8961-69a838b3ecfb" />


## Kubernetes Resources

<img width="736" height="185" alt="image" src="https://github.com/user-attachments/assets/611e8478-810a-4864-b50b-f6a3fba1137d" />

### Service (LoadBalancer)

<img width="857" height="159" alt="image" src="https://github.com/user-attachments/assets/36ea7602-d8c0-4722-befb-7f0163dd49f6" />

## Application Output

### Initial Version (v1)


<img width="801" height="282" alt="image" src="https://github.com/user-attachments/assets/6bb89421-83be-4276-98da-771398c65363" />

---

## GitOps Working Proof


### Updated Output (v2)

Output Change

<img width="794" height="235" alt="image" src="https://github.com/user-attachments/assets/29e37853-024e-4d16-af0e-42e9cb911245" />


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

Bhumika Mahale
