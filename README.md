🏪 Inventory Management System
A comprehensive Django-based inventory management system with authentication, product management, and category organization.

✨ Features
🔐 User Authentication - Secure login and registration system

📦 Product Management - Add, edit, delete, and view products

🗂️ Category Organization - Organize products by categories

🔍 Search Functionality - Find products quickly

📱 Responsive Design - Works on desktop and mobile devices

🎨 Clean UI - User-friendly interface with Bootstrap styling

📋 Prerequisites
Before running this project, make sure you have installed:

Python 3.8 or higher

Pipenv (for virtual environment management)

Git

🚀 Installation Guide
1. Clone the Repository
git clone https://github.com/AgustinDeLeonTorres/invProjectDjango.git
cd invProjectDjango

2. Set Up Virtual Environment
# Install pipenv if you haven't already
pip install pipenv

# Create and activate virtual environment
pipenv shell

# Install dependencies
pipenv install

3. Configure Database
# Apply migrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

4. Run Development Server
python manage.py runserver

Visit http://127.0.0.1:8000/ in your browser to access the application.

📁 Project Structure
invProjectDjango/
├── invApp/
│   ├── migrations/     # Database migrations
│   ├── templates/      # HTML templates
│   │   ├── home.html
│   │   ├── layout.html
│   │   ├── product_confirm_delete.html
│   │   ├── product_form.html
│   │   └── product_list.html
│   ├── __init__.py
│   ├── admin.py        # Admin site configuration
│   ├── apps.py
│   ├── forms.py        # Django forms
│   ├── models.py       # Database models
│   ├── tests.py
│   ├── urls.py         # App URL routes
│   └── views.py        # View functions
├── invProject/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py     # Project settings
│   ├── urls.py         # Main URL routes
│   └── wsgi.py
├── db.sqlite3          # Database file (not in production)
├── manage.py           # Django management script
├── Pipfile             # Dependencies list
└── Pipfile.lock        # Locked dependencies

🎯 Usage
For Users
Register a new account or login with existing credentials

Browse products in the inventory

Use search functionality to find specific items

View product details and availability

For Administrators
Access the admin panel at /admin

Manage products, categories, and users

Perform CRUD operations on inventory items

Monitor system activity

🔧 Configuration
Environment Variables
Create a .env file in the project root for production:

SECRET_KEY=your-secret-key-here
DEBUG=False
ALLOWED_HOSTS=yourdomain.com,localhost

Database Settings
The project uses SQLite by default. For production, consider switching to PostgreSQL:
# In settings.py
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'mydatabase',
        'USER': 'mydatabaseuser',
        'PASSWORD': 'mypassword',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}

🤝 Contributing
We welcome contributions! Please follow these steps:

Fork the project

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

👥 Authors
Agustin De Leon Torres - GitHub Profile

🙏 Acknowledgments
Django framework team

Bootstrap for styling components

Django community for excellent documentation and tutorials

⭐ Star this repository if you found it helpful!