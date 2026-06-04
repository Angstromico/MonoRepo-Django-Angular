# Full-Stack Django & Angular HR Management Project

This project provides a comprehensive prompt designed to generate a complete Full-Stack application for Human Resources management. It leverages **Django REST Framework** for the backend and **Angular** for the frontend.

## Project Overview

The generated application consists of:
- **Backend**: A robust REST API built with Django, using **PostgreSQL** as the primary database running inside a **Docker** container. It includes CORS configuration to allow seamless communication with the frontend.
- **Frontend**: A modern, responsive web interface built with Angular (using standalone components) that allows users to perform CRUD (Create, Read, Update, Delete) operations on employee records.

## Key Features
- **Employee CRUD**: Manage employee data including name, department, and salary.
- **Containerized Database**: Uses Docker Compose to easily spin up a PostgreSQL instance.
- **CORS Support**: Pre-configured to handle cross-origin requests between the Angular dev server (port 4200) and the Django server (port 8080).
- **Pedagogical Approach**: The prompt generates a guide that explains every step, making it ideal for learning or rapid prototyping.

## How to Use the Prompt
1. Copy the content of `prompt_django_rest.txt`.
2. Paste it into your preferred LLM (like Gemini, ChatGPT, or Claude).
3. Follow the generated step-by-step guide to build your application.

## Prerequisites
- **Python 3.x**
- **Node.js & Angular CLI**
- **Docker & Docker Compose**
- **Postman** (for API testing)

## Infrastructure (Docker)
The prompt includes the creation of a `docker-compose.yml` file to run PostgreSQL:
- **Image**: `postgres:latest`
- **Database Name**: `hr_db`
- **User**: `postgres`
- **Password**: `postgres`
- **Port**: `5432`
