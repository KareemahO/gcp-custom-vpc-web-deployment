# gcp-custom-vpc-web-deployment
Deploying a static website on Google Cloud using a custom VPC, Compute Engine, Linux, and Nginx.

# Project Overview
This project demonstrates the deployment of a static website on Google Cloud using a custom Virtual Private Cloud (VPC). 

The infrastructure includes a custom VPC with separate public and private subnets, a Compute Engine virtual machine, VPC firewall rules, and an Nginx web server. The website will be deployed on the VM and accessed through its external IP address.


The project focuses on understanding network segmentation, IPv4 addressing, cloud networking, Linux administration, firewall configuration, and basic web server deployment.
# Objectives

Create and configure a custom VPC network.
Design public and private subnets using CIDR notation.
Provision a Compute Engine virtual machine.
Configure firewall rules to control inbound web traffic.
Install and configure Nginx on Ubuntu.
Deploy a static website.
Verify website accessibility.
Practise cloud resource management and cost-conscious infrastructure cleanup.
# Architecture
           
                    INTERNET
                        |
                        |
                 External IP
                        |
                VPC Firewall Rules
                        |
               Compute Engine VM
                        |
                      Nginx
                        |
                 Website Files
                 
The VPC contains two subnets:
# kareemah-web-vpc
       |
       |--- public-subnet
       |      10.10.1.0/24
       |      Web server VM
       |
       |--- private-subnet
              10.10.2.0/24
              Reserved for private resources
              
              
# Technologies
              
Google Cloud Platform (GCP)
Virtual Private Cloud (VPC)
IPv4 and CIDR notation
Compute Engine
VPC firewall rules
Ubuntu Linux
Nginx
HTML, CSS and JavaScript
Implementation Progress
Stage
Task
Status
1. Create custom VPC
Completed
2. Create public and private subnets
Completed
3. Provision Compute Engine VM
Pending
4. Configure firewall rules
Pending
5. Install Nginx
Pending
6. Deploy website files
Pending
7. Test website accessibility
Pending
8. Clean up billable resources

# Network Configuration
Resource Configuration
VPC name: kareemah-web-vpc
Subnet creation mode: Custom
Public subnet range: 10.10.1.0/24
Private subnet range: 10.10.2.0/24
Region: us-central1
# Key Concepts
This project explores the following concepts:
VPC: A logically isolated network environment for cloud resources.
Subnetting: Dividing an IP address range into smaller network ranges.
CIDR: A notation for representing IP address ranges.
Firewall rules: Controls that determine which network traffic is allowed or denied.
Compute Engine: Google's virtual machine service.
Nginx: A web server that serves the website files to visitors.
Cost Management
This project is designed to minimise unnecessary cloud expenditure.
After implementation and testing, billable resources will be deleted when no longer required. Relevant attached disks, reserved IP addresses, and other billable resources will also be checked.
The VPC and subnets can remain available for documentation and future experimentation.
