# Setup
## env

0/ mkdir for project

1/ create  new env
python3 -m venv Project_name_here   # (--system-site-packages # for all packages available for new env)


2/ activate env
source Project_name_here/bin/activate

## files

0/ create file for app (any_name.py) THIS HOLDS ALL @app.route decorators for all file locations

# start flask server

1/ (command line:) export FLASK_APP=any_name.py

2/ flask run

# create structure
## create folders

1 / static (for css files)

2/ templates (for all templates)

## create structure files
1/ create layout.html  (bootstrap implementation (header, body ) , menubar,  etc, pl: google analitics)

layout.html MUST HAVE in the body:

{% block content %}

{% endblock content %} # ide jön majd a content from the child

2/ create home/about etc .html-s, inheriting static stuff from layout.html



3/ edit any_name.py @app.route decorators like this : 

@app.route("/home")

def home():

    return render_template('home.html')
    
# pythoneverywhere + github

1/ create or use existing pythoneverywhere account.
## github
2/ on development device create new repo.
3/ create new repo on github (import repo from local --nem emlékszem pontosan, kb igy )

## pythoneverywhere
4/ on pythoneverywhere use console and git pull.
5/ set fecasoft_pythonanywhere_com_wsgi.py  -> set app name -> set 
'''
# add your project directory to the sys.path
project_home = '/home/FecaSoft/FLASK_tut'
'''

'''
# import flask app but need to call it "application" for WSGI to work
from tutorial import app as application  # noqa
'''
    



