# 🎓 Planikaa Portal

> A comprehensive educational web platform built with **Django**, featuring exam analysis, blogging, student resources, and a modern user interface.

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg?logo=python&logoColor=white)](https://python.org)
[![Django](https://img.shields.io/badge/Django-4.2+-green.svg?logo=django)](https://www.djangoproject.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Release](https://img.shields.io/github/v/release/Mohammad-Hasan-Kaman/planikaa-portal?color=blue)](https://github.com/Mohammad-Hasan-Kaman/planikaa-portal/releases)


---

## 🚀 Purpose & Target Audience

**Planikaa Portal** is designed for students and educators seeking a unified platform for academic management, exam analysis, and resource sharing. It provides a powerful **web-based solution** accessible from any modern browser.

| Audience | Usage Method |
|----------|--------------|
| **End Users** | Access the web interface locally or via server deployment. |
| **Developers** | Clone the repository, install dependencies, and configure `.env` to run the Django server. |

---

## ✨ Key Features

- 📊 **Exam & Competition Analysis (`analyzer`, `konkur`):**
  - Advanced tools for analyzing exam results and competition data.
  - Visual dashboards and statistical reporting.
- 📝 **Educational Blog (`blog`):**
  - Share articles, tutorials, and educational content.
  - Integrated with user authentication and comments.
- 💬 **Review & Feedback System (`reviews`):**
  - Student and educator feedback loop for course improvement.
- 🎨 **Modern & Responsive Interface:**
  - Clean Django templates with modern styling and **Jalali (Persian) calendar** support.
  - Fully responsive design for mobile, tablet, and desktop browsers.
- 🛡️ **Secure Authentication:**
  - Powered by `django-allauth` for robust user management.
- 📅 **Persian Calendar Integration:**
  - Support for Jalali dates and Persian locale (`jdatetime`, `jalali_core`).

---

## 📥 Installation & Setup

### Prerequisites
- **Python 3.10+**
- **PostgreSQL** (Recommended for production, SQLite for development)
- **Node.js** (Optional, for static assets if pre-processed)

### 1. Clone the Repository
```bash
git clone https://github.com/Mohammad-Hasan-Kaman/planikaa-portal.git
cd planikaa-portal/edu
```

### 2. Create Virtual Environment
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory:
```env
SECRET_KEY=your-secret-key-here
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3
# Add other necessary variables (API keys, etc.)
```

### 5. Run Migrations
```bash
python manage.py migrate
```

### 6. Run the Application

**Option A: Django Web Server**
```bash
python manage.py runserver
```
Access at `http://127.0.0.1:8000`

---

## 🛠 Tech Stack & Libraries

| Component | Technology |
|-----------|------------|
| **Backend** | Django 4.2+, Python 3.10+ |
| **Web UI** | Django Templates, HTML5, CSS3, JavaScript |
| **Authentication** | django-allauth, PyJWT |
| **Database** | SQLite (Dev), PostgreSQL (Prod) |
| **Localization** | jdatetime, jalali_core |
| **Data Analysis** | Pillow, Pygments (syntax highlighting) |
| **Security** | Argon2, cryptography, passlib |

---

## 📂 Project Structure

```
planikaa-portal/
├── analyzer/          # Exam analysis logic
├── blog/              # Blogging module
├── konkur/            # Competition/Exam management
├── reviews/           # Feedback system
├── core/              # Core utilities and shared logic
├── static/            # Static assets (CSS, JS, images)
├── templates/         # HTML templates
├── media/             # User-uploaded files (excluded from git)
├── manage.py          # Django management script
├── requirements.txt   # Python dependencies
├── .env               # Environment variables (DO NOT COMMIT)
└── db.sqlite3         # Database (excluded in dev)
```

---

## 🤝 Contributing

Found a bug or have a feature request? Please open an [Issue](https://github.com/Mohammad-Hasan-Kaman/planikaa-portal/issues).
Contributions are welcome! See [`CONTRIBUTING.md`](CONTRIBUTING.md) for guidelines.

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Support

If you find this tool useful, please give it a **star**! ⭐

[![Stars](https://img.shields.io/github/stars/Mohammad-Hasan-Kaman/planikaa-portal?style=for-the-badge&logo=github&color=blue)](https://github.com/Mohammad-Hasan-Kaman/planikaa-portal/stargazers)

---
*Maintained by Mohammad Hasan Kaman | Last updated: July 2026*

> **Note:** This project is a work in progress. Some features may be under development or testing.
