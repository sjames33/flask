
README.md for 'flask' (Flaskr tutorial)

Flaskr -- a mini-blog-like-app -- is the app that you build for the official Flask tutorial. 

Official tutorial:
https://flask.palletsprojects.com/en/2.2.x/tutorial/

Used this one to start:
https://github.com/pallets/flask


Other git repos:
https://github.com/pallets/flask/tree/main/examples/tutorial
https://github.com/mjhea0/flaskr-tdd 

Mine (forked):
https://github.com/sjames33/flask


/Users/stevejames/Projects/Udacity/FSND-Virtual-Machine/vagrant/flask


Needed python 3.9, so setup a venv:

/Users/stevejames/Projects/Udacity/FSND-Virtual-Machine/vagrant/flask/examples/tutorial/venv


---------------------------------


Install:

# clone the repository
$ git clone https://github.com/pallets/flask
$ cd flask
# checkout the correct version
$ git tag  # shows the tagged versions
$ git checkout latest-tag-found-above
$ cd examples/tutorial


Create a virtualenv and activate it:

$ python3 -m venv venv
$ . venv/bin/activate



Install Flaskr:

$ pip install -e .
Or if you are using the main branch, install Flask from source before installing Flaskr:

$ pip install -e ../..
$ pip install -e .
Run

$ flask --app flaskr init-db
$ flask --app flaskr --debug run
Open http://127.0.0.1:5000 in a browser.

Test

$ pip install '.[test]'
$ pytest
Run with coverage report:

$ coverage run -m pytest
$ coverage report
$ coverage html  # open htmlcov/index.html in a browser