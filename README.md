# AWS 3-Tier Architecture

## 📌 Project Overview

Designed a secure, scalable, and highly available AWS 3-tier architecture demonstrating separation of networking, application, and database layers.

The architecture follows a layered approach where internet traffic reaches the application through an Application Load Balancer, while the database layer remains isolated in private subnets.

## 🏗️ Architecture

```text
Internet Users
      ↓
Application Load Balancer
      ↓
EC2 Instances
      ↓
Amazon RDS

##☁️ AWS Components

### Networking Layer
- Amazon VPC
- Public Subnet 1
- Public Subnet 2
- Private Subnet 1
- Private Subnet 2
- Internet Gateway
- Route Tables
- Multiple Availability Zones

### Application Layer
- Application Load Balancer
- EC2 Instances
- Auto Scaling Group

### Database Layer
- Amazon RDS
- Private Subnets

## 🔐 Security Design

### Load Balancer Security Group
- Allows HTTP traffic on port 80
- Allows HTTPS traffic on port 443

### EC2 Security Group
- Allows application traffic only from the Load Balancer Security Group

### Database Security Group
- Allows database traffic only from the EC2 Security Group

This creates controlled communication between the different layers.

## 🔄 Traffic Flow

Internet User
      ↓
Application Load Balancer
      ↓
EC2 Instances
      ↓
Amazon RDS Database


## 📈 High Availability & Scalability
- Multiple Availability Zones
- Multiple public and private subnets
- Application Load Balancer for traffic distribution
- Auto Scaling Group for scalable EC2 capacity
- Amazon RDS as the database layer


## 🎯 Key Concepts Demonstrated
- AWS VPC networking
- Public and private subnets
- Route tables and Internet Gateway
- Application Load Balancing
- EC2 and Auto Scaling
- Security Groups
- Amazon RDS
- Multi-AZ architecture
- 3-tier application architecture

## 🛠️ Technologies
AWS | VPC | EC2 | Application Load Balancer | Auto Scaling | RDS | Security Groups

