# Patient Management API

A RESTful backend API built using **FastAPI** and **Pydantic v2** to manage patient records.

## Features
- Create, read, update, and delete patients
- Input validation with Pydantic models
- Computed fields (BMI & health verdict)
- Sorting using query parameters
- Proper HTTP status codes & error handling
- JSON-based persistence (learning prototype)

## Tech Stack
- Python
- FastAPI
- Pydantic v2
- Uvicorn

## API Endpoints
- GET /patient/{id}
- GET /view
- POST /create
- PUT /edit/{id}
- DELETE /delete/{id}
- GET /sort?sort_by=bmi&order=asc

## How to Run
```bash
pip install -r requirements.txt
uvicorn app.main:app --reload
