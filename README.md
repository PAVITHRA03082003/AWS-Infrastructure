# AWS-Infrastructure
AWS Infrastructure Projects is a collection of hands-on projects demonstrating real-world AWS setups using CloudFormation (YAML). It includes examples like Auto Scaling Groups with ALB, showcasing scalable, highly available architectures deployed via IaC.      

This repository contains hands-on AWS infrastructure projects that demonstrate real-world usage of core AWS services using Infrastructure as Code (IaC) with CloudFormation (YAML) templates.

**Project Structure**

pgsql
Copy
Edit
AWS-Infrastructure-Projects/
├── ASG-autoscaling-groups/

│   ├── ASG.yaml

│   └── Auto-scaling-groups.pdf

├── README.md

**Projects Included**

1. Auto Scaling Group (ASG) Setup
File: ASG.yaml

Description: CloudFormation template to launch a scalable and highly available EC2-based web application using:

Launch Templates

Auto Scaling Groups

Target Groups & Application Load Balancer (ALB)

Documentation: Refer to Auto-scaling-groups.pdf for detailed architecture, explanation, and deployment flow.

**How to Use:-**

Sign in to your AWS Console.

Navigate to CloudFormation service.

Click Create Stack → With new resources (standard).

Upload the ASG.yaml template file.

Follow the stack creation wizard and specify required parameters.

Monitor the stack creation process and verify resources in EC2 and Auto Scaling dashboards.

**Prerequisites**

Active AWS account

IAM role or user with permissions for CloudFormation, EC2, VPC, Auto Scaling, and ALB

(Optional) AWS CLI installed and configured if deploying via CLI

**Deployment via AWS CLI (Optional)**

bash
Copy
Edit
aws cloudformation create-stack \
--stack-name MyASGStack \
--template-body file://ASG-autoscaling-groups/ASG.yaml \
--capabilities CAPABILITY_NAMED_IAM
