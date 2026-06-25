# AWS 3-Tier Architecture Project

## Project Overview

This project demonstrates a secure and scalable AWS 3-Tier Architecture design.

## Architecture Components

### Networking Layer

* VPC
* Public Subnet 1
* Public Subnet 2
* Private Subnet 1
* Private Subnet 2
* Internet Gateway
* Route Tables

### Application Layer

* Application Load Balancer
* EC2 Instances
* Auto Scaling Group

### Database Layer

* Amazon RDS

## Security Design

### Load Balancer Security Group

* Allow HTTP (80)
* Allow HTTPS (443)

### EC2 Security Group

* Allow traffic only from Load Balancer Security Group

### Database Security Group

* Allow traffic only from EC2 Security Group

## Traffic Flow

Internet User
→ Load Balancer
→ EC2 Instances
→ RDS Database

## High Availability

* Multiple Availability Zones
* Multiple Public Subnets
* Multiple Private Subnets
* Auto Scaling Group

## Outcome

Designed a secure, scalable, and highly available AWS 3-Tier Architecture following cloud best practices.
