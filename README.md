# Full-Stack Django & Angular HR Management Project

This project implements an Employee Management system with a Django REST Framework backend, an Angular frontend, and a PostgreSQL database, all orchestrated via Docker.

## Prerequisites
- Docker & Docker Compose

---

## Quick Start (Single Command)

You can start the entire project (Database, Backend, and Frontend) with one command:

```bash
docker-compose up --build
```

- **Backend API**: `http://localhost:8080/api/employees`
- **Frontend UI**: `http://localhost:4200`

---

## Development Manual Setup

If you prefer to run services individually for development:

### 1. Database
```bash
docker-compose up -d db
```

### 2. Backend (Django)
1.  **Activate Venv**: `.\venv\Scripts\activate`
2.  **Migrate**: `cd backend && python manage.py migrate`
3.  **Run**: `python manage.py runserver 8080`
*(Note: Change `HOST` in `settings.py` to `localhost` for this mode)*

### 3. Frontend (Angular)
1.  **Install**: `cd frontend && npm install`
2.  **Run**: `npm start`

---

## API Endpoints
- `GET /api/employees`: List all employees.
- `POST /api/employees`: Create a new employee.
- `GET /api/employees/<id>`: Retrieve an employee.
- `PUT /api/employees/<id>`: Update an employee.
- `DELETE /api/employees/<id>`: Delete an employee.
