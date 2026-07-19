---
title: "Worklog"
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

This worklog documents a 13-week internship journey at **AWS First Cloud Journey** (from April 17, 2026 to July 30, 2026). Throughout this period, the student conducted in-depth research on AWS cloud services and successfully deployed the **Pet Resort & Care System** — a full-stack web application for pet spa booking and product shopping.

---

### 📅 Phase 1: AWS Technology & Services Research (Weeks 1 - 10)

*   **Week 1 (17/04 - 23/04/2026):** [Cloud Foundations & Reporting Tools](1.1-Week1/)
    *   Get familiar with the AWS ecosystem, create an AWS Free Tier account, and apply initial security. Set up and practice building static sites locally using Hugo.
*   **Week 2 (24/04 - 30/04/2026):** [Access Control & Authorization with AWS IAM](1.2-Week2/)
    *   Study IAM authentication, apply Least Privilege principles by creating IAM Users, Groups, Customer Managed Policies, and configuring secure IAM Roles.
*   **Week 3 (01/05 - 08/05/2026):** [VPC Network Infrastructure Basics](1.3-Week3/)
    *   Learn VPC (Virtual Private Cloud) fundamentals. Calculate IP CIDR blocks, divide Public/Private Subnets, and configure appropriate Route Tables for a multi-tier architecture.
*   **Week 4 (09/05 - 17/05/2026):** [Advanced Routing & Traffic Flow Control](1.4-Week4/)
    *   Configure NAT Gateway routing for Private Subnet Internet access. Establish secure private connections to AWS services using Interface and Gateway VPC Endpoints.
*   **Week 5 (18/05 - 24/05/2026):** [Cloud Storage with Amazon S3](1.5-Week5/)
    *   Host the static Frontend website on S3, manage object storage lifecycle, and configure secure bucket policies for API media uploads.
*   **Week 6 (25/05 - 01/06/2026):** [CDN Distribution & Edge Protection with WAF](1.6-Week6/)
    *   Leverage CloudFront CDN for global website acceleration. Create WAF Web ACL rules integrated with CloudFront to block malicious traffic and web vulnerabilities.
*   **Week 7 (02/06 - 09/06/2026):** [Virtual Servers with Amazon EC2](1.7-Week7/)
    *   Launch Linux EC2 instances, establish secure Security Groups, and install Amazon Corretto JDK 17 to host the Spring Boot Backend API.
*   **Week 8 (10/06 - 17/06/2026):** [Load Balancing & Auto Scaling](1.8-Week8/)
    *   Configure Target Groups and an Application Load Balancer (ALB). Set up Launch Templates and EC2 Auto Scaling Groups to scale servers dynamically based on CPU utilization.
*   **Week 9 (18/06 - 25/06/2026):** [Relational Databases & Cache Clusters](1.9-Week9/)
    *   Deploy Amazon RDS MySQL under a Multi-AZ (Primary/Standby) model for high availability. Configure a Redis cluster with ElastiCache for session caching.
*   **Week 10 (26/06 - 02/07/2026):** [Monitoring, Alerting & Security Configuration](1.10-Week10/)
    *   Encrypt sensitive configurations using KMS and Secrets Manager. Track system health via CloudWatch Metrics/Logs and set up email alerts with Amazon SNS.

---

### 🚀 Phase 2: Design, Deployment & Final Release (Weeks 11 - 13)

*   **Week 11 (03/07 - 10/07/2026):** [Architecture Design & Data Flow Mapping](1.11-Week11/)
    *   Consolidate all studied technologies to design a secure, fault-tolerant 3-tier system architecture. Map detailed data flows between Frontend, Backend, and Database.
*   **Week 12 (11/07 - 20/07/2026):** [Multi-tier System Cloud Deployment](1.12-Week12/)
    *   Deploy the entire application to AWS: host Frontend on S3+CloudFront, create a custom AMI from EC2, configure Auto Scaling behind ALB, and integrate RDS and ElastiCache.
*   **Week 13 (21/07 - 30/07/2026):** [QA Load Testing, Security Hardening & Project Release](1.13-Week13/)
    *   Run performance load testing using Artillery, troubleshoot CORS and Database URL connection issues, optimize cloud spending (FinOps), and compile the final internship report.
