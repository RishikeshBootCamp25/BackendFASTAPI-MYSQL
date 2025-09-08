# Backend development with FASTAPI-MYSQL
This project serves as an introductory backend application built with FastAPI, SQLAlchemy, and MySQL. It provides a simple API that can be tested through Swagger UI and managed using MySQL Workbench.

---

## Features
- REST API built with **FastAPI**
- Database connection using **SQLAlchemy ORM**
- Data storage and queries in **MySQL**
- Interactive API docs with **Swagger UI**
- Type safety and validation using **Pydantic BaseModel**
- Beginner-friendly project structure
- Easy to extend for personal projects or portfolios

---

## Project Structure
fastapi/project/backend_fastapi_mysql/

- app/

- main.py # Entry point for FastAPI app

- database.py # MySQL connection setup

- models.py # SQLAlchemy models

- schemas.py # Pydantic BaseModels

- crud.py # Database operations

- routers/ # API route handlers

- requirements.txt # Project dependencies

- .env.example # Environment variables (DB credentials)

- README.md # Project documentation

---

**Setup and Usage**
## Clone the repository
git clone https://github.com/YourUsername/FastAPI-MySQL.git

cd FastAPI-MySQL

---

## Create a virtual environment and install packages
python -m venv venv

source venv/bin/activate   # (Linux/Mac)

venv\Scripts\activate      # (Windows)

pip install -r requirements.txt

This keeps your project’s Python libraries separate and avoids version conflicts.

---

## Add your database settings
Create a .env file (copy from .env.example) and update with your MySQL details:
DATABASE_URL=mysql+mysqlconnector://username:password@localhost:3306/db_name

This keeps your DB password and secrets safe (not inside the code).

---

## Start the FastAPI server
uvicorn main:app --reload

This will start your backend at http://127.0.0.1:8000/.

---

## Test the API

Open in your browser:

1. Swagger UI: http://127.0.0.1:8000/docs

2. ReDoc: http://127.0.0.1:8000/redoc

Swagger UI is auto-generated and lets you test your endpoints without Postman.

