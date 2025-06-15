# Manara-AWS-Project
# 🚀 Scalable Web Application with ALB and Auto Scaling (Manara AWS Graduation Project)

## 📌 Project Overview

This project demonstrates how to deploy a **highly available and scalable web application** on AWS using EC2, Elastic Load Balancing (ALB), and Auto Scaling Groups (ASG). It follows AWS best practices in terms of security, performance, and cost optimization.

---

## 🧱 Architecture Summary

The infrastructure is based on an EC2 architecture and includes:

- **EC2 Instances** in Web and App tiers, placed across two Availability Zones.
- **Application Load Balancer (ALB)** distributes incoming HTTP traffic.
- **Auto Scaling Groups (ASG)** for both Web and App tiers.
- **Amazon RDS** deployed in Multi-AZ for high availability.
- **IAM Roles** for secure access control.
- **Amazon CloudWatch + SNS** for monitoring and alert notifications.
- **Route 53**, **Internet Gateway**, and **NAT Gateway** for full VPC connectivity.

---

## 🖼️ Architecture Diagram

![Architecture Diagram](./architecture.png)

This diagram shows a multi-tier application architecture across 2 AZs with public and private subnets, ASG, ALB, RDS, and monitoring.

---

## 🧰 AWS Services Used

- **Amazon EC2** – Hosts the web and application tier
- **Elastic Load Balancer (ALB)** – Distributes traffic across AZs
- **Auto Scaling Group (ASG)** – Scales EC2 instances based on demand
- **Amazon RDS** – Relational database in Multi-AZ deployment
- **IAM** – Role-based permissions for EC2 and RDS
- **CloudWatch & SNS** – Monitors system performance and sends alerts
- **Amazon Route 53** – DNS management
- **VPC Components** – Public/Private Subnets, NAT Gateway, Internet Gateway

---

## 🎯 Learning Outcomes

- Deploy secure, scalable EC2 applications
- Implement high availability using ALB & ASG
- Integrate IAM, RDS, CloudWatch & SNS
- Design a fault-tolerant and cost-effective AWS architecture

---

## 📂 File Structure

