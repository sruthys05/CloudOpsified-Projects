# Improvements - Cloud Infrastructure Monitoring & Incident Management System

## Current Result
Automated incident diagnostics for 6+ error scenarios.

## Planned / Possible Improvements

- [ ] Add CloudWatch Alarms + SNS for automatic paging (Email/Slack/Teams)
- [ ] Store incidents in a database (PostgreSQL / DynamoDB) instead of in-memory
- [ ] Add a dashboard (Grafana or CloudWatch Dashboard) for MTTR and incident counts
- [ ] Use ML/LLM-based log summarization for unknown error patterns
- [ ] Containerize with Docker and deploy on ECS/EKS
- [ ] Add auth (JWT / API keys) and rate limiting to the APIs
- [ ] Infrastructure as Code with Terraform or CloudFormation
- [ ] Unit tests + pipeline quality gates (pytest, flake8, Bandit)
