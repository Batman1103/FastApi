# 🚀 FastAPI Project

A high-performance REST API built with **FastAPI**, featuring automatic API documentation, data validation, and asynchronous support.

## 📌 Features

- ⚡ Fast and asynchronous API endpoints
- 📖 Automatic API documentation (Swagger UI & ReDoc)
- ✅ Request and response validation using Pydantic
- 🔒 Environment variable support with `.env`
- 🗄️ Database integration (SQLite/PostgreSQL/MySQL)
- 🧪 Easy testing and development setup
- 📦 Modular project structure

---

## 🛠️ Tech Stack

- **Backend:** FastAPI
- **Server:** Uvicorn
- **Validation:** Pydantic
- **Database:** SQLAlchemy
- **Authentication:** JWT (Optional)
- **Environment Management:** Python-dotenv

---

## 📂 Project Structure

```bash
FastAPI-Project/
│
├── app/
│   ├── main.py
│   ├── models/
│   ├── schemas/
│   ├── routes/
│   ├── services/
│   ├── database/
│   └── utils/
│
├── requirements.txt
├── .env
├── .gitignore
├── README.md
└── Dockerfile
```

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Create a Virtual Environment

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux/Mac
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ⚙️ Environment Variables

Create a `.env` file in the root directory.

```env
DATABASE_URL=sqlite:///./test.db
SECRET_KEY=your_secret_key
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30
```

---

## ▶️ Running the Application

```bash
uvicorn app.main:app --reload
```

The server will start at:

```bash
http://127.0.0.1:8000
```

---

## 📚 API Documentation

Swagger UI:

```bash
http://127.0.0.1:8000/docs
```

ReDoc:

```bash
http://127.0.0.1:8000/redoc
```

---

## 📌 Example Endpoint

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def home():
    return {"message": "Welcome to FastAPI"}
```

Response:

```json
{
  "message": "Welcome to FastAPI"
}
```

---

## 🧪 Running Tests

```bash
pytest
```

---

## 🐳 Docker Support

Build the Docker image:

```bash
docker build -t fastapi-app .
```

Run the container:

```bash
docker run -p 8000:8000 fastapi-app
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Added new feature"
```

4. Push the branch

```bash
git push origin feature-name
```

5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author
Harshit Namdev

