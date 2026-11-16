# Architecture Flow - Automated Deployment & Infrastructure Monitoring

![Architecture Diagram](images/architecture.png)

## Diagram (Mermaid - renders on GitHub)

```mermaid
flowchart LR
    git["Git Repository"]
    ado["Azure DevOps CI/CD Pipeline"]
    win["Windows Server (EC2)"]
    ps["PowerShell Scripts health + backup"]
    sql["MS SQL Server"]
    s3["Amazon S3 Backups"]
    cw["AWS CloudWatch Metrics & Alarms"]
    git -->|commit| ado
    ado -->|deploy| win
    win -->|runs| ps
    ps -->|backup / restore| sql
    sql -->|upload .bak| s3
    ps -->|health metrics| cw
```

## Components
- **Git Repository**
- **Azure DevOps CI/CD Pipeline**
- **Windows Server (EC2)**
- **PowerShell Scripts health + backup**
- **MS SQL Server**
- **Amazon S3 Backups**
- **AWS CloudWatch Metrics & Alarms**

## Tech Stack
AWS (EC2, S3, CloudWatch), Azure DevOps, Windows Server, PowerShell, MS SQL Server, Git
