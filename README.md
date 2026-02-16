# aws-3tier-webapp
Projects -------- AWS 3-Tier Web Application Deploymen
README.md
architecture-diagram.png
screenshots/
   ├── alb.png
   ├── ec2.png
   ├── rds.png
   ├── working-app.png
   # AWS 3-Tier Web Application Deployment

## Architecture Overview
- Route 53
- Public Application Load Balancer
- Web Tier (EC2 - Public Subnet)
- Internal Load Balancer
- App Tier (EC2 - Private Subnet, Python Flask on Port 5000)
- RDS (MySQL - Private Subnet)
- VPC with 6 subnets across 2 AZ

## Security
- Security group chaining between layers
- RDS accessible only from App Tier
- Bastion Host for SSH access

## Key Features
- High Availability across 2 Availability Zones
- Private database isolation
- Internal Load Balancer between Web and App tier
- Cost optimization after testing (resources terminated)

## Status
Project successfully deployed and validated.
Infrastructure terminated to avoid billing.


