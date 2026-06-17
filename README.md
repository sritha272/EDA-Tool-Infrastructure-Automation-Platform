# EDA-Tool-Infrastructure-Automation-Platform
Full-stack platform automating EDA tool configuration, execution, and monitoring — React, FastAPI, PostgreSQL, Docker, CI/CD on Linux. 88% reliability, 80% reduction in manual processing.

- **Frontend (React):** Configuration forms, job launch controls, real-time status monitoring, and historical job browsing
- **Backend (FastAPI):** Async request handling, parameter validation, job orchestration, REST API layer
- **Database (PostgreSQL):** Job definitions, configurations (stored as structured JSON), execution history, logs, and user data
- **Tool Execution Layer (Python/C++):** Orchestration scripts in Python; performance-critical parsing of large tool output files in C++
- **CI/CD (Jenkins + GitHub Actions):** Automated build, test, and deployment pipeline for the platform itself
- **Containerization (Docker):** Consistent deployment across environments

## Key Features

- Web-based job configuration with schema-driven dynamic forms
- Real-time log streaming via Server-Sent Events
- Full job history with searchable, filterable past runs
- Role-based access control with JWT authentication
- Automated input validation against tool parameter schemas

## Results

- **88%** automated test pass rate / overall execution reliability
- **80%** reduction in manual processing compared to CLI-based workflows
- **Sub-2-second** response latency for all interactive operations

## Tech Stack

`Python` `C++` `React` `FastAPI` `PostgreSQL` `Docker` `Jenkins` `GitHub Actions` `Linux`

## Testing

- Unit tests: `pytest` (Python), `Google Test` (C++)
- Integration tests against a containerized test database
- End-to-end tests simulating full user workflows

## Setup

```bash
# Clone the repo
git clone https://github.com/yourusername/eda-automation-platform.git
cd eda-automation-platform

# Backend
cd backend
pip install -r requirements.txt --break-system-packages
uvicorn main:app --reload

# Frontend
cd frontend
npm install
npm start

# Run with Docker Compose
docker-compose up --build
```

## License

MIT
