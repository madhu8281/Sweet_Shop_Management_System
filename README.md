# Sweet Nest – Sweet Shop Management System

Sweet Nest is a full-stack Sweet Shop Management System built using Python, Django and SQLite3.
The project follows Test-Driven Development (TDD) principles and demonstrates API development, secure user authentication, inventory management, and a modern frontend for managing sweets.

---
## Live Site

> Deployed via Netlify — https://madhavi.pythonanywhere.com/

---

### Features

### Backend (Django REST API)

* User Authentication (Register/Login with JWT)
* Secure API endpoints for sweets and inventory
* Role-based access (Admin can add/update/delete/restock sweets)
* Purchase system that auto-decreases stock
* Search and filter sweets by name, category, or price
* Database: SQLite3 (auto-handled with Django ORM)
* Admin panel for managing users & sweets

### Frontend (SPA)

* User-friendly interface for login & registration
* Dashboard showing all available sweets
* Search & filter functionality
* Purchase button (disabled if stock = 0)
* Admin-only controls to manage sweets

---

##  Tech Stack

**Backend**

* Python 3.9
* Django + Django REST Framework
* SQLite3 (default Django DB)

**Frontend**

* Django templates
* HTML, CSS, JavaScript

**Other Tools**

* JWT Authentication
* Git for version control
* AI assistance for brainstorming & productivity

---

## API Endpoints

### Auth

* `POST /api/auth/register` → Register a user
* `POST /api/auth/login` → Login & get JWT

### Sweets (Protected)

* `POST /api/product` → Add a new sweet
* `GET /api/product` → View all sweets
* `GET /api/product` → Search sweets (by name, category, price)
* `PUT /api/product/:id` → Update sweet details
* `DELETE /api/product/:id` → Delete a sweet (Admin only)

---

## Testing

The project follows **TDD (Test-Driven Development)**.
Tests include:

* User registration & login
* Sweet CRUD operations
* Purchase & restock functionality
* Search functionality

---

## Setup Instructions

1. **Clone the repo**

```bash
git clone https://github.com/madhu8281/Sweet_Shop_Management_System.git
cd Sweet_Shop_Management_System
```

2. **Create a virtual environment**

```bash
cmd
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
pip install python_decouple
pip install django-admin-honeypot
pip install django-storages
pip install django==3.*   
pip install django-admin-thumbnails

```

4. **Run migrations**

```bash
python manage.py migrate
```

5. **Create a superuser**

```bash
python manage.py createsuperuser
```

6. **Run server**

```bash
python manage.py runserver
```

7. Open `http://127.0.0.1:8000/` 

8. Admin Panel is secured `http://127.0.0.1:8000/securelogin`

---

##  Screenshots

Screenshot pdf file is there in this folder SWEET_SHOP_MANAGEMENT_SYSTEM

---

## My AI Usage

I used AI tools responsibly to speed up development and brainstorming:

* **ChatGPT**

  * Helped me draft API endpoint structures and refine my README.
  * Assisted in writing descriptions for sweet categories and product listings.
  * Suggested Django settings fixes (e.g., SMTP setup, paginator color styling).

### Reflection

AI helped me save time on boilerplate code, documentation, and debugging.
However, all core business logic, customization, and design decisions were **done by me manually** to ensure I understood the implementation.

---
