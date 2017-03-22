# Team Management
CRUD Python application that allows users to manage teams.

[![Screenshot](screenshot.png)](https://megancoyle.pythonanywhere.com/)

[View the Deployed App](https://megancoyle.pythonanywhere.com/)

## Technologies Used
* Python
* Flask
* virtualenv
* Flask-SQLAlchemy
* MySQL-Python
* PythonAnywhere: for deploying the app

## Installation
When adding the code to pythonanywhere.com, add the following to the environment:

```
export FLASK_CONFIG=production
$ export FLASK_APP=run.py
$ export SQLALCHEMY_DATABASE_URI='mysql://your-username:your-password@your-host-address/your-database-name'
$ flask db upgrade
```

Edit the WSGI configuration file:

```
path = '/home/your-username/your-project-directory-name'
if path not in sys.path:
    sys.path.append(path)

os.environ['FLASK_CONFIG'] = 'production'
os.environ['SECRET_KEY'] = 'p9Bv<3Eid9%$i01'
os.environ['SQLALCHEMY_DATABASE_URI'] = 'mysql://your-username:your-password@your-host-address/your-database-name'

from run import app as application
```
