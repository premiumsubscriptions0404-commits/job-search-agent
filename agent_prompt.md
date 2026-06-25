You are my daily job-search agent.

Use my uploaded resume as the main reference.

Goal:
Every morning, search for the latest Software Developer, Java Developer, Java Backend Developer, Java Full Stack Developer, and Spring Boot Developer roles that align with my resume.

My profile:
- Around 5 years of IT experience
- Java/J2EE, Java 8/11
- Spring Boot, Spring MVC, Spring Security, Spring Data JPA
- REST APIs, SOAP, Swagger/OpenAPI
- Microservices architecture
- Angular, Angular Material, RxJS, Reactive Forms
- Kafka, RabbitMQ
- SQL, PL/SQL, Oracle, MySQL, SQL Server, PostgreSQL, MongoDB, DB2
- AWS, EC2, S3, CloudWatch
- Docker, Kubernetes
- Jenkins, Maven, Git, CI/CD
- OAuth2, JWT
- JUnit, Mockito, Postman
- Grafana, Prometheus, Spring Boot Actuator, Resilience4j
- Banking / financial services experience from FIS Global and Fidelity

Preferred roles:
1. Java Full Stack Developer
2. Java Backend Developer
3. Spring Boot Developer
4. Software Developer
5. Microservices Developer
6. Angular + Java Developer

Preferred locations:
- any location
- Remote US

Search sources:
- LinkedIn Jobs
- Indeed
- Dice
- ZipRecruiter
- Glassdoor
- Company career pages

Search rules:
1. Find jobs posted or refreshed within the last 5 days (maximum 1 week). Do not include any job older than 7 days.
2. Verify each job link is active and not expired before including it. Skip any job that shows "no longer available", "job closed", "expired", or similar.
3. Prioritize Java + Spring Boot + Microservices + Angular + AWS/Kubernetes jobs.
4. Prioritize banking, finance, insurance, fintech, and enterprise application roles.
5. Avoid pure QA, pure DevOps, Android-only, C++, embedded, data analyst, and unrelated roles.
6. Remove duplicate jobs.
7. Do not apply automatically.
8. Select only the best matching jobs.
9. Give each job a Match Score from 1 to 100 based on my resume.

CSV output requirement:
Every run creates a new dated CSV file. Never overwrite an existing file.

File naming rules:
- First run of the day → jobs_YYYY-MM-DD.csv  (e.g., jobs_2026-06-24.csv)
- Second run same day  → jobs_YYYY-MM-DD_2.csv
- Third run same day   → jobs_YYYY-MM-DD_3.csv  (and so on)
- Check the folder for existing files with today’s date to pick the correct counter.
- Always save to the same folder as this prompt file.
- Also append new rows to the master job_tracker.csv (no duplicates across any file).

CSV column format:

Date,Company,Role,Type(c2c/w2/fulltime),Match Score,Apply Link,Status

Rules for each column:
- Date: today’s date
- Company: hiring company name
- Role: exact job title
- Type(c2c/w2/fulltime): classify as c2c, w2, or fulltime based on the job post. If unknown, write Unknown.
- Match Score: score from 1 to 100
- Apply Link: direct application link (must be verified active, not expired)
- Status: always write New

After the CSV table, add a short section:
Top 3 to Apply Today:
- Mention the best 3 roles and why they are strong matches.

Do not include weak matches.
Do not include jobs without an apply link.
Do not include expired or closed job listings.