---
title: "Worklog - Week 10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:
* Coordinate with the team to sketch the Architecture Diagram, taking primary responsibility for designing the Edge & Delivery layer for the Frontend.
* Research the AWS Well-Architected Framework standard to optimize the static delivery flow design and CI/CD integration.
* Review and merge the Frontend component diagram with the team's Backend VPC infrastructure, ensuring feasibility and alignment with the actual source code.

### Tasks completed during the week:
| Day | Detailed Tasks | Start Date | End Date | References |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 1 | - Analyze the data flow from the End-user perspective to sketch the Frontend layer.<br>- Use Draw.io to draft components: Route 53, CloudFront, S3 (Frontend), and S3 (Media). | 06/22/2026 | 06/22/2026 | AWS Architecture Icon Set |
| 2 | - Research the AWS Well-Architected Framework documentation (focusing on Performance Efficiency and Security pillars).<br>- Apply theory to check if the current CDN design optimizes speed and security. | 06/23/2026 | 06/23/2026 | AWS Well-Architected Framework |
| 3 | - Discuss diagram integration: Map the API call flow from CloudFront (Frontend) through the Internet Gateway to the team's Application Load Balancer / EC2 (Backend).<br>- Check the logic of routing arrows. | 06/24/2026 | 06/24/2026 | Team System Block Diagram |
| 4 | - Add the Continuous Integration/Continuous Deployment (CI/CD) flow to the diagram: Visualize the GitHub Actions process of automatically building ReactJS source code and syncing static files to Amazon S3. | 06/25/2026 | 06/25/2026 | CI/CD Architecture Patterns |
| 5 | - Finalize and standardize the Architecture Blueprint interface with the team.<br>- Write documentation explaining the function of each block in the Edge layer in detail and update progress to Hugo. | 06/26/2026 | 06/26/2026 | |

### Achievements of the week:

#### A. Design and standardize Edge & Delivery Architecture
* **Visualize Frontend and CI/CD flow:**
  * Successfully drew the optimal access flow for customers: User -> Route 53 (DNS) -> CloudFront (CDN Caching) -> S3 Bucket (ReactJS).
  * Included the automation process in the architecture diagram: Clearly presented the GitHub Actions step executing `npm build` and automatically deploying to the storage infrastructure, accurately reflecting the team's actual workflow.
* **Cross-layer Integration:**
  * Successfully merged the Frontend layer with the Backend VPC network of other members. Clearly identified Endpoints and the direction of data arrows from the Client calling the API through the Load Balancer into the Private Subnet logically.

#### B. Well-Architected Alignment
* **Optimize performance and security:**
  * Instead of just referring to community templates, proactively applied the pillars of the AWS Well-Architected Framework to the design.
  * Ensured CloudFront acts as a shield (Edge Security), forcing access via HTTPS and protecting the S3 Bucket from unauthorized direct access through Origin Access Control (OAC).

#### C. Practical Deployment Focus
* **Eliminate complexity, focus on feasibility:**
  * Agreed with the team to eliminate the idea of drawing Serverless services (like AWS Lambda) to process uploaded images. Decided to apply the method of storing pet image files directly to the S3 Media Bucket via Pre-signed URLs from the Backend.
  * This decision helps the architecture diagram closely follow the actual coding capabilities, keeping the system simple, easy to operate, and defensible before the Mentor panel.