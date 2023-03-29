**Terraform Configuration for AWS VPC, EC2 and RDS**

**This project contains terraform configuration files on creating EC2 and RDS instances inside a Custom VPC on AWS. Here is the architecture of what will be created:**


![Diagram_New](https://user-images.githubusercontent.com/1199909/228685494-566b0ffb-c84c-421e-abf9-e86b52edcc4a.png)


# devops-task

# Requirements

* EC2 instances should be accessible anywhere on the internet via HTTP
* Only you should be able to access the EC2 instances via SSH
* RDS should be on a private subnet and inaccessible via the internet
* Only the EC2 instances should be able to communicate with RDS


# How will we accomplish there tasks

1. Create a VPC
2. Create an Internet Gateway and attach it to the VPC
3. Create 3 subnets: 1 public for EC2 and 2 private for RDS
4. Create 2 route tables: 1 public and 1 private
5. Create 2 security groups: 1 for EC2 and 1 for RDS
6. Create the DB subnet group
7. Create the MySQL RDS database
8. Create the EC2 instance
9. Verify that everything is set up correctly


Prerequisites

* AWS CLI installed and configured
* Terraform installed
