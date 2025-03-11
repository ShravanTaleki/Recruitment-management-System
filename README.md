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
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate     # On Windows
```

### 3. Install Dependencies
```sh
pip install -r requirements.txt
```

### 4. Apply Migrations
```sh
python manage.py migrate
```

### 5. Run the Django Backend
```sh
cd recruitment_backend
python manage.py runserver
```
Access it at: `http://127.0.0.1:8000/`

### 6. Run the Streamlit Frontend
```sh
cd ..
streamlit run app.py
```

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

