# AWS Cloud Practitioner – Quick Revision Cheat Sheet

This file is my last-minute revision sheet for the **AWS CLF-C02 exam**.  
It contains the most important concepts that appear frequently in exam questions.

---

# Cloud Computing Basics

**Cloud = On-demand IT resources over the internet with pay-as-you-go pricing**

### Advantages of Cloud

- No upfront infrastructure cost
- Scale instantly
- High availability
- Global deployment in minutes
- Pay only for what you use

---

# AWS Global Infrastructure

Region → Multiple Availability Zones (AZ)

Example:

Toronto Region = `ca-central-1`

Key rule:

Region = Geographic location  
AZ = Isolated data center inside region

Edge Locations = Used by CloudFront (CDN)

---

# Shared Responsibility Model

AWS manages:

- Physical security
- Hardware
- Networking
- Data center operations

Customer manages:

- Data
- Passwords
- IAM permissions
- OS updates (EC2)
- Application security

Shortcut:

EC2 → customer controls more  
S3 → AWS controls more

---

# IAM (Identity & Access Management)

Root user:

Full access (avoid using)

Best practice:

Create IAM users + enable MFA

IAM Components:

Users = individuals  
Groups = collection of users  
Roles = temporary permissions  
Policies = permission documents

Always follow:

Least Privilege Principle

---

# Core AWS Services

EC2 → Virtual server

S3 → Object storage

RDS → Managed relational database

Lambda → Serverless compute

VPC → Private cloud network

CloudFront → Content delivery network

DynamoDB → NoSQL database

---

# ⚡ Compute Services Comparison

EC2 → full control

Lambda → no server management

Elastic Beanstalk → deploy apps automatically

---

# S3 Storage Classes

Standard → frequent access

Standard-IA → infrequent access

One Zone-IA → single AZ backup

Glacier → archive storage

Glacier Deep Archive → cheapest storage

Rule:

More archive = cheaper + slower retrieval

---

# Security Services

IAM → access control

Shield → DDoS protection

WAF → web filtering firewall

KMS → encryption key manager

GuardDuty → threat detection

Inspector → vulnerability scanning

---

# Pricing Models

On-Demand → flexible, expensive

Reserved → cheaper long-term

Spot → cheapest but interruptible

Savings Plans → flexible discount model

---

# Billing Support Plans

Basic → free

Developer → business hours support

Business → 24/7 support

Enterprise → full support + TAM

---

# Well-Architected Framework

5 Pillars:

Operational Excellence

Security

Reliability

Performance Efficiency

Cost Optimization

Shortcut memory trick:

**OSRPC**

---

# Networking Basics

VPC = private network

Internet Gateway = public internet access

Security Group = instance firewall

NACL = subnet firewall

Security Group → stateful

NACL → stateless

---

# High Availability vs Fault Tolerance

High Availability = minimal downtime

Fault Tolerance = zero downtime

Example:

Multi-AZ = High availability

Multi-Region = Fault tolerance

---

# Exam Tips I Remember Before Test

Questions asking **cheapest** → Glacier

Questions asking **global CDN** → CloudFront

Questions asking **temporary permissions** → IAM Roles

Questions asking **NoSQL database** → DynamoDB

Questions asking **DDoS protection** → AWS Shield

Questions asking **private network** → VPC

Questions asking **serverless compute** → Lambda

---

# Final Reminder

Think:

Security → IAM

Storage → S3

Compute → EC2

Serverless → Lambda

Database → RDS / DynamoDB

Network → VPC
