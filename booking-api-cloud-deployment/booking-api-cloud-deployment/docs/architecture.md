# Architecture Flow - Booking API - Cloud Deployment & Monitoring

![Architecture Diagram](images/architecture.png)

## Diagram (Mermaid - renders on GitHub)

```mermaid
flowchart LR
    usr["Customer / Client"]
    api["Flask Booking API (EC2)"]
    s3["Amazon S3 booking data / artifacts"]
    ses["Amazon SES Email Notifications"]
    cw["AWS CloudWatch Logs & Metrics"]
    git["Git Repository"]
    ado["Azure DevOps Pipeline + PowerShell deploy"]
    usr -->|book / cancel / status| api
    api -->|store| s3
    api -->|send email| ses
    api -->|logs| cw
    git -->|push| ado
    ado -->|deploy| api
```

## Components
- **Customer / Client**
- **Flask Booking API (EC2)**
- **Amazon S3 booking data / artifacts**
- **Amazon SES Email Notifications**
- **AWS CloudWatch Logs & Metrics**
- **Git Repository**
- **Azure DevOps Pipeline + PowerShell deploy**

## Tech Stack
Python, Flask, AWS EC2, S3, CloudWatch, SES, Azure DevOps, Git, PowerShell
