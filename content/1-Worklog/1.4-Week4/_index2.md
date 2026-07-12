---
title: "Worklog - Week 4"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:
- Research independent virtual network architecture (Amazon VPC) to build a secure system deployment environment.
- Approach cloud database management solutions with Amazon RDS and practice optimal configuration labs.
- Set up network-layer access control mechanisms (Security Groups) for data storage components.

| Day | Tasks & Completed Assignments | Start Date | End Date | References |
|:---:|:---|:---:|:---:|:---|
| 1 | Learn Amazon VPC theory: Concepts of CIDR block, how to divide Public Subnet (for open resources) and Private Subnet (for internal resources that need IP hiding). | 05/11/2026 | 05/11/2026 | Amazon VPC Documentation |
| 2 | Research Amazon RDS service: Compare the self-managed model (Database on EC2) and the AWS-managed model (Managed Service) in terms of operations and backups. | 05/12/2026 | 05/12/2026 | Amazon RDS Documentation |
| 3 | Practice Lab creating a Relational Database (MySQL) on Amazon RDS, exploring storage options and automated Backup mechanisms. | 05/13/2026 | 05/13/2026 | AWS RDS Console |
| 4 | Network layer security configuration: Create a separate Security Group for the Database, set up a Rule to only allow connections from internal IP ranges within the Private Subnet, completely blocking direct access from the Internet. | 05/14/2026 | 05/14/2026 | AWS Security Best Practices |
| 5 | Research advanced RDS architecture: Understand how the Multi-AZ (High Availability) redundancy mechanism works and how to scale read capacity with Read Replicas. | 05/15/2026 | 05/15/2026 | Amazon RDS Architecture Documentation |

### Achievements of the week:

*   **Systems Thinking:** Master the principles of secure network design on the Cloud, knowing how to segregate resources into Subnets with different security levels.
*   **Database Administration:** Successfully initialize and verify the operational status of a MySQL Database server on Amazon RDS in a test Lab environment.
*   **Infrastructure Security:** Successfully establish the Security Group firewall layer (Inbound/Outbound Rules) to completely isolate the Database, protecting data against cyber attack risks.