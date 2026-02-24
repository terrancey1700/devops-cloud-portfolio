# Architecture Overview

## Static Portfolio Deployment

User - Amazon S3 Static Website Hosting - Public HTTP Endpoint

---

## Serverless Application

Client - AWS Lambda (Function URL) - CloudWatch Logs

---

## Secure Database Deployment

Client - VPC Security Group (restricted /32 IP) - Amazon RDS (PostgreSQL) - SSL-enforced connection

---

## Golden Image Factory

Packer - Cloud-Init - Ansible provisioning - Versioned AMI artifact - AWS account

---

## Observability Stack

Docker Compose - Prometheus - Node Exporter - Grafana - Alertmanager(Slack)
