# 📊 Job Tracker Backend

This is the backend for **Job Tracker** — a full-stack project designed to help job seekers organize, track, and manage their job applications efficiently. Built with love using **FastAPI**, **Docker**, and **PostgreSQL**, and powered by **Poetry** for Python dependency management.

---

## 🚀 Features

- ✅ FastAPI-powered REST API
- ✅ PostgreSQL database via Docker Compose
- ✅ Async SQLAlchemy ORM with Alembic migrations
- ✅ Clean project structure (`app/`, `models/`, `schemas/`, `api/`)
- ✅ Environment management with `.env` and `python-dotenv`
- ✅ Production-ready Docker setup
- ✅ Live reload & dev volumes in `docker-compose.dev.yaml`

---

## 🧱 Tech Stack

| Layer      | Tool                 |
| ---------- | -------------------- |
| Language   | Python 3.12          |
| Framework  | FastAPI              |
| ORM        | SQLAlchemy + asyncpg |
| DB         | PostgreSQL 15        |
| Packaging  | Poetry               |
| Migrations | Alembic              |
| Dev Env    | Docker + Compose     |
| API Server | Uvicorn              |

---

## ⚙️ Getting Started (Dev)

````bash
# Clone the repo
git clone https://github.com/shrestha-ankit/job-tracker-backend.git
cd job-tracker-backend

# Make sure you have Docker + Docker Compose installed
cp .env.example .env  # create your own .env file

# Start backend + Postgres
docker compose -f docker-compose.dev.yaml up --build
Then visit:

arduino
Copy
Edit
http://localhost:8000/
📦 Project Structure
bash
Copy
Edit
job-tracker-backend/
├── app/
│   ├── main.py              # Entry point
│   ├── api/                 # API routes
│   ├── models/              # SQLAlchemy models
│   ├── schemas/             # Pydantic schemas
│   ├── db/                  # DB session, config
│   └── core/                # Configs, security, etc.
├── Dockerfile
├── Dockerfile.dev
├── docker-compose.yaml
├── docker-compose.dev.yaml
├── .env.example
├── .gitignore
├── pyproject.toml
└── README.md
🛠️ Roadmap
 Auth system (JWT)

 CRUD for jobs & applications

 User roles & ownership

 CI/CD with GitHub Actions

 Admin dashboard (separate frontend)

👨‍💻 Author
Ankit Shrestha
🧠 Software Engineer | 🇳🇵 Nepal
📧 ankit.shrestha196@gmail.com
🌐 ankitshrestha.com

🧪 API Docs
Once running, check out:

bash
Copy
Edit

🛡️ License
MIT — do whatever, just don’t blame me if your coffee spills.

⭐️ Like the project?
Star it. Fork it. Use it. Break it. PRs welcome.
Let’s build something awesome. 🛠️

yaml
Copy
Edit

---

### 🧼 Bonus: create `.env.example`

You can make a dummy `.env.example` for others:

```env
# .env.example
DATABASE_URL=postgresql+asyncpg://postgres:postgres@db:5432/jobtracker
````
