# multilingual_faq_project
This is a full-stack web application built with Django (backend) and React (frontend). It allows users to ask and answer Frequently Asked Questions (FAQs) in multiple languages. The application provides translation support, making it accessible to a diverse user base.

Tech Stack
Backend: Django, Django REST Framework (DRF)
Frontend: React, Tailwind CSS
Database: PostgreSQL / SQLite (for development)
Translation API: Google Translate API (optional)
Authentication: JWT (JSON Web Token)

Features
CRUD operations for FAQs (Create, Read, Update, Delete)
Multilingual support for FAQs
Search and filter functionality
User authentication & role-based access control
Responsive UI with Tailwind CSS

Project Setup
git clone https://github.com/your-repo/multilingual_faq_project.git
cd multilingual_faq_project

Install Backend Dependencies
cd multilingual_faq_project

Apply Migrations & Create Superuser
python manage.py migrate
python manage.py createsuperuser  # Create an admin user

 Run Django Server
 python manage.py runserver

 Frontend Setup (React)
 Navigate to Frontend Directory & Install Dependencies
cd frontend
npm install
npm start

 Project Structure
 multilingual_faq_project/
│── backend/               # Django backend
│   ├── faq/               # FAQ app (Django)
│   ├── users/             # Authentication & users app
│   ├── settings.py        # Django settings
│   ├── urls.py            # API routes
│── frontend/              # React frontend
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── App.js         # Main App component
│   │   ├── index.js       # React entry point
│── .env                   # Environment variables
│── requirements.txt       # Backend dependencies
│── package.json           # Frontend dependencies
│── README.md              # Project documentation

 Environment Variables
 # Backend
SECRET_KEY=your-secret-key
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3  # Use PostgreSQL in production

# Frontend
REACT_APP_API_URL=http://127.0.0.1:8000/api/


 Project Progress & Issues Faced

✅ Completed

Backend setup with Django & DRF

Frontend setup with React & Tailwind CSS

Basic CRUD operations for FAQs

User authentication with JWT

API integration between frontend & backend

🚧 In Progress

Multilingual translation API integration

UI/UX improvements

Deployment setup

⚠️ Issues Faced & Fixes

Frontend not displaying

Issue: React app started (npm start), but the page was blank.

Fix: Checked the console (F12 > Console) and found API URL mismatch. Updated .env:

REACT_APP_API_URL=http://127.0.0.1:8000/api/

rm -rf** not working in PowerShell**

Issue: Command failed while deleting node_modules in Windows PowerShell.

Fix: Used:

Remove-Item -Recurse -Force node_modules

cd** command error (Path not found)**

Issue: Trying to navigate to a non-existing folder.

Fix: Verified the actual folder path using ls or dir and corrected the command.

Database migration issues

Issue: Django migrations failed with database errors.

Fix: Ran:

python manage.py makemigrations
python manage.py migrate

npm audit fix** warnings**

Issue: Found deprecated packages while running npm install.

Fix: Updated dependencies and used npm audit fix --force cautiously.

🛠 Build for Production

1️⃣ Backend (Django)

python manage.py collectstatic

2️⃣ Frontend (React)

npm run build

🎯 Future Improvements

✅ Add user profile management

✅ Implement AI-powered FAQ suggestions

✅ Improve UI/UX with animations

✅ Deploy on AWS/GCP

🤝 Contributing

Feel free to contribute! Fork the repo, create a new branch, and submit a pull request. 🚀

📜 License

MIT License © 2025
 
