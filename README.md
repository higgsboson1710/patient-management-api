# 🏥 Patient Management API

A clean and RESTful backend API built using **FastAPI** and **Pydantic v2** to manage patient records efficiently.

---

## 🚀 Features
- ➕ Create, 📄 Read, ✏️ Update, ❌ Delete patients
- ✅ Strong request validation using Pydantic
- 📊 Computed fields: **BMI** and health **verdict**
- 🔍 Sorting via query parameters
- ⚠️ Proper HTTP status codes & error handling
- 🗂️ JSON-based persistence (prototype stage)

---

## 🛠️ Tech Stack
- 🐍 Python
- ⚡ FastAPI
- 🧩 Pydantic v2
- 🚀 Uvicorn

---

## 🔗 API Endpoints

| Method | Endpoint | Description |
|------|---------|------------|
| GET | `/patients` | Get all patients |
| GET | `/patients/{id}` | Get patient by ID |
| POST | `/patients` | Create a new patient |
| PUT | `/patients/{id}` | Update patient |
| DELETE | `/patients/{id}` | Delete patient |
| GET | `/sort?sort_by=bmi&order=asc` | Sort patients |

---

## ▶️ How to Run Locally

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload
