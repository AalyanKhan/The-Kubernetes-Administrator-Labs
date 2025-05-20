# The Kubernetes Administrator Labs

A comprehensive collection of hands-on labs and examples for learning Kubernetes administration, covering everything from basic concepts to advanced topics for CKA (Certified Kubernetes Administrator) exam preparation.

## 📚 Table of Contents

- [Overview](#overview)
- [Lab Structure](#lab-structure)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Lab Modules](#lab-modules)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This repository contains 20 comprehensive lab modules designed to help you master Kubernetes administration. Each module focuses on specific aspects of Kubernetes, from basic concepts to advanced networking and security topics. The labs are structured to provide hands-on experience with real-world scenarios.

## 🏗️ Lab Structure

Each lab module contains:
- **Commands**: Essential kubectl commands and operations
- **YAML Manifests**: Ready-to-use Kubernetes resource definitions
- **Scripts**: Automation scripts for cluster setup and management
- **Useful Links**: Additional resources and documentation

## 🔧 Prerequisites

- Basic understanding of containerization concepts
- Access to a Kubernetes cluster (local or cloud)
- kubectl command-line tool installed
- Basic familiarity with YAML syntax

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AalyanKhan/The-Kubernetes-Administrator-Labs.git
   cd The-Kubernetes-Administrator-Labs
   ```

2. **Set up your Kubernetes cluster:**
   - Follow the installation guide in `02. Install Cluster/`
   - Or use a managed Kubernetes service (EKS, GKE, AKS)

3. **Start with the basics:**
   - Begin with `01. K8s Core Concepts/`
   - Progress through each module sequentially

## 📖 Lab Modules

### 01. K8s Core Concepts
- Understanding pods, services, and deployments
- Basic kubectl operations
- Cluster architecture overview

### 02. Install Cluster
- Manual cluster installation
- containerd setup
- Kubernetes component installation

### 03. Deploy Application
- Application deployment strategies
- Service configuration
- Basic networking concepts

### 04. External Access
- NodePort services
- LoadBalancer services
- Ingress controllers

### 05. Users and Permissions
- RBAC (Role-Based Access Control)
- Service accounts
- Cluster roles and bindings

### 06. Debugging & Troubleshooting
- Common debugging techniques
- Log analysis
- Resource inspection

### 07. Multi-container Pods
- Sidecar patterns
- Init containers
- Pod communication

### 08. Data Persistence
- Volumes and PersistentVolumes
- PersistentVolumeClaims
- Storage classes

### 09. Secret & ConfigMap
- Configuration management
- Secret handling
- Environment variables

### 10. Resource Requests & Limits
- CPU and memory management
- Resource quotas
- Quality of Service (QoS)

### 11. Taints & Tolerations, NodeAffinity
- Node selection strategies
- Pod placement
- Workload distribution

### 12. Readiness & Liveness Probes
- Health checks
- Application monitoring
- Self-healing capabilities

### 13. Rolling Updates
- Deployment strategies
- Zero-downtime updates
- Rollback procedures

### 14. Etcd Backup & Restore
- Cluster backup strategies
- Disaster recovery
- Data consistency

### 15. K8s Rest API
- API server interaction
- Custom resource definitions
- API authentication

### 16. Upgrade K8s Cluster
- Cluster upgrade procedures
- Version management
- Compatibility considerations

### 17. Contexts with Multiple Clusters
- Multi-cluster management
- Context switching
- Cross-cluster operations

### 18. Renew K8s Certificates
- Certificate management
- Security best practices
- Automated renewal

### 19. Network Policy
- Network segmentation
- Security policies
- Traffic control

### 20. CKA Exam Tips
- Exam preparation strategies
- Common pitfalls
- Time management

## 🛠️ Usage Examples

### Deploy a Simple Application
```bash
# Create a deployment
kubectl apply -f "03. Deploy Application/nginx-deployment.yaml"

# Expose the deployment
kubectl apply -f "03. Deploy Application/nginx-service.yaml"

# Check the status
kubectl get pods,svc
```

### Set up RBAC
```bash
# Create a role
kubectl apply -f "05. Users and Permissions/dev-cr.yaml"

# Create a role binding
kubectl apply -f "05. Users and Permissions/dev-crb.yaml"
```

### Configure Network Policies
```bash
# Deploy demo applications
kubectl apply -f "19. Network Policy/demo-database.yaml"
kubectl apply -f "19. Network Policy/demo-frontend.yaml"

# Apply network policies
kubectl apply -f "19. Network Policy/demo-np-database.yaml"
kubectl apply -f "19. Network Policy/demo-np-frontend.yaml"
```

## 📝 Notes

- All YAML files are tested and ready to use
- Commands are organized by functionality for easy reference
- Scripts include error handling and validation
- Examples follow Kubernetes best practices

## 🤝 Contributing

Contributions are welcome! Please feel free to submit:
- Bug fixes
- Additional examples
- Documentation improvements
- New lab modules

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Useful Resources

- [Kubernetes Official Documentation](https://kubernetes.io/docs/)
- [CKA Exam Curriculum](https://github.com/cncf/curriculum)
- [Kubernetes Best Practices](https://kubernetes.io/docs/concepts/configuration/overview/)
- [Kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)

## 🔒 Security Updates (2025)

This repository has been updated for 2025 compatibility:
- ✅ Kubernetes 1.28+ support
- ✅ Latest secure container images
- ✅ Fixed deprecated ingress annotations
- ✅ Updated repository URLs
- ✅ Security patches for all components

---

**Happy Learning! 🚀**

*Created by Aalyan Khan - For CKA exam preparation and Kubernetes mastery*
