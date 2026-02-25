# project



## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React + TypeScript + FSD |
| Backend | NestJS + Node.js |
| Database | PostgreSQL |
| Cache | Redis |
| Containerization | Docker + Docker Compose |
| CI/CD | GitHub Actions |

## Project Structure

```
project/
├── frontend/          # React + TypeScript + FSD
├── backend/           # NestJS + Node.js
├── docs/              # Documentation & API contracts
│   ├── api/           # OpenAPI specs
│   └── architecture/  # Architecture decisions
├── docker-compose.yml
└── .github/
    └── workflows/     # CI/CD pipelines
```

## Development Workflow

This project follows **GitFlow**:
- `main` — production
- `develop` — integration branch  
- `feature/BE-XXX-name` — backend features
- `feature/FE-XXX-name` — frontend features
- `fix/BE-XXX-name` or `fix/FE-XXX-name` — bug fixes

## Getting Started

```bash
# Clone the repository
git clone https://github.com/Sakradnes/project
cd project

# Start with Docker
docker-compose up -d

# Frontend dev server
cd frontend && npm install && npm run dev

# Backend dev server  
cd backend && npm install && npm run start:dev
```

## Documentation

- API Documentation: Available at `http://localhost:3000/api/docs` (Swagger)
- Frontend Architecture: See `docs/architecture/frontend.md`
- Backend Architecture: See `docs/architecture/backend.md`
