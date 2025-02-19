# Django Blog API with Swagger UI Documentation

This repository contains a Django REST Framework-based Blog API with interactive documentation powered by Swagger UI. The API allows users to create, read, update, and delete blog posts, comments, and categories, with comprehensive API documentation available through an interactive interface.

## Features

- RESTful API for managing blog posts, comments, and categories
- Interactive API documentation with Swagger UI
- User authentication and permissions
- Nested routing for post comments
- Automatic OpenAPI schema generation

### 🚀 Live Demo

Check out the detailed blog post about this project: [How to Use Swagger UI with Django](https://dev.to/kihuni/how-to-use-swagger-ui-with-django-4l4a)

Prerequisites

Python 3.8+
Django 4.2+
Django REST Framework
drf-spectacular
drf-nested-routers

### Installation

**Clone the repository:**

```
git clone https://github.com/yourusername/blogapi.git
cd blogapi
```

**Create and activate a virtual environment:**

```
python -m venv blogapi_env
source blogapi_env/bin/activate  # On Windows: blogapi_env\Scripts\activate

```
**Install dependencies:**

```
pip install -r requirements.txt
```
**Run migrations:**

```
python manage.py makemigrations
python manage.py migrate

```
**Create a superuser:**

```
python manage.py createsuperuser
```
**Start the development server:**

```
python manage.py runserver

```

### API Endpoints

The API provides the following endpoints:

_Posts_

```
GET /api/posts/ - List all posts
POST /api/posts/ - Create a new post
GET /api/posts/{id}/ - Retrieve a post
PUT /api/posts/{id}/ - Update a post
DELETE /api/posts/{id}/ - Delete a post

```
_Comments_
```
GET /api/posts/{post_id}/comments/ - List comments for a post
POST /api/posts/{post_id}/comments/ - Create a comment on a post
GET /api/posts/{post_id}/comments/{id}/ - Retrieve a comment
PUT /api/posts/{post_id}/comments/{id}/ - Update a comment
DELETE /api/posts/{post_id}/comments/{id}/ - Delete a comment
```
_Categories_

```
GET /api/categories/ - List all categories
POST /api/categories/ - Create a new category
GET /api/categories/{id}/ - Retrieve a category
PUT /api/categories/{id}/ - Update a category
DELETE /api/categories/{id}/ - Delete a category
```
_Documentation_

```
/api/docs/ - Swagger UI documentation interface
/api/schema/ - OpenAPI schema
```

_API Documentation_

After starting the server, visit `http://127.0.0.1:8000/api/docs/ ` to access the interactive API documentation powered by Swagger UI.
