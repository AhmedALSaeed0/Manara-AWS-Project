Manara-AWS-Project
🚀 Scalable Web Application with ALB and Auto Scaling (Manara AWS Graduation Project)
📌 Project Overview
This project demonstrates how to deploy a highly available and scalable web application on Amazon Web Services (AWS) using key infrastructure components such as EC2, Application Load Balancer (ALB), and Auto Scaling Groups (ASG). It aligns with AWS architectural best practices to ensure performance, reliability, security, and cost-efficiency.

🧱 Architecture Summary
The architecture is based on EC2 instances across multiple Availability Zones and includes:

EC2 Instances for both Web and App Tiers.

Application Load Balancer (ALB) for distributing incoming traffic.

Auto Scaling Groups (ASG) to automatically manage EC2 scaling.

Amazon RDS (MySQL/PostgreSQL) in Multi-AZ deployment.

IAM Roles for controlled access to AWS services.

Amazon CloudWatch & Amazon SNS for monitoring and alerting.

Amazon Route 53, Internet Gateway, and NAT Gateway for network connectivity and routing.

🖼️ Solution Architecture Diagram


The diagram shows a multi-tier architecture split across two Availability Zones using both public and private subnets, ALB, ASG, RDS, NAT Gateways, and monitoring integrations with IAM and SNS.

🧰 Key AWS Services Used
Amazon EC2 – Hosts the Web Tier and App Tier

Application Load Balancer (ALB) – Distributes traffic across AZs

Auto Scaling Groups (ASG) – Automatically scales EC2 instances

Amazon RDS (MySQL/PostgreSQL) – Multi-AZ backend database

IAM – Instance and role-based access control

Amazon CloudWatch – Monitoring and performance metrics

Amazon SNS – Alert notifications via email

Amazon Route 53 – DNS-based routing for users

NAT Gateways & Internet Gateway – Internet access for public and private resources

VPC – Custom networking with isolated subnets

🎯 Learning Outcomes
By completing this project, you will learn to:

Deploy secure and scalable EC2-based web applications.

Implement high availability and fault tolerance using ALB and ASG.

Use CloudWatch and SNS for real-time performance monitoring and alerting.

Apply IAM roles and security groups to maintain access control and separation of concerns.

Architect a system that follows cost optimization and reliability best practices.

🧾 Project Requirements (from Manara Guidelines)
Project 1: Scalable Web Application with ALB and Auto Scaling
Architecture: EC2-based

Description:
Deploy a simple web application on AWS using EC2 instances, ensuring high availability and scalability with Elastic Load Balancing (ALB) and Auto Scaling Groups (ASG). The project demonstrates best practices for compute scalability, security, and cost optimization.

Key AWS Services Used:

EC2: Launch instances for the web app.

ALB: Distributes traffic across multiple instances.

ASG: Ensures instances scale based on demand.

Amazon RDS (Optional): Backend database with Multi-AZ.

IAM: Role-based access to instances.

CloudWatch & SNS: Monitor performance and send alerts.

Learning Outcomes:

Setting up secure and scalable EC2-based web applications

Implementing high availability using ALB and ASG

Optimizing costs and performance using Auto Scaling policies

📂 File Structure
bash
Copy
Edit
.
├── README.md                   # Project documentation
├── architecture.png            # Solution architecture diagram
├── deployment-guide.md         # (Optional) Step-by-step deployment guide
├── /src                        # (Optional) Source code for the web application
├── /templates                  # (Optional) Infrastructure-as-Code (Terraform/CFN)
├── /docs
│   └── manara-project-description.pdf  # Original Manara project brief
🎥 Optional Deliverables
✅ Live Demo URL (If deployed): You can host it using EC2 public IP or Route 53 domain

✅ Video Walkthrough (Optional): Record and upload a short video to YouTube, then add the link here.

📎 References
AWS EC2 Docs

AWS Auto Scaling

AWS ALB

AWS CloudWatch

AWS SNS
