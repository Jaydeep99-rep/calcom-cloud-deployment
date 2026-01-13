# Cloud-Based Calendar Management System (Cal.com Deployment)

## Project Overview
This project involves deploying an open-source calendar management system (Cal.com) on the cloud to help professionals manage meetings efficiently across multiple platforms. The solution enables centralized scheduling, calendar synchronization, and automated meeting bookings.

The application was deployed using containerization to ensure scalability, reliability, and ease of maintenance.

---

## Domain
Cloud Computing / DevOps

---

## Technology Stack

| Component              | Technology Used |
|-----------------------|-----------------|
| Cloud Platform        | AWS EC2 |
| Operating System      | Ubuntu Linux |
| Containerization      | Docker |
| Orchestration         | Docker Compose |
| Application           | Cal.com (Open Source) |
| Database              | PostgreSQL |
| Cache                 | Redis |
| Version Control       | Git & GitHub |
| Calendar Integration  | Google Calendar (OAuth 2.0) |

---

## Architecture Overview
The system follows a container-based architecture where each service runs independently and communicates over a Docker network.

**High-level flow:**
- User accesses the application via a web browser
- Requests are handled by the Cal.com web application
- Persistent data is stored in PostgreSQL
- Redis is used for caching and session management
- Google Calendar API is used for calendar synchronization

---

## Deployment Environment
- AWS EC2 (Free Tier)
- Ubuntu Linux
- Docker Engine
- Docker Compose

---

## Project Structure

---

## Deployment Steps

1. Launch an Ubuntu EC2 instance on AWS  
2. Install Docker and Docker Compose  
3. Clone the Cal.com repository  
4. Create and configure `docker-compose.yml`  
5. Configure environment variables in `.env`  
6. Pull official Cal.com Docker images  
7. Start services using Docker Compose  
8. Verify container health and application availability  
9. Integrate Google Calendar using OAuth 2.0  

---

## Key Docker Services

### Cal.com Application
- Runs as a Docker container
- Exposed on port `3000`
- Handles scheduling, bookings, and integrations

### PostgreSQL Database
- Stores user data, events, and availability
- Uses Docker volumes for persistence

### Redis Cache
- Improves performance
- Manages sessions and frequently accessed data

---

## Verification
- Containers verified using `docker compose ps`
- Logs checked using `docker compose logs`
- Application accessible at `http://<EC2-Public-IP>:3000`
- Login and scheduling functionality tested successfully

---

## Security Considerations
- Environment variables used for credentials
- No secrets committed to GitHub
- OAuth authentication used for Google Calendar integration

---

## Learning Outcomes
- Practical experience with cloud deployment
- Hands-on Docker and Docker Compose usage
- Understanding of containerized architectures
- OAuth-based API integration
- Debugging and log analysis in production environments

---

## Author
**Jaydeep Barot**  
Cloud Computing Intern  

---

## Disclaimer
This project was developed as part of an internship assignment for educational purposes. All sensitive credentials have been removed or replaced with placeholders.

