# AWS-Infrastructure-as-a-code
 AWS CloudFormation VPC Setup
This project defines a Virtual Private Cloud (VPC) architecture using AWS CloudFormation and Application Composer. It includes a full network setup with public/private subnets, routing, gateways, and essential components for a highly available and scalable cloud environment.

 File
website.yaml: CloudFormation template defining the network infrastructure.
 Components
The stack provisions the following AWS resources:

VPC: Primary Virtual Private Cloud.

Subnets:

2 Public Subnets (PublicSubnet1, PublicSubnet2)

2 Private Subnets (PrivateSubnet1, PrivateSubnet2)

Route Tables:

Public and Private route tables

Associations for each subnet

Gateways:

Internet Gateway (IGW)

NAT Gateway with Elastic IP (EIP)

Routing:

Public routes to IGW

Private routes to NAT Gateway

Connectivity:

VPC to IGW connection

 Deployment Instructions
Open AWS Application Composer
Navigate to AWS Application Composer.

Upload the Template
Click on Template → Import YAML and upload the website.yaml file.

Validate the Stack
Click Validate to check for template syntax or dependency errors.

Deploy
Once validated, click Update template or deploy via CloudFormation.

 Security
Make sure to configure appropriate Security Groups and IAM Roles based on your application requirements.

 Notes
Ensure you're operating in the correct AWS region (e.g., us-east-1).

This template is a foundational network stack—ideal for launching EC2, ECS, or other AWS services within a structured VPC.
