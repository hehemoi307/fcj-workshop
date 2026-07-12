---
title: "Worklog - Week 7"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:
* Optimize workflow: Transition from using the web interface (AWS Console) to managing cloud resources directly in Visual Studio Code (VS Code).
* Deep dive into AWS system monitoring and Observability tools.
* Manage sensitive information security (passwords, connection strings) using secret management services.

### Tasks completed during the week:
| Day | Tasks & Completed Assignments | Start Date | End Date | References |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Install AWS CLI and AWS Toolkit extension on Visual Studio Code.<br>- Practice authentication (AWS Configure) and manage basic resources (like S3, EC2) directly from the UI and integrated Terminal of VS Code. | 06/01/2026 | 06/01/2026 | AWS Toolkit for VS Code |
| 2 | - Research Amazon CloudWatch service: Understand concepts of Metrics, Logs, and Alarms.<br>- Practice creating a CloudWatch Alarm to automatically send an email when the virtual server's CPU exceeds the allowed threshold. | 06/02/2026 | 06/02/2026 | Amazon CloudWatch Docs |
| 3 | - Distinguish between CloudWatch and AWS CloudTrail.<br>- Enable CloudTrail to record the entire history of API calls. Practice downloading JSON-formatted log files to VS Code to read, understand, and analyze the trace structure. | 06/03/2026 | 06/03/2026 | AWS CloudTrail User Guide |
| 4 | - Research AWS Secrets Manager and AWS Systems Manager (Parameter Store) services.<br>- Practice lab on securely storing sensitive information (like Database passwords) instead of hardcoding directly into the source code. | 06/04/2026 | 06/04/2026 | AWS Secrets Manager Docs |
| 5 | - Package knowledge and write a short blog summarizing the differences between CloudWatch and CloudTrail.<br>- Update the weekly worklog content to the local Hugo system using VS Code. | 06/05/2026 | 06/05/2026 | |

### Achievements of the week:

* **Optimize Working Environment:** Successfully integrate the AWS environment directly into the VS Code source code editor. Using AWS CLI and AWS Toolkit makes creating, editing, and deleting resources much faster and more professional compared to clicking on the web interface.
* **Observability Mindset:**
  * Clearly understand how to monitor system performance and health through CloudWatch charts.
  * Successfully establish a security tracking mechanism with CloudTrail, practicing the skill of reading complexly structured JSON log files.
* **Application Data Security:** Master the method of safely managing environment variables and Database connection strings via Secrets Manager, completely eliminating the risk of exposing passwords in the source code.