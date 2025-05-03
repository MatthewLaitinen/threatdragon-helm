# 🛡️ OWASP Threat Dragon Helm Chart

A Helm chart for deploying [OWASP Threat Dragon](https://owasp.org/www-project-threat-dragon/) — a modeling tool used to create threat model diagrams — on Kubernetes.

## 📦 Chart Details

This Helm chart installs the OWASP Threat Dragon application, including its UI and API components, into a Kubernetes cluster. It is customizable and supports configuration for persistent storage, ingress, and environment variables.

---

## 🚀 Installation

### Prerequisites

- Kubernetes
- Helm
- [GitHub](https://www.threatdragon.com/docs/configure/github.html) or [GitLab](https://www.threatdragon.com/docs/configure/gitlab.html) configured for access
- (Optional) Ingress Controller like NGINX

### Add the Helm Repository

```bash
helm repo add threat-dragon https://github.com/MatthewLaitinen/threatdragon-helm
helm repo update
helm install my-threat-dragon ./threatdragon-helm/threat-dragon
