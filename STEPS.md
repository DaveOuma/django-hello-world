# Getting Started with Django
This is a guide to setting up a simple Django project that displays "Hello World" on a webpage. It covers the essential steps of creating a virtual environment, installing Django, building a project structure, and running the development server.

## Prerequisites
- Python 3.6 or later ([Download Python](https://www.python.org/downloads/))
- pip (usually comes bundled with Python)
- Setting Up a Virtual Environment (Recommended)

To set up a virtual environment:
1. Open your terminal or command prompt.
2. Navigate to the directory where you want to create your Django project.
3. Run the following command to create a virtual environment named "env":
    ```bash
    python -m venv env
    ```
    Use code with caution.
4. Activate the virtual environment:
    - **Windows**:
        ```bash
        .\env\Scripts\activate
        ```
    - **macOS/Linux**:
        ```bash
        source env/bin/activate
        ```

## Installing Django
With the virtual environment activated, install Django using pip:
```bash
pip install django

# # Creating a Django Project
Use the Django command-line tools to create a new project named myproject:

django-admin startproject myproject

This will create a directory named myproject containing the core Django project structure.

# # Creating a Django App
Navigate into the myproject directory:

cd myproject

# # Create a new Django app named myapp:

python manage.py startapp myapp

This will create a directory named myapp with the basic structure of a Django app.

# # Defining URL Routes
Open the urls.py file located in your project directory (myproject).
Define URL routes. Here's an example that maps the root URL (/) to a view function:


# myproject/urls.py

from django.contrib import admin
from django.urls import path
from myapp import views

urlpatterns = [
    path('', views.hello_world, name='hello_world'),
    path('admin/', admin.site.urls),
]

# # Creating View Functions
Open the views.py file located in your app directory (myapp).
Create a view function to handle the request for the root URL:

# myapp/views.py

from django.http import HttpResponse

def hello_world(request):
    return HttpResponse("Hello World")

This simple view function returns an HTTP response with the message "Hello World".

# # Running the Development Server
Start the Django development server by running the following command in your project directory (myproject):

python manage.py runserver

This will start the server, usually listening on http://127.0.0.1:8000/.

# # Accessing the Webpage
Open a web browser and navigate to http://127.0.0.1:8000/.
You should see the "Hello World" message displayed on the webpage.
Congratulations! You've successfully created a basic Django project. This guide provides a foundation for building more complex Django applications.