---
title: "Worklog - Week 9"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:
* Optimize page load performance (Performance Tuning) and secure environment configurations for the ReactJS Frontend source code.
* Deeply research the caching mechanism of Amazon CloudFront and static resource monitoring tools.
* Test and handle exception scenarios (Edge Cases) on the user interface (UI/UX) in the local environment before deploying to the Cloud.

### Tasks completed during the week:
| Day | Detailed Tasks | Start Date | End Date | References |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Review and optimize ReactJS source code.<br>- Implement Code Splitting and Lazy Loading techniques to reduce static bundle size, helping accelerate the First Contentful Paint. | 06/15/2026 | 06/15/2026 | React Performance Optimization |
| 2 | - Deep dive into **Amazon CloudFront** theory.<br>- Study concepts like Time-to-Live (TTL), Cache Policies, and the Cache Invalidation mechanism when updating new website versions. | 06/16/2026 | 06/16/2026 | Amazon CloudFront Documentation |
| 3 | - Secure Frontend source code: Separate configurations such as the API Base URL and third-party service Public Keys from the pure source code.<br>- Configure using Environment Variables via the `.env` file. | 06/17/2026 | 06/17/2026 | React Environment Variables |
| 4 | - Learn how to monitor the Frontend via **Amazon CloudWatch**.<br>- Learn to analyze S3 and CloudFront metrics (like Cache Hit/Miss Rate, bandwidth consumption, 4xx/5xx error rates). | 06/18/2026 | 06/18/2026 | AWS CloudWatch Metrics |
| 5 | - Perform testing for local Error Scenarios on the UI: Simulate network disconnection, non-responsive Backend API, or expired JWT Token returns.<br>- Configure `Axios Interceptors` to intercept and handle errors centrally. | 06/19/2026 | 06/19/2026 | Guide to Axios Error Handling |

### Achievements of the week:

* **Optimize code and Frontend performance (Frontend Performance Tuning):**
  * Significantly reduced the JavaScript payload downloaded on the first visit by applying Lazy Loading for components that are not immediately visible, making the Pet Resort website load smoother.
  * Implemented configuration protection solutions: Completely eliminated hardcoding Backend API URLs into the source code. Switched the structure to dynamic loading via the `.env` file, ensuring absolute safety when pushing code to the GitHub repository.

* **Master the content delivery network mechanism (CDN Caching & Monitoring):**
  * Clearly understood how CloudFront caches data at Edge Locations. Know how to execute Invalidation to clear old cache, forcing the CDN to update to the latest website content immediately.
  * Recognized key metrics (Cache Hit Rate, Error Rate) on CloudWatch to monitor the health of the static content delivery system after going live.

* **Perfect user experience in error scenarios (Robust UI Error Handling):**
  * Upgraded the Frontend error handling flow with `Axios Interceptors`: When the system receives a 401 (Unauthorized) error code due to an expired JWT, the Frontend smoothly redirects users to the `LoginPage` automatically, instead of displaying a white screen.
  * Successfully built friendly Fallback UI / Error Boundaries screens, helping retain customers when the Backend suddenly crashes.

* **Prepare deployment documentation:**
  * Compiled a list of all required Environment Variables on the Frontend side to prepare for the automated injection into the CI/CD pipeline (GitHub Actions) in the upcoming phases.