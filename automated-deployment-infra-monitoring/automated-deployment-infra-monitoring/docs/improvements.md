# Improvements - Automated Deployment & Infrastructure Monitoring

## Current Result
Automated deployments and server health checks, with SQL Server backups stored in Amazon S3.

## Planned / Possible Improvements

- [ ] S3 lifecycle rules (Standard -> IA -> Glacier) and versioning for backups
- [ ] Automated restore testing to verify backups are valid
- [ ] Backup encryption (KMS) and checksum verification
- [ ] CloudWatch Alarms + SNS alerts on failed backups / unhealthy servers
- [ ] Approval gates and staging -> production environments in the pipeline
- [ ] Move secrets to AWS Secrets Manager / Azure Key Vault
- [ ] Centralized logging and dashboards
- [ ] Infrastructure as Code (Terraform / CloudFormation)
