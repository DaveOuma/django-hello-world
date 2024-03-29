# Django Hello World

This is a simple Django project that demonstrates how to display "Hello World" on a webpage.

## Setup Instructions

Follow these steps to set up the project:

1. **Install virtualenv**: First, open Command Prompt in normal mode. You can do this by pressing Windows+R and then typing "cmd" and hitting Enter. In Command Prompt, navigate to your project directory. For example:
    ```
    cd C:\Users\user\Desktop\UserDjangoProject  \\replace "UserDjangoProject" with the directory of your project\\
    ```
    Then install virtualenv using pip:
    ```
    pip install virtualenv
    ```

2. **Create a Virtual Environment**: After installing virtualenv, create a new virtual environment using:
    ```
    virtualenv -p python3 venv
    ```

3. **Activate the Virtual Environment**: Activate the virtual environment by running the activation script. It will look like this:
    ```
    venv\Scripts\activate or source venv\Scripts\activate or for linux source yourenvironmentname/bin/activate
    ```
    After activation, you should see `(venv)` in your command prompt, indicating that the virtual environment is active.

4. **Install Django**: With the virtual environment activated, install Django using pip:
    ```
    pip install django
    ```

5. **Create Django Project and App**: Once Django is installed, you can create a new Django project and app as follows:
    ```
    django-admin startproject myproject
    cd myproject
    python manage.py startapp myapp
    ```

6. **Define URL Route and View Function**: Define a URL route in the `urls.py` file of the project and create a view function in the app's `views.py` file that returns an HTTP response with the "Hello World" message. Map the URL route to the view function.

7. **Run the Django Development Server**: Start the Django development server by running:
    ```
    python manage.py runserver
    ```
    Access the webpage to see the "Hello World" message displayed.

8. **Deactivate the Virtual Environment**: When you're done working on the project, deactivate the virtual environment using:
    ```
    deactivate
    ```

## Author

- David Ouma
- Contact: davidomuga@gmail.com

