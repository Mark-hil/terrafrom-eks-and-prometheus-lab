## Prometheus & Terraform Labs
Welcome to the Prometheus & Terraform Labs repository! This is your hands-on guide to setting up monitoring with Prometheus and managing cloud infrastructure using Terraform. Whether you're just getting started with Infrastructure-as-Code or looking to integrate monitoring into your cloud environments, this repo is here to help you learn by doing.

##  What’s Inside?
This repository is organized into two key parts:

## Prometheus Monitoring Stack
Set up a complete monitoring system using Prometheus, Grafana, and Node Exporter.

Track system performance and build beautiful, interactive dashboards in Grafana.

## Terraform Infrastructure
Use Terraform to provision AWS infrastructure like EC2 instances, VPCs, and EKS clusters.

Learn how to manage infrastructure securely and efficiently using modular, reusable code.

## What You’ll Learn
By working through these labs, you’ll gain practical experience with:

Deploying a Prometheus-based monitoring solution.

Using Terraform to automate infrastructure on AWS.

Best practices for combining observability and infrastructure management in real-world environments.

## Repository Structure

```bash
.
├── Promethuse-grafana-dashboard/          # Monitoring Dashboards & Setup
│   ├── Metrics Dashboards
│   │   ├── 95th percentile.png
│   │   ├── Application-uptime.png
│   │   ├── average-reponse-time.png
│   │   ├── cpu-usage.png
│   │   ├── memory-usage.png
│   │   └── throughput.png
│   └── promethuse-lab/                    # Prometheus Lab Components
│       ├── app/                           # Sample Application
│       ├── promethes-grafana-alert/       # Alerting Configuration
│       └── test-dasbord.json
│
└── terraform-EKS/                         # EKS Infrastructure
    ├── modules/                           # Terraform Modules
    │   ├── ec2/                          # EC2 Instance Configuration
    │   ├── eks/                          # EKS Cluster Setup
    │   ├── k8s/                          # Kubernetes Resources
    │   ├── monitoring/                   # Monitoring Stack
    │   ├── s3-backend/                   # Remote State Backend
    │   ├── security_group/               # Security Groups
    │   └── vpc/                          # Network Configuration
    └── scripts/                          # Automation Scripts
```
🛠 Getting Started
To start exploring the labs:

Clone the repository:
```bash
git clone https://github.com/Mark-hil/terrafrom-eks-with-module-approach.git
cd terrafrom-eks-and-prometheus-lab
```
Pick a project:

Head to the prometheus/ folder to set up monitoring tools.

Dive into the terraform/ folder to work on AWS infrastructure.

Each directory contains its own README with detailed setup instructions.
