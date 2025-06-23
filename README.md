# IITB-Course-Management
I built this project as part of an assignment for an internship opportunity at IIT Bombay. It manages university courses and their scheduled instances, using a React frontend, Spring Boot backend, and Docker for full-stack deployment.
# 🏫 IIT Bombay Course Management Webpage

This is a full-stack course management system built as part of an internship assignment for IIT Bombay. It allows users to manage university-level courses and course instances with prerequisite tracking, semester-wise scheduling, and validation rules.

---

## 🧰 Tech Stack

| Layer        | Technology                      |
|--------------|----------------------------------|
| Frontend     | React (with Vite)               |
| Backend      | Spring Boot (Java)              |
| Database     | H2 (in-memory)                  |
| Containerization | Docker, Docker Compose      |
| Build Tools  | Maven, NPM                      |
| Styling      | HTML/CSS (base styling)         |

---

## 🚀 Features

- 📘 Create, read, and delete courses
- 🔗 Add multiple prerequisites per course
- ⚠️ Prevent deletion if a course is a prerequisite elsewhere
- 🗓️ Create and view course instances by year and semester
- 🧹 Clean, simple UI for quick testing
- 🐳 Fully Dockerized for easy setup and deployment

---

## 🛠️ Running the App with Docker

### Prerequisites:
- Docker Desktop installed and running

### Steps:

```bash
git clone https://github.com/your-username/iitb-course-management.git
cd iitb-course-management
docker compose up --build
Then open:

Frontend: http://localhost:3000

Backend: http://localhost:8080/api/courses

🔗 API Endpoints (Backend)
Method	Endpoint	Description
GET	/api/courses	Get all courses
POST	/api/courses	Create a course
GET	/api/courses/{id}	Get a specific course
DELETE	/api/courses/{id}	Delete a course
POST	/api/instances	Create a course instance
GET	/api/instances/{year}/{semester}	Get instances for a semester
DELETE	/api/instances/{year}/{sem}/{id}	Delete an instance

📁 Project Structure

iitb-course-management/
├── backend/         ← Spring Boot app
│   ├── src/
│   └── Dockerfile
├── frontend/        ← React app
│   ├── src/
│   └── Dockerfile
|── docker-compose.yml


✍️ Author
Aditi Kumari
Developer & Internship Applicant
