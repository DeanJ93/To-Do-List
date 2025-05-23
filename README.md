# Flask Todo List Application

A modern, responsive todo list web application built with Flask. Features user authentication, dark mode support, and a clean interface for managing tasks.

## Features

- User Authentication (Register/Login)
- Create, Read, Update, Delete (CRUD) operations for todos
- Mark todos as complete/incomplete
- Separate views for active and completed tasks
- Dark mode support with persistent preference
- Responsive design
- Modern minimalist UI

## Technical Stack

- Backend: Flask
- Database: SQLite with SQLAlchemy
- Frontend: HTML, CSS, JavaScript
- Authentication: Flask-Login
- Password Security: Werkzeug Security

## Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd To-Do-List
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
.\venv\Scripts\Activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Initialize the database:
```bash
python main.py
```

5. Run the application:
```bash
python main.py
```

The application will be available at `http://127.0.0.1:5000/`

## Project Structure

```
To-Do-List/
├── main.py              # Main application file
├── requirements.txt     # Project dependencies
├── instance/           
│   └── todos.db        # SQLite database
├── static/
│   ├── styles.css      # Global styles
│   └── todos.css       # Todo-specific styles
└── templates/
    ├── base.html       # Base template
    ├── login.html      # Login page
    ├── register.html   # Registration page
    └── todos.html      # Main todo list page
```

## Usage

1. Register a new account or login with existing credentials
2. Add new todos using the input field at the top
3. Mark todos as complete by clicking the checkbox
4. Edit todos by clicking the "Edit" button
5. Delete todos using the "Delete" button
6. Toggle between light and dark mode using the theme button

## Security Features

- Passwords are hashed using Werkzeug Security
- User sessions are managed securely
- CSRF protection enabled
- User data is isolated per account

## Development

To run the application in development mode:

```bash
python main.py
```

The application will automatically reload when changes are detected.

## License

[MIT License](https://opensource.org/licenses/MIT)
