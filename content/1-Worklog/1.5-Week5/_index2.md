---
title: "Worklog - Week 5"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:
- Research core Compute Services on the AWS platform.
- Learn how to apply virtual servers (Amazon EC2) and serverless architecture (AWS Lambda) in modern web models.
- Practice evaluating trade-offs of compute services to propose optimal deployment solutions.

| Day | Tasks & Completed Assignments | Start Date | End Date | References |
|:---:|:---|:---:|:---:|:---|
| 1 | Research Amazon EC2 in detail: Learn about Amazon Machine Image (AMI), Instance Types, and how to use EC2 User Data to automate environment setup upon launch. | 05/18/2026 | 05/18/2026 | Amazon EC2 Documentation |
| 2 | Approach the Serverless model: Learn the concept of Function-as-a-Service (FaaS) and the event-driven processing mechanism of AWS Lambda. | 05/19/2026 | 05/19/2026 | AWS Lambda Documentation |
| 3 | Application theory analysis: Compare IaaS (EC2) and FaaS (Lambda) models in terms of Operational Overhead, automatic Scaling mechanisms, and cost factors. | 05/20/2026 | 05/20/2026 | AWS Compute Blog |
| 4 | Research Architecture Patterns: Evaluate how to combine AWS Lambda with Amazon S3 (e.g., using Lambda to automatically process images when a new file is uploaded to an S3 Bucket). | 05/21/2026 | 05/21/2026 | AWS Event Triggers Lab Data |
| 5 | Synthesize system analysis knowledge learned during the week, compile documentation, and update progress to the local Hugo report page. | 05/22/2026 | 05/22/2026 | |

### Achievements of the week:

*   **Compute Architecture:** Clearly distinguish the difference between provisioning and maintaining a virtual server (EC2) versus executing code on demand without managing servers (Lambda).
*   **Automation Mindset:** Grasp how to use EC2 User Data for startup environment setup and the idea of using S3 Triggers to invoke Lambda, making system operations more flexible.
*   **Solution Analysis:** Accumulate the ability to identify suitable Use Cases for each type of compute service, setting the premise for the upcoming Architecture Proposal phase.