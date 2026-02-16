# Week 2 – Infrastructure as Code using AWS CloudFormation

## Objective
To demonstrate Infrastructure as Code (IaC) skills by provisioning AWS resources
using CloudFormation templates instead of manual configuration.

## Services Used
- AWS CloudFormation
- Amazon EC2
- Amazon VPC
- Amazon Subnet
- Amazon Security Groups
- AWS IAM

## Infrastructure Overview
The CloudFormation template provisions:
- A custom VPC
- A public subnet
- A security group allowing SSH access
- An EC2 instance (Free Tier eligible)

All resources are created automatically using a YAML template.

## Deployment Steps
1. Open AWS CloudFormation console
2. Create a new stack
3. Upload the CloudFormation YAML template
4. Provide stack name and parameters
5. Create the stack
6. Verify stack status as CREATE_COMPLETE

## Validation
- Stack creation verified in CloudFormation console
- EC2 instance verified in EC2 console
- Resources confirmed under CloudFormation Resources tab

## Error Handling & Fixes
- Updated AMI ID to match the AWS region
- Corrected instance type to Free Tier eligible (t2.micro)
- Recreated stack successfully after fixes

## CI/CD Pipeline – Design (Week 3)
In Week 3, this repository will be integrated with a CI/CD pipeline using:
- AWS CodePipeline
- AWS CodeBuild

Planned pipeline stages:
- Source: GitHub repository
- Build: CloudFormation template validation
- Deploy: Automated stack deployment

## Author
Shivaprasad
