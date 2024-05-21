# Task Smash

Task Smash is a simple task management application built using Flask, SQLite, and SCSS. It allows users to add, update, and delete tasks in a user-friendly web interface.

## Features

- Add new tasks
- View all tasks
- Update existing tasks
- Delete tasks

## Technologies Used

- Flask: A micro web framework for Python.
- SQLite: A lightweight, disk-based database.
- SCSS: A preprocessor scripting language that is interpreted or compiled into CSS.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- Python 3.x
- Flask
- Flask-SCSS
- Flask-SQLAlchemy

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/task-smash.git
   cd task-smash
   ```

2. Create a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:

   ```bash
   pip install Flask Flask-SCSS Flask-SQLAlchemy
   ```

4. Run the application:

   ```bash
   python app.py
   ```

5. Open your web browser and go to `http://127.0.0.1:5000/`.

## Project Structure

```plaintext
.
├── app.py
├── templates
│   ├── base.html
│   ├── index.html
│   └── edit.html
├── static
│   └── style.scss
└── database.db
```

### `app.py`

The main application file that initializes Flask, configures the database, and defines routes for the application.

### `templates/`

This directory contains the HTML templates for the application.

- `base.html`: The base template that other templates extend.
- `index.html`: The home page template that displays tasks and provides a form to add new tasks.
- `edit.html`: The template for editing existing tasks.

### `static/`

This directory contains static files such as SCSS stylesheets.

- `style.scss`: The SCSS stylesheet for the application.

## Routes

- `/`: The home page where tasks are displayed and new tasks can be added.
- `/delete/<int:id>`: Route to delete a task by its ID.
- `/edit/<int:id>`: Route to edit a task by its ID.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Flask documentation: [Flask Docs](https://flask.palletsprojects.com/)
- SQLite documentation: [SQLite Docs](https://www.sqlite.org/docs.html)
- SCSS documentation: [Sass Docs](https://sass-lang.com/documentation)
