# Todo-WebApp

A simple web application built with Flask that allows users to create, update, and delete tasks. This app uses SQLite for database management.

## Features

- **Create Tasks**: Add new tasks to your todo list.
- **Read Tasks**: View all tasks sorted by their creation date.
- **Update Tasks**: Modify the content of existing tasks.
- **Delete Tasks**: Remove tasks from your list.

## Technologies Used

- **Flask**: A lightweight web application framework for Python.
- **SQLAlchemy**: An ORM (Object Relational Mapper) for handling database operations.
- **SQLite**: A lightweight, disk-based database.

## Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd Todo-WebApp
   
2. **Set up a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. **Install the required packages:**

   ```bash
   pip install Flask Flask-SQLAlchemy

4. **Run the application:**

   ```bash
   python app.py run

## Routes

- `GET /`: Display all tasks and a form to add new tasks.
- `POST /`: Add a new task to the database.
- `GET /delete/<int:id>`: Delete a task by its ID.
- `GET /update/<int:id>`: Display a form to update a task.
- `POST /update/<int:id>`: Update the task's content.

## Templates

- `index.html`: The main page for displaying tasks and adding new ones.
- `update.html`: A form for updating existing tasks.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.

## Acknowledgements

- [Flask Documentation](https://flask.palletsprojects.com/)
- [SQLAlchemy Documentation](https://www.sqlalchemy.org/)
