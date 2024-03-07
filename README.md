## Task: Design a Flask application that allows users to create, read, update, and delete (CRUD) tasks.

## Design

**HTML Files**

1. **index.html**: This file will serve as the main page of the application. It will display a list of all tasks and provide a form to create new tasks.
2. **create.html**: This file will contain a form for creating new tasks.
3. **edit.html**: This file will contain a form for editing existing tasks.

**Routes**

1. **/**: This route will render the **index.html** file and display a list of all tasks stored in the database.
2. **/create**: This route will render the **create.html** file and allow users to create new tasks. Upon form submission, it will create a new task in the database and redirect to the home page.
3. **/edit/<task_id>**: This route will render the **edit.html** file and allow users to edit an existing task. Upon form submission, it will update the task in the database and redirect to the home page.
4. **/delete/<task_id>**: This route will delete the specified task from the database and redirect to the home page.

**Overall Structure**

The overall structure of the application is as follows:

- The user interacts with the application through the HTML files, which display forms for creating, editing, and deleting tasks.
- The routes defined in the Python Flask application handle the user's requests and interact with the database to perform the necessary operations.
- The database stores the tasks, which are displayed to the user on the home page.

**Installation and Setup**

1. Install Python 3.6 or higher.
2. Install Flask using pip: `pip install Flask`
3. Create a new directory for your Flask project and navigate to it.
4. Create a new virtual environment using `python3 -m venv venv` and activate it using `source venv/bin/activate`.
5. Install the necessary dependencies using `pip install Flask-SQLAlchemy` for database integration and `pip install Flask-WTF` for forms.
6. Create a `config.py` file to define your database connection and other configurations.
7. Create a `models.py` file to define your database models.
8. Create your Flask application instance in a `__init__.py` file.
9. Define your routes in a `routes.py` file.
10. Run your application using `flask run`.

**Contributing to the Project**

Contributions to this project are welcome! Please follow these guidelines:

- Fork the repository on GitHub.
- Create a new branch for your changes.
- Make your changes and write tests to cover them.
- Submit a pull request with a clear description of your changes.
- Follow the PEP-8 coding style conventions.