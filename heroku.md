
# Running Locally

## virtual enviroment
py -3.12 -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt

# Deploying on heroku

heroku create
git push heroku main
heroku ps:scale web=1
heroku open
heroku logs --tail
heroku ps:scale web=0
heroku ps:scale web=1



# Local heroku
heroku local --port 5001 -f Procfile.windows
heroku local --port 5001

# pushing local changes
pip install -r requirements.txt
heroku local --port 5001 -f Procfile.windows
git push heroku main
heroku open


# adding a heroku add on
heroku addons:create papertrail
heroku addons
heroku addons:open papertrail


# start console

heroku run python manage.py shell

heroku run bash


# Config variables

heroku config:set TIMES=2
heroku config


# create database
heroku addons:create heroku-postgresql:mini
heorku config


""" at the end of requirements.txt
psycopg[c]; sys_platform == "linux"
psycopg[binary]; sys_platform != "linux
"""

""" at the end of Procfile
release: ./manage.py migrate --no-input
"""