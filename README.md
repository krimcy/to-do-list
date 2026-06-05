# 📝 Flask To-Do List App with User Authentication

A simple and beginner-friendly Flask application that allows users to register, log in, and manage their personal to-do lists.

## 🚀 Features

- User Registration
- User Login & Logout
- Secure Password Hashing
- Session-Based Authentication
- Add New Tasks
- Mark Tasks as Complete
- Delete Tasks
- User-Specific To-Do Lists
- SQLite Database
- Flask-Login Authentication

---

## 📂 Project Structure

```text
todo_flask_app/
│
├── app.py
├── models.py
├── requirements.txt
│
├── templates/
│   ├── base.html
│   ├── login.html
│   ├── register.html
│   └── index.html
│
└── static/
    └── style.css
```

---

## 🛠️ Technologies Used

- Python 3
- Flask
- Flask-Login
- Flask-SQLAlchemy
- SQLite
- Werkzeug Security

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/todo_flask_app.git
cd todo_flask_app
```

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Start the Flask development server:

```bash
python app.py
```

The application will be available at:

```text
http://127.0.0.1:5000
```

---

## 🔐 Authentication

### Register

Create a new account using:

```text
http://127.0.0.1:5000/register
```

### Login

Access your account using:

```text
http://127.0.0.1:5000/login
```

### Logout

Click the logout link from the dashboard.

---

## 🗄️ Database

The application automatically creates a SQLite database file:

```text
todo.db
```

Database tables:

### User

| Field | Type |
|---------|---------|
| id | Integer |
| username | String |
| password | String (hashed) |

### Todo

| Field | Type |
|---------|---------|
| id | Integer |
| task | String |
| completed | Boolean |
| user_id | Foreign Key |

---

## 📸 Application Workflow

1. User registers an account.
2. User logs in.
3. User adds tasks.
4. User marks tasks as completed.
5. User deletes tasks.
6. User logs out.

Each user can only view and manage their own tasks.

---

## 🔒 Security Features

- Passwords are hashed using Werkzeug.
- Protected routes require authentication.
- User authorization checks prevent modification of other users' tasks.
- Session management handled by Flask-Login.

---

## 📋 Future Improvements

- Bootstrap UI
- Task Due Dates
- Task Categories
- Task Priority Levels
- Password Reset Functionality
- Email Verification
- REST API Endpoints
- Docker Support
- Deployment on Render, Railway, or AWS

---

## 🧪 Example Credentials

You can create your own account through the registration page.

Example:

```text
Username: demo
Password: password123
```

---

## 📜 License

This project is open source and available under the MIT License.

---

## 👨‍💻 Author

Created as a learning project for Flask authentication and CRUD operations.

Feel free to fork, modify, and improve the project.
