---
title: "Worklog - Week 8"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives: Load Balancing & Auto Scaling
*   Duration: from **10/06/2026** to **17/06/2026**.
*   Core focus: Learning and accomplishing tasks regarding **Load Balancing & Auto Scaling**.

| Day | Work & Tasks Accomplished | Start Date | End Date | References |
|:---:|:---|:---:|:---:|:---|
| 1 | Study Application Load Balancer (ALB). Create a Target Group for port 8080 and provision ALB in Public Subnets. | 10/06/2026 | 11/06/2026 | ALB Developer Guide |
| 2 | Research EC2 Auto Scaling. Create a Launch Template storing instance type, custom AMI, and User Data script. | 12/06/2026 | 14/06/2026 | Launch Templates Docs |
| 3 | Provision Auto Scaling Group (ASG) integrated with the ALB Target Group. | 15/06/2026 | 16/06/2026 | Auto Scaling Groups Guide |
| 4 | Configure Target Tracking Scaling Policy on CPUUtilization: Desired 2, Min 2, Max 4. | 17/06/2026 | 17/06/2026 | ASG Dynamic Scaling Policies |

### Key Accomplishments of the Week:

*   **Understand ALB request routing and distribution.**
*   **Configure highly resilient Auto Scaling Group architectures.**
*   **Use EC2 User Data to bootstrap Spring Boot applications automatically on scaling events.**
