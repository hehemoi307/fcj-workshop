---
title: "Worklog - Week 11"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Receive feedback from Admin/Mentor to adjust the communication flow at the Edge Layer and finalize the overall AWS architecture diagram.
* Take primary responsibility for deploying the static Frontend interface (ReactJS) and setting up the content delivery network (CloudFront) for the Pet Resort & Care System project.
* Coordinate with the team to complete the security infrastructure and integrate the cache (ElastiCache) to increase the system's response speed.

### Tasks completed during the week:
| Day | Tasks | Start Date | End Date | References |
| :---: | :--- | :---: | :---: | :--- |
| 2 | - Receive feedback from Admin: Adjust the CloudFront routing flow for the Frontend and Media Bucket to optimize Caching and avoid cross-origin errors.<br>- Finalize the final AWS architecture diagram with the team. | 06/29/2026 | 06/29/2026 | Feedback from Admin AWS Study Group |
| 3 | - Coordinate Network & Security layer deployment: Initialize VPC, divide Subnets.<br>- Set up Security Groups: Configure Inbound rules allowing traffic from CloudFront into the Application Load Balancer (ALB) safely. | 06/30/2026 | 06/30/2026 | AWS Documentation (VPC, Security Groups) |
| 4 | - Participate in Data Tier deployment: While the team builds Amazon RDS MySQL, proceed to configure the Amazon ElastiCache (Redis) cluster following the Cache-Aside pattern to reduce the load on the primary Database. | 07/01/2026 | 07/01/2026 | AWS Documentation (RDS, ElastiCache) |
| 5 | - Reconfigure Environment Variables of the ReactJS build, update the Base URL to point directly to the ALB Endpoint just initialized by the team.<br>- Test the API flow from local to the EC2 server. | 07/02/2026 | 07/03/2026 | React Environment Config |
| 7 | - Deploy Edge Tier: Upload static ReactJS source code to S3 Frontend, create S3 Media for image storage.<br>- Configure CloudFront to route requests and attach AWS WAF firewall to protect the website from security risks (like SQL Injection, XSS). | 07/04/2026 | 07/04/2026 | AWS Documentation (CloudFront, S3, WAF) |

### Achievements of the week:

#### A. Architecture Finalization
* Successfully fixed logic errors in the Data Flow design based on Admin's suggestions: Clearly separated the role of CloudFront combined with S3 for the static Frontend, and the direct Media resource calling flow.
* Firmly finalized the project architecture diagram, fully prepared for the final project defense and acceptance process.

#### B. Edge & Delivery Deployment
* Successfully brought the *Pet Resort & Care System* interface to the real Cloud environment.
* Successfully integrated CloudFront CDN, making the website load extremely fast thanks to the distribution mechanism across Edge Locations and ensuring data encryption with HTTPS.
* Attached Web Application Firewall (WAF) to CloudFront, successfully setting up basic Rules to block malicious external access, adhering to the defense-in-depth security principle.

#### C. Team Core Infrastructure Setup
* **VPC & Networking:** Successfully divided Subnets, Route Tables, and Internet Gateway, ensuring High Availability (Multi-AZ) for the entire system.
* **Multi-layer Security (Security Groups):** Detailed configuration of firewall rules for the ALB, Backend, Database, and Cache, safely isolating internal resources from the Public network.
* **Database (Amazon RDS):** Successfully launched the MySQL database instance (`petshop-database-1`), securely stored internal Endpoint parameters, and optimized configuration options to control monthly costs.