# ☁️ Cloud & DevOps Engineering

> **Cloud • Infrastructure • Automation • Containers • Kubernetes • Monitoring • CI/CD**

A complete learning roadmap covering **Cloud Computing, Microsoft Azure, Terraform, Git, Docker, Kubernetes, Ansible, Prometheus, Grafana, Azure DevOps, and GitHub Actions**.

---

## 🎯 Objective

This learning path is designed to build strong practical knowledge in:

- ☁️ Cloud Computing
- 🌐 Networking
- 🔵 Microsoft Azure
- 🏗️ Infrastructure as Code
- 🔧 Version Control
- 🐳 Containerization
- ☸️ Container Orchestration
- ⚙️ Configuration Management
- 📊 Monitoring & Visualization
- 🚀 CI/CD
- 🔐 Cloud & Infrastructure Security

---

# 1️⃣ ☁️ CLOUD COMPUTING

### Data Center

- What is a Data Center
- Parts of a Data Center
- On-Premises Data Center
- Cloud Data Center

### Cloud Service Models

- IaaS – Infrastructure as a Service
- PaaS – Platform as a Service
- SaaS – Software as a Service

### Basic Networking

- IP Address
- IP Address Classes
- CIDR – Classless Inter-Domain Routing
- DNS – Domain Name System
- Networking Fundamentals

### Important Keywords

- Cloud
- Region
- Availability Zone
- Data Center
- Virtualization
- Scalability
- Elasticity
- High Availability
- Fault Tolerance
- Disaster Recovery

---

# 2️⃣ 🔵 MICROSOFT AZURE

## 2.1 Resource Group

- Resource Group
- Resource Organization
- Resource Management

## 2.2 Basic Networking

### 2.2.1 IP Address

- Public IP
- Private IP
- Static IP
- Dynamic IP

### 2.2.2 CIDR

- CIDR notation
- Network range
- Subnet calculation

### 2.2.3 DNS

- Domain Name System
- Name Resolution
- Public DNS
- Private DNS

### 2.2.4 VNet

- Virtual Network
- Subnets
- Network Configuration

## 2.3 Azure Account

- Azure Account Creation
- Azure Portal
- Subscription
- Resource Management

## 2.4 VNet Peering

- Virtual Network Peering
- VNet-to-VNet Communication
- Regional Peering
- Global Peering

## 2.5 NSG

**Network Security Group**

- NSG Rules
- Inbound Rules
- Outbound Rules
- Priority
- Allow / Deny

### NSG at NIC Level

- Network Interface Security
- VM-level traffic control

### NSG at Subnet Level

- Subnet-level security
- Network traffic filtering

## 2.6 ASG

**Application Security Group**

- Application-based grouping
- Simplified NSG rules
- VM grouping

## 2.7 Azure Load Balancer

- Layer 4 Load Balancing
- Backend Pool
- Health Probe
- Load Balancing Rules
- Public Load Balancer
- Internal Load Balancer

## 2.8 Azure Application Gateway

- Layer 7 Load Balancing
- HTTP/HTTPS Routing
- URL-based Routing
- SSL Termination
- WAF

## 2.9 Traffic Manager

- DNS-based Traffic Routing
- Endpoint Monitoring
- Priority Routing
- Performance Routing
- Geographic Routing

## 2.10 Azure App Service

- Web Applications
- Application Deployment
- App Service Plans
- Environment Variables
- Scaling

## 2.11 Azure Front Door

- Global Application Delivery
- CDN
- Routing
- SSL/TLS
- WAF
- Global Load Balancing

## 2.12 Storage Account

- Blob Storage
- File Storage
- Queue Storage
- Table Storage
- Storage Containers

## 2.13 Identity Management

- Storage Account Access
- Access Keys
- SAS
- RBAC
- Managed Identity

## 2.14 Image Creation

- VM Images
- Custom Images
- Image-based Deployment

## 2.15 VMSS

**Virtual Machine Scale Sets**

- VM Scaling
- Autoscaling
- Load Balancing
- High Availability

## 2.16 Azure Bastion

- Secure VM Access
- Browser-based RDP
- Browser-based SSH
- No Public IP required on VM

## 2.17 Recovery Services Vault

- Backup Management
- Disaster Recovery
- Backup Policies
- Recovery Points

## 2.18 Recovery Services Vault Recovery

- VM Recovery
- File Recovery
- Backup Recovery
- Disaster Recovery

## 2.19 Azure SQL

- Azure SQL Database
- Database Deployment
- Database Security
- Backup
- High Availability

## 2.20 Hub and Spoke

- Hub VNet
- Spoke VNets
- Centralized Networking
- Shared Services
- Network Security

## 2.21 Azure VPN

- Site-to-Site VPN
- Point-to-Site VPN
- Secure Connectivity
- Hybrid Networking

## 2.22 Microsoft Entra ID

Formerly known as **Azure Active Directory**

- Users
- Groups
- Roles
- Authentication
- Authorization
- Identity Management

## 2.23 Azure Monitor

- Metrics
- Logs
- Alerts
- Monitoring
- Application Insights
- Log Analytics

## 2.24 Azure Logic Apps

- Workflow Automation
- Application Integration
- Event-based Automation
- API Integration
- Scheduled Automation

---

# 3️⃣ 🏗️ TERRAFORM

## 3.1 Introduction

- Infrastructure as Code
- Terraform Architecture
- Providers
- Resources
- State

## 3.2 VNet Peering

- Azure VNet Peering using Terraform
- Resource Dependencies

## 3.3 Variables

- Input Variables
- Variable Types
- `.tfvars`
- Environment-based Configuration

## 3.4 VM Creation

- Azure VM Deployment
- Networking
- Storage
- NSG
- VM Configuration

## 3.5 Data Types

- String
- Number
- Boolean
- List
- Map
- Set
- Object

## 3.6 Workspace

- Terraform Workspaces
- Environment Separation
- State Management

## 3.7 Depends On

- Explicit Dependencies
- Resource Creation Order

## 3.8 Data Block & Import

- Data Sources
- Existing Infrastructure
- `terraform import`

## 3.9 Modules

- Reusable Infrastructure
- Root Modules
- Child Modules
- Module Variables
- Module Outputs

## 3.10 Provisioners

- File Provisioner
- Local-Exec
- Remote-Exec
- Provisioner Use Cases

---

# 4️⃣ 🌿 GIT & GITHUB

## 4.1 Introduction

- Version Control
- Repository
- Commit
- Branch
- Remote Repository

### 4.1.1 Centralized Version Control

- Central Repository
- Client-Server Model

### 4.1.2 Distributed Version Control

- Local Repository
- Remote Repository
- Distributed Development

## 4.2 GitHub Introduction

- Repository
- Branches
- Pull Requests
- Issues
- Actions

## 4.3 Git Areas

- Working Directory
- Staging Area
- Local Repository
- Remote Repository

## 4.4 Git Installation

- Git Installation
- Git Configuration
- Username
- Email

## 4.5 Git PAT

**Personal Access Token**

- Token Creation
- Repository Access
- Authentication
- Token Management

## 4.6 Git Basic Commands

```bash
git init
git clone
git status
git add
git commit
git push
git pull
git fetch
git branch
git checkout
git switch
git merge
git log
git remote
