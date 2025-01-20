## Overview
Simple RESTful APIs using Python, Flask and Flask-SQLAlchemy.

## Flask
Flask is a micro web framework written in Python.

#3 Flask-SQLAlchemy
Flask-SQLAlchemy is an extension for Flask that adds support for SQLAlchemy to your application and work with the ORM [Object–relational mapping]

## Follow the steps
1. Open a Terminal
2. Creating an application folder
3. Setting up a Python virtual environment
    python3 -m venv api-env
4. Access the virtual environment
    source api-env/bin/activate
5. Install Flask
    pip3 install flask
6. Install Flask-SQLAlchemy
    pip3 install flask-sqlalchemy
7. Create an app requirement file
    pip3 freeze > requirments.txt
8. Create a main file
    touch main.py
9. Run the application
    http://127.0.0.1:5000

## API Endpoints
1. Displaying list of destinations <br/>
   http://127.0.0.1:5000/destinations<br/>
   Method: GET
   
3. Add Destination
   http://127.0.0.1:5000/destination<br/>
   Method: POST<br/>
   Request Payload:
   ```JSON
   {
        "destination": "Pokhara",
        "country": "Nepal",
        "rating": 4.5
    }
   ```
5. Update Destination
   http://127.0.0.1:5000/destination/<destination_id><br/>
   Method: PUT<br/>
   Request Payload:
   ```JSON
   {
        "destination": "Pokhara",
        "country": "Nepal",
        "rating": 4.5
    }
   ```
7. Delete Destination
   http://127.0.0.1:5000/destination/4<br/>
   Method: DELETE
