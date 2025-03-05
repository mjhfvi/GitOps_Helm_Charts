# DevSecOps Showcase Project

## 📌 Overview

This projects repositories are designed to demonstrate DevSecOps best practices by automating security, CI/CD,
and GitOps workflows using modern tooling.
It incorporates security controls at every stage of the software development lifecycle (SDLC),
ensuring secure and reliable deployments.

## 🧰 Projects list

1. Jenkins Blue-Green Deployment with Helm: [Jenkins Deployment]("https://github.com/mjhfvi/GitOps_Jenkins_Deployment)
   - jenkins iac config include:
     - GitOps Pipeline Jobs
     - pre configure Jenkins loggers
     - pre configure Credentials and Certificates
     - pre configure 'Jenkins Shared Library'
     - pre installed Plugins
2. Terraform Module for iam Security Events Monitor in AWS: [AWS iam Security Events Monitor]("https://github.com/mjhfvi/terraform-aws-iam-security-events-monitor)
   - modular code with multiple variables:
     - setup security monitor for log events like 'create user', ' create access key' and more
     - send alerts in email or sms
3. Helm Charts: [Helm Charts]("https://github.com/mjhfvi/GitOps_Helm_Charts")
   - Kali Linux chart for Kubernetes security and Network Troubleshooting

## 🎯 Key Features

- **Automation**: Automated workflows for CI/CD, security scanning, and infrastructure provisioning.
- **GitOps**: Declarative infrastructure and application management using Git as the single source of truth.
- **Jenkins**: CI/CD pipelines to build, test, scan, and deploy applications securely.
- **Kubernetes (K8s) & Helm**: Deployment and management of containerized applications with security best practices.
- **Security Enhancements**: Static and dynamic analysis, vulnerability scanning, and compliance checks.
- **Pre-commit Hooks**: Automated code linting, security scans, and formatting before commits.
- **Python Scripts**: Custom automation and security utilities.
- **Terraform**: Infrastructure as Code (IaC) to provision cloud resources securely.

## 🛠️ Tech Stack

- **CI/CD**: Jenkins, GitHub Actions
- **Infrastructure**: Kubernetes, Helm, Terraform
- **Security**: Pre-commit, Trivy, Snyk, Checkov, SonarCube
- **Automation**: Python scripts, Bash scripting
- **Monitoring & Logging**: OpenSearch, Prometheus, Grafana

## 🔧 Setup & Installation

### Prerequisites

Ensure you have the following tools installed:

- Docker & Kubernetes
- Helm
- Terraform
- Jenkins
- Pre-commit
- Python 3.x

## 🚀 CI/CD Pipeline Workflow

1. **Code Commit & Pre-commit Hooks**: Run security scans, linting, and formatting checks.
2. **Jenkins Build & Test**: Automated testing, SAST/DAST security scanning.
3. **Terraform Deployment**: Securely provision infrastructure.
4. **K8s Deployment via Helm**: Deploy applications with security policies.
5. **Monitoring & Compliance**: Continuous security validation and alerting.

## 🔒 Security Controls Implemented

- **Infrastructure Scanning**: Terraform security checks with Checkov.
- **Container Security**: Image scanning with Trivy.
- **Code Security**: Pre-commit security checks, SAST tools like Bandit, [Pre-Commit Extended Information](./documentation/PRECOMMIT.md)

## 📌 Future Enhancements

- Integrate Open Policy Agent (OPA) for policy enforcement.
- Implement full GitOps using ArgoCD.
- Enhance dynamic security testing with OWASP ZAP.
- Implement Traefik for blue-green Deployment

## 📧 Contact

For any questions or collaboration opportunities, reach out via [LinkedIn](https://www.linkedin.com/in/mjhfvi) or email at `mjhfvi@gmail.com`.
