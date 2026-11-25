Hi, I'm Tanmay Kumar

Backend software engineer in Bengaluru. I build APIs, data pipelines and event-driven systems in Java, Python and Node.js, mostly on PostgreSQL, Kafka and AWS.

2 years as a Software Engineer at Pretium (U.S. single-family rental platform), after a year as an analyst at Bayer
AWS Certified Solutions Architect – Associate (verify on Credly)
Open to backend and full-stack SDE roles · Bengaluru or remote
Projects

##log-aggregator · Java 21, Kafka, Kafka Streams, Kafka Connect, Avro, PostgreSQL, Docker Compose

A log pipeline built from scratch and run locally with Docker Compose:

Shipper: tails rotating log files and publishes Avro events through Schema Registry with an idempotent producer
Stream processor (Kafka Streams): parses, enriches, filters and samples events; unparseable lines go to a dead-letter topic
Sinks (Kafka Connect): OpenSearch, S3 (MinIO), and a PostgreSQL sink connector I wrote myself. It is idempotent (keyed on topic, partition and offset), writes each batch in one transaction, and retries transient failures with backoff.
Monitoring: Prometheus and Grafana, with a consumer-lag alert
Quality: 70+ JUnit, Mockito and Testcontainers tests, run in GitHub Actions CI

##release-notes-simplified · Node.js, Express, PostgreSQL (Neon), Prisma, VS Code extension

A VS Code extension that shows Java release notes in plain English:

An Express API, deployed on Railway, scrapes and parses JDK release notes, stores them in PostgreSQL, and uses an LLM to summarise them.
A GitHub Actions cron job refreshes the data daily through a secret-authenticated endpoint.
At work
Request-tracking APIs and notifications (Java, Spring) for a resident app used by 250k+ residents
Yardi-integrated rent-readiness pipeline that cut time-to-lease by 5–7 days
Nightly reconciliation job that keeps Yardi and the internal PostgreSQL database in sync
LLM lease-extraction pipeline (Python) that turns lease PDFs into validated, structured data
Tech

Languages: Java, Python, JavaScript, SQL
Backend & streaming: Spring, Node.js, Express, REST APIs, Kafka, Kafka Streams, Kafka Connect, Avro
Data: PostgreSQL, MySQL, Redis, OpenSearch, BigQuery
Cloud & tooling: AWS, GCP, Docker, GitHub Actions, Prometheus, Grafana, Git

LinkedIn · tanmaykumar971@gmail.com
