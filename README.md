# FastAPI Todo List App

This is a full-stack web application built with FastAPI, Python, and SQLite. It allows users to register, login, and manage a list of tasks.

## Features

- User registration: Users can create an account by providing a unique username, email, name, and password.
    
- User login: Registered users can log in using their credentials.
    
- User logout: Users can log out of their account.
    
- Task management: Users can view their list of tasks, add new tasks, and delete existing tasks.
    

## Installation

1. Clone the repository:

      ```git clone <repository_url>```

2. Navigate to the project directory:

      ```cd fastapi-todo-list```

3. Create a virtual environment (optional but recommended):

      ``` python -m venv env ```

4. Activate the virtual environment:
  
      ```source env/bin/activate```

5. Install the dependencies:

      ```pip install -r requirements.txt```

6. Set environment variables:

    - Create a `.env` file in the project root directory and add the following variables:
    `SECRET_KEY=<your_secret_key>`
    
    - Replace `<your_secret_key>` with a secret key of your choice.

7. Initialize the SQLite database:

      ```alembic upgrade head```
  
      This will create the necessary database tables.

8. Start the application:

    ```uvicorn main:app --reload```

The app will be accessible at [http://localhost:8000](http://localhost:8000/).

## Usage

- Access the application in your web browser at [http://localhost:8000](http://localhost:8000/).
    
- Register a new account by clicking on the "Register" link.
    
- Log in using your credentials.
    
- Once logged in, you will be redirected to the tasks page where you can view, add, and delete tasks.
    
- To log out, click on the "Logout" link.
