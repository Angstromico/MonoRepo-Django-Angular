# Full-Stack Django & Angular HR Management Project

This project implements an Employee Management system with a Django REST Framework backend, an Angular frontend, and a PostgreSQL database.

## Project Structure
- `backend/`: Django REST Framework project.
- `frontend/`: Angular standalone application.
- `docker-compose.yml`: Infrastructure for the PostgreSQL database.

## Prerequisites
- Python 3.10+
- Node.js & npm (Latest LTS)
- Docker & Docker Compose

---

## Getting Started

### 1. Start the Database
The project uses PostgreSQL running in a Docker container.
```bash
# From the project root
docker-compose up -d
```
*The database will be available on `localhost:5432` with credentials defined in `docker-compose.yml`.*

### 2. Start the Backend (Django)
1.  **Activate the Virtual Environment**:
    ```bash
    # Windows
    .\venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```
2.  **Run Migrations**:
    ```bash
    cd backend
    python manage.py migrate
    ```
3.  **Start the Server**:
    ```bash
    python manage.py runserver 8080
    ```
*The API will be available at `http://localhost:8080/api/employees`.*

### 3. Start the Frontend (Angular)
1.  **Install Dependencies** (First time only):
    ```bash
    cd frontend
    npm install
    ```
2.  **Start the Development Server**:
    ```bash
    npm start
    ```
*The application will be available at `http://localhost:4200`.*

---

## API Endpoints
- `GET /api/employees`: List all employees.
- `POST /api/employees`: Create a new employee.
- `GET /api/employees/<id>`: Retrieve an employee.
- `PUT /api/employees/<id>`: Update an employee.
- `DELETE /api/employees/<id>`: Delete an employee.
