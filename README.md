# Dynamic Web Application Deployment on AWS with Docker, Amazon ECR, and ECS

## Overview
This project involves deploying a **dynamic web application** on AWS using **Docker containers** and **Amazon ECS**. The infrastructure setup follows best practices for scalability and security, leveraging **AWS resources** such as **VPC, NAT Gateway, Security Groups, RDS, ALB, and Route 53**.

## Architecture
A **three-tier architecture** was implemented with:
- **Frontend & Backend** running in **Docker containers** on **AWS ECS**
- **Database Layer** using **Amazon RDS**
- **Load Balancing & Routing** through **ALB and Route 53**

## Technologies Used
- **AWS ECS (Elastic Container Service)**
- **Amazon ECR (Elastic Container Registry)**
- **Amazon RDS (Relational Database Service)**
- **Docker**
- **Flyway** (for database migration)
- **GitHub** (for version control)
- **Visual Studio Code** (for development)
- **Amazon Route 53** (for domain management)
- **SSL Certificate** (for secure connections)

---

## Project Setup & Deployment Steps

### 1. Local Environment Setup
- Installed and configured **GitHub**
- Created **SSH key pairs** and added the **public key to GitHub**
- Set up **Visual Studio Code**
- Created a **Docker Hub account**

### 2. AWS Infrastructure Setup
- Built a **three-tier VPC** for network isolation
- Created a **NAT Gateway** for secure outbound traffic
- Configured **Security Groups** for controlled access
- Deployed an **Amazon RDS instance** for database storage

### 3. Containerizing the Web Application
- Created a **GitHub repository** to store the application code
- Developed a **Dockerfile** for the dynamic web application
- Used **build arguments** and **environment variables** for flexibility

### 4. Pushing Docker Image to Amazon ECR
- Built the **Docker image** locally
- Authenticated with **Amazon ECR**
- Pushed the containerized application to the **ECR repository**

### 5. Deploying on AWS ECS & Configuring Services
- Used **Flyway** to migrate data to **Amazon RDS**
- Created an **ECS service** to run the containerized application
- Configured an **Application Load Balancer (ALB)** for traffic management
- Registered an **SSL Certificate** for secure HTTPS access
- Created a **DNS Record in Route 53** to map the domain to the application

### 6. Final Deployment & Testing
- Ensured the **web application was fully functional** on AWS
- Conducted **security and performance testing**
- Monitored logs and metrics for optimization

---

## Reference Materials
- **Architecture Diagram** (Uploaded in the repository)
- **Deployment Scripts** (Available in the repository)

## Conclusion
This project successfully demonstrates deploying a **containerized dynamic web application** on AWS using **Docker, ECR, and ECS**. The setup ensures **scalability, security, and high availability** by leveraging AWS services efficiently.

Feel free to clone the repository and explore the deployment process further. 🚀

