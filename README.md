## 📝 Flask To-Do List Web App

This is a simple To-Do List web application built using the **Flask** framework and **SQLite** as the backend database. It allows users to add and delete tasks dynamically via a clean web interface.

---

## 📌 Features

- Add new tasks
- View existing tasks
- Delete tasks
- Data stored in SQLite database
- Deployed on PythonAnywhere

---

## 🚀 Live Demo

🌐 [View the live app here](https://yourusername.pythonanywhere.com)  
> Replace with your actual deployed link on PythonAnywhere

---

## 🛠️ Tech Stack

- **Backend**: Python (Flask)
- **Frontend**: HTML (Jinja2 templating)
- **Database**: SQLite
- **Hosting**: PythonAnywhere

---

## 📁 Project Structure

```

flask\_todo/
│
├── app.py                # Main Flask application
├── todo.db               # SQLite database (auto-created)
├── requirements.txt      # Python dependencies
├── templates/
│   └── index.html        # HTML template
└── venv/                 # Virtual environment (optional - don't upload to GitHub)

````

---

## 💻 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/flask-todo.git
   cd flask-todo

2. Create and activate virtual environment:

   ```bash
   python -m venv venv
   venv\Scripts\activate         # On Windows
   # OR
   source venv/bin/activate      # On macOS/Linux

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create the database:

   ```bash
   python
   >>> from app import db
   >>> db.create_all()
   >>> exit()
   ```

5. Run the app:

   ```bash
   python app.py
   ```

6. Visit in browser:

   ```
   http://127.0.0.1:5000
   ```


## ☁️ Deployment on PythonAnywhere

1. Create a free account at [PythonAnywhere](https://www.pythonanywhere.com)
2. Upload your project files to your PythonAnywhere account
3. Set up a **Manual Web App** and configure your WSGI file:

   ```python
   import sys
   sys.path.insert(0, '/home/yourusername/flask_todo')
   from app import app as application
   ```
4. Install Flask via the Bash console:

   ```bash
   pip3 install --user flask flask_sqlalchemy
   ```
5. Reload the web app to apply changes

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).
