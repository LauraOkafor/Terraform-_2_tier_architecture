Deploying a 2-Tier Architecture on AWS Using Terraform

Introduction
This project demonstrates the implementation of a 2-tier architecture on AWS using Terraform. The architecture consists of a public-facing application layer and a private database layer, ensuring security and scalability.

Architecture Overview
The 2-tier architecture consists of:

* VPC: A Virtual Private Cloud to host resources securely.

* Subnets:
    * Public Subnet (for web servers)

    * Private Subnet (for database servers)

* Internet Gateway & Route Tables: To enable internet access for the public subnet.

* Security Groups:
    * Web server security group (allows HTTP/HTTPS traffic)

    * Database security group (restricts access to the web servers only)

* EC2 Instances:
    * Web Server (in the public subnet)

    * Database Server (in the private subnet)

* RDS Instance: Hosted in the private subnet for database services.

* Elastic Load Balancer (ELB): To distribute traffic to web servers.

Prerequisites
Before deploying, ensure you have the following:
* AWS CLI installed and configured

* Terraform installed

* An AWS account
