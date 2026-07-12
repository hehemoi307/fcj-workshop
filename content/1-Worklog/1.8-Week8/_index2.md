---
title: "Worklog - Week 8"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:
* Complete the optimization and packaging of the Pet Resort project's ReactJS source code into static assets for the Production environment.
* Research and analyze Frontend deployment solutions on AWS: Using a fully managed service (AWS Amplify) vs. Building native infrastructure (Amazon S3 combined with CloudFront).
* Unify the roadmap with the team and mentor: Pivot to manually configuring S3 and CloudFront to practice advanced network and storage administration skills.

### Tasks completed during the week:
| Day | Detailed Tasks | Start Date | End Date | References |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Pause new UI development, learn the optimization process (Minify/Uglify) and compile ReactJS source code.<br>- Read documentation on the static build mechanism to prepare for cloud deployment. | 06/08/2026 | 06/08/2026 | React Deployment Guide |
| 2 | - Practice running the `npm run build` command in the VS Code Terminal to compile the Pet Resort Frontend project into the `build` folder.<br>- Analyze and resolve warnings regarding large Chunk sizes to optimize load speed. | 06/09/2026 | 06/09/2026 | Webpack & NPM Docs |
| 3 | - Install the `serve` library package to independently test the `build` folder in the localhost environment.<br>- Double-check navigation flows (React Router) to ensure no 404 errors occur when running in Production mode. | 06/10/2026 | 06/10/2026 | React Router Documentation |
| 4 | - Gain a preliminary understanding of **AWS Amplify** — a platform service that fully automates CI/CD, connects to GitHub, and hosts static websites easily with just a few clicks.<br>- Analyze the Trade-off between Amplify (fast, automated) and the S3 + CloudFront model (manual configuration, deep control). | 06/11/2026 | 06/11/2026 | AWS Amplify Hosting Guide |
| 5 | - Consult with the team and mentor on the overall architectural solution. The Backend chose EC2, so the Frontend also decided to choose **S3 + CloudFront** instead of Amplify.<br>- Reason: Manually setting up the Caching mechanism, configuring Bucket Policy security, and requesting SSL/TLS certificates will provide much more solid infrastructure knowledge. | 06/12/2026 | 06/12/2026 | AWS CloudFront Best Practices |

### Achievements of the week:

* **Master the Frontend packaging process (Static Build & Optimization):**
  * Clearly understand the difference between the `development` environment (running via dev-server with Hot Reload) and the `production` environment (HTML, CSS, JS files have been compressed and minified).
  * Successfully handle the packaging of the ReactJS project and confirm the static source code works perfectly without Routing errors when running independently.

* **Form an architecture evaluation mindset (Architecture Evaluation):**
  * Grasp the pros and cons of Hosting solutions on AWS for the Frontend (Amplify vs S3 + CDN).
  * Know how to ask evaluation questions: Between deploying quickly to meet the deadline and configuring manually to deeply understand the nature of the system, what is more important for the internship goals?

* **Clearly define the infrastructure deployment roadmap for the sprint phase:**
  * Synchronize the direction with the whole team: Accept the "harder" path of manually setting up Amazon S3 combined with the CloudFront content delivery network. This choice requires a lot of effort in configuring permissions and caching but perfectly meets the program's goal of accumulating in-depth practical experience.