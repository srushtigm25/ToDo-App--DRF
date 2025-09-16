A RESTful API for managing ToDo items, built with Django and Django Rest Framework (DRF).
This project demonstrates how to design and implement CRUD APIs with authentication and database integration.

🚀 Features

CRUD operations for ToDo items (Create, Read, Update, Delete)

Each item includes:

title

description

status (pending/completed)

created_at & updated_at timestamps

User authentication (optional) → each user manages their own ToDos

SQLite database for easy development & testing

🛠️ Tech Stack

Python 3.x

Django

Django Rest Framework (DRF)

SQLite (default DB, can be swapped with PostgreSQL/MySQL)

⚙️ Installation & Setup

Clone the repository

git clone https://github.com/srushtigm25/ToDo-App--DRF.git
cd ToDo-App--DRF


Create & activate a virtual environment

python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows


Install dependencies

pip install -r requirements.txt


Run migrations

python manage.py migrate


Start development server

python manage.py runserver

📌 API Endpoints (Examples)
Method	Endpoint	Description
GET	/api/todos/	List all ToDos
POST	/api/todos/	Create a new ToDo
GET	/api/todos/{id}/	Retrieve a ToDo
PUT	/api/todos/{id}/	Update a ToDo
DELETE	/api/todos/{id}/	Delete a ToDo

(If auth enabled → requires login)

🔒 Authentication (Optional)

Token-based authentication using DRF’s built-in system

Each user can only manage their own ToDos
