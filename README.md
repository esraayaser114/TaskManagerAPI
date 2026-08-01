# 📝 Task Manager API

A simple RESTful Task Manager API built with **FastAPI**, **SQLAlchemy**, and **SQLite**.  
This project demonstrates the implementation of CRUD (Create, Read, Update, Delete) operations for managing daily tasks.

---

# 🚀 Features

- Create a new task
- Retrieve all tasks
- Retrieve a task by its ID
- Update an existing task
- Delete a task
- Automatic task creation timestamp
- Input validation using Pydantic
- Error handling with proper HTTP status codes
- Interactive API documentation with Swagger UI

---

# 🛠 Technologies Used

- Python 3.10
- FastAPI
- SQLAlchemy
- SQLite
- Uvicorn
- Pydantic

---

# 📂 Project Structure

```
TaskManagerAPI/
│
├── app/
│   ├── main.py          # API routes
│   ├── models.py        # Database models
│   ├── schemas.py       # Request & response schemas
│   ├── crud.py          # CRUD operations
│   ├── database.py      # Database configuration
│   └── __init__.py
│
├── tasks.db             # SQLite database
├── requirements.txt
├── README.md
└── .gitignore
```

---

# ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/TaskManagerAPI.git
```

### 2. Navigate to the project

```bash
cd TaskManagerAPI
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Application

Start the FastAPI server using:

```bash
uvicorn app.main:app --reload
```

The application will be available at:

```
http://127.0.0.1:8000
```

---

# 📖 API Documentation

Swagger UI:

```
http://127.0.0.1:8000/docs
```

ReDoc:

```
http://127.0.0.1:8000/redoc
```

---

# 📌 API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/tasks` | Create a new task |
| GET | `/tasks` | Retrieve all tasks |
| GET | `/tasks/{id}` | Retrieve a task by ID |
| PUT | `/tasks/{id}` | Update an existing task |
| DELETE | `/tasks/{id}` | Delete a task |

---

# 📋 Task Model

```json
{
  "id": 1,
  "title": "Study FastAPI",
  "description": "Complete CRUD assignment",
  "status": "pending",
  "created_at": "2026-08-01T22:08:48"
}
```

---

# ✅ HTTP Status Codes

| Code | Description |
|------|-------------|
| 200 | Successful request |
| 201 | Task created successfully |
| 404 | Task not found |
| 422 | Validation error |

---

# 🧪 Testing

The API was tested successfully using:

- FastAPI Swagger UI
- Browser

All CRUD operations were verified successfully.

---

# 👩‍💻 Author

**Esraa Yaser**

GitHub:
https://github.com/esraayaser114