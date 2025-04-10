# Recruitment Management System

## Overview
The **Recruitment Management System** is a web application designed to streamline the hiring process. It helps recruiters manage job postings, applications, and candidate details efficiently.
A full-stack recruitment management system integrating a Django backend with a Streamlit-based frontend. This system allows users to manage job applications, candidate data, and recruitment processes efficiently. It provides a seamless experience for recruiters to track candidates, post job listings, and streamline the hiring workflow. The backend is built with Django, while the frontend utilizes Streamlit for interactive dashboards.


## Features
- **Streamlit Frontend**: User-friendly interface for managing job applications.
- **Django Backend**: Handles business logic, database interactions, and API endpoints.
- **SQLite Database**: Stores job listings, candidates, and application details.
- **REST API**: Connects the frontend with the backend.
- **Media Upload Support**: Stores resumes and other candidate documents.

## Tech Stack
- **Frontend**: Streamlit
- **Backend**: Django (Python)
- **Database**: SQLite
- **Version Control**: Git & GitHub
- **Server**: Nginx (optional for deployment)

## Installation

### 1. Clone the Repository
```sh
git clone https://github.com/ShravanTaleki/Recruitment-management-System.git
cd Recruitment-management-System
```

### 2. Set Up Virtual Environment (Optional but Recommended)
```sh
python -m venv venv
# For macOS/Linux
source venv/bin/activate
# For Windows
venv\Scripts\activate
```

### 3. Install Dependencies
```sh
pip install -r requirements.txt
```

### 4. Apply Migrations
```sh
cd recruitment_backend
python manage.py makemigrations
python manage.py migrate
```

### 5. Create a Superuser (Admin Account)
```sh
python manage.py createsuperuser
```
> Follow the prompts to enter a username, email, and password.

### 6. Run the Django Backend
```sh
python manage.py runserver
```
Access it at: `http://127.0.0.1:8000/`  
Django Admin Panel: `http://127.0.0.1:8000/admin`

### 7. Run the Streamlit Frontend
Open a new terminal (or tab), then:
```sh
cd ..
streamlit run streamlit_main_source_code.py
```
This will launch the Streamlit UI in your default web browser.


## Usage
1. Recruiters can post job listings.
2. Candidates can apply for jobs.
3. Recruiters can review applications and shortlist candidates.
4. Admins can manage users and job listings.

## Folder Structure
```
Recruitment-management-System/
│── recruitment_backend/     # Django Backend
│   ├── jobs/                # Job management module
│   ├── recruitment_backend/ # Django settings and main app
│   ├── media/               # Uploaded resumes and files
│   ├── db.sqlite3           # SQLite Database
│   ├── manage.py            # Django Admin CLI
│── main.py                  # Streamlit Backend Handler
│── requirements.txt         # Python dependencies
│── README.md                # Project Documentation
```


  
## Future Improvements
- Add authentication (JWT-based login system)
- Deploy on cloud (AWS/GCP/Azure)
- Support multiple databases (PostgreSQL, MySQL)
- Implement AI-based resume screening

---

