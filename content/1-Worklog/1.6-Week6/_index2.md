---
title: "Worklog - Week 6"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:
- Be present at the office to participate in self-study days, synchronize progress, and solve architectural problems with team members.
- Review and consolidate the foundation of 4 AWS core service pillars (Compute, Network, Storage, Security).
- Deep dive into solutions for accelerating page load speed and distributing static content globally.

| Day | Tasks & Completed Assignments | Start Date | End Date | References |
|:---:|:---|:---:|:---:|:---|
| 1 | Self-study at the office: Review the IAM authorization system. Focus on writing Custom Policies to grant secure access to static resources. | 05/25/2026 | 05/25/2026 | AWS IAM Documentation |
| 2 | Deep review of Amazon S3: Carefully study the CORS (Cross-Origin Resource Sharing) mechanism and security risks when opening a Public Bucket to host a website. | 05/26/2026 | 05/26/2026 | Amazon S3 Guide |
| 3 | Participate in a network architecture discussion with the team: Understand the data flow from Frontend (Public access) calling to Backend (hidden in VPC/Private Subnet). | 05/27/2026 | 05/27/2026 | |
| 4 | Research content delivery solutions: Read documentation on Amazon CloudFront (CDN), analyze the advantages of combining S3 and CloudFront (Cache speed, SSL/HTTPS support). | 05/28/2026 | 05/28/2026 | AWS CloudFront Blog |
| 5 | Package self-study content. Note down some questions about the CDN Cache Invalidation mechanism to ask for the Mentor's advice. Update worklog to Hugo. | 05/29/2026 | 05/29/2026 | |

### Achievements of the week:

*   **Foundation Consolidation:** Complete and package all foundational knowledge about AWS core services, becoming more confident in selecting services for system design.
*   **Finalize Frontend Plan:** Clearly define the interface deployment strategy: Not only stop at normal S3 Static Hosting but also integrate CloudFront CDN to ensure fast website loading and HTTPS security certificates.
*   **Working Skills:** Maintain effective self-study discipline at the office, interact with and support other team members to clarify the overall architectural picture.