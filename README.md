# cs50-9-birthdays - Summary
Web application to keep track of friends’ birthdays. This is an exercise for Harvard's CS50 online course.

![birthdays web app](https://github.com/Nimikro/cs50-9-birthdays/blob/main/birthdays.png)

# About this program

In `application.py`, you’ll find the start of a Flask web application. The application has one route (`/`) that accepts both `POST` requests (after the `if`) and `GET` requests (after the `else`). When the `/` route is requested via `GET`, the `index.html` template is rendered. When the `/` route is requested via `POST`, the user is redirected back to `/` via `GET`.

`birthdays.db` is a SQLite database with one table, `birthdays`, that has four columns: `id`, `name`, `month`, and `day`. There are a few rows already in this table, though the web application supports the ability to insert rows into this table!

In the `static` directory is a `styles.css` file containing the CSS code for this web application. No need to edit this file, though you’re welcome to if you’d like!

In the `templates` directory is an `index.html` file that will be rendered when the user views the web application.

# Usage

You will need [Python](https://www.python.org/downloads/) and [Flask](https://flask.palletsprojects.com/en/1.1.x/installation/) installed on your computer to run this application.

Start by installing [Python 3](https://www.python.org/downloads/). Here's a [guide on the installation](https://wiki.python.org/moin/BeginnersGuide/Download). Once you have Python, and clonned this repository, run the following commands:

To install pip, run:
```
sudo apt install python3-pip
```
To install Flask, run:
```
sudo apt install python3-flask
```
Define the correct file as the default Flask application:

Unix Bash (Linux, Mac, etc.):
```
export FLASK_APP=birthdays.py
```
Windows CMD:
```
set FLASK_APP=birthdays.py
```
Windows PowerShell:
```
$env:FLASK_APP = "birthdays.py"
```
Run Flask and you're good to go!
```
flask run
```
