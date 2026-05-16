# Customer Incident Command Center

Backend service for managing and tracking customer support incidents.

Built with Spring Boot and PostgreSQL, containerized via Docker for local development consistency.

---

## Tech Stack

- Java
- Spring Boot
- PostgreSQL
- Docker / Docker Compose

---

## Project Structure

- `src/` — Spring Boot application
- `docker-compose.yml` — PostgreSQL container configuration
- `.env.example` — Environment variable template
- `.env` — Local environment configuration (not committed)

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/joel-jude/customer-incident-command-center.git
cd customer-incident-command-center
```

### 2. Create environment variables

```bash
cp .env.example .env
```

Edit .env if needed:

```env
POSTGRES_USER=incident_user
POSTGRES_PASSWORD=dev_password
POSTGRES_DB=incident_db
```

### 3. Start PostgreSQL with Docker

```bash
docker compose up -d
```

Database will be available at:
localhost:5432
