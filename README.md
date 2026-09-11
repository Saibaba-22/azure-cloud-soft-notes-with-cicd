# ☁️ Azure Cloud with CI/CD

## 🛠️ Technologies & Practical Usage

### ☁️ Cloud — Azure

**Microsoft Azure** is used to provide cloud infrastructure and services for hosting applications.

**Practical:**

* Create Resource Groups
* Create Virtual Networks and Subnets
* Deploy Virtual Machines
* Create Azure Kubernetes Service (AKS)
* Configure Networking and Security
* Deploy applications on Azure

---

### 🏗️ IaC — Terraform

**Terraform** is used to create and manage Azure infrastructure using code.

**Practical:**

* Create Resource Groups
* Create VNets and Subnets
* Create NSGs
* Deploy VMs
* Create AKS
* Manage infrastructure using `terraform plan` and `terraform apply`

---

### 🔀 Version Control — Git

**Git** is used to manage and track source-code changes.

**Practical:**

* Create repositories
* Create branches
* Commit changes
* Merge branches
* Push code to GitHub
* Manage project versions

---

### 🐳 Containerization — Docker

**Docker** is used to package applications and dependencies into containers.

**Practical:**

* Create Dockerfiles
* Build Docker images
* Run containers
* Manage container logs
* Push images to a container registry

---

### ☸️ Orchestration — Kubernetes

**Kubernetes** is used to deploy, manage, scale and maintain containers.

**Practical:**

* Create Pods
* Create Deployments
* Create Services
* Scale applications
* Perform rolling updates
* Manage containerized applications on AKS

---

### ⚙️ Configuration Management — Ansible

**Ansible** is used to automate server configuration and application setup.

**Practical:**

* Install packages
* Configure Linux servers
* Install Docker/Nginx
* Manage configuration files
* Start and stop services
* Automate server setup

---

### 📊 Monitoring — Prometheus

**Prometheus** is used to collect and store infrastructure and application metrics.

**Practical:**

* Monitor CPU
* Monitor memory
* Monitor Kubernetes nodes
* Monitor Pods
* Monitor application metrics
* Create metric queries

---

### 📈 Visualization — Grafana

**Grafana** is used to visualize metrics collected by Prometheus.

**Practical:**

* Create dashboards
* Monitor CPU and memory
* Monitor Kubernetes
* View application performance
* Create alerts
* Analyze system health

---

### 🔄 CI/CD — GitHub Actions

**GitHub Actions** is used to automate Continuous Integration and Continuous Deployment.

**Practical:**

```text
Git Push
   ↓
Build
   ↓
Test
   ↓
Docker Build
   ↓
Push Image
   ↓
Deploy to Azure / AKS
```

---

### 🔄 CI/CD — Azure DevOps

**Azure DevOps** provides tools for building automated CI/CD pipelines.

**Practical:**

```text
Developer
   ↓
Git Repository
   ↓
Azure Pipeline
   ↓
Build
   ↓
Test
   ↓
Docker Image
   ↓
Azure Container Registry
   ↓
AKS
   ↓
Application
```

---

## 🚀 Overall Technology Flow

```text
☁️ Azure
   ↑
🏗️ Terraform
   ↑
🔀 Git
   ↓
🔄 GitHub Actions / Azure DevOps
   ↓
🐳 Docker
   ↓
☸️ Kubernetes / AKS
   ↓
⚙️ Ansible
   ↓
📊 Prometheus
   ↓
📈 Grafana
```

## 🎯 Skills Covered

☁️ Azure
🏗️ Terraform
🔀 Git
🐳 Docker
☸️ Kubernetes
⚙️ Ansible
📊 Prometheus
📈 Grafana
🔄 GitHub Actions
🔄 Azure DevOps

**End-to-End:** Cloud → IaC → Version Control → Containerization → Orchestration → Configuration → Monitoring → Visualization → CI/CD
