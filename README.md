# 🏗️ Manara-AWS-Project  
## 🚀 Scalable Web Application with ALB and Auto Scaling (Manara AWS Graduation Project)

---

## 🧾 Project Requirements (from Manara Guidelines)

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

## 📌 Project Overview

This project demonstrates how to deploy a **highly available** and **scalable web application** on AWS using key infrastructure components such as **EC2**, **Application Load Balancer (ALB)**, and **Auto Scaling Groups (ASG)**. It follows AWS best practices to ensure performance, reliability, security, and cost-efficiency.

---

## 🧱 Architecture Summary

The infrastructure is based on **EC2 instances across multiple Availability Zones (AZs)** and includes:

- **EC2 Instances** for the web and application tiers.
- **Application Load Balancer (ALB)** to distribute HTTP traffic across AZs.
- **Auto Scaling Groups (ASG)** to automatically increase or decrease EC2 instances based on demand.
- **Amazon RDS (MySQL/PostgreSQL)** deployed in **Multi-AZ** for fault-tolerant data storage.
- **IAM Roles** to securely grant permissions to EC2 instances and services.
- **Amazon CloudWatch & SNS** to monitor system metrics and send notifications.
- **Amazon Route 53**, **Internet Gateway**, and **NAT Gateway** for DNS resolution and internet access within the VPC.

---

## 🔗 How the Services Are Linked Together

Here’s how all the AWS components interact to build a secure and scalable architecture:

1. **User requests (HTTP/HTTPS)** come through **Route 53** which resolves the domain name and routes traffic to the **Application Load Balancer (ALB)**.
2. The **ALB**, deployed in public subnets, forwards the traffic to **EC2 instances in the Web Tier** (within private or public subnets), managed by a **Web Auto Scaling Group (ASG)**.
3. The **Web EC2 instances** may connect to a separate **App Tier** (also managed by another **ASG**) if the application is multi-layered.
4. Both the **Web** and **App EC2 instances** may connect to the **Amazon RDS** database, which is hosted in **private subnets** across two AZs for high availability.
5. **CloudWatch** monitors CPU utilization, latency, and other metrics. When thresholds are breached, **Auto Scaling Groups** launch or terminate instances automatically.
6. **SNS (Simple Notification Service)** sends email or SMS alerts based on CloudWatch alarms.
7. **IAM Roles** are attached to EC2 instances to grant secure access to services like CloudWatch, S3, or RDS—without using static credentials.
8. **NAT Gateways** provide internet access to instances in private subnets (for OS/package updates).
9. **Internet Gateway** allows outbound internet traffic from public subnets.

---

## 🖼️ Solution Architecture Diagram

![AWS diagram](https://github.com/user-attachments/assets/f81e0169-17c5-40fb-b78b-5682429281c8)

This diagram visualizes the complete setup: a multi-tier architecture across 2 Availability Zones, public and private subnets, ALB, ASGs, NAT Gateways, RDS, and monitoring services.

---

## 🧰 Key AWS Services Used

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

---

