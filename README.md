# 🍋 Little Lemon Restaurant API

> **Meta Back-End Developer Capstone Project**  
> *Final assignment for the Meta Backend Developer Professional Certificate on Coursera*

## 📋 Project Overview

This project implements a fully functional REST API for the Little Lemon restaurant using the Django REST Framework. The API handles menu management, table bookings, user authentication, and database operations with MySQL.

### Key Features
- 🔐 User registration and token-based authentication
- 📋 Full CRUD operations for menu items
- 🪑 Table booking management system
- 🗄️ MySQL database integration
- ✅ Comprehensive unit testing
- 🔄 Djoser authentication endpoints

---

## 🚀 API Endpoints

### Menu Items

| Endpoint | Method | Description | Auth Required | Status |
|----------|--------|-------------|---------------|--------|
| `/api/menu/items` | GET | Retrieve all menu items | No | 200 |
| `/api/menu/items` | POST | Create a new menu item | No | 201 |
| `/api/menu/items/{id}` | GET | Retrieve specific menu item | No | 200 |
| `/api/menu/items/{id}` | PUT | Update menu item | No | 200 |
| `/api/menu/items/{id}` | PATCH | Partially update menu item | No | 200 |
| `/api/menu/items/{id}` | DELETE | Delete menu item | No | 200 |

### Table Bookings

| Endpoint | Method | Description | Auth Required | Status |
|----------|--------|-------------|---------------|--------|
| `/api/booking/tables` | GET | Retrieve all bookings | Yes | 200 |
| `/api/booking/tables` | POST | Create a new booking | Yes | 201 |
| `/api/booking/tables/{id}` | GET | Retrieve specific booking | Yes | 200 |
| `/api/booking/tables/{id}` | PUT | Update booking | Yes | 200 |
| `/api/booking/tables/{id}` | PATCH | Partially update booking | Yes | 200 |
| `/api/booking/tables/{id}` | DELETE | Delete booking | Yes | 200 |

### Authentication (Djoser)

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/registration/` | POST | Register new user |
| `/api/auth/token/login/` | POST | Obtain authentication token |
| `/api/auth/token/logout/` | POST | Logout user |

---

## 🛠️ Technology Stack

- **Backend:** Django 4.x, Django REST Framework
- **Database:** MySQL
- **Authentication:** Djoser, Token Authentication
- **Testing:** Django Test Framework
- **Version Control:** Git & GitHub

---

## 📦 Installation & Setup

### Prerequisites
- Python 3.8+
- MySQL Server
- Git

### Local Development Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/little-lemon.git
cd little-lemon
```

2. **Create and activate virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Configure MySQL database**
```python
# settings.py
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'littlelemon_db',
        'USER': 'your_username',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

5. **Run migrations**
```bash
python manage.py makemigrations
python manage.py migrate
```

6. **Create superuser**
```bash
python manage.py createsuperuser
```

7. **Run development server**
```bash
python manage.py runserver
```

---

## 🧪 Testing

Run the test suite to verify functionality:
```bash
python manage.py test
```

---

## 🔍 Peer Review Checklist

When reviewing this project, please verify:

- [ ] Django serves static HTML content
- [ ] Project is committed to a Git repository
- [ ] Backend connects to MySQL database
- [ ] Menu API endpoints are implemented and functional
- [ ] Booking API endpoints are implemented and functional
- [ ] User registration and authentication are set up
- [ ] Unit tests are included and passing
- [ ] API can be tested with Insomnia REST client

---

## 🤝 Contributing

This is a course capstone project. For suggestions or improvements, please feel free to fork the repository and submit a pull request.

---

## 📝 License

This project was created for educational purposes as part of the Meta Back-End Developer Professional Certificate.

---

## 👤 Author

**Maaz Ahmed**  

---

## 🙏 Acknowledgments

- Meta Back-End Developer Professional Certificate team
- Coursera for providing the learning platform
- Django REST Framework community

---

**Happy Reviewing! 🍋**

---
