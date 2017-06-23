# Team Management
CRUD Python application that allows users to manage teams.

[![Screenshot](screenshot.png)](https://team-management-py.herokuapp.com/)

[View the Deployed App](https://team-management-py.herokuapp.com/)

## Technologies Used
* Python
* Flask
* virtualenv
* Flask-SQLAlchemy
* MySQL-Python
* Heroku

## Installation
When running locally, make sure to set up your virtual environment and database:
* `virtualenv venv` to create the environment for the project
* If you're running a mac, use `source my_project/bin/activate` to activate the environment
* Install requirements with `pip install -r requirements.text`
* Deactivate the environment with `deactivate`
* Run mysql, then `mysql -u root`
* Create a user with `CREATE USER 'dt_admin'@'localhost' IDENTIFIED BY 'dt2016';`
* Create the database with `CREATE DATABASE dreamteam_db;`
* Add privileges with `GRANT ALL PRIVILEGES ON dreamteam_db . * TO 'dt_admin'@'localhost';`
* Run the following code before running the app:
```
export FLASK_CONFIG=development
export FLASK_APP=run.py
flask run
```
