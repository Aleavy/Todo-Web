Todo-WebApp
A simple web application built with Flask that allows users to create, update, and delete tasks. This app uses SQLite for database management.

Features
Create Tasks: Add new tasks to your todo list.
Read Tasks: View all tasks sorted by their creation date.
Update Tasks: Modify the content of existing tasks.
Delete Tasks: Remove tasks from your list.
Technologies Used
Flask: A lightweight web application framework for Python.
SQLAlchemy: An ORM (Object Relational Mapper) for handling database operations.
SQLite: A lightweight, disk-based database.
Installation
Clone the repository:

bash
Copiar código
git clone <repository-url>
cd Todo-WebApp
Set up a virtual environment (optional but recommended):

bash
Copiar código
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required packages:

bash
Copiar código
pip install Flask Flask-SQLAlchemy
Create the database:

Run the following commands in a Python shell to create the database:

python
Copiar código
from yourapp import db
db.create_all()
Replace yourapp with the name of your Python file (without the .py extension).

Usage
Run the application:

bash
Copiar código
python yourapp.py
Replace yourapp.py with the name of your main application file.

Access the web app:

Open your web browser and go to http://127.0.0.1:5000/.

Routes
GET /: Display all tasks and a form to add new tasks.
POST /: Add a new task to the database.
GET /delete/<int:id>: Delete a task by its ID.
GET /update/<int:id>: Display a form to update a task.
POST /update/<int:id>: Update the task's content.
Templates
index.html: The main page for displaying tasks and adding new ones.
update.html: A form for updating existing tasks.
Contributing
Contributions are welcome! Please feel free to submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Flask Documentation
SQLAlchemy Documentation
