# 🚀 DevOps Package Manager

<p align="center">
  <b>The Open-Source DevOps Package Manager</b>
</p>

<p align="center">
  Install Docker, Kubernetes, Terraform, Jenkins & 15+ DevOps tools with one command.
</p>

---

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-orange?logo=linux" />
  <img src="https://img.shields.io/badge/Built%20With-Bash-black?logo=shell" />
  <img src="https://img.shields.io/badge/Containerization-Docker-blue?logo=docker" />
  <img src="https://img.shields.io/badge/Orchestration-Kubernetes-blue?logo=kubernetes" />
  <img src="https://img.shields.io/badge/IaC-Terraform%20%7C%20Ansible-red?logo=terraform,ansible" />
  <img src="https://img.shields.io/badge/CI-Jenkins%20%7C%20GitLab Runner-violet" />
  <img src="https://img.shields.io/badge/Monitoring-Prometheus%20%7C%20Grafana%20%7C%20ELK-purple" />
  <img src="https://img.shields.io/badge/Security-SonarQube%20%7C%20Trivy-brown" />
  <img src="https://img.shields.io/badge/Cloud CLI-AWS CLI%20%7C%20Azure CLI%20%7C%20GCloud-orange" />
  <img src="https://img.shields.io/badge/Tools-15%2B-green" />
  <img src="https://img.shields.io/badge/license-MIT-blue" />
</p>

---

# 🔥 What Is This?

DevOps Package Manager is a modular, production-ready command-line tool that installs and manages essential DevOps infrastructure tools.

No more copying 40-step installation docs.

---

# ✨ Features

- Install 15+ DevOps tools
- Built-in search engine
- Auto-update system
- Safe rollback support
- CI-validated scripts
- Modular plugin architecture
- Official vendor repositories only
- OS auto-detection
- Release automation

---

## 📦 Included DevOps Tools Categories

| Category        | Tools |
|---------------|--------|
| Containerization | Docker |
| Orchestration | Kubernetes (kubeadm), Helm |
| CI/CD | Jenkins, GitLab Runner |
| IaC | Terraform, Ansible |
| Monitoring | Prometheus, Grafana, ELK |
| Cloud CLI | AWS CLI, Azure CLI, GCloud |
| Security | Trivy, SonarQube |

---

# 📂 FOLDER STRUCTURE  

```bash
devops-package-manager/  
│   
├── devops  # Main CLI
├── install.sh  
├── VERSION  
├── LICENSE  
├── README.md  
│  
├── core/  
│   ├── updater.sh  
│   ├── os-detect.sh  
│   ├── logger.sh  
│  
├── config/  
│   └── tools.yaml  
│  
├── modules/  
│   ├── docker/install.sh  
│   ├── kubernetes/install.sh  
│   ├── terraform/install.sh  
│   ├── ansible/install.sh  
│   ├── jenkins/install.sh  
│   ├── prometheus/install.sh  
│   ├── grafana/install.sh  
│   ├── elk/install.sh
│   ├── sonarqube/install.sh  
│   ├── trivy/install.sh  
│   ├── awscli/install.sh  
│   ├── azurecli/install.sh  
│   ├── gcloud/install.sh  
│  
├── search/  
│   └── search.py  
│
└── .github/workflows/  
    ├── ci.yml  
    └── release.yml  
```   
##### Modular design allows adding new tools without modifying core CLI.
---

# ⚡ Quick Install (Recommended)

Install globally with one command:

```bash
curl -fsSL https://raw.githubusercontent.com/Syed-Dadapeer226/devops-package-manager/main/install.sh | bash
```

After installation:
```bash
devops version
```

## 📥 Manual Installation  
Step 1 — Clone Repository
```bash
git clone https://github.com/Syed-Dadapeer226/devops-package-manager.git
cd devops-package-manager
```
Step 2 — Make Executable
```bash
chmod +x devops
```
Step 3 — Run CLI
```bash
./devops list
```
---

# 🚀 Basic Usage

- ### List Available Tools
  ```bash
  devops list
  ```
- ### Search Tool
  ```bash
  devops search docker
  ```
- ### Install Tool
  ```bash
  devops install docker
  ```

- Check System Compatibility
  ```bash
  devops doctor
  ```

---

# 🎯 Version Pinning

### Install specific versions:
```bash
devops install docker@24.0
```
```bash
devops install terraform@1.6.0
```

If no version is specified, latest stable version is installed.

---

# 🔄 Auto Update System

- ### Check for updates:
  ```bash
  devops update --check
  ```

- ### Update to latest release:
  ```bash
  devops update
  ```

- ### Force self-update:
  ```bash
  devops self-update
  ```

- ### Rollback to previous version:
  ```bash
  devops rollback
  ```
Updates are fetched securely from GitHub Releases.

---

# 🌐 Remote Plugin Registry

### Install tools not included locally:
```bash
devops install redis
```
```bash
devops install argocd
```
The CLI fetches modules dynamically from a remote registry repository.

---

# 🚀 Full DevOps Environment Setup

### Install complete DevOps stack:
```bash
devops install full-stack
```

Installs:
- Docker
- Kubernetes
- Terraform
- Ansible
- Jenkins
- Monitoring stack

Perfect for:

- New VMs  
- Bootcamps  
- DevOps labs  
- Cloud practice environments

---

# 🎯 Profile-Based Installation

Install predefined stacks:

- ### Cloud Engineer Stack
  ```bash
  devops install profile:cloud
  ```
  Includes:
  - AWS CLI
  - Azure CLI
  - GCloud
  - Terraform

- ### CI/CD Stack
  ```bash
  devops install profile:cicd
  ```
  Includes:
  - Docker
  - Jenkins
  - GitLab Runner

- ### Monitoring Stack
  ```bash
  devops install profile:monitoring
  ```
  Includes:
  - Prometheus
  - Grafana
  - ELK

---

# ⚔ Why Not Install Manually?

|    Manual Setup  | DevOps Package Manager |  
|------------------------|------------------------|  
| 30+ commands per tool  |	      1 command       |  
| Inconsistent setup	   |       Standardized     |  
| No update system	     |   Built-in auto-update |  
| Hard to maintain	     |   Modular architecture |  
| No version control	   |      Version pinning   |  

---

# 🤝 Contributing

1. Fork repository
2. Add module under ```modules/```
3. Update ```config/tools.yaml```
4. Submit Pull Request

We welcome contributions 🚀

---

# ⭐ Support

If this project helps you:  
👉 Star the repository  
👉 Share with your DevOps team  
👉 Contribute new modules  

---

# 📜 License

MIT License

---
