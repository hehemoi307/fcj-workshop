---
title: "Worklog - Week 12"
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:
* Complete the monitoring configuration (Monitoring) and evaluate load capacity (Load Testing) for the entire *Pet Resort & Care System* on the AWS environment.
* Perform review and cost optimization (FinOps) by cleaning up redundant resources.
* Summarize the 12-week internship journey, package technical documentation, and prepare slides and Demo scripts for the project acceptance session.

### Tasks completed during the week:
| Day | Tasks | Start Date | End Date | References |
| :---: | :--- | :---: | :---: | :--- |
| 2 | - End-to-End Testing: Run through all overall test scenarios from start to finish to ensure functional flows (Registration, Booking, Payment) operate seamlessly without abnormal latency. | 07/06/2026 | 07/06/2026 | Team System Test Scenarios |
| 3 | - Monitoring & Alarms: Review the Dashboards on Amazon CloudWatch.<br>- Check the alert flows (Alarms) to ensure the system is always under control in case of incidents. | 07/07/2026 | 07/07/2026 | AWS CloudWatch Docs |
| 4 | - Load/Stress Testing: Coordinate with the team to simulate heavy traffic to test the response capability, architectural stability, and coordination between resources under load. | 07/08/2026 | 07/08/2026 | System Performance Guide |
| 5 | - Resource Optimization (FinOps): Double-check the cost spreadsheet (AWS Billing Console), clean up unused test resources (old snapshots, draft buckets, idle IPs) to ensure team costs do not exceed the budget. | 07/09/2026 | 07/09/2026 | AWS Billing Console |
| 6 | - Finalize Deliverables: Work with the team to finalize the Architecture Blueprint, write the summary report, and rehearse the presentation script (Demo) for the project defense. | 07/10/2026 | 07/10/2026 | Project Documentation |

### Achievements of the week:

* **System Operations (At a basic level):** The *Pet Resort & Care System* can operate stably on the real Cloud environment and smoothly handle core functional flows. However, through load testing, the team identified some bottlenecks that need further architectural optimization to scale up in the future.
* **Monitoring & Cost Optimization:** Successfully established a basic monitoring flow and cleaned up resources effectively, keeping costs at a safe level. Even so, the current logging system is quite fragmented, requiring the integration of a more in-depth centralized log analysis solution for easier debugging.
* **Shortcomings & Lessons Learned:** Concluding the 12-week internship, I realized that the current system is mainly deployed and configured manually. The lack of a fully automated CI/CD (Continuous Integration/Continuous Deployment) pipeline is a weakness that must be addressed to minimize risks when updating new versions.
* **Internship Summary:** Successfully packaged all technical documentation and prepared a confident, open-minded mentality for the project defense. The knowledge acquired during this internship provides a solid launchpad for me to dive deeper into cloud architecture and automation in the future.