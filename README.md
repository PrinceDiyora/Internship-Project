# Supply Chain Management System (SCMS)

A modular Supply Chain Management System with the following components:
- **LOGIN**: User authentication and role-based access (Admin, Manager, Employee, Project Manager, etc.)
- **PRODUCTMANAGER**: Product management (CRUD, inventory, etc.)
- **SHOP**: E-commerce shop for placing orders
- **SUPPLYCHAIN**: Backend and frontend for supply chain order processing

---

## Directory Structure

```
SCMS FULL/
  LOGIN/           # Authentication backend & frontend
  PRODUCTMANAGER/  # Product management GUI
  SHOP/            # Shop backend (Django REST) & frontend (PyQt)
  SUPPLYCHAIN/     # Supply chain backend (Django REST) & frontend (PyQt)
```

---

## Prerequisites
- Python 3.8+
- pip (Python package manager)

---


### Backend

#### Setup & Run
```bash
cd LOGIN/backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Frontend

#### Run
```bash
cd LOGIN/frontend
python frontend.py
```

---


---

## Database
- SQLite is used by default for all Django backends.
- Run `python manage.py migrate` in each backend directory to initialize the database.

---

## Notes
- For email notifications in SUPPLYCHAIN, configure your SendGrid API key and sender email in environment variables or directly in the code.
- All PyQt5 frontends require a desktop environment.
- For best results, run each backend server on a different port (default: 8000, 8001, etc.) and update frontend API URLs if needed.

---
