# Manara-AWS-Project  
## Scalable Web Application with ALB and Auto Scaling (Manara AWS Graduation Project)

---

## Project Requirements (from Manara Guidelines)

> ### Project 1: Scalable Web Application with ALB and Auto Scaling  
> **Architecture:** EC2-based  
>  
> **Description:**  
> Deploy a simple web application on AWS using EC2 instances, ensuring high availability and scalability with Elastic Load Balancing (ALB) and Auto Scaling Groups (ASG). The project demonstrates best practices for compute scalability, security, and cost optimization.  
>  
> **Key AWS Services Used:**  
> - EC2: Launch instances for the web app.  
> - ALB: Distributes traffic across multiple instances.  
> - ASG: Ensures instances scale based on demand.  
> - Amazon RDS (Optional): Backend database with Multi-AZ.  
> - IAM: Role-based access to instances.  
> - CloudWatch & SNS: Monitor performance and send alerts.  
>  
> **Learning Outcomes:**  
> - Setting up secure and scalable EC2-based web applications  
> - Implementing high availability using ALB and ASG  
> - Optimizing costs and performance using Auto Scaling policies  

---

## Project Overview

This project demonstrates how to deploy a **highly available** and **scalable web application** on AWS using key infrastructure components such as **EC2**, **Application Load Balancer (ALB)**, and **Auto Scaling Groups (ASG)**. It follows AWS best practices to ensure performance, reliability, security, and cost-efficiency.

---

## Solution Architecture Diagram

![AWS diagram](https://github.com/user-attachments/assets/46393df8-bc9a-4eba-a054-5ace548ddd85)

This diagram visualizes the complete setup: a multi-tier architecture across 2 Availability Zones, public and private subnets, ALB, ASGs, NAT Gateways, RDS, and monitoring services.

---

## AWS Services Used

- **Amazon EC2** – Hosts the web and application servers
- **Application Load Balancer (ALB)** – Balances traffic between EC2 instances
- **Auto Scaling Group (ASG)** – Automatically adjusts EC2 capacity
- **Amazon RDS** – Relational database (MySQL/PostgreSQL) in Multi-AZ
- **IAM** – Secures access between services
- **Amazon CloudWatch** – Collects and tracks metrics
- **Amazon SNS** – Sends alerts and notifications
- **Amazon Route 53** – DNS service to route users to the application
- **NAT Gateway & Internet Gateway** – Provide controlled internet access to public and private resources
- **Amazon VPC** – Isolated network with subnets and routing
- **Security Groups** – Virtual firewalls controlling inbound and outbound traffic for EC2, RDS, and ALB
- **Route Tables** – Define how traffic is routed between subnets, NAT Gateways, and Internet Gateways

---

