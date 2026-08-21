---
tags: [path, cloud-computing, roadmap]
difficulty: 3
---

# Cloud Computing Path

Build and manage infrastructure on remote servers (AWS, Azure, GCP).

## What You Will Do

- Design scalable architectures.
- Automate deployment with code (Infrastructure as Code).
- Manage databases and storage in the cloud.
- Monitor costs and performance.

## Roadmap

### Phase 1: The Basics (Months 1-3)
- **Networking Review**: IP, DNS, Subnets, Firewalls.
- **Linux/Windows Server**: OS fundamentals.
- **Virtualization**: How VMs work.
- **Cloud Provider Choice**: Pick one (AWS recommended).

### Phase 2: Core Services (Months 4-6)
- **Compute**: EC2 (AWS), VMs (Azure).
- **Storage**: S3, Blob Storage.
- **Networking**: VPC, Load Balancers.
- **Databases**: RDS, DynamoDB.
- **IAM**: Users, roles, permissions.

### Phase 3: Advanced & Automation (Months 7-9)
- **Serverless**: Lambda, Functions.
- **Containers**: Docker, Kubernetes (EKS/AKS).
- **IaC**: Terraform or CloudFormation.
- **CI/CD**: Pipelines for automated deployment.

## Domain Goodies

- **AWS Skill Builder**: Official free training from Amazon.
- **Microsoft Learn**: Free Azure modules and paths.
- **Google Cloud Skills Boost**: Qwiklabs for GCP.
- **Cloud Resume Challenge**: Build a resume site using only cloud services.

## Ebooks

See [[ebooks/README|Cloud Computing Ebooks]] for detailed book lists.

## Communities

See [[communities/README|Cloud Computing Communities]] for forums and Discords.

## Practice Projects

Build these projects to solidify your skills and create a portfolio:

### Project 1: Cloud Resume Challenge (Weeks 1-4)
**Goal**: Deploy a complete website using cloud services only.
- **Frontend**: HTML/CSS resume hosted on S3 (AWS) or Blob Storage (Azure)
- **Backend**: Visitor counter using Lambda/Azure Functions + DynamoDB/CosmosDB
- **CI/CD**: Automated deployment with GitHub Actions
- **HTTPS**: Configure CloudFront CDN with custom domain
- **Documentation**: Write a blog post about your architecture
- Use the [[../../00-TEMPLATES/Project-Tracker|Project Tracker Template]] to plan each step
- This is a famous challenge—follow cloudresumechallenge.dev for guidance

### Project 2: Three-Tier Web Application (Weeks 5-8)
**Goal**: Build a production-like architecture.
- **Web Tier**: EC2 instances behind an Application Load Balancer
- **App Tier**: Auto-scaling group of application servers
- **Data Tier**: RDS (MySQL/PostgreSQL) with read replicas
- **Networking**: 
  - Public and private subnets across multiple availability zones
  - NAT Gateway for outbound traffic
  - Security Groups and NACLs for access control
- **Monitoring**: CloudWatch dashboards and alarms
- Document your network diagram and security decisions

### Project 3: Serverless Image Processing Pipeline (Weeks 9-11)
**Goal**: Master event-driven serverless architecture.
- User uploads image to S3 bucket
- S3 trigger invokes Lambda function
- Lambda processes image (resize, add watermark) using PIL/Pillow
- Store processed image in separate S3 bucket
- Update metadata in DynamoDB
- Send success notification via SNS/SES
- Calculate total cost per 1000 images (compare to EC2 approach)

### Project 4: Containerized Microservices with Kubernetes (Weeks 12-15)
**Goal**: Learn container orchestration.
- Dockerize a simple web application (frontend + backend + database)
- Push images to ECR (Elastic Container Registry) or ACR
- Deploy to EKS (Elastic Kubernetes Service) or AKS:
  - Create deployment manifests
  - Configure services and ingress
  - Set up horizontal pod autoscaling
- Implement rolling updates and rollbacks
- Monitor with Prometheus and Grafana (optional advanced)

### Project 5: Infrastructure as Code (IaC) Automation (Weeks 16-18)
**Goal**: Automate everything with Terraform or CloudFormation.
- Choose Terraform (multi-cloud) or AWS CloudFormation
- Write code to provision entire infrastructure:
  - VPC with public/private subnets
  - EC2 instances with security groups
  - RDS database
  - S3 buckets with lifecycle policies
  - IAM roles and policies
- Store code in Git repository
- Implement CI/CD pipeline to validate and deploy IaC
- Compare costs: manual vs. automated deployment time

## Challenge

Complete these quick tasks to test your knowledge:

- [ ] Create a free tier AWS/Azure account.
- [ ] Launch a virtual machine and connect via SSH.
- [ ] Host a static HTML page on cloud storage (S3/Blob).
- [ ] Set up a billing alarm to notify you when spending exceeds $5.
