# Improvements - Booking API - Cloud Deployment & Monitoring

## Current Result
Automated deployment through Azure DevOps CI/CD and Git, with monitoring and email notifications in place.

## Planned / Possible Improvements

- [ ] Use RDS / DynamoDB for bookings instead of file or S3 storage
- [ ] Put the API behind an Application Load Balancer with Auto Scaling
- [ ] Add idempotency keys to avoid duplicate bookings
- [ ] Queue emails with SQS + Lambda for retries
- [ ] Add Swagger / OpenAPI docs and request validation (Marshmallow / Pydantic)
- [ ] Blue/green or rolling deployments with rollback
- [ ] Use IAM roles and Secrets Manager, no hard-coded credentials
- [ ] HTTPS via ACM + CloudFront / ALB, WAF for protection
