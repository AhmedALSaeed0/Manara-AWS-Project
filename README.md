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

Here’s ho
