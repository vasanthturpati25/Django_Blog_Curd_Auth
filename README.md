# 📝 Django Blog Web Application

A fully functional **Blog Web Application** built using Django, implementing complete CRUD operations along with **user authentication and authorization**.


## 🚀 Features

- User Registration & Login system
- Authentication-based access control
- Create, Read, Update, Delete (CRUD) blog posts
- Only authenticated users can create posts
- Only post owners can edit or delete their posts
- Author displayed on each post
- Dynamic URL routing with parameters
- Reusable templates using inheritance
- Secure form handling with CSRF protection
- User feedback using Django messages framework


## 🛠️ Tech Stack

- Python
- Django
- HTML5
- CSS3
- SQLite


## 📚 What I Learned

- Setting up Django project and applications  
- Creating models and managing database using migrations  
- Implementing model relationships (ForeignKey: Post → User)  
- Interacting with database using Django ORM  
- Implementing user authentication (login, logout, register)  
- Handling authorization (restricting access to post owners)  
- Protecting views using `login_required` decorator  
- Managing sessions and user context  
- Handling HTTP requests using function-based views  
- Configuring URL routing and dynamic parameters  
- Using named URLs with `{% url %}`  
- Rendering dynamic data using templates  
- Implementing template inheritance  
- Using conditional template logic for access control  
- Handling forms using POST method  
- Securing forms with CSRF tokens  
- Using `get_object_or_404` for error handling  
- Using Django messages framework for feedback  
- Redirecting users after actions  
- Fetching and ordering data using QuerySets  


## 🔐 Authentication & Authorization

- Users must log in to access the application  
- Each post is linked to a specific user (author)  
- Only the post owner can:
  - Edit the post  
  - Delete the post  


## 🎯 CRUD Operations

- ➕ Create Post  
- 📖 Read/View Posts  
- ✏️ Update Post (owner only)  
- ❌ Delete Post (owner only)  


## ⚙️ Setup Instructions

```bash
git clone https://github.com/vasanthturpati25/Django_Blog_Website_App.git
cd Django_Blog_Website_App

python -m venv venv

# Activate virtual environment
venv\Scripts\activate      # Windows
source venv/bin/activate   # Linux/Mac

pip install django

python manage.py makemigrations
python manage.py migrate

python manage.py runserver
