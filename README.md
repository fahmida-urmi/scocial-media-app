Key Features
Authentication System

Register with a username, email, and password
Login/logout functionality
Password management with security features
Post Handling

A global feed displaying posts from all users
Personal profile page showcasing the user's posts
Option to create posts with text and images
Capability to edit or delete posts
User Experience

Clear and user-friendly navigation
Fully responsive layout
Consistent design leveraging template inheritance
Notifications to inform users about actions
Technologies Used
Backend: Django 5.1.6
Frontend: HTML, CSS,Bootsrap, JavaScript
Database: SQLite
Image Processing: Pillow 11.1.0
Installation Guide
Clone the repository:https://github.com/fahmida-urmi/scocial-media-app.git

bash
Copy
Edit
git clone 
cd SocialAPP
Set up a virtual environment (optional but recommended):

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
Install the required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run database migrations:

bash
Copy
Edit
python manage.py migrate
Launch the development server:

bash
Copy
Edit
python manage.py runserver
Open your browser and go to http://127.0.0.1:8000.

Test Login Details
Admin Account
Username: admin
Password: admin
Sample User Accounts


User 1

Username: fahmida_rahman
Password: urmi@1234

User2

Username: amaya
Password: amayajannah1234




ERD Files
ERD with Relationships: ERD_With_Relationship.jpg
ERD without Relationships: SocialAPP_ERD.jpg
Project Structure
markdown
Copy
Edit
Social_Media_App/
├── media/
├── social_app/
│   ├── __pycache__/
│   └── migrations/
├── templatetags/
│   ├── __pycache__/
│   ├── __init__.py
│   ├── custom_filters.py
│   ├── form_tags.py
│   └── models.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── social_project/
│   ├── __pycache__/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── static/
│   └── js/
│       └── comments.js
├── templates/
│   ├── registration/
│   │   └── login.html
│   ├── social_app/
│   │   ├── home.html
│   │   ├── landing.html
│   │   ├── post_confirm_delete.html
│   │   ├── post_form.html
│   │   ├── profile.html
│   │   └── register.html
│   └── base.html
├── venv/
├── create_users.py
├── db.sqlite3
├── manage.py
└── requirements.txt
Required Libraries
ini
Copy
Edit
asgiref==3.8.1
Django==5.1.6
pillow==11.1.0
sqlparse==0.5.3
tzdata==2025.1
Key Functionalities
Global Feed

Displays posts from all users
Optimized queries with Django ORM
Paginated posts for better performance
User Profile Page

Personal post management options
Option to edit and delete posts
Secure access to profile data
Post Management

Create posts with text and images
Edit or remove your own posts
Deletion confirmation process
Authentication

Utilizes Django's built-in authentication
Secured views with the login_required decorator
Manages user sessions