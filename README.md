# 🌐 Multi-Tier Application: Scalable Deployment on AWS

## 👋 Hello and Welcome!

This project showcases the successful migration and deployment of a complex **Multi-Tier Java Web Application** onto a robust, scalable infrastructure on Amazon Web Services (AWS). It represents a critical shift from a local virtualized environment to a production-ready cloud architecture, demonstrating core DevOps and Cloud Engineering principles.

### 🏆 Project Highlights & Key Achievements

100% AWS Deployment: Completed a full "Lift and Shift" migration to AWS, leveraging its native managed services for enhanced stability and scale.
Security Architecture: Implemented a multi-layered security model using granular **Security Groups** to ensure only necessary traffic flows between the Web, Application, and Data tiers.
Scalability & HA: Engineered the application tier with an **Auto Scaling Group (ASG)** behind an **Application Load Balancer (ALB)**, guaranteeing the application can handle traffic spikes and remain highly available.
Structured Deployment: Followed a precise, repeatable deployment roadmap, ensuring every component, from DNS to Caching, was configured correctly.

---

## ☁️ The Production Architecture (AWS Mapping)

This table shows how the application's traditional components were mapped and enhanced using AWS managed services:

---

## 🗺️ AWS Deployment Roadmap: My Process

The deployment was executed in structured phases, ensuring stability and correctness:

### Phase 1: Foundation & Security

1. Security Setup: Established **EC2 Key Pairs** and defined granular **Security Groups** for the Web, App, and Backend tiers.
2. Core Compute: Launched all dedicated **EC2 Instances** for the application and messaging services into private subnets.
3. Internal Networking: Configured a **Route 53 Private Hosted Zone** to enable secure and simple hostname resolution between internal services.

### Phase 2: Application, Scaling & Traffic

4. Build & Artifact Deployment: Compiled the code using **Maven** and uploaded the production-ready WAR file to a private **S3** bucket for reliable distribution to the EC2 instances.
5. Elasticity: Configured the **Auto Scaling Group (ASG)**, defining launch templates and scaling policies to dynamically adjust the number of application servers based on load.
6. Public Access: Created the **Application Load Balancer (ALB)** to manage external traffic. A public **Route 53** record was then pointed to the ALB to finalize external DNS routing.
7. Validation: Performed comprehensive checks to confirm all services were communicating correctly, the ASG was scaling, and the application was fully accessible.

🛠️ Key Technologies Used

Cloud Platform: AWS
Core Application: Java, Spring MVC, Spring Security, Spring Data JPA
Networking & Compute: EC2, ALB, ASG, VPC, Route 53
Data Services: RDS (MySQL), ElastiCache (Memcached)
DevOps Tools: Maven, S3
Security: Security Groups, Key Pairs, IAM

<img width="996" height="476" alt="image" src="https://github.com/user-attachments/assets/f16503b3-3a5e-46e5-87ba-acfb317a36e5" />


