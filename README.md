FastAPI Google OAuth Example

This project is an example of using FastAPI to create a web application that integrates with Google OAuth for user authentication. The application includes routes for user login, logout, and displaying a welcome page after successful authentication.

**Project Structure**

your_project/
├── main.py
├── templates/
│   ├── home.html
│   ├── welcome.html
│   └── errors.html
├── static/
├── .gitignore
└── config.py

**Prerequisites**
Python 3.7+
Google Cloud Platform project with OAuth 2.0 credentials

**Installation**
1. Clone the repository:
   git clone https://github.com/yourusername/yourproject.git
   cd yourproject

2. Create a virtual environment and activate it:
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. Install dependencies:
   pip install fastapi uvicorn jinja2 authlib

4. Set up OAuth 2.0 credentials:
   Go to the Google Cloud Console.
   Create a new project or select an existing one.
   Enable the "Google+ API" and create OAuth 2.0 credentials.
   Set the authorized redirect URI to http://localhost:8000/auth.
   Copy the CLIENT_ID and CLIENT_SECRET values.

5. Create a config.py file in the root directory with the following content:
   CLIENT_ID = "your-google-client-id"
   CLIENT_SECRET = "your-google-client-secret"

6. Create necessary directories and files:
   Create a templates directory with home.html, welcome.html, and errors.html.
   Create a static directory for your static files.

