<p align="center">
  <img src="lms_app/static/images/logo-name.png" width="300" alt="LMS Logo">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flask-2.3.x-informational?logo=flask" alt="Flask">
  <img src="https://img.shields.io/badge/SQLAlchemy-2.0-important?logo=sqlite" alt="SQLAlchemy">
  <img src="https://img.shields.io/badge/License-MIT-success" alt="License">
  <img src="https://img.shields.io/badge/Version-1.0.0-blueviolet" alt="Version">
</p>

<h3 align="center">📚 Modern Library Management System | 🔐 Role-Based Access | 🌓 Dark Mode</h3>

---

<div align="center">
  
[![Live Demo](https://img.shields.io/badge/TRY_LIVE_DEMO-%2300b894?style=for-the-badge&logo=firefox)](https://your-demo-link.com)
[![Report Issue](https://img.shields.io/badge/REPORT_ISSUE-%23e84393?style=for-the-badge&logo=github)](https://github.com/your-repo/issues)

</div>

---

## 🎯 **Key Features**

<div align="center">
  
| **Authentication** 🔐 | **Book Management** 📖 | **Analytics** 📊 |
|-----------------------|------------------------|------------------|
| Role-based access control | Borrow/return tracking | Visual dashboard |
| Admin registration portal | Inventory management | Overdue fines stats |
| Secure password hashing | ISBN validation | User activity logs |

</div>

---

## 🧩 Tech Stack
<div align="center">

| Component          | Technology                                                                                |
|--------------------|-------------------------------------------------------------------------------------------|
| Backend Framework  | <img src="https://img.shields.io/badge/Flask-2.3.x-informational?logo=flask" width="150"> |
| Database ORM       | <img src="https://img.shields.io/badge/SQLAlchemy-2.0-important" width="150">             |
| Frontend           | <img src="https://img.shields.io/badge/Jinja2-3.x-blueviolet" width="150">                |
| Styling            | <img src="https://img.shields.io/badge/Bootstrap-5.3-8A2BE2" width="150">                 |

</div>

---

## 🛠️ Prerequisites

- **Python 3.8+**
- **Pip** (Python package installer)
- **SQLite3** (Pre-installed with Python, but confirm with `sqlite3 --version`)

---

## 📥 Installation & Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/FLGCAPULI/BookIT.git
   cd BookIT
   ```

2. **Set Up Virtual Environment (Optional but Recommended):**

   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Environment Variables (Windows CMD):**

   ```cmd
   set FLASK_APP=main.py
   ```

   _For PowerShell:_

   ```powershell
   $env:FLASK_APP="main.py"
   ```

---

## 🗄️ Database Setup

1. **Initialize Migrations:**

   ```bash
   flask db init
   ```

2. **Generate Migration Script:**

   ```bash
   flask db migrate -m "Initial migration"
   ```

3. **Apply Migrations:**

   ```bash
   flask db upgrade
   ```

---

## 🚀 Running the Application

Start the Flask development server:

```bash
flask run
```

The app will run at:

```
For the host:
http://localhost:5000/ 

for others in your local network:
http://IPv4:5000/
```

---

## 👑 **Admin Access**

1. **Register as Admin:**  
   Open the following URL in your browser:

   ```
   http://localhost:5000/adminreg?key=sinigangmix
   ```

2. **Fill in the admin registration form.**  
3. **After registration, log in using your admin credentials.**  

---

## 📁 Project Structure

```
LMS/
│
├── lms_app/
│   ├── __init__.py         # Flask app factory
│   ├── models.py           # Database models (User, Book, Transaction, Feedback)
│   ├── routes.py           # Flask routes
│   ├── templates/          # Jinja2 templates
│   └── static/             # Static files (CSS, JS, images)
│
├── migrations/             # Database migrations (Flask-Migrate)
├── instance/               # database
├── main.py                 # Flask app entry point
├── config.py               # App configurations
├── requirements.txt        # Python dependencies
└── README.md               # You're here!
```

---

## 🧯 Troubleshooting

**💥 `sqlite3` Not Recognized?**  
- Add SQLite to your system PATH or reinstall SQLite.

**💥 Flask Can't Locate App?**  
- Ensure `FLASK_APP=main.py` is set in your environment variables.

**💥 Migration Issues?**  
- Reset migrations:

  ```bash
  rmdir /s /q migrations
  del library_db.sqlite3
  flask db init
  flask db migrate -m "Reset migrations"
  flask db upgrade
  ```
---

## 🌱 Contribution

<p align="center">
  <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge" alt="Contributions Welcome">
</p>

1. Fork the repository
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

<div align="center">
  <sub>Built with ❤️ by <a href="https://github.com/FLGCAPULI">FLGCAPULI</a></sub> <a href="https://github.com/Jethro-Cortez">Jethro Cortez</a></sub> | <sub>📧 <a href="mailto:franzlester20@gmail.com">Contact Maintainer</a></sub>
</div>
