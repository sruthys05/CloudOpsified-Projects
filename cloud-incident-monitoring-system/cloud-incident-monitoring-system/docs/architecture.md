# Architecture Flow - Cloud Infrastructure Monitoring & Incident Management System

![Architecture Diagram](images/architecture.png)

## Diagram (Mermaid - renders on GitHub)

```mermaid
flowchart LR
    app["Monitored APIs / Apps"]
    api["FastAPI Monitoring API"]
    cls["Error Classifier (6+ scenarios)"]
    inc["Incident Tracker (create / update / close)"]
    cw["AWS CloudWatch Logs & Alarms"]
    ps["PowerShell Health Checks"]
    ado["Azure DevOps CI/CD + Git"]
    app -->|errors / logs| api
    api -->|analyze| cls
    cls -->|diagnosis| inc
    api -->|structured logs| cw
    ps -->|health status| api
    ado -->|deploy| api
```

## Components
- **Monitored APIs / Apps**
- **FastAPI Monitoring API**
- **Error Classifier (6+ scenarios)**
- **Incident Tracker (create / update / close)**
- **AWS CloudWatch Logs & Alarms**
- **PowerShell Health Checks**
- **Azure DevOps CI/CD + Git**

## Tech Stack
Python, FastAPI, AWS CloudWatch, Azure DevOps, Git, PowerShell
