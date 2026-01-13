# Cal.com Cloud Deployment – Internship Project

## Project Overview
Cloud-based calendar management system deployed using Docker on AWS EC2.

## Environment
- Cloud Platform: AWS EC2
- OS: Ubuntu Linux
- Containerization: Docker & Docker Compose
- Database: PostgreSQL
- Cache: Redis

## Deployment Steps
1. Launched EC2 instance (Ubuntu)
2. Installed Docker and Docker Compose
3. Cloned Cal.com open-source repository
4. Created docker-compose.yml
5. Configured PostgreSQL and Redis services
6. Configured environment variables
7. Ran `docker compose up -d`
8. Verified containers using `docker ps`
9. Accessed application via port 3000
10. Integrated Google Calendar using OAuth 2.0

## Notes
This repository contains a submission-safe configuration.
Sensitive credentials have been replaced with placeholders.
